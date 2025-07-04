:source: faz_report_config_layout.py

:orphan:

.. _faz_report_config_layout:

faz_report_config_layout -- Config layout.
++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 1.5.0

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
 <li><span class="li-head">version_check</span> If set to True, it will check whether the parameters used are supported by the corresponding version of FortiAnazlyer locally based on FNDN data. A warning will be returned in version_check_warning if there is a mismatch. This warning is only a suggestion and may not be accurate. <span class="li-normal">type: bool</span> <span class="li-normal"> default: True</span> </li>
 <li><span class="li-head">rc_succeeded</span> The rc codes list with which the conditions to succeed will be overriden <span class="li-normal">type: list</span> </li>
 <li><span class="li-head">rc_failed</span> The rc codes list with which the conditions to fail will be overriden <span class="li-normal">type: list</span> </li>
 <li><span class="li-head">state</span> The directive to create, update or delete an object <span class="li-normal">type: str</span> <span class="li-required">required: true</span> <span class="li-normal"> choices: present, absent</span> </li>
 <li><span class="li-head">adom</span> The parameter in requested url <span class="li-normal">type: str</span> <span class="li-required">required: true</span> </li>
 <li><span class="li-head">report_config_layout</span> Config layout. <span class="li-normal">type: dict</span></li>
 <ul class="ul-self">
 <li><span class="li-head">body</span> <span class="li-normal">type: str</span>  <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">component</span> reference: /report/adom/&lt;adom-name&gt;/config/layout/&lt;layout-id&gt;/component <span class="li-normal">type: list of dict</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 <ul class="ul-self">
 <li><span class="li-head">component_id</span> <span class="li-normal">type: int</span>  <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">type</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [graphic, column-break, macro, section, chart, heading2, heading3, heading1, page-break, text]</span>  <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">variable</span> reference: /report/adom/&lt;adom-name&gt;/config/layout/&lt;layout-id&gt;/component/&lt;component-id&gt;/variable <span class="li-normal">type: list of dict</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 <ul class="ul-self">
 <li><span class="li-head">not</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">var</span> <span class="li-normal">type: str</span>  <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">var_value</span> <span class="li-normal">type: str</span>  <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">description</span> <span class="li-normal">type: str</span>  <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">drilldown_flag</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">status</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">var_expression</span> <span class="li-normal">type: str</span>  <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">var_type</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [ip, integer, string, datetime]</span>  <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">view_mask</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 0</span>  <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 </ul>
 </li>
 <li><span class="li-head">alignment</span> <span class="li-normal">type: int</span>  <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">bg_color</span> <span class="li-normal">type: str</span>  <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">category</span> <span class="li-normal">type: str</span>  <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">chart</span> <span class="li-normal">type: str</span>  <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">chart_option</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [calc-average, none]</span>  <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">column</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [1, 2]</span>  <span class="li-normal">default: </span>  <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">customized</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 0</span>  <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">device_mode</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [variable, specify]</span>  <span class="li-normal">default: variable</span>  <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">devices</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: All_FortiGate</span>  <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">drill_down_report</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">filter_logic</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [all, any]</span>  <span class="li-normal">default: all</span>  <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">filter_mode</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [override, inherit]</span>  <span class="li-normal">default: inherit</span>  <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">font_color</span> <span class="li-normal">type: str</span>  <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">font_family</span> <span class="li-normal">type: str</span>  <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">font_size</span> <span class="li-normal">type: int</span>  <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">font_type</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [bold-italic, bold, undefined, italic, normal]</span>  <span class="li-normal">default: undefined</span>  <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">graphic</span> <span class="li-normal">type: str</span>  <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">include_other</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: enable</span>  <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">ldap_query</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [auto, enable, disable]</span>  <span class="li-normal">default: auto</span>  <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">ldap_server</span> <span class="li-normal">type: str</span>  <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">ldap_user_case_change</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [upper, lower, disable]</span>  <span class="li-normal">default: </span>  <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">left_margin</span> <span class="li-normal">type: int</span>  <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">macro</span> <span class="li-normal">type: str</span>  <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">not_vdom</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">period_end</span> [YYYY-MM-DD], [HH:MM:SS] <span class="li-normal">type: list of dict</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 <ul class="ul-self">
 </ul>
 </li>
 <li><span class="li-head">period_last_n</span> <span class="li-normal">type: int</span>  <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">period_mode</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [variable, specify]</span>  <span class="li-normal">default: variable</span>  <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">period_opt</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [faz, dev]</span>  <span class="li-normal">default: </span>  <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">period_start</span> [YYYY-MM-DD], [HH:MM:SS] <span class="li-normal">type: list of dict</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 <ul class="ul-self">
 </ul>
 </li>
 <li><span class="li-head">right_margin</span> <span class="li-normal">type: int</span>  <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">table_color</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [default, blue, green, red]</span>  <span class="li-normal">default: default</span>  <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">text</span> <span class="li-normal">type: str</span>  <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">time_period</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [last-n-weeks, last-month, last-7-days, last-week, yesterday, this-month, this-week, last-30-days, last-quarter, last-2-weeks, this-quarter, last-n-days, last-14-days, this-year, other, today, last-n-hours]</span>  <span class="li-normal">default: </span>  <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">title</span> <span class="li-normal">type: str</span>  <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">vdom</span> <span class="li-normal">type: str</span>  <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">week_start</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [wed, sun, fri, thr, mon, tue, sat]</span>  <span class="li-normal">default: </span>  <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">width</span> <span class="li-normal">type: int</span>  <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 </ul>
 </li>
 <li><span class="li-head">description</span> <span class="li-normal">type: str</span>  <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">footer</span> reference: /report/adom/&lt;adom-name&gt;/config/layout/&lt;layout-id&gt;/footer <span class="li-normal">type: list of dict</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 <ul class="ul-self">
 <li><span class="li-head">footer_id</span> <span class="li-normal">type: int</span>  <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">type</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [text, graphic, minicover]</span>  <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">graphic</span> <span class="li-normal">type: str</span>  <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">text</span> <span class="li-normal">type: str</span>  <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 </ul>
 </li>
 <li><span class="li-head">header</span> reference: /report/adom/&lt;adom-name&gt;/config/layout/&lt;layout-id&gt;/header <span class="li-normal">type: list of dict</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 <ul class="ul-self">
 <li><span class="li-head">header_id</span> <span class="li-normal">type: int</span>  <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">type</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [text, graphic, minicover]</span>  <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">graphic</span> <span class="li-normal">type: str</span>  <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">text</span> <span class="li-normal">type: str</span>  <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 </ul>
 </li>
 <li><span class="li-head">language</span> <span class="li-normal">type: str</span>  <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">layout_id</span> <span class="li-normal">type: int</span>  <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">subtitle</span> <span class="li-normal">type: str</span>  <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">title</span> <span class="li-normal">type: str</span>  <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">alignment</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [right, center, left]</span>  <span class="li-normal">default: left</span>  <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">bg_color</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: #FFFFFF</span>  <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">category</span> <span class="li-normal">type: str</span>  <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">chart_heading_level</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 2</span>  <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">chart_info_display</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">coverpage_background_image</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: {sys_img_path}/def_cover_bgimg_ver1.png</span>  <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">coverpage_bottom_image</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: </span>  <a id='label144' href="javascript:ContentClick('label145', 'label144');" onmouseover="ContentPreview('label145');" onmouseout="ContentUnpreview('label145');" title="click to collapse or expand..."> more... </a>
 <div id="label145" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">coverpage_custom_text1</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: </span>  <a id='label146' href="javascript:ContentClick('label147', 'label146');" onmouseover="ContentPreview('label147');" onmouseout="ContentUnpreview('label147');" title="click to collapse or expand..."> more... </a>
 <div id="label147" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">coverpage_custom_text2</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: </span>  <a id='label148' href="javascript:ContentClick('label149', 'label148');" onmouseover="ContentPreview('label149');" onmouseout="ContentUnpreview('label149');" title="click to collapse or expand..."> more... </a>
 <div id="label149" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">coverpage_enable_create_time</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: enable</span>  <a id='label150' href="javascript:ContentClick('label151', 'label150');" onmouseover="ContentPreview('label151');" onmouseout="ContentUnpreview('label151');" title="click to collapse or expand..."> more... </a>
 <div id="label151" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">coverpage_enable_time_period</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: enable</span>  <a id='label152' href="javascript:ContentClick('label153', 'label152');" onmouseover="ContentPreview('label153');" onmouseout="ContentUnpreview('label153');" title="click to collapse or expand..."> more... </a>
 <div id="label153" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">coverpage_footer_bgcolor</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: transparent</span>  <a id='label154' href="javascript:ContentClick('label155', 'label154');" onmouseover="ContentPreview('label155');" onmouseout="ContentUnpreview('label155');" title="click to collapse or expand..."> more... </a>
 <div id="label155" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">coverpage_footer_left</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: </span>  <a id='label156' href="javascript:ContentClick('label157', 'label156');" onmouseover="ContentPreview('label157');" onmouseout="ContentUnpreview('label157');" title="click to collapse or expand..."> more... </a>
 <div id="label157" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">coverpage_footer_right</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: </span>  <a id='label158' href="javascript:ContentClick('label159', 'label158');" onmouseover="ContentPreview('label159');" onmouseout="ContentUnpreview('label159');" title="click to collapse or expand..."> more... </a>
 <div id="label159" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">coverpage_text_color</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: #000000</span>  <a id='label160' href="javascript:ContentClick('label161', 'label160');" onmouseover="ContentPreview('label161');" onmouseout="ContentUnpreview('label161');" title="click to collapse or expand..."> more... </a>
 <div id="label161" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">coverpage_title</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: {default}</span>  <a id='label162' href="javascript:ContentClick('label163', 'label162');" onmouseover="ContentPreview('label163');" onmouseout="ContentUnpreview('label163');" title="click to collapse or expand..."> more... </a>
 <div id="label163" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">coverpage_top_image</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: </span>  <a id='label164' href="javascript:ContentClick('label165', 'label164');" onmouseover="ContentPreview('label165');" onmouseout="ContentUnpreview('label165');" title="click to collapse or expand..."> more... </a>
 <div id="label165" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">coverpage_top_image_position</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [right, center, left]</span>  <span class="li-normal">default: center</span>  <a id='label166' href="javascript:ContentClick('label167', 'label166');" onmouseover="ContentPreview('label167');" onmouseout="ContentUnpreview('label167');" title="click to collapse or expand..."> more... </a>
 <div id="label167" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">dev_type</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [FortiSandbox, FortiWeb, Fabric, Syslog, FortiCache, FortiAuthenticator, FortiMail, FortiProxy, FortiManager, FortiNAC, FortiAnalyzer, FortiClient, FortiDDoS, FortiGate, FortiFirewall]</span>  <span class="li-normal">default: FortiGate</span>  <a id='label168' href="javascript:ContentClick('label169', 'label168');" onmouseover="ContentPreview('label169');" onmouseout="ContentUnpreview('label169');" title="click to collapse or expand..."> more... </a>
 <div id="label169" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">folder_id</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 0</span>  <a id='label170' href="javascript:ContentClick('label171', 'label170');" onmouseover="ContentPreview('label171');" onmouseout="ContentUnpreview('label171');" title="click to collapse or expand..."> more... </a>
 <div id="label171" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">font_color</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: #000000</span>  <a id='label172' href="javascript:ContentClick('label173', 'label172');" onmouseover="ContentPreview('label173');" onmouseout="ContentUnpreview('label173');" title="click to collapse or expand..."> more... </a>
 <div id="label173" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">font_family</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: "Open Sans"</span>  <a id='label174' href="javascript:ContentClick('label175', 'label174');" onmouseover="ContentPreview('label175');" onmouseout="ContentUnpreview('label175');" title="click to collapse or expand..."> more... </a>
 <div id="label175" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">font_size</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 12</span>  <a id='label176' href="javascript:ContentClick('label177', 'label176');" onmouseover="ContentPreview('label177');" onmouseout="ContentUnpreview('label177');" title="click to collapse or expand..."> more... </a>
 <div id="label177" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">font_type</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [bold-italic, bold, undefined, italic, normal]</span>  <span class="li-normal">default: normal</span>  <a id='label178' href="javascript:ContentClick('label179', 'label178');" onmouseover="ContentPreview('label179');" onmouseout="ContentUnpreview('label179');" title="click to collapse or expand..."> more... </a>
 <div id="label179" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">footer_bgcolor</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: #FFFFFF</span>  <a id='label180' href="javascript:ContentClick('label181', 'label180');" onmouseover="ContentPreview('label181');" onmouseout="ContentUnpreview('label181');" title="click to collapse or expand..."> more... </a>
 <div id="label181" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">header_bgcolor</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: #FFFFFF</span>  <a id='label182' href="javascript:ContentClick('label183', 'label182');" onmouseover="ContentPreview('label183');" onmouseout="ContentUnpreview('label183');" title="click to collapse or expand..."> more... </a>
 <div id="label183" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">hide_report_title</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 0</span>  <a id='label184' href="javascript:ContentClick('label185', 'label184');" onmouseover="ContentPreview('label185');" onmouseout="ContentUnpreview('label185');" title="click to collapse or expand..."> more... </a>
 <div id="label185" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">hide_rowid</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 0</span>  <a id='label186' href="javascript:ContentClick('label187', 'label186');" onmouseover="ContentPreview('label187');" onmouseout="ContentUnpreview('label187');" title="click to collapse or expand..."> more... </a>
 <div id="label187" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">include_empty_charts</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: enable</span>  <a id='label188' href="javascript:ContentClick('label189', 'label188');" onmouseover="ContentPreview('label189');" onmouseout="ContentUnpreview('label189');" title="click to collapse or expand..."> more... </a>
 <div id="label189" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">is_template</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label190' href="javascript:ContentClick('label191', 'label190');" onmouseover="ContentPreview('label191');" onmouseout="ContentUnpreview('label191');" title="click to collapse or expand..."> more... </a>
 <div id="label191" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">left_margin</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 6</span>  <a id='label192' href="javascript:ContentClick('label193', 'label192');" onmouseover="ContentPreview('label193');" onmouseout="ContentUnpreview('label193');" title="click to collapse or expand..."> more... </a>
 <div id="label193" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">protected</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label194' href="javascript:ContentClick('label195', 'label194');" onmouseover="ContentPreview('label195');" onmouseout="ContentUnpreview('label195');" title="click to collapse or expand..."> more... </a>
 <div id="label195" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">report_tag</span> <span class="li-normal">type: str</span>  <span class="li-normal">default: </span>  <a id='label196' href="javascript:ContentClick('label197', 'label196');" onmouseover="ContentPreview('label197');" onmouseout="ContentUnpreview('label197');" title="click to collapse or expand..."> more... </a>
 <div id="label197" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">right_margin</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 6</span>  <a id='label198' href="javascript:ContentClick('label199', 'label198');" onmouseover="ContentPreview('label199');" onmouseout="ContentUnpreview('label199');" title="click to collapse or expand..."> more... </a>
 <div id="label199" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">folders</span> reference: /sql-report/layout/folders <span class="li-normal">type: list of dict</span>
 <a id='label200' href="javascript:ContentClick('label201', 'label200');" onmouseover="ContentPreview('label201');" onmouseout="ContentUnpreview('label201');" title="click to collapse or expand..."> more... </a>
 <div id="label201" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.0.0 -> latest</code></p>
 </div>
 <ul class="ul-self">
 <li><span class="li-head">folder_id</span> <span class="li-normal">type: int</span>  <a id='label202' href="javascript:ContentClick('label203', 'label202');" onmouseover="ContentPreview('label203');" onmouseout="ContentUnpreview('label203');" title="click to collapse or expand..."> more... </a>
 <div id="label203" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.0.0 -> latest</code></p>
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
      - name: Config layout.
        fortinet.fortianalyzer.faz_report_config_layout:
          # bypass_validation: false
          # rc_succeeded: [0, -2, -3, ...]
          # rc_failed: [-2, -3, ...]
          adom: <your own value>
          state: present # <value in [present, absent]>
          report_config_layout:
            layout_id: 0 # Required variable, integer
            # body: <value of string>
            # component:
            #   - component_id: <value of integer>
            #     type: <value in [graphic, column-break, macro, ...]>
            #     variable:
            #       - not: <value in [enable, disable]>
            #         var: <value of string>
            #         var_value: <value of string>
            #         description: <value of string>
            #         drilldown_flag: <value in [enable, disable]>
            #         status: <value in [enable, disable]>
            #         var_expression: <value of string>
            #         var_type: <value in [ip, integer, string, ...]>
            #         view_mask: <value of integer>
            #     alignment: <value of integer>
            #     bg_color: <value of string>
            #     category: <value of string>
            #     chart: <value of string>
            #     chart_option: <value in [calc-average, none]>
            #     column: <value in [1, 2]>
            #     customized: <value of integer>
            #     device_mode: <value in [variable, specify]>
            #     devices: <value of string>
            #     drill_down_report: <value in [enable, disable]>
            #     filter_logic: <value in [all, any]>
            #     filter_mode: <value in [override, inherit]>
            #     font_color: <value of string>
            #     font_family: <value of string>
            #     font_size: <value of integer>
            #     font_type: <value in [bold-italic, bold, undefined, ...]>
            #     graphic: <value of string>
            #     include_other: <value in [enable, disable]>
            #     ldap_query: <value in [auto, enable, disable]>
            #     ldap_server: <value of string>
            #     ldap_user_case_change: <value in [upper, lower, disable]>
            #     left_margin: <value of integer>
            #     macro: <value of string>
            #     not_vdom: <value in [enable, disable]>
            #     period_end: <value of dict>
            #     period_last_n: <value of integer>
            #     period_mode: <value in [variable, specify]>
            #     period_opt: <value in [faz, dev]>
            #     period_start: <value of dict>
            #     right_margin: <value of integer>
            #     table_color: <value in [default, blue, green, ...]>
            #     text: <value of string>
            #     time_period: <value in [last-n-weeks, last-month, last-7-days, ...]>
            #     title: <value of string>
            #     vdom: <value of string>
            #     week_start: <value in [wed, sun, fri, ...]>
            #     width: <value of integer>
            # description: <value of string>
            # footer:
            #   - footer_id: <value of integer>
            #     type: <value in [text, graphic, minicover]>
            #     graphic: <value of string>
            #     text: <value of string>
            # header:
            #   - header_id: <value of integer>
            #     type: <value in [text, graphic, minicover]>
            #     graphic: <value of string>
            #     text: <value of string>
            # language: <value of string>
            # subtitle: <value of string>
            # title: <value of string>
            # alignment: <value in [right, center, left]>
            # bg_color: <value of string>
            # category: <value of string>
            # chart_heading_level: <value of integer>
            # chart_info_display: <value in [enable, disable]>
            # coverpage_background_image: <value of string>
            # coverpage_bottom_image: <value of string>
            # coverpage_custom_text1: <value of string>
            # coverpage_custom_text2: <value of string>
            # coverpage_enable_create_time: <value in [enable, disable]>
            # coverpage_enable_time_period: <value in [enable, disable]>
            # coverpage_footer_bgcolor: <value of string>
            # coverpage_footer_left: <value of string>
            # coverpage_footer_right: <value of string>
            # coverpage_text_color: <value of string>
            # coverpage_title: <value of string>
            # coverpage_top_image: <value of string>
            # coverpage_top_image_position: <value in [right, center, left]>
            # dev_type: <value in [FortiSandbox, FortiWeb, Fabric, ...]>
            # folder_id: <value of integer>
            # font_color: <value of string>
            # font_family: <value of string>
            # font_size: <value of integer>
            # font_type: <value in [bold-italic, bold, undefined, ...]>
            # footer_bgcolor: <value of string>
            # header_bgcolor: <value of string>
            # hide_report_title: <value of integer>
            # hide_rowid: <value of integer>
            # include_empty_charts: <value in [enable, disable]>
            # is_template: <value in [enable, disable]>
            # left_margin: <value of integer>
            # protected: <value in [enable, disable]>
            # report_tag: <value of string>
            # right_margin: <value of integer>
            # folders:
            #   - folder_id: <value of integer>
  


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