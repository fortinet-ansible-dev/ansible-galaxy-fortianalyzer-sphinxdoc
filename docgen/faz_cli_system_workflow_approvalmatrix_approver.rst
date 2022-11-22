:source: faz_cli_system_workflow_approvalmatrix_approver.py

:orphan:

.. _faz_cli_system_workflow_approvalmatrix_approver:

faz_cli_system_workflow_approvalmatrix_approver -- Approver.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

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

- ansible>=2.9.0



FortiAnalyzer Version Compatibility
------------------------------------
.. raw:: html

 <br>
 <table>
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">6.2.1 </code></td>
 <td><code class="docutils literal notranslate">6.2.2 </code></td>
 <td><code class="docutils literal notranslate">6.2.3 </code></td>
 <td><code class="docutils literal notranslate">6.2.5 </code></td>
 <td><code class="docutils literal notranslate">6.2.6 </code></td>
 <td><code class="docutils literal notranslate">6.4.1 </code></td>
 <td><code class="docutils literal notranslate">6.4.2 </code></td>
 <td><code class="docutils literal notranslate">6.4.3 </code></td>
 <td><code class="docutils literal notranslate">6.4.4 </code></td>
 <td><code class="docutils literal notranslate">6.4.5 </code></td>
 <td><code class="docutils literal notranslate">7.0.0 </code></td>
 </tr>
 <tr>
 <td>cli_system_workflow_approvalmatrix_approver</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 <p>



Parameters
----------

.. raw:: html

 <ul>
 <li><span class="li-head">enable_log</span> - Enable/Disable logging for task <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal"> default: False</span> </li>
 <li><span class="li-head">proposed_method</span> - The overridden method for the underlying Json RPC request <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal"> choices: set, update, add</span> </li>
 <li><span class="li-head">bypass_validation</span> - Only set to True when module schema diffs with FortiAnalyzer API structure, module continues to execute without validating parameters <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal"> default: False</span> </li>
 <li><span class="li-head">rc_succeeded</span> - The rc codes list with which the conditions to succeed will be overriden <span class="li-normal">type: list</span> <span class="li-required">required: false</span> </li>
 <li><span class="li-head">rc_failed</span> - The rc codes list with which the conditions to fail will be overriden <span class="li-normal">type: list</span> <span class="li-required">required: false</span> </li>
 <li><span class="li-head">state</span> - The directive to create, update or delete an object <span class="li-normal">type: str</span> <span class="li-required">required: true</span> <span class="li-normal"> choices: present, absent</span> </li>
 <li><span class="li-head">approval-matrix</span> - The parameter in requested url <span class="li-normal">type: str</span> <span class="li-required">required: true</span> </li>
 <li><span class="li-head">cli_system_workflow_approvalmatrix_approver</span> - Approver. <span class="li-normal">type: dict</span></li>
 <ul class="ul-self">
 <li><span class="li-head">member</span> - Member of approver. <span class="li-normal">type: str</span>  <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">6.2.1 </code></td>
 <td><code class="docutils literal notranslate">6.2.2 </code></td>
 <td><code class="docutils literal notranslate">6.2.3 </code></td>
 <td><code class="docutils literal notranslate">6.2.5 </code></td>
 <td><code class="docutils literal notranslate">6.2.6 </code></td>
 <td><code class="docutils literal notranslate">6.4.1 </code></td>
 <td><code class="docutils literal notranslate">6.4.2 </code></td>
 <td><code class="docutils literal notranslate">6.4.3 </code></td>
 <td><code class="docutils literal notranslate">6.4.4 </code></td>
 <td><code class="docutils literal notranslate">6.4.5 </code></td>
 <td><code class="docutils literal notranslate">7.0.0 </code></td>
 <td><code class="docutils literal notranslate">7.2.0 </code></td>
 </tr>
 <tr>
 <td>member</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>False</td>
 </tr>
 </table>
 </div>
 </li>
 <li><span class="li-head">seq_num</span> - Entry number. <span class="li-normal">type: int</span>  <span class="li-normal">default: 0</span>  <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">6.2.1 </code></td>
 <td><code class="docutils literal notranslate">6.2.2 </code></td>
 <td><code class="docutils literal notranslate">6.2.3 </code></td>
 <td><code class="docutils literal notranslate">6.2.5 </code></td>
 <td><code class="docutils literal notranslate">6.2.6 </code></td>
 <td><code class="docutils literal notranslate">6.4.1 </code></td>
 <td><code class="docutils literal notranslate">6.4.2 </code></td>
 <td><code class="docutils literal notranslate">6.4.3 </code></td>
 <td><code class="docutils literal notranslate">6.4.4 </code></td>
 <td><code class="docutils literal notranslate">6.4.5 </code></td>
 <td><code class="docutils literal notranslate">7.0.0 </code></td>
 <td><code class="docutils literal notranslate">7.2.0 </code></td>
 </tr>
 <tr>
 <td>seq_num</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>True</td>
 <td>False</td>
 </tr>
 </table>
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

 - collections:
   - fortinet.fortianalyzer
   connection: httpapi
   hosts: fortianalyzer-inventory
   tasks:
   - faz_cli_system_workflow_approvalmatrix_approver:
       approval-matrix: root
       cli_system_workflow_approvalmatrix_approver:
         member: foomember
         seq_num: 1
       state: present
     name: Approver.
   vars:
     ansible_httpapi_port: 443
     ansible_httpapi_use_ssl: true
     ansible_httpapi_validate_certs: false



Return Values
-------------


Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:


.. raw:: html

 <ul>
 <li> <span class="li-return">request_url</span> - The full url requested <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: /sys/login/user</span></li>
 <li> <span class="li-return">response_code</span> - The status of api request <span class="li-normal">returned: always</span> <span class="li-normal">type: int</span> <span class="li-normal">sample: 0</span></li>
 <li> <span class="li-return">response_message</span> - The descriptive message of the api response <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: OK</li>
 <li> <span class="li-return">response_data</span> - The data body of the api response <span class="li-normal">returned: optional</span> <span class="li-normal">type: list or dict</span></li>
 </ul>





Status
------

- This module is not guaranteed to have a backwards compatible interface.


Authors
-------

- Link Zheng (@chillancezen)
- Jie Xue (@JieX19)
- Frank Shen (@fshen01)
- Hongbin Lu (@fgtdev-hblu)


.. hint::

    If you notice any issues in this documentation, you can create a pull request to improve it.



