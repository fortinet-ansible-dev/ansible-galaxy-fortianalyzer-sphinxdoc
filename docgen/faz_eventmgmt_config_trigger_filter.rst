:source: faz_eventmgmt_config_trigger_filter.py

:orphan:

.. _faz_eventmgmt_config_trigger_filter:

faz_eventmgmt_config_trigger_filter -- filter
+++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 1.8.0

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
- This module supports check mode and diff mode.

Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15.0


FortiAnalyzer Version Compatibility
------------------------------------
.. raw:: html

 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.2.1</code></p>




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
 <li><span class="li-head">state</span> The directive to create, update or delete an object <span class="li-normal">type: str</span> <span class="li-required">required: true</span> <span class="li-normal"> choices: present, absent</span> </li>
 <li><span class="li-head">adom</span> The parameter in requested url <span class="li-normal">type: str</span> <span class="li-required">required: true</span> </li>
 <li><span class="li-head">trigger_id</span> The parameter in requested url <span class="li-normal">type: str</span> <span class="li-required">required: true</span> </li>
 <li><span class="li-head">eventmgmt_config_trigger_filter</span> Filter <span class="li-normal">type: dict</span></li>
 <ul class="ul-self">
 <li><span class="li-head">dev_type</span> <span class="li-normal">type: raw</span>  <span class="li-normal">choices: [FortiSandbox, FortiWeb, Fabric, Syslog, FortiCache, FortiAuthenticator, FortiMail, FortiProxy, FortiManager, FortiNAC, FortiAnalyzer, FortiClient, FortiDDoS, FortiGate, FortiFirewall]</span>  <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.2.1</code></p>
 </div>
 </li>
 <li><span class="li-head">id</span> <span class="li-normal">type: int</span>  <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.2.1</code></p>
 </div>
 </li>
 <li><span class="li-head">rule</span> reference: /eventmgmt/adom/&lt;adom-name&gt;/config/trigger/&lt;trigger_id&gt;/filter/&lt;filter_id&gt;/rule <span class="li-normal">type: list of dict</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.2.1</code></p>
 </div>
 <ul class="ul-self">
 <li><span class="li-head">id</span> <span class="li-normal">type: int</span>  <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.2.1</code></p>
 </div>
 </li>
 <li><span class="li-head">key</span> <span class="li-normal">type: str</span>  <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.2.1</code></p>
 </div>
 </li>
 <li><span class="li-head">value</span> <span class="li-normal">type: str</span>  <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.2.1</code></p>
 </div>
 </li>
 <li><span class="li-head">value_type</span> <span class="li-normal">type: int</span>  <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.2.1</code></p>
 </div>
 </li>
 <li><span class="li-head">oper</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [less-than, not-contain, less-or-equal, equal, great-or-equal, not-equal, contain, great-than]</span>  <span class="li-normal">default: equal</span>  <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 </ul>
 </li>
 <li><span class="li-head">subject</span> <span class="li-normal">type: str</span>  <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.2.1</code></p>
 </div>
 </li>
 <li><span class="li-head">tag</span> <span class="li-normal">type: str</span>  <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.2.1</code></p>
 </div>
 </li>
 <li><span class="li-head">enable</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: enable</span>  <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">eventstatus</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: </span>  <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">eventtype</span> <span class="li-normal">type: str</span>  <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">extrainfo</span> <span class="li-normal">type: str</span>  <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">extrainfo_type</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [default, custom]</span>  <span class="li-normal">default: default</span>  <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">filter_expr</span> <span class="li-normal">type: str</span>  <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">groupby1</span> <span class="li-normal">type: str</span>  <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">groupby2</span> <span class="li-normal">type: str</span>  <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">logtype</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: traffic</span>  <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">rule_relation</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 0</span>  <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">severity</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [high, medium, critical, low]</span>  <span class="li-normal">default: medium</span>  <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">thres_count</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 1</span>  <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">thres_duration</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 30</span>  <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">utmevent</span> <span class="li-normal">type: str</span>  <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">indicator</span> reference: /log-alert/trigger/filter/indicator <span class="li-normal">type: list of dict</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.0.3 -> v7.2.1</code></p>
 </div>
 <ul class="ul-self">
 <li><span class="li-head">count</span> <span class="li-normal">type: int</span>  <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.0.3 -> v7.2.1</code></p>
 </div>
 </li>
 <li><span class="li-head">name</span> <span class="li-normal">type: str</span>  <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.0.3 -> v7.2.1</code></p>
 </div>
 </li>
 <li><span class="li-head">type</span> <span class="li-normal">type: str</span>  <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.0.3 -> v7.2.1</code></p>
 </div>
 </li>
 </ul>
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
    hosts: fortianalyzers
    connection: httpapi
    gather_facts: false
    vars:
      ansible_network_os: fortinet.fortianalyzer.fortianalyzer
      ansible_httpapi_port: 443
      ansible_httpapi_use_ssl: true
      ansible_httpapi_validate_certs: false
    tasks:
      - name: Filter
        fortinet.fortianalyzer.faz_eventmgmt_config_trigger_filter:
          # bypass_validation: false
          # rc_succeeded: [0, -2, -3, ...]
          # rc_failed: [-2, -3, ...]
          adom: <your own value>
          trigger_id: <your own value>
          state: present # <value in [present, absent]>
          eventmgmt_config_trigger_filter:
            id: 0 # Required variable, integer
            # dev_type: <any type of data>
            # rule:
            #   - id: <value of integer>
            #     key: <value of string>
            #     value: <value of string>
            #     value_type: <value of integer>
            #     oper: <value in [less-than, not-contain, less-or-equal, ...]>
            # subject: <value of string>
            # tag: <value of string>
            # enable: <value in [enable, disable]>
            # eventstatus: <value of string>
            # eventtype: <value of string>
            # extrainfo: <value of string>
            # extrainfo_type: <value in [default, custom]>
            # filter_expr: <value of string>
            # groupby1: <value of string>
            # groupby2: <value of string>
            # logtype: <value of string>
            # rule_relation: <value of integer>
            # severity: <value in [high, medium, critical, ...]>
            # thres_count: <value of integer>
            # thres_duration: <value of integer>
            # utmevent: <value of string>
            # indicator:
            #   - count: <value of integer>
            #     name: <value of string>
            #     type: <value of string>
  


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