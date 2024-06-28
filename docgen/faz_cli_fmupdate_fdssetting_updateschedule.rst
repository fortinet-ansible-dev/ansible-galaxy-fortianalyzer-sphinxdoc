:source: faz_cli_fmupdate_fdssetting_updateschedule.py

:orphan:

.. _faz_cli_fmupdate_fdssetting_updateschedule:

faz_cli_fmupdate_fdssetting_updateschedule -- Configure the schedule when built-in FortiGuard retrieves antivirus and IPS updates.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 1.0.0

.. warning::
   Starting in version 2.0.0, all variables will be named in the underscore naming convention.

   - Possible variable names before 2.0.0: ``variable-name``, ``variable name``, ``variable.name``
   - Corresponding variable names since 2.0.0: ``variable_name``
  
   FortiAnalyzer Ansible v1.4+ supports both previous argument name and new underscore name.
   You will receive deprecation warnings if you keep using the previous argument name.
   You can ignore the warning by setting deprecation_warnings=False in ansible.cfg.

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


FortiAnalyzer Version Compatibility
------------------------------------
.. raw:: html

 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>




Parameters
----------
.. raw:: html

 <ul>
 <li><span class="li-head">access_token</span> The token to access FortiAnalyzer without using ansible_username and ansible_password. <span class="li-normal">type: str</span></li>
 <li><span class="li-head">bypass_validation</span> Only set to True when module schema diffs with FortiAnalyzer API structure, module continues to execute without validating parameters <span class="li-normal">type: bool</span> <span class="li-normal"> default: False</span> </li>
 <li><span class="li-head">enable_log</span> Enable/Disable logging for task <span class="li-normal">type: bool</span> <span class="li-normal"> default: False</span> </li>
 <li><span class="li-head">forticloud_access_token</span> Access token of forticloud analyzer API users. <span class="li-normal">type: str</span> </li>
 <li><span class="li-head">log_path</span> The path to save log. Used if enable_log is true. Please use absolute path instead of relative path. If the log_path setting is incorrect, the log will be saved in /tmp/fortianalyzer.ansible.log<span class="li-normal">type: str</span> <span class="li-normal"> default: "/tmp/fortianalyzer.ansible.log"</span> </li>
 <li><span class="li-head">proposed_method</span> The overridden method for the underlying Json RPC request <span class="li-normal">type: str</span> <span class="li-normal"> choices: set, update, add</span> </li>
 <li><span class="li-head">version_check</span> If set to True, it will check whether the parameters used are supported by the corresponding version of FortiAnazlyer locally based on FNDN data. A warning will be returned in version_check_warning if there is a mismatch. This warning is only a suggestion and may not be accurate. <span class="li-normal">type: bool</span> <span class="li-normal"> default: False</span> </li>
 <li><span class="li-head">rc_succeeded</span> The rc codes list with which the conditions to succeed will be overriden <span class="li-normal">type: list</span> </li>
 <li><span class="li-head">rc_failed</span> The rc codes list with which the conditions to fail will be overriden <span class="li-normal">type: list</span> </li>
 <li><span class="li-head">cli_fmupdate_fdssetting_updateschedule</span> Configure the schedule when built-in FortiGuard retrieves antivirus and IPS updates. <span class="li-normal">type: dict</span></li>
 <ul class="ul-self">
 <li><span class="li-head">day</span> Configure the day the update will occur, if the freqnecy is weekly (Sunday - Saturday, default = Monday). <span class="li-normal">type: str</span>  <span class="li-normal">choices: [Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, Saturday]</span>  <span class="li-normal">default: Monday</span>  <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">frequency</span> Configure update frequency: every - time interval, daily - once a day, weekly - once a week (default = every). <span class="li-normal">type: str</span>  <span class="li-normal">choices: [every, daily, weekly]</span>  <span class="li-normal">default: every</span>  <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">status</span> Enable/disable scheduled updates. <span class="li-normal">type: str</span>  <span class="li-normal">choices: [disable, enable]</span>  <span class="li-normal">default: enable</span>  <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">time</span> Time interval between updates, or the hour and minute when the update occurs (hh: 0 - 23, mm: 0 - 59 or 60 = random, default = 00:10). <span class="li-normal">type: str</span> <span class="li-normal">elements: str</span> <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 </li>
 </ul>
 </ul>


Notes
-----
.. note::

   - To create or update an object, use state: present directive.
   - To delete an object, use state: absent directive
   - Normally, running one module can fail when a non-zero rc is returned. you can also override the conditions to fail or succeed with parameters rc_failed and rc_succeeded

Examples
--------
.. code-block:: yaml+jinja

  - name: Example playbook
    connection: httpapi
    hosts: fortianalyzers
    tasks:
      - name:
          Configure the schedule when built-in FortiGuard retrieves antivirus and
          IPS updates.
        fortinet.fortianalyzer.faz_cli_fmupdate_fdssetting_updateschedule:
          cli_fmupdate_fdssetting_updateschedule:
            day: Sunday
            frequency: weekly
            status: enable
            time: "0:0"
    vars:
      ansible_network_os: fortinet.fortianalyzer.fortianalyzer
      ansible_httpapi_port: 443
      ansible_httpapi_use_ssl: true
      ansible_httpapi_validate_certs: false
  


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