
Run Your First Playbook
==============================

This document explains how to run your first FortiAnalyzer Ansible playbook.

--------------

With FortiAnalyzer Galaxy collection, you are always recommended to run
FortiAnalyzer module in ``httpapi`` manner. The first step is to prepare your
host inventory with which you can use ``ansible-vault`` to encrypt or
decrypt your secrets for the sake of confidentiality.

Prepare host inventory
~~~~~~~~~~~~~~~~~~~~~~

In this case, create a file named ``hosts``:

::

   [fortianalyzers]
   fortianalyzer01 ansible_host=192.168.190.130 ansible_user="admin" ansible_password="password"
   fortianalyzer02 ansible_host=192.168.190.131 ansible_user="admin" ansible_password="password"

   [fortianalyzers:vars]
   ansible_network_os=fortinet.fortianalyzer.fortianalyzer
   ansible_httpapi_port=443
   ansible_httpapi_use_ssl=true
   ansible_httpapi_validate_certs=false

Write the playbook
~~~~~~~~~~~~~~~~~~

An Example
----------

In the example: ``test.yml``, we are going to create a script on FortiAnalyzer:

::

   - hosts: fortianalyzers
     connection: httpapi
     vars:
       # You don't need to specify the following vars if you specified them in the host file.
       # ansible_network_os: fortinet.fortianalyzer.fortianalyzer
       # ansible_httpapi_port: 443
       # ansible_httpapi_use_ssl: true
       # ansible_httpapi_validate_certs: false
     tasks:
       - name: Alert console
         fortinet.fortianalyzer.faz_cli_system_global:
            cli_system_global:
                language: english


Parameter Usages
----------------

There are several mandatory options in the example:

-  **adom** : ``adom`` is the administrative domain that an API is going to run inside. In most cases, ``global`` or ``root`` is what you need.
-  **state** : ``state`` is indicating the action the module is going to take. by giving ``present``, the module will create or update the object, while ``absent`` tells the module to delete the object in the FortiAnalyzer.
-  other module specific parameters are defined differently, you can find their usages in each `module page`_.

.. _module page: modules.html

Run the playbook
~~~~~~~~~~~~~~~~

::

   ansible-playbook -i hosts test.yml

you can also observe the verbose output by adding option at the tail:
``-vvv``.
