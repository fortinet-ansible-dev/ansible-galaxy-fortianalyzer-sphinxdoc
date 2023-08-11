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