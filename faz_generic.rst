:source: faz_generic.py

:orphan:

.. _faz_generic:

faz_generic -- The Generic FortiAnalyzer module.
+++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 1.0.0


.. contents::
   :local:
   :depth: 1


Synopsis
--------

- This module is able to configure a FortiAnalyzer device.
- Examples include all parameters and values need to be adjusted to data sources before usage.


Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15.0



Parameters
----------

.. raw:: html

  <ul>
  <li><span class="li-head">access_token</span> The token to access FortiAnalyzer without using ansible_username and ansible_password. <span class="li-normal">type: str</span> <span class="li-required">required: false</span></li>
  <li><span class="li-head">enable_log</span> Enable/Disable logging for task <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal"> default: False</span> </li>
  <li><span class="li-head">forticloud_access_token</span> Access token of forticloud analyzer API users. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
  <li><span class="li-head">log_path</span> The path to save log. Used if enable_log is true. Please use absolute path instead of relative path. If the log_path setting is incorrect, the log will be saved in /tmp/fortianalyzer.ansible.log<span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal"> default: "/tmp/fortianalyzer.ansible.log"</span> </li>
  <li><span class="li-head">rc_succeeded</span> The rc codes list with which the conditions to succeed will be overriden <span class="li-normal">type: list</span> <span class="li-required">required: false</span> </li>
  <li><span class="li-head">rc_failed</span> The rc codes list with which the conditions to fail will be overriden <span class="li-normal">type: list</span> <span class="li-required">required: false</span> </li>
  <li><span class="li-head">method</span> The method of API request, grouped with parameter params. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: [add, set, update, get, delete, exec, move, clone]</span>  </li>
  <li><span class="li-head">params</span> The parameter body of API request, grouped with parameter method. <span class="li-normal">type: list</span> <span class="li-required">required: false</span> </li>
  <li><span class="li-head">json</span> The raw json formatted string, it must contain method and params.<span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
  <li><span class="li-head">jsonrpc</span> Some APIs may require jsonrpc set as 2.0 (such as fortiview, report, etc.)<span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
  </ul>



Notes
-----
.. note::


   - Full API reference: https://fndn.fortinet.net/index.php?/fortiapi/175-fortianalyzer/

   - When all three parameters are given at the same time, json has higher priority over method&params. 

   - Normally, running one module can fail when a non-zero rc is returned. you can also override the conditions to fail or succeed with parameters rc_failed and rc_succeeded

Examples
--------

.. code-block:: yaml+jinja

 - hosts: faz01
   connection: httpapi
   collections:
    - fortinet.fortianalyzer
   vars:
    adom: "root"
    ansible_httpapi_use_ssl: True
    ansible_httpapi_validate_certs: False
    ansible_httpapi_port: 443
   tasks:
     - name: 'login a user'
       faz_generic:
             method: 'exec'
             params:
                - url: 'sys/login/user'
                  data:
                   - user: 'admin'
                     passwd: 'ca$hc0w'

  - name: Example playbook
    hosts: fortianalyzers
    connection: httpapi
    vars:
      adom: "root"
      ansible_httpapi_use_ssl: true
      ansible_httpapi_validate_certs: false
      ansible_httpapi_port: 443
    tasks:
      - name: Login a user
        fortinet.fortianalyzer.faz_generic:
          method: "exec"
          params:
            - url: "sys/login/user"
              data:
                - user: "APIUser"
                  passwd: "Fortinet1!e"
      - name: Login another user
        fortinet.fortianalyzer.faz_generic:
          json: |
            {
             "method":"exec",
             "params":[
              {
                   "url":"sys/login/user",
                   "data":[
                      {
                         "user":"APIUser",
                         "passwd":"Fortinet1!"
                      }
                    ]
               }
              ]
            }


Return Values
-------------


Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:


.. raw:: html

  <ul>
    <li><span class="li-return">meta</span> The result of the request. <span class="li-normal">returned: always</span> <span class="li-normal">type: dict</span></li>
    <ul class="ul-self">
      <li><span class="li-return">request_url</span> The full url requested. <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: /sys/login/user</span></li>
      <li><span class="li-return">response_code</span> The status of api request. <span class="li-normal">returned: always</span> <span class="li-normal">type: int</span> <span class="li-normal">sample: 0</span></li>
      <li><span class="li-return">response_data</span> The data body of the api response. <span class="li-normal">returned: optional</span> <span class="li-normal">type: list or dict</span></li>
      <li><span class="li-return">response_message</span> The descriptive message of the api response. <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: OK</span></li>
      <li><span class="li-return">system_information</span> The information of the target system. <span class="li-normal">returned: always</span> <span class="li-normal">type: dict</span></li>
    </ul>
    <li><span class="li-return">rc</span> The status the request. <span class="li-normal">returned: always</span> <span class="li-normal">type: int</span> <span class="li-normal">sample: 0</span></li>
    <li><span class="li-return">version_check_warning</span> Warning if the parameters used in the playbook are not supported by the current fortianalyzer version. <span class="li-normal">returned: if params are not supported in the current version</span> <span class="li-normal">type: list</span></li>
  </ul>



Status
------

- This module is not guaranteed to have a backwards compatible interface.


Authors
-------

- Xinwei Du (@dux-fortinet)
- Maxx Liu (@MaxxLiu22)
- Link Zheng (@chillancezen)
- Jie Xue (@JieX19)
- Frank Shen (@fshen01)
- Hongbin Lu (@fgtdev-hblu)
