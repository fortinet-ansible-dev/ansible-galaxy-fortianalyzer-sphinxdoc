Frequently Asked Questions (FAQ)
================================

|

**TABLE OF CONTENTS:**
 - `How To Specify General Variables In One Place?`_
 - `What You Need To Know About Logging.`_
 - `When to Use Parameter bypass_validation?`_
 - `How To Monitor FortiAnalyzer Task?`_
 - `How To Use FortiAnalyzer Ansible without Providing Username and Password?`_
 - `How To Use FortiAnalyzer Ansible With FortiAnalyzer Cloud?`_
 - `Error: No fact modules available and we could not find a fact module for your network OS`_

|


How To Specify General Variables In One Place?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You can specify general variables in one place by using module_defaults.

By using "group/fortinet.fortianalyzer.all", you can specify the general variables for all modules.
By using "group/fortinet.fortianalyzer.adom", you can specify the adom value for all modules that support adom.

::

   - name: Your playbook.
     hosts: fortianalyzers
     connection: httpapi
     module_defaults:
       group/fortinet.fortianalyzer.all:
         enable_log: true
         # access_token: "YOUR ACCESS TOKEN"
         # forticloud_access_token: "YOUR CLOUD ACCESS TOKEN"
         # rc_succeeded: [0, -2, -3]
         # rc_failed: [-2, -3]
       group/fortinet.fortianalyzer.adom:
         adom: "root"
       group/fortinet.fortianalyzer.state:
         state: "present"  # present (create/update) or absent (delete)
     tasks:
       - name: Your task
         fortinet.fortianalyzer.faz_<module>:
           <param>: <value>

Here is an example:

::

   - name: Set module defaults.
     hosts: fortianalyzers
     connection: httpapi
     module_defaults:
       group/fortinet.fortianalyzer.all:
         enable_log: true
         # access_token: "YOUR ACCESS TOKEN"
         # forticloud_access_token: "YOUR CLOUD ACCESS TOKEN"
         # rc_succeeded: [0, -2, -3]
         # rc_failed: [-2, -3]
       group/fortinet.fortianalyzer.adom:
         adom: "root"
       group/fortinet.fortianalyzer.state:
         state: present  # present (create/update) or absent (delete)
     tasks:
       - name: Get fact.
         fortinet.fortianalyzer.faz_fact:
           enable_log: false # Already set in module_defaults, yet you can override module default settings
           facts:
             selector: "dvmdb_device"
             params:
               adom: root
       - name: Create device group table.
         fortinet.fortianalyzer.faz_dvmdb_group:
           # enable_log: true      # Already set in module_defaults
           # adom: root            # Already set in module_defaults
           # state: present        # Already set in module_defaults
           dvmdb_group:
             name: foogroup
             os_type: fos
             type: normal
             desc: Created by Ansible


What You Need To Know About Logging. 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

FortiAnalyzer Ansible has requests and intermediate data stored in a log file ``/tmp/fortianalyzer.ansible.log`` to ease troubleshooting. 

Logging is only enabled by setting ``enable_log`` option for a task.



When to Use Parameter bypass_validation?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You are not encouraged to use ``bypass_validation`` except that you are sure something is wrong with the parameter definition and you want to fix them on you own immediately.
by setting `bypass_validation` to `True`, the content of parameters is not examined, thus enabling you to send any parameters to FortiAnalyzer backend server.

To use this parameter, you are likely to look up the defnition for an API on `fortiapi spec page`_. 



How To Monitor FortiAnalyzer Task?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

There are lots of FortiAnalyzer APIs which return a task identifier. the task itself is running in the remote FortiAnalyzer server.
you must poll the task periodically to see whether the task terminates or goes wrong.

::

  - name: poll the task
    fmgr_fact:
      facts:
        selector: "task_task"
        params:
          task: "{{installing_task.meta.response_data.taskid}}"
    register: taskinfo
    until: taskinfo.meta.response_data.percent == 100
    retries: 30
    delay: 5
    failed_when: taskinfo.meta.response_data.state == 'error'


- ``until`` -  the condition to quit polling, this is the condition to quit normally
- ``retries`` - how many times you want to try to check the status of running task.
- ``delay`` - checking frequency: `1/delay`.
- ``failed_when`` - failing condition in which you regard the task a failure, this is the condition to quit abnormally


How To Use FortiAnalyzer Ansible without Providing Username and Password?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

FortiAnalyzer Ansible collection supports three different ways to login.

1. Providing ansible_user and ansible_password.
2. Using access token.
3. Using the Forticloud access token (only for the FortiAnalyzer managed by Forticloud).

To avoid unexpected behaviour, please only use one login method at a time.

If both ansible_user and ansible_password and access token are provided, the ansible_user and ansible_password will be used.

The access token login method is only valid for the latest versions of FortiAnalyzer v7.

If you want to use the access token to login FortiAnalyzer Ansible, please go to the CLI interface of FortiAnalyzer and enter the following command:

::

  config system admin user
    edit api_user_example_name
      set profileid Super_User
      set user_type api
      set rpc-permit read-write
    next
  end


Then, use ``execute api-user generate-key api_user_example_name`` and you will get an API key.

::

  FAZ-VM64 # execute api-user generate-key api_user_example_name
  New API key: XXXXXXXXXXXXXXX
  

You can use this API key in your playbook, and you don't need to provide ansible_user and ansible_password anymore.

Here is an example of how to use access token:

::

  - hosts: fortianalyzers
    connection: httpapi
    collections:
      - fortinet.fortianalyzer
    vars:
      ansible_httpapi_use_ssl: yes
      ansible_httpapi_validate_certs: no
      ansible_httpapi_port: 443
    tasks:
      - name: get fact
        fmgr_fact:
          access_token: <your access_token>
          facts:
            selector: "sys_status"
        register: result
      - name: Display response
        debug:
          var: result


How To Use FortiAnalyzer Ansible With FortiAnalyzer Cloud?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

FortiAnalyzer can be managed by forticloud. Example of a fortianalyzer cloud host: ``1234567.us-west-1.fortianalyzer.forticloud.com``.

It's possible to authenticate Ansible client with forticloud API access token.
``forticloud_access_token`` is the module option to enable forticloud access token based authentication. 

To obatin access token, it's required to register an API user in https://support.fortinet.com/iam/#/api-user and download the crendentials which contains
needed API user ID and password. it's strongly recommended that you keep it safe!

below is an example to obtain access token:
::


  - hosts: fortianalyzers
    collections:
      - fortinet.fortianalyzer
    connection: httpapi
    vars:
      ansible_httpapi_use_ssl: True
      ansible_httpapi_validate_certs: False
      ansible_httpapi_port: 443
      FORTICLOUD_APIID: "3EE835AF-F9F8-48........"
      FORTICLOUD_PASSWD: "36b25667c61b2.........."
    tasks:
      - name: Generate Access Token From FortiCloud Auth Server.
        uri:
          url: https://customerapiauth.fortinet.com/api/v1/oauth/token/
          method: POST
          body_format: json
          return_content: true
          headers:
            Content-Type: application/json
          body: '{"username": "{{ FORTICLOUD_APIID }}", "password": "{{ FORTICLOUD_PASSWD }}", "client_id": "FortiAnalyzer", "grant_type": "password"}'
        register: tokeninfo

then in subsequent tasks, we can reference returned token:

::

    - name: get fact
      faz_fact:
        forticloud_access_token: '{{ tokeninfo.json.access_token }}'
        enable_log: true
        facts:
          selector: "sys_status"
      register: result
    - name: Display response
      debug:
        var: result

Access token usually expires in hours, you should always renew one in case of failure.



Error: No fact modules available and we could not find a fact module for your network OS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Solution 1 (Recommended): Add vars "ansible_facts_modules: setup" to the host file to avoid this error.
`What is host file?`_

::

   [fortianalyzers]
   fortianalyzer01 ansible_host=192.168.111.1 ansible_user="admin" ansible_password="password"
   fortianalyzer02 ansible_host=192.168.111.2 ansible_user="admin" ansible_password="password"

   [fortianalyzers:vars]
   ansible_network_os=fortinet.fortianalyzer.fortianalyzer
   ansible_facts_modules=setup  # add here
   ansible_httpapi_port=443
   ansible_httpapi_use_ssl=true
   ansible_httpapi_validate_certs=false


Solution 2: Add vars "ansible_facts_modules: setup" to your playbook.

::

  - name: Your task
    hosts: fortianalyzers
    connection: httpapi
    vars:
      ansible_facts_modules: setup # add here
    tasks:
      - name: Your task
        fortinet.fortianalyzer.faz_fact:
          facts:
            selector: "eventmgmt_alerts"
            params:
              adom: "root"
              limit: 1
        register: response
      - name: Display response
        debug:
          var: response


Solution 3: Add "gather_facts: false" to your playbook.

::

  - name: Your task
    hosts: fortianalyzers
    connection: httpapi
    gather_facts: false # add here
    tasks:
      - name: Your task
        fortinet.fortianalyzer.faz_fact:
          facts:
            selector: "eventmgmt_alerts"
            params:
              adom: "root"
              limit: 1
        register: response
      - name: Display response
        debug:
          var: response


.. _fortiapi spec page: https://fndn.fortinet.net/index.php?/fortiapi/175-fortianalyzer/
.. _What is host file?: https://docs.ansible.com/ansible/latest/inventory_guide/intro_inventory.html