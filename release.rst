Release Notes
==============================

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


Release Galaxy 1.3.1
~~~~~~~~~~~~~~~~~~~~~~

Release Target
---------------

FortiAnalyzer version: ``v6.2``, ``v6.4``, ``v7.0``, ``v7.2`` and ``v7.4``

Bugfixes
--------

- Require ansible core to be at least 2.13.0


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
