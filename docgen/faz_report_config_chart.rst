:source: faz_report_config_chart.py

:orphan:

.. _faz_report_config_chart:

faz_report_config_chart -- Config chart.
++++++++++++++++++++++++++++++++++++++++

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
 <li><span class="li-head">report_config_chart</span> Config chart. <span class="li-normal">type: dict</span></li>
 <ul class="ul-self">
 <li><span class="li-head">category</span> <span class="li-normal">type: str</span>  <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">description</span> <span class="li-normal">type: str</span>  <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">dev_type</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [FortiSandbox, FortiWeb, Fabric, Syslog, FortiCache, FortiAuthenticator, FortiMail, FortiProxy, FortiManager, FortiNAC, FortiAnalyzer, FortiClient, FortiDDoS, FortiGate, FortiFirewall]</span>  <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">disp_name</span> <span class="li-normal">type: str</span>  <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">drill_down_table</span> reference: /report/adom/&lt;adom-name&gt;/config/chart/&lt;chart_name&gt;/drill-down-table <span class="li-normal">type: list of dict</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 <ul class="ul-self">
 <li><span class="li-head">chart</span> <span class="li-normal">type: str</span>  <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">flag</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">table_id</span> <span class="li-normal">type: int</span>  <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">chart_group</span> <span class="li-normal">type: str</span>  <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">page_break_after</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">show_title</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 </ul>
 </li>
 <li><span class="li-head">name</span> <span class="li-normal">type: str</span>  <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">table_columns</span> reference: /report/adom/&lt;adom-name&gt;/config/chart/&lt;chart_name&gt;/table-columns <span class="li-normal">type: list of dict</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 <ul class="ul-self">
 <li><span class="li-head">data_type</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [aggregate, raw, drilldown]</span>  <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">header</span> <span class="li-normal">type: str</span>  <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">id</span> <span class="li-normal">type: int</span>  <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">column_attr</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [app-id, email-recver, timespan, obf-url, cal-percent, vuln, bandwidth, dev-type, severity, percent, trend, attack, html, ipsec-tunnel, web-cat, ip-country, email-sender, search, virus, user, state-icon, count, none, dst-country, url, appcat, time, kbps]</span>  <span class="li-normal">default: none</span>  <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">column_graph_type</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [none, bar, line-down, line-up]</span>  <span class="li-normal">default: none</span>  <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">column_num</span> <span class="li-normal">type: int</span>  <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">column_span</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 1</span>  <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">column_width</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 0</span>  <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">data_binding</span> <span class="li-normal">type: str</span>  <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">data_top</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 3</span>  <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">legend</span> <span class="li-normal">type: str</span>  <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 </ul>
 </li>
 <li><span class="li-head">variable_template</span> reference: /report/adom/&lt;adom-name&gt;/config/chart/&lt;chart_name&gt;/variable-template <span class="li-normal">type: list of dict</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> latest</code></p>
 </div>
 <ul class="ul-self">
 <li><span class="li-head">not</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">var</span> <span class="li-normal">type: str</span>  <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">var_value</span> <span class="li-normal">type: str</span>  <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.1 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">description</span> <span class="li-normal">type: str</span>  <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">drilldown_flag</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">status</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">var_expression</span> <span class="li-normal">type: str</span>  <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">var_type</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [ip, integer, string, datetime]</span>  <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">view_mask</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 0</span>  <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 </ul>
 </li>
 <li><span class="li-head">chart_type</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [map, none, chord, bar, area, pie, donut, radar, table, line]</span>  <span class="li-normal">default: none</span>  <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">dataset</span> <span class="li-normal">type: str</span>  <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">drill_down_agg</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">drill_down_desc</span> <span class="li-normal">type: str</span>  <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">drill_down_title</span> <span class="li-normal">type: str</span>  <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">favorite</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">hidden</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">include_other</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: enable</span>  <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">line_subtype</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [back-to-back, stacked, basic]</span>  <span class="li-normal">default: stacked</span>  <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">order_by</span> <span class="li-normal">type: str</span>  <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">order_desc</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">protected</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">resolve_hostname</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">resolve_hostname_mode</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [variable, specify]</span>  <span class="li-normal">default: variable</span>  <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">scale</span> <span class="li-normal">type: int</span>  <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">show_table</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">x_axis_data_binding</span> <span class="li-normal">type: str</span>  <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">x_axis_data_top</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 6</span>  <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">x_axis_include_other</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">x_axis_label</span> <span class="li-normal">type: str</span>  <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">y_axis_data_binding</span> <span class="li-normal">type: str</span>  <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">y_axis_group</span> <span class="li-normal">type: str</span>  <span class="li-normal">choices: [enable, disable]</span>  <span class="li-normal">default: disable</span>  <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">y_axis_group_by</span> <span class="li-normal">type: str</span>  <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">y_axis_group_top</span> <span class="li-normal">type: int</span>  <span class="li-normal">default: 3</span>  <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">y_axis_label</span> <span class="li-normal">type: str</span>  <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">y2_axis_data_binding</span> <span class="li-normal">type: str</span>  <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">y2_axis_label</span> <span class="li-normal">type: str</span>  <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.2.2 -> v6.2.13</code></p>
 </div>
 </li>
 <li><span class="li-head">tags</span> <span class="li-normal">type: str</span>  <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v6.4.3 -> v7.4.2</code></p>
 </div>
 </li>
 <li><span class="li-head">chart_style</span> <span class="li-normal">type: str</span>  <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
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
    hosts: fortianalyzers
    connection: httpapi
    gather_facts: false
    vars:
      ansible_network_os: fortinet.fortianalyzer.fortianalyzer
      ansible_httpapi_port: 443
      ansible_httpapi_use_ssl: true
      ansible_httpapi_validate_certs: false
    tasks:
      - name: Config chart.
        fortinet.fortianalyzer.faz_report_config_chart:
          # bypass_validation: false
          # rc_succeeded: [0, -2, -3, ...]
          # rc_failed: [-2, -3, ...]
          adom: <your own value>
          state: present # <value in [present, absent]>
          report_config_chart:
            name: "your value" # Required variable, string
            # category: <value of string>
            # description: <value of string>
            # dev_type: <value in [FortiSandbox, FortiWeb, Fabric, ...]>
            # disp_name: <value of string>
            # drill_down_table:
            #   - chart: <value of string>
            #     flag: <value in [enable, disable]>
            #     table_id: <value of integer>
            #     chart_group: <value of string>
            #     page_break_after: <value in [enable, disable]>
            #     show_title: <value in [enable, disable]>
            # table_columns:
            #   - data_type: <value in [aggregate, raw, drilldown]>
            #     header: <value of string>
            #     id: <value of integer>
            #     column_attr: <value in [app-id, email-recver, timespan, ...]>
            #     column_graph_type: <value in [none, bar, line-down, ...]>
            #     column_num: <value of integer>
            #     column_span: <value of integer>
            #     column_width: <value of integer>
            #     data_binding: <value of string>
            #     data_top: <value of integer>
            #     legend: <value of string>
            # variable_template:
            #   - not: <value in [enable, disable]>
            #     var: <value of string>
            #     var_value: <value of string>
            #     description: <value of string>
            #     drilldown_flag: <value in [enable, disable]>
            #     status: <value in [enable, disable]>
            #     var_expression: <value of string>
            #     var_type: <value in [ip, integer, string, ...]>
            #     view_mask: <value of integer>
            # chart_type: <value in [map, none, chord, ...]>
            # dataset: <value of string>
            # drill_down_agg: <value in [enable, disable]>
            # drill_down_desc: <value of string>
            # drill_down_title: <value of string>
            # favorite: <value in [enable, disable]>
            # hidden: <value in [enable, disable]>
            # include_other: <value in [enable, disable]>
            # line_subtype: <value in [back-to-back, stacked, basic]>
            # order_by: <value of string>
            # order_desc: <value in [enable, disable]>
            # protected: <value in [enable, disable]>
            # resolve_hostname: <value in [enable, disable]>
            # resolve_hostname_mode: <value in [variable, specify]>
            # scale: <value of integer>
            # show_table: <value in [enable, disable]>
            # x_axis_data_binding: <value of string>
            # x_axis_data_top: <value of integer>
            # x_axis_include_other: <value in [enable, disable]>
            # x_axis_label: <value of string>
            # y_axis_data_binding: <value of string>
            # y_axis_group: <value in [enable, disable]>
            # y_axis_group_by: <value of string>
            # y_axis_group_top: <value of integer>
            # y_axis_label: <value of string>
            # y2_axis_data_binding: <value of string>
            # y2_axis_label: <value of string>
            # tags: <value of string>
            # chart_style: <value of string>
  


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