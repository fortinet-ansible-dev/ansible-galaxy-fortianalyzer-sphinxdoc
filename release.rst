Release Notes
==============================

Release Galaxy 1.9.0
~~~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4``, ``v7.0``, ``v7.2`` and ``v7.4``

Minor Changes
-------------

- Supported FortiAnalyzer 7.6.3. 2 new modules.

Bugfixes
--------

- Added "gather_facts" to all example playbooks.
- Fixed a BUG that occurred when username/password and access token were used at the same time.

New Modules
-----------

- fortinet.fortianalyzer.faz_cli_fmupdate_fgdsetting - Cli fmupdate fgd setting
- fortinet.fortianalyzer.faz_cli_system_log_deviceselector - Cli system log device selector


|


Release Galaxy 1.8.1
~~~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4``, ``v7.0``, ``v7.2`` and ``v7.4``

Minor Changes
-------------

- Supported FortiAnalyzer 7.2.9, 7.2.10, 7.4.6, 7.6.2

Bugfixes
--------

- Corrected the mainkey of some "eventmgmt" modules.
- Modified example playbooks to support ansible-lint check.

|

Release Galaxy 1.8.0
~~~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4``, ``v7.0``, ``v7.2`` and ``v7.4``

Minor Changes
-------------

- Added 16 eventmgmt modules.
- Supported FortiAnalyzer 6.2.13, 6.4.15, 7.0.13, 7.2.8, 7.4.4, 7.4.5, 7.6.1 API schemas.

Bugfixes
--------

- Supported all sanity tests of ansible-core 2.18.0

New Modules
-----------

- fortinet.fortianalyzer.faz_eventmgmt_alerts_ack - Acknowledge alert events.
- fortinet.fortianalyzer.faz_eventmgmt_alerts_assign - Assign alert events
- fortinet.fortianalyzer.faz_eventmgmt_alerts_comment - Handle alert comments.
- fortinet.fortianalyzer.faz_eventmgmt_alerts_import - Import basic handlers.
- fortinet.fortianalyzer.faz_eventmgmt_alerts_read - Mark a specific alert event as read.
- fortinet.fortianalyzer.faz_eventmgmt_alerts_unack - Unacknowledge alert events.
- fortinet.fortianalyzer.faz_eventmgmt_basichandlers_import - Import basic handlers.
- fortinet.fortianalyzer.faz_eventmgmt_config_basichandler - Config basic-handler.
- fortinet.fortianalyzer.faz_eventmgmt_config_correlationhandler - Config correlation-handler.
- fortinet.fortianalyzer.faz_eventmgmt_config_dataselector - Config data-selector.
- fortinet.fortianalyzer.faz_eventmgmt_config_notificationprofile - Config notification-profile.
- fortinet.fortianalyzer.faz_eventmgmt_config_trigger - trigger
- fortinet.fortianalyzer.faz_eventmgmt_config_trigger_device - device
- fortinet.fortianalyzer.faz_eventmgmt_config_trigger_filter - filter
- fortinet.fortianalyzer.faz_eventmgmt_config_trigger_filter_rule - rule
- fortinet.fortianalyzer.faz_eventmgmt_correlationhandlers_import - Import correlation handlers.


Release Galaxy 1.7.0
~~~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4``, ``v7.0``, ``v7.2`` and ``v7.4``

Minor Changes
-------------

- Supported FortiAnalyzer 7.2.6, 7.2.7, 7.6.0 API schemas.
- Supported check mode for all modules except "faz_generic".
- Supported diff mode for some modules.

Bugfixes
--------

- Improved code logic, reduced redundant requests for system information.
- Improved faz_fact document.
- Improved readme document.

New Modules
-----------

- fortinet.fortianalyzer.faz_cli_system_admin_user_policyblock - Policy block write access.


Release Galaxy 1.6.0
~~~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4``, ``v7.0``, ``v7.2`` and ``v7.4``

Minor Changes
-------------

- Supported FortiAnalyzer 7.4.3 API schemas. 1 new module.
- Supported ansible-core 2.17

Bugfixes
--------

- Added more report selectors in faz_fact.
- Changed type of "schedule_valid_end" and "schedule_valid_start" in module faz_report_config_schedule from list of dict to string.

New Modules
-----------

- fortinet.fortianalyzer.faz_cli_system_log_ueba - UEBAsettings.



Release Galaxy 1.5.0
~~~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4``, ``v7.0``, ``v7.2`` and ``v7.4``

Minor Changes
-------------

- Added report serial modules.
- Supported FortiAnalyzer 7.0.12, 7.2.5.
- Added parameter version_check. If set to True, it will check whether the parameters used are supported by the corresponding version of FortiAnazlyer.

Bugfixes
--------

- Improved 10 modules to support "state:absent".
- Improved bypass_validation. If you now set bypass_validation to true, it will allow you to send parameters that are not defined in the schema.
- Improved documentation, added description for all "no description" modules.
- Improved faz_fact, it can support selectors start with "report".

New Modules
-----------

- fortinet.fortianalyzer.faz_report_config_chart - Config chart.
- fortinet.fortianalyzer.faz_report_config_chart_drilldowntable - Config drill-down-table.
- fortinet.fortianalyzer.faz_report_config_chart_tablecolumns - Config table-columns.
- fortinet.fortianalyzer.faz_report_config_chart_variabletemplate - Config variable-template.
- fortinet.fortianalyzer.faz_report_config_dataset - Config dataset.
- fortinet.fortianalyzer.faz_report_config_dataset_variable - Config variable.
- fortinet.fortianalyzer.faz_report_config_layout - Config layout.
- fortinet.fortianalyzer.faz_report_config_layout_component - Config component.
- fortinet.fortianalyzer.faz_report_config_layout_component_variable - Config variable.
- fortinet.fortianalyzer.faz_report_config_layout_footer - Config footer.
- fortinet.fortianalyzer.faz_report_config_layout_header - Config header.
- fortinet.fortianalyzer.faz_report_config_layoutfolder - Config layout-folder.
- fortinet.fortianalyzer.faz_report_config_macro - Config macro.
- fortinet.fortianalyzer.faz_report_config_output - Config output.
- fortinet.fortianalyzer.faz_report_config_output_emailrecipients - Config email-recipients.
- fortinet.fortianalyzer.faz_report_config_schedule - Config schedule.
- fortinet.fortianalyzer.faz_report_config_schedule_addressfilter - Config address-filter.
- fortinet.fortianalyzer.faz_report_config_schedule_devices - Config devices.
- fortinet.fortianalyzer.faz_report_config_schedule_filter - Config filter.
- fortinet.fortianalyzer.faz_report_config_schedule_reportlayout - Config report-layout.
- fortinet.fortianalyzer.faz_report_configfile_import - Import report config files.
- fortinet.fortianalyzer.faz_report_graphfile - Handle graph files.
- fortinet.fortianalyzer.faz_report_graphfile_delete - Handle graph files.
- fortinet.fortianalyzer.faz_report_reports_data_delete - Handle generated reports.
- fortinet.fortianalyzer.faz_report_run - Start report requests.
- fortinet.fortianalyzer.faz_report_run_delete - Handle report requests by task ID.
- fortinet.fortianalyzer.faz_report_template_delete - Delete report template language package files.
- fortinet.fortianalyzer.faz_report_template_import - Import report templates.
- fortinet.fortianalyzer.faz_report_template_install - Install report template language packages from files.



Release Galaxy 1.4.0
~~~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4``, ``v7.0``, ``v7.2`` and ``v7.4``

Minor Changes
-------------

- Added deprecated warning to invalid argument name, please change the invalid argument name such as "var-name", "var name" to "var_name".
- Changed minimum required ansible-core version to 2.15.0
- Supported FortiAnalyzer 6.4.14, 7.0.11, 7.4.2

Bugfixes
--------

- Changed "revision" to "v_range" to reduce the size of the code.
- Improved the logic of plugin code.
- Renamed the input argument "message" in "faz_sys_reboot" to "faz_message".

New Modules
-----------

- fortinet.fortianalyzer.faz_cli_system_admin_profile_writepasswdprofiles - Profile list.
- fortinet.fortianalyzer.faz_cli_system_admin_profile_writepasswduserlist - User list.



Release Galaxy 1.3.2
~~~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4``, ``v7.0``, ``v7.2`` and ``v7.4``

Bugfixes
--------

- Added missing enum values for some arguments.
- Improve logic to decide whether the local data and remote FortiAnalyzer are
  the same.
- Require ansible core to be at least 2.14.0
- Support FortiAnalyzer 7.0.10



Release Galaxy 1.3.1
~~~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4``, ``v7.0``, ``v7.2`` and ``v7.4``

Bugfixes
--------

- Require ansible core to be at least 2.13.0



Release Galaxy 1.3.0
~~~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4``, ``v7.0``, ``v7.2`` and ``v7.4``


Minor Changes
-------------

- Add 4 new modules.
- Add module digest page in the document.
- Support newest patches from v6.2 to v7.4

Bugfixes
--------

- Fixed the bug that would report an error when providing access_token and username/password at the same time.
- Improve code robustness.

New Modules
-----------

- fortinet.fortianalyzer.faz_cli_system_csf - Add this device to a Security Fabric or set up a new Security Fabric on this device.
- fortinet.fortianalyzer.faz_cli_system_csf_fabricconnector - Fabric connector configuration.
- fortinet.fortianalyzer.faz_cli_system_csf_trustedlist - Pre-authorized and blocked security fabric nodes.
- fortinet.fortianalyzer.faz_cli_system_log_pcapfile - Log pcap-file settings.



Release Galaxy 1.2.0
~~~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4``, ``v7.0``, ``v7.2`` and ``v7.4``

Minor Changes
-------------

- Support fortianalyzer cloud.
- Support IAM access token login method.
- Support Fortianalyze v7.4, 1 new modules, faz_cli_system_socfabric_trustedlist.



Release Galaxy 1.1.0
~~~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4``, ``v7.0`` and ``v7.2``

Minor Changes
-------------

- Support newest versions in ``v6.2``, ``v6.4``, ``v7.0`` and ``v7.2``.
- Fixed Many sanity test warnings and errors.
- faz_fact and faz_rename support more URLs.
- Added param log_path for every module. You can specify the place to save the log when enable_log is True.

Bug Fixes
-------------
- Fixed an issue where some selectors in faz_fact were named incorrectly.
- Fixed version_added in the document. The value of this parameter is the version each module first supported in the FortiAnalyzer Ansible Collection.



Release Galaxy 1.0.3
~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4``, ``v7.0`` and ``v7.2``

Major Changes
-------------

- Deprecate default genrated README in plugin directory.
- Update meta/runtime.yaml requirement.
- Update python and ansible requirement in top-level README.



Release Galaxy 1.0.2
~~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4``, ``v7.0`` and ``v7.2``

Major Changes
--------------

- Fixed Many sanity test warnings and errors.
- Support API schema 7.2.0, 25 new APIs, 8 new modules.
- Supported Ansible Changelogs.



Release Galaxy 1.0.1
~~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4`` and ``v7.0``

Bugfix
------------

- fix enable_log option setting issue with new netcommon plugin.
- fix some document typos in sphinx and module.
- fix readthedoc build requirement.


Release Galaxy 1.0.0
~~~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4`` and ``v7.0``

Module Category
----------------

+-------------------------------+--------------------------+---------------------------------+
| Module Category               | Supported JPRC methods   | Location                        |
+===============================+==========================+=================================+
| Object Oriented Modules       | add/update(set)/delete   | `ref <modules.html>`__          |
+-------------------------------+--------------------------+---------------------------------+
| Facts Gathering Modules       | get                      | `ref <fact.html>`__             |
+-------------------------------+--------------------------+---------------------------------+
| Daemon Modules                | exec                     | `ref <daemon_modules.html>`__   |
+-------------------------------+--------------------------+---------------------------------+
| Generic Modules               | (all methods)            | `ref <generic.html>`__          |
+-------------------------------+--------------------------+---------------------------------+

Features
------------

-  Full FortiAnalyzer JRPC URLs coverage (more than 170 modules).
-  Flexible error handling mechanism.
