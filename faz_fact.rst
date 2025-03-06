:source: faz_fact.py

:orphan:

.. _faz_fact:

faz_fact -- Gather FortiAnalyzer Facts.
+++++++++++++++++++++++++++++++++++++++

.. versionadded:: 1.0.0


.. contents::
   :local:
   :depth: 1


Synopsis
--------

- This module is able to configure a FortiAnalyzer device.
- Examples include all parameters and values need to be adjusted to data sources before usage.
- Tested with FortiAnalyzer v6.x and v7.x.


Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15.0


Parameters
----------

.. raw:: html

  <ul>
    <li><span class="li-head">access_token</span> The token to access FortiAnalyzer without using ansible_username and ansible_password. <span class="li-normal">type: str</span></li>
    <li><span class="li-head">enable_log</span> Enable/Disable logging for task <span class="li-normal">type: bool</span> <span class="li-normal"> default: False</span> </li>
    <li><span class="li-head">forticloud_access_token</span> Access token of forticloud analyzer API users. <span class="li-normal">type: str</span> </li>
    <li><span class="li-head">log_path</span> The path to save log. Used if enable_log is true. Please use absolute path instead of relative path. If the log_path setting is incorrect, the log will be saved in /tmp/fortianalyzer.ansible.log<span class="li-normal">type: str</span> <span class="li-normal"> default: "/tmp/fortianalyzer.ansible.log"</span> </li>
    <li><span class="li-head">version_check</span> If set to True, it will check whether the parameters used are supported by the corresponding version of FortiAnazlyer locally based on FNDN data. A warning will be returned in version_check_warning if there is a mismatch. This warning is only a suggestion and may not be accurate. <span class="li-normal">type: bool</span> <span class="li-normal"> default: True</span> </li>
    <li><span class="li-head">rc_succeeded</span> The rc codes list with which the conditions to succeed will be overriden <span class="li-normal">type: list</span> </li>
    <li><span class="li-head">rc_failed</span> The rc codes list with which the conditions to fail will be overriden <span class="li-normal">type: list</span> </li>
    <li><span class="li-head">facts</span> Gathering fortianalyzer facts. <span class="li-normal">type: dict</span></li>
    <ul class="ul-self">
      <li><span class="li-head">fields</span> Limit the output by returning only the attributes specified in the string array.  <span class="li-normal">type: list</span></li>
      <li><span class="li-head">filter</span> Filter the result according to a set of criteria. <span class="li-normal">type: list</span></li>
      <li><span class="li-head">option</span> Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. See more details in FNDN API documents. <span class="li-normal">type: str</span></li>
      <li><span class="li-head">sortings</span> Sorting rules list: items are returned in ascending(1) or descending(-1) order of fields in the list. <span class="li-normal">type: list of dict</span></li>
      <li><span class="li-head">selector</span> Selector of the retrieved fortianalyzer facts <span class="li-normal">type: str</span> <span class="li-required">choices:</span></li>
      <li style="list-style: none;">
      <section class="accordion">
        <input type="checkbox" name="collapse" id="handle2">
        <h2 class="handle"><label for="handle2"><u>Show full selector list...</u></label></h2>
        <div class="content">
          <ul class="ul-self">
              <li><span class="li-required">cli_fmupdate_analyzer_virusreport</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_avips_advancedlog</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_avips_webproxy</span> - available versions:
              <span class="li-normal">6.2.1-7.4.0</span>
              </li>
              <li><span class="li-required">cli_fmupdate_customurllist</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_diskquota</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_fctservices</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_fdssetting</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_fdssetting_pushoverride</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_fdssetting_pushoverridetoclient</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_fdssetting_pushoverridetoclient_announceip</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_fdssetting_serveroverride</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_fdssetting_serveroverride_servlist</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_fdssetting_updateschedule</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_fwmsetting</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_fwmsetting_upgradetimeout</span> - available versions:
              <span class="li-normal">7.0.5-7.0.13, >= 7.2.2</span>
              </li>
              <li><span class="li-required">cli_fmupdate_multilayer</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_publicnetwork</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_serveraccesspriorities</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_serveraccesspriorities_privateserver</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_serveroverridestatus</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_service</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_webspam_fgdsetting</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_webspam_fgdsetting_serveroverride</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_webspam_fgdsetting_serveroverride_servlist</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_fmupdate_webspam_webproxy</span> - available versions:
              <span class="li-normal">6.2.1-7.4.0</span>
              </li>
              <li><span class="li-required">cli_metafields_system_admin_user</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_admin_group</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_admin_group_member</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_admin_ldap</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_admin_ldap_adom</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_admin_profile</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_admin_profile_datamaskcustomfields</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_admin_profile_writepasswdprofiles</span> - available versions:
              <span class="li-normal">>= 7.4.2</span>
              </li>
              <li><span class="li-required">cli_system_admin_profile_writepasswduserlist</span> - available versions:
              <span class="li-normal">>= 7.4.2</span>
              </li>
              <li><span class="li-required">cli_system_admin_radius</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_admin_setting</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_admin_tacacs</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_admin_user</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_admin_user_adom</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_admin_user_adomexclude</span> - available versions:
              <span class="li-normal">6.2.1-7.0.2</span>
              </li>
              <li><span class="li-required">cli_system_admin_user_dashboard</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_admin_user_dashboardtabs</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_admin_user_metadata</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_admin_user_policyblock</span> - available versions:
              <span class="li-normal">>= 7.6.0</span>
              </li>
              <li><span class="li-required">cli_system_admin_user_policypackage</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_admin_user_restrictdevvdom</span> - available versions:
              <span class="li-normal">6.2.1-6.2.3</span>
              </li>
              <li><span class="li-required">cli_system_alertconsole</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_alertemail</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_alertevent</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_alertevent_alertdestination</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_autodelete</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_autodelete_dlpfilesautodeletion</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_autodelete_logautodeletion</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_autodelete_quarantinefilesautodeletion</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_autodelete_reportautodeletion</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_backup_allsettings</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_centralmanagement</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_certificate_ca</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_certificate_crl</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_certificate_local</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_certificate_oftp</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_certificate_remote</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_certificate_ssh</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_connector</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_csf</span> - available versions:
              <span class="li-normal">>= 7.4.1</span>
              </li>
              <li><span class="li-required">cli_system_csf_fabricconnector</span> - available versions:
              <span class="li-normal">>= 7.4.1</span>
              </li>
              <li><span class="li-required">cli_system_csf_trustedlist</span> - available versions:
              <span class="li-normal">>= 7.4.1</span>
              </li>
              <li><span class="li-required">cli_system_dns</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_docker</span> - available versions:
              <span class="li-normal">6.2.1-6.2.1, >= 6.4.1</span>
              </li>
              <li><span class="li-required">cli_system_fips</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_fortiview_autocache</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_fortiview_setting</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_global</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_guiact</span> - available versions:
              <span class="li-normal">6.2.1-7.0.11, 7.2.0-7.2.4, 7.4.0-7.4.0</span>
              </li>
              <li><span class="li-required">cli_system_ha</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_ha_peer</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_ha_privatepeer</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_ha_vip</span> - available versions:
              <span class="li-normal">>= 7.0.5</span>
              </li>
              <li><span class="li-required">cli_system_interface</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_interface_ipv6</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_interface_member</span> - available versions:
              <span class="li-normal">>= 6.4.9</span>
              </li>
              <li><span class="li-required">cli_system_localinpolicy</span> - available versions:
              <span class="li-normal">>= 7.2.0</span>
              </li>
              <li><span class="li-required">cli_system_localinpolicy6</span> - available versions:
              <span class="li-normal">>= 7.2.0</span>
              </li>
              <li><span class="li-required">cli_system_locallog_disk_filter</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_locallog_disk_setting</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_locallog_fortianalyzer2_filter</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_locallog_fortianalyzer2_setting</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_locallog_fortianalyzer3_filter</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_locallog_fortianalyzer3_setting</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_locallog_fortianalyzer_filter</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_locallog_fortianalyzer_setting</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_locallog_memory_filter</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_locallog_memory_setting</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_locallog_setting</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_locallog_syslogd2_filter</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_locallog_syslogd2_setting</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_locallog_syslogd3_filter</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_locallog_syslogd3_setting</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_locallog_syslogd_filter</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_locallog_syslogd_setting</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_log_alert</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_log_devicedisable</span> - available versions:
              <span class="li-normal">>= 6.4.4</span>
              </li>
              <li><span class="li-required">cli_system_log_fospolicystats</span> - available versions:
              <span class="li-normal">>= 7.0.2</span>
              </li>
              <li><span class="li-required">cli_system_log_interfacestats</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_log_ioc</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_log_maildomain</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_log_pcapfile</span> - available versions:
              <span class="li-normal">>= 7.4.1</span>
              </li>
              <li><span class="li-required">cli_system_log_ratelimit</span> - available versions:
              <span class="li-normal">>= 6.4.8</span>
              </li>
              <li><span class="li-required">cli_system_log_ratelimit_device</span> - available versions:
              <span class="li-normal">6.4.8-7.0.2</span>
              </li>
              <li><span class="li-required">cli_system_log_ratelimit_ratelimits</span> - available versions:
              <span class="li-normal">>= 7.0.3</span>
              </li>
              <li><span class="li-required">cli_system_log_settings</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_log_settings_rollinganalyzer</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_log_settings_rollinglocal</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_log_settings_rollingregular</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_log_topology</span> - available versions:
              <span class="li-normal">6.4.7-6.4.15, >= 7.0.2</span>
              </li>
              <li><span class="li-required">cli_system_log_ueba</span> - available versions:
              <span class="li-normal">>= 7.4.3</span>
              </li>
              <li><span class="li-required">cli_system_logfetch_clientprofile</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_logfetch_clientprofile_devicefilter</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_logfetch_clientprofile_logfilter</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_logfetch_serversettings</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_logforward</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_logforward_devicefilter</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_logforward_logfieldexclusion</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_logforward_logfilter</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_logforward_logmaskingcustom</span> - available versions:
              <span class="li-normal">>= 7.0.0</span>
              </li>
              <li><span class="li-required">cli_system_logforwardservice</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_mail</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_metadata_admins</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_ntp</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_ntp_ntpserver</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_passwordpolicy</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_performance</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_report_autocache</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_report_estbrowsetime</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_report_group</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_report_group_chartalternative</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_report_group_groupby</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_report_setting</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_route</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_route6</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_saml</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_saml_fabricidp</span> - available versions:
              <span class="li-normal">6.2.1-6.2.1, >= 6.4.1</span>
              </li>
              <li><span class="li-required">cli_system_saml_serviceproviders</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_sniffer</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_snmp_community</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_snmp_community_hosts</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_snmp_community_hosts6</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_snmp_sysinfo</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_snmp_user</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_socfabric</span> - available versions:
              <span class="li-normal">>= 7.0.0</span>
              </li>
              <li><span class="li-required">cli_system_socfabric_trustedlist</span> - available versions:
              <span class="li-normal">>= 7.4.0</span>
              </li>
              <li><span class="li-required">cli_system_sql</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_sql_customindex</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_sql_customskipidx</span> - available versions:
              <span class="li-normal">6.2.1-6.2.1, >= 6.2.3</span>
              </li>
              <li><span class="li-required">cli_system_sql_tsindexfield</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_sslciphersuites</span> - available versions:
              <span class="li-normal">6.4.8-6.4.15, >= 7.0.2</span>
              </li>
              <li><span class="li-required">cli_system_status</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_syslog</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_webproxy</span> - available versions:
              <span class="li-normal">6.4.8-6.4.15, >= 7.0.3</span>
              </li>
              <li><span class="li-required">cli_system_workflow_approvalmatrix</span> - available versions:
              <span class="li-normal">6.2.1-6.2.9, 6.4.1-6.4.7, 7.0.0-7.0.2, >= 7.6.0</span>
              </li>
              <li><span class="li-required">cli_system_workflow_approvalmatrix_approver</span> - available versions:
              <span class="li-normal">6.2.1-6.2.9, 6.4.1-6.4.7, 7.0.0-7.0.2, >= 7.6.0</span>
              </li>
              <li><span class="li-required">dvmdb_adom</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">dvmdb_device</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">dvmdb_device_haslave</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">dvmdb_device_vdom</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">dvmdb_folder</span> - available versions:
              <span class="li-normal">>= 6.4.2</span>
              </li>
              <li><span class="li-required">dvmdb_group</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">eventmgmt_alertfilter</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">eventmgmt_alertincident_stats</span> - available versions:
              <span class="li-normal">>= 7.6.0</span>
              </li>
              <li><span class="li-required">eventmgmt_alertlogs</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">eventmgmt_alertlogs_count</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">eventmgmt_alerts</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">eventmgmt_alerts_count</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">eventmgmt_alerts_export</span> - available versions:
              <span class="li-normal">>= 7.0.0</span>
              </li>
              <li><span class="li-required">eventmgmt_alerts_extradetails</span> - available versions:
              <span class="li-normal">6.2.1-6.2.1, >= 6.4.1</span>
              </li>
              <li><span class="li-required">eventmgmt_basichandlers_export</span> - available versions:
              <span class="li-normal">>= 7.2.2</span>
              </li>
              <li><span class="li-required">eventmgmt_config_basichandler</span> - available versions:
              <span class="li-normal">>= 7.2.2</span>
              </li>
              <li><span class="li-required">eventmgmt_config_correlationhandler</span> - available versions:
              <span class="li-normal">>= 7.2.2</span>
              </li>
              <li><span class="li-required">eventmgmt_config_dataselector</span> - available versions:
              <span class="li-normal">>= 7.2.2</span>
              </li>
              <li><span class="li-required">eventmgmt_config_notificationprofile</span> - available versions:
              <span class="li-normal">>= 7.2.2</span>
              </li>
              <li><span class="li-required">eventmgmt_config_trigger</span> - available versions:
              <span class="li-normal">6.2.1-7.2.1</span>
              </li>
              <li><span class="li-required">eventmgmt_config_trigger_device</span> - available versions:
              <span class="li-normal">6.2.1-7.2.1</span>
              </li>
              <li><span class="li-required">eventmgmt_config_trigger_filter</span> - available versions:
              <span class="li-normal">6.2.1-7.2.1</span>
              </li>
              <li><span class="li-required">eventmgmt_config_trigger_filter_rule</span> - available versions:
              <span class="li-normal">6.2.1-7.2.1</span>
              </li>
              <li><span class="li-required">eventmgmt_correlationhandlers_export</span> - available versions:
              <span class="li-normal">>= 7.2.2</span>
              </li>
              <li><span class="li-required">fazsys_enduseravatar</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">fazsys_forticare_licinfo</span> - available versions:
              <span class="li-normal">>= 7.2.1</span>
              </li>
              <li><span class="li-required">fazsys_language_fonts_export</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">fazsys_language_fonts_list</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">fazsys_language_translationfile_export</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">fazsys_language_translationfile_list</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">fazsys_lograte_history</span> - available versions:
              <span class="li-normal">>= 7.6.0</span>
              </li>
              <li><span class="li-required">fazsys_monitor_logforwardstatus</span> - available versions:
              <span class="li-normal">>= 7.2.2</span>
              </li>
              <li><span class="li-required">fazsys_monitor_system_performance_status</span> - available versions:
              <span class="li-normal">>= 7.6.0</span>
              </li>
              <li><span class="li-required">fazsys_storageinfo</span> - available versions:
              <span class="li-normal">>= 7.6.0</span>
              </li>
              <li><span class="li-required">fazsys_storageinfohistory</span> - available versions:
              <span class="li-normal">>= 7.6.0</span>
              </li>
              <li><span class="li-required">fortiview_run</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">incidentmgmt_attachments</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">incidentmgmt_attachments_count</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">incidentmgmt_epeuhistory</span> - available versions:
              <span class="li-normal">>= 6.4.2</span>
              </li>
              <li><span class="li-required">incidentmgmt_incident_stats</span> - available versions:
              <span class="li-normal">>= 7.6.0</span>
              </li>
              <li><span class="li-required">incidentmgmt_incidents</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">incidentmgmt_incidents_count</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">ioc_license_state</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">ioc_rescan_history</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">ioc_rescan_run</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">logview_logfields</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">logview_logfiles_data</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">logview_logfiles_search</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">logview_logfiles_state</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">logview_logsearch</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">logview_logsearch_count</span> - available versions:
              <span class="li-normal">>= 7.0.1</span>
              </li>
              <li><span class="li-required">logview_logstats</span> - available versions:
              <span class="li-normal">6.2.1-6.2.1, >= 6.4.1</span>
              </li>
              <li><span class="li-required">logview_pcapfile</span> - available versions:
              <span class="li-normal">>= 7.0.3</span>
              </li>
              <li><span class="li-required">report_config_chart</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_chart_drilldowntable</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_chart_tablecolumns</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_chart_variabletemplate</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_dataset</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_dataset_variable</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_layout</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_layout_component</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_layout_component_variable</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_layout_footer</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_layout_header</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_layoutfolder</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_macro</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_output</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_output_emailrecipients</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_schedule</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_schedule_addressfilter</span> - available versions:
              <span class="li-normal">>= 6.4.3</span>
              </li>
              <li><span class="li-required">report_config_schedule_devices</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_schedule_filter</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_config_schedule_reportlayout</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_graphfile</span> - available versions:
              <span class="li-normal">>= 7.2.2</span>
              </li>
              <li><span class="li-required">report_graphfile_data</span> - available versions:
              <span class="li-normal">>= 7.2.2</span>
              </li>
              <li><span class="li-required">report_graphfile_list</span> - available versions:
              <span class="li-normal">>= 7.2.2</span>
              </li>
              <li><span class="li-required">report_reports_data</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_reports_state</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_run</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_template_export</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_template_language</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">report_template_list</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">soar_alert_indicator</span> - available versions:
              <span class="li-normal">>= 7.6.0</span>
              </li>
              <li><span class="li-required">soar_config_connectors</span> - available versions:
              <span class="li-normal">>= 6.4.2</span>
              </li>
              <li><span class="li-required">soar_config_playbooks</span> - available versions:
              <span class="li-normal">>= 6.4.2</span>
              </li>
              <li><span class="li-required">soar_fosconnector_automationrules</span> - available versions:
              <span class="li-normal">>= 6.4.2</span>
              </li>
              <li><span class="li-required">soar_incident_indicator</span> - available versions:
              <span class="li-normal">>= 7.6.0</span>
              </li>
              <li><span class="li-required">soar_indicator</span> - available versions:
              <span class="li-normal">>= 7.6.0</span>
              </li>
              <li><span class="li-required">soar_indicator_enrichment</span> - available versions:
              <span class="li-normal">>= 7.6.0</span>
              </li>
              <li><span class="li-required">soar_playbook_export</span> - available versions:
              <span class="li-normal">>= 7.0.0</span>
              </li>
              <li><span class="li-required">soar_playbook_monitor</span> - available versions:
              <span class="li-normal">6.4.2-7.2.1, 7.6.0-7.6.1</span>
              </li>
              <li><span class="li-required">soar_playbook_run</span> - available versions:
              <span class="li-normal">>= 6.4.2</span>
              </li>
              <li><span class="li-required">soar_playbook_runlog</span> - available versions:
              <span class="li-normal">>= 7.6.0</span>
              </li>
              <li><span class="li-required">soar_subnet_export</span> - available versions:
              <span class="li-normal">>= 7.0.0</span>
              </li>
              <li><span class="li-required">soar_task_monitor</span> - available versions:
              <span class="li-normal">6.4.2-7.4.6, >= 7.6.2</span>
              </li>
              <li><span class="li-required">sys_ha_status</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">sys_status</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">task_task</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">task_task_history</span> - available versions:
              <span class="li-normal">6.2.2-6.2.13</span>
              </li>
              <li><span class="li-required">task_task_line</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">task_task_line_history</span> - available versions:
              <span class="li-normal">6.2.1-6.2.1, >= 6.4.1</span>
              </li>
              <li><span class="li-required">ueba_endpoints</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">ueba_endpoints_stats</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">ueba_endpoints_vuln</span> - available versions:
              <span class="li-normal">>= 7.4.0</span>
              </li>
              <li><span class="li-required">ueba_endusers</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">ueba_endusers_stats</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">ueba_otview</span> - available versions:
              <span class="li-normal">>= 7.4.0</span>
              </li>
          </ul>
        </div>
      </section>
      <li><span class="li-head">params</span> The parameter for each selector. E.g., some "get" JSON APIs support "loadsub", "meta field", "range"... <span class="li-normal">type: dict</span> <span class="li-required">choices:</span></li>
      <li style="list-style: none;">
      <section class="accordion">
        <input type="checkbox" name="collapse" id="handle3">
        <h2 class="handle"><label for="handle3"><u>More details about parameter: <b>params</b>...</u></label></h2>
        <div class="content">
        <ul class="ul-self">
            <li><span class="li-normal">params for <b>cli_fmupdate_analyzer_virusreport</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_avips_advancedlog</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_avips_webproxy</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_customurllist</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_diskquota</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_fctservices</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_fdssetting</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_fdssetting_pushoverride</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_fdssetting_pushoverridetoclient</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_fdssetting_pushoverridetoclient_announceip</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">announce-ip</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_fdssetting_serveroverride</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_fdssetting_serveroverride_servlist</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">servlist</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_fdssetting_updateschedule</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_fwmsetting</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_fwmsetting_upgradetimeout</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_multilayer</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_publicnetwork</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_serveraccesspriorities</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_serveraccesspriorities_privateserver</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">private-server</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_serveroverridestatus</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_service</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_webspam_fgdsetting</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_webspam_fgdsetting_serveroverride</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_webspam_fgdsetting_serveroverride_servlist</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">servlist</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_fmupdate_webspam_webproxy</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_metafields_system_admin_user</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_group</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">group</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_group_member</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">group</span> (Required)</li>
                <li><span class="li-required">member</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_ldap</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">ldap</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_ldap_adom</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">ldap</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_profile</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">profile</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_profile_datamaskcustomfields</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">datamask-custom-fields</span> (Required)</li>
                <li><span class="li-required">profile</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_profile_writepasswdprofiles</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">profile</span> (Required)</li>
                <li><span class="li-required">write-passwd-profiles</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_profile_writepasswduserlist</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">profile</span> (Required)</li>
                <li><span class="li-required">write-passwd-user-list</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_radius</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">radius</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_setting</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_tacacs</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">tacacs</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_user</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">user</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_user_adom</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">user</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_user_adomexclude</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom-exclude</span> (Required)</li>
                <li><span class="li-required">user</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_user_dashboard</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">dashboard</span> (Required)</li>
                <li><span class="li-required">user</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_user_dashboardtabs</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">dashboard-tabs</span> (Required)</li>
                <li><span class="li-required">user</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_user_metadata</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">meta-data</span> (Required)</li>
                <li><span class="li-required">user</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_user_policyblock</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">policy-block</span> (Required)</li>
                <li><span class="li-required">user</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_user_policypackage</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">policy-package</span> (Required)</li>
                <li><span class="li-required">user</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_admin_user_restrictdevvdom</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">restrict-dev-vdom</span> (Required)</li>
                <li><span class="li-required">user</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_alertconsole</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_alertemail</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_alertevent</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">alert-event</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_alertevent_alertdestination</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">alert-destination</span> (Required)</li>
                <li><span class="li-required">alert-event</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_autodelete</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_autodelete_dlpfilesautodeletion</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_autodelete_logautodeletion</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_autodelete_quarantinefilesautodeletion</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_autodelete_reportautodeletion</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_backup_allsettings</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_centralmanagement</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_certificate_ca</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">ca</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_certificate_crl</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">crl</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_certificate_local</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">local</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_certificate_oftp</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_certificate_remote</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">remote</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_certificate_ssh</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">ssh</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_connector</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_csf</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_csf_fabricconnector</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">fabric-connector</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_csf_trustedlist</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">trusted-list</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_dns</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_docker</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_fips</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_fortiview_autocache</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_fortiview_setting</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_global</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_guiact</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_ha</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_ha_peer</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">peer</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_ha_privatepeer</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">private-peer</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_ha_vip</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">vip</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_interface</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">interface</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_interface_ipv6</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">interface</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_interface_member</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">interface</span> (Required)</li>
                <li><span class="li-required">member</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_localinpolicy</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">local-in-policy</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_localinpolicy6</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">local-in-policy6</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_disk_filter</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_disk_setting</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_fortianalyzer2_filter</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_fortianalyzer2_setting</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_fortianalyzer3_filter</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_fortianalyzer3_setting</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_fortianalyzer_filter</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_fortianalyzer_setting</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_memory_filter</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_memory_setting</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_setting</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_syslogd2_filter</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_syslogd2_setting</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_syslogd3_filter</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_syslogd3_setting</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_syslogd_filter</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_locallog_syslogd_setting</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_log_alert</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_log_devicedisable</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">device-disable</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_log_fospolicystats</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_log_interfacestats</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_log_ioc</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_log_maildomain</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">mail-domain</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_log_pcapfile</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_log_ratelimit</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_log_ratelimit_device</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">device</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_log_ratelimit_ratelimits</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">ratelimits</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_log_settings</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_log_settings_rollinganalyzer</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_log_settings_rollinglocal</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_log_settings_rollingregular</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_log_topology</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_log_ueba</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_logfetch_clientprofile</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">client-profile</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_logfetch_clientprofile_devicefilter</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">client-profile</span> (Required)</li>
                <li><span class="li-required">device-filter</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_logfetch_clientprofile_logfilter</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">client-profile</span> (Required)</li>
                <li><span class="li-required">log-filter</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_logfetch_serversettings</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_logforward</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">log-forward</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_logforward_devicefilter</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">device-filter</span> (Required)</li>
                <li><span class="li-required">log-forward</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_logforward_logfieldexclusion</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">log-field-exclusion</span> (Required)</li>
                <li><span class="li-required">log-forward</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_logforward_logfilter</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">log-filter</span> (Required)</li>
                <li><span class="li-required">log-forward</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_logforward_logmaskingcustom</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">log-forward</span> (Required)</li>
                <li><span class="li-required">log-masking-custom</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_logforwardservice</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_mail</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">mail</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_metadata_admins</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">admins</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_ntp</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_ntp_ntpserver</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">ntpserver</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_passwordpolicy</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_performance</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_report_autocache</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_report_estbrowsetime</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_report_group</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">group</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_report_group_chartalternative</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">chart-alternative</span> (Required)</li>
                <li><span class="li-required">group</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_report_group_groupby</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">group</span> (Required)</li>
                <li><span class="li-required">group-by</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_report_setting</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_route</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">route</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_route6</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">route6</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_saml</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_saml_fabricidp</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">fabric-idp</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_saml_serviceproviders</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">service-providers</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_sniffer</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">sniffer</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_snmp_community</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">community</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_snmp_community_hosts</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">community</span> (Required)</li>
                <li><span class="li-required">hosts</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_snmp_community_hosts6</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">community</span> (Required)</li>
                <li><span class="li-required">hosts6</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_snmp_sysinfo</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_snmp_user</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">user</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_socfabric</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_socfabric_trustedlist</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">trusted-list</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_sql</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_sql_customindex</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">custom-index</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_sql_customskipidx</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">custom-skipidx</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_sql_tsindexfield</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">ts-index-field</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_sslciphersuites</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">ssl-cipher-suites</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_status</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_syslog</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">syslog</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_webproxy</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>cli_system_workflow_approvalmatrix</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">approval-matrix</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>cli_system_workflow_approvalmatrix_approver</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">approval-matrix</span> (Required)</li>
                <li><span class="li-required">approver</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>dvmdb_adom</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">expand member</span> (Optional) Fetch all or selected attributes of object members.</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">meta fields</span> (Optional) Specify the meta field attributes to be returned in the result. If none specified, no meta field attribute will be returned.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>object member</b> - Return a list of object members along with other attributes. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'object member', 'syntax']</li>
                  </ul>
                <li><span class="li-required">range</span> (Optional) Limit the number of output. For a range of [a, n], the output will contain <i>n</i> elements, starting from the <i>a<sup>th</sup></i> matching result.</li>
                <li><span class="li-required">sortings</span> (Optional) Specify the sorting of the returned result.</li>
            </ul>
            <li><span class="li-normal">params for <b>dvmdb_device</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">device</span> (Required)</li>
                <li><span class="li-required">expand member</span> (Optional) Fetch all or selected attributes of object members.</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">meta fields</span> (Optional) Specify the meta field attributes to be returned in the result. If none specified, no meta field attribute will be returned.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>object member</b> - Return a list of object members along with other attributes. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'object member', 'syntax']</li>
                  </ul>
                <li><span class="li-required">range</span> (Optional) Limit the number of output. For a range of [a, n], the output will contain <i>n</i> elements, starting from the <i>a<sup>th</sup></i> matching result.</li>
                <li><span class="li-required">sortings</span> (Optional) Specify the sorting of the returned result.</li>
            </ul>
            <li><span class="li-normal">params for <b>dvmdb_device_haslave</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">device</span> (Required)</li>
                <li><span class="li-required">ha_slave</span> (Required)</li>
                <li><span class="li-required">expand member</span> (Optional) Fetch all or selected attributes of object members.</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>object member</b> - Return a list of object members along with other attributes. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'object member', 'syntax']</li>
                  </ul>
                <li><span class="li-required">range</span> (Optional) Limit the number of output. For a range of [a, n], the output will contain <i>n</i> elements, starting from the <i>a<sup>th</sup></i> matching result.</li>
                <li><span class="li-required">sortings</span> (Optional) Specify the sorting of the returned result.</li>
            </ul>
            <li><span class="li-normal">params for <b>dvmdb_device_vdom</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">device</span> (Required)</li>
                <li><span class="li-required">vdom</span> (Required)</li>
                <li><span class="li-required">expand member</span> (Optional) Fetch all or selected attributes of object members.</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">meta fields</span> (Optional) Specify the meta field attributes to be returned in the result. If none specified, no meta field attribute will be returned.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>object member</b> - Return a list of object members along with other attributes. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'object member', 'syntax']</li>
                  </ul>
                <li><span class="li-required">range</span> (Optional) Limit the number of output. For a range of [a, n], the output will contain <i>n</i> elements, starting from the <i>a<sup>th</sup></i> matching result.</li>
                <li><span class="li-required">sortings</span> (Optional) Specify the sorting of the returned result.</li>
            </ul>
            <li><span class="li-normal">params for <b>dvmdb_folder</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">folder</span> (Required)</li>
                <li><span class="li-required">expand member</span> (Optional) Fetch all or selected attributes of object members.</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>object member</b> - Return a list of object members along with other attributes. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'object member', 'syntax']</li>
                  </ul>
                <li><span class="li-required">range</span> (Optional) Limit the number of output. For a range of [a, n], the output will contain <i>n</i> elements, starting from the <i>a<sup>th</sup></i> matching result.</li>
                <li><span class="li-required">sortings</span> (Optional) Specify the sorting of the returned result.</li>
            </ul>
            <li><span class="li-normal">params for <b>dvmdb_group</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">group</span> (Required)</li>
                <li><span class="li-required">expand member</span> (Optional) Fetch all or selected attributes of object members.</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">meta fields</span> (Optional) Specify the meta field attributes to be returned in the result. If none specified, no meta field attribute will be returned.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>object member</b> - Return a list of object members along with other attributes. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'object member', 'syntax']</li>
                  </ul>
                <li><span class="li-required">range</span> (Optional) Limit the number of output. For a range of [a, n], the output will contain <i>n</i> elements, starting from the <i>a<sup>th</sup></i> matching result.</li>
                <li><span class="li-required">sortings</span> (Optional) Specify the sorting of the returned result.</li>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_alertfilter</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">alertid</span> (Optional) Alert IDs.</li>
                <li><span class="li-required">ruleid</span> (Optional) The rule id of the rule configured in correlated typed handler.</li>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_alertincident_stats</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">time-range</span> (Optional) Time range for source data selection.</li>
                <li><span class="li-required">timescale</span> (Optional) Time scale. Only valid for type 'severity-timescale'.</li>
                  <ul class="ul-self">
                      <li>Enum: ['month', 'hour']</li>
                      <li>Example: "month"</li>
                  </ul>
                <li><span class="li-required">timezone</span> (Optional) The timezone index or name. Time range in request and date/time if any in response will follow this timezone. See Appendix</li>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_alertlogs</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">alertid</span> (Optional) Alert IDs.</li>
                <li><span class="li-required">limit</span> (Optional) The max number of records to get.</li>
                  <ul class="ul-self">
                      <li>Example: 1000</li>
                  </ul>
                <li><span class="li-required">offset</span> (Optional) offset of records to get.</li>
                <li><span class="li-required">rulename</span> (Optional) The rule name of the rule configured in correlated typed handler.</li>
                <li><span class="li-required">time-order</span> (Optional) Sort result in descending or ascending order by time</li>
                  <ul class="ul-self">
                      <li>Enum: ['desc', 'asc']</li>
                      <li>Example: "desc"</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_alertlogs_count</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">alertid</span> (Optional) Alert IDs.</li>
                <li><span class="li-required">rulename</span> (Optional) The rule name of the rule configured in correlated typed handler.</li>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_alerts</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">filter</span> (Optional) Filter expression. 'event_value', 'severity', 'trigger_name', 'count', 'comment' and 'flags' are supported. i.e.: trigger_name='Local Device Event' and severity >= 3</li>
                <li><span class="li-required">limit</span> (Optional) The max number of records to get.</li>
                  <ul class="ul-self">
                      <li>Example: 1000</li>
                  </ul>
                <li><span class="li-required">offset</span> (Optional) offset of records to get.</li>
                <li><span class="li-required">time-range</span> (Optional) Time range for data selection.</li>
                <li><span class="li-required">timezone</span> (Optional) The timezone index or name. Time range in request and date/time if any in response will follow this timezone. See Appendix</li>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_alerts_count</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">filter</span> (Optional) Filter expression. 'ackflag', 'assigned', 'mgmt_state', 'triggername', 'eventtype', 'severity', 'eventstatus' and 'tag' are supported. i.e.: ackflag = no and triggername='Local Device Event'. Note: the field 'ackflag' supports = yes/no, !=yes/no and <>yes/no ,  the field 'assigned' only supports = yes/no or !=yes/no, the field 'mgmt_state' only supports (!)= acknowledged/triaged/pending_triage</li>
                <li><span class="li-required">group-by</span> (Optional) Get alert count by group.</li>
                  <ul class="ul-self">
                      <li>Enum: ['severity', 'trigger', 'severity_timescale', 'eventtype', 'mgmt_state', 'severity_epdevtype']</li>
                  </ul>
                <li><span class="li-required">time-range</span> (Optional) Time range for source data selection.</li>
                <li><span class="li-required">timescale</span> (Optional) Time scale. Only valid for type 'severity-timescale'.</li>
                  <ul class="ul-self">
                      <li>Enum: ['month', 'hour']</li>
                      <li>Example: "month"</li>
                  </ul>
                <li><span class="li-required">timezone</span> (Optional) The timezone index or name. Time range in request and date/time if any in response will follow this timezone. See Appendix</li>
                <li><span class="li-required">type</span> (Optional) Get alert count by type.</li>
                  <ul class="ul-self">
                      <li>Enum: ['severity', 'trigger', 'severity-timescale']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_alerts_export</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">attachment</span> (Optional) Objects that will be exported with event handlers.</li>
                <li><span class="li-required">data-format</span> (Optional) The format of the exporting data.</li>
                  <ul class="ul-self">
                      <li>Enum: ['zip', 'txt', 'cli']</li>
                      <li>Example: "zip"</li>
                  </ul>
                <li><span class="li-required">filter</span> (Optional) A filter for selecting exporting event handlers. <a href="objects.htm#filter">Filter Refrence</a></li>
                  <ul class="ul-self">
                      <li>Example: ['id', 'in', 1, 10041]</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_alerts_extradetails</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">alertids</span> (Optional) Alert IDs.</li>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_basichandlers_export</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">attachment</span> (Optional) Objects that will be exported with basic handlers.</li>
                <li><span class="li-required">data-format</span> (Optional) The format of the exporting data.</li>
                  <ul class="ul-self">
                      <li>Enum: ['zip', 'txt', 'cli']</li>
                      <li>Example: "zip"</li>
                  </ul>
                <li><span class="li-required">filter</span> (Optional) A filter for selecting exporting basic handlers. <a href="objects.htm#filter">Filter Refrence</a></li>
                  <ul class="ul-self">
                      <li>Example: ['handler-id', 'in', 1, 10041]</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_config_basichandler</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_config_correlationhandler</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_config_dataselector</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_config_notificationprofile</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_config_trigger</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_config_trigger_device</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">trigger_id</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_config_trigger_filter</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">trigger_id</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_config_trigger_filter_rule</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">filter_id</span> (Required)</li>
                <li><span class="li-required">trigger_id</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>eventmgmt_correlationhandlers_export</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">attachment</span> (Optional) Objects that will be exported with correlation handlers.</li>
                <li><span class="li-required">data-format</span> (Optional) The format of the exporting data.</li>
                  <ul class="ul-self">
                      <li>Enum: ['zip', 'txt', 'cli']</li>
                      <li>Example: "zip"</li>
                  </ul>
                <li><span class="li-required">filter</span> (Optional) A filter for selecting exporting correlation handlers. <a href="objects.htm#filter">Filter Refrence</a></li>
                  <ul class="ul-self">
                      <li>Example: ['handler-id', 'in', 1, 10041]</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>fazsys_enduseravatar</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">user</span> (Optional) A structure that hold the users info. One user is identified by ('epid' and 'euid') or ('name' and 'fctuid')</li>
            </ul>
            <li><span class="li-normal">params for <b>fazsys_forticare_licinfo</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>fazsys_language_fonts_export</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">font</span> (Optional) Font name, e.g. 'UnBatang', 'Open Sans', etc, filter for exporting font file.</li>
                  <ul class="ul-self">
                      <li>Example: ['UnBatang', 'Open Sans']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>fazsys_language_fonts_list</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">font</span> (Optional) Font name, e.g. 'UnBatang', 'Open Sans', etc, filter for exporting font file.</li>
                  <ul class="ul-self">
                      <li>Example: ['UnBatang', 'Open Sans']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>fazsys_language_translationfile_export</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">language</span> (Optional) Language code list, e.g. 'en', 'zh', 'ja' etc, filter for exporting language translation file.</li>
                  <ul class="ul-self">
                      <li>Example: ['en', 'zh']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>fazsys_language_translationfile_list</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">language</span> (Optional) </li>
            </ul>
            <li><span class="li-normal">params for <b>fazsys_lograte_history</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">time-range</span> (Optional) Time range for source data selection.</li>
            </ul>
            <li><span class="li-normal">params for <b>fazsys_monitor_logforwardstatus</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">id</span> (Optional) An array of the log forwarding server ID. If the ID array is empty or omitted, status of all log forwarding servers will be returned.</li>
            </ul>
            <li><span class="li-normal">params for <b>fazsys_monitor_system_performance_status</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>fazsys_storageinfo</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">filter</span> (Optional) The field filter string.</li>
            </ul>
            <li><span class="li-normal">params for <b>fazsys_storageinfohistory</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">time-range</span> (Optional) Time range for source data selection.</li>
            </ul>
            <li><span class="li-normal">params for <b>fortiview_run</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">tid</span> (Required)</li>
                <li><span class="li-required">view-name</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>incidentmgmt_attachments</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">attachtype</span> (Optional) The attachment type.</li>
                  <ul class="ul-self">
                      <li>Enum: ['alertevent', 'note', 'file', 'report', 'log', 'comment', 'logsearchfilter', 'uploadfile']</li>
                  </ul>
                <li><span class="li-required">incid</span> (Optional) The incident ID.</li>
                  <ul class="ul-self">
                      <li>Example: "IN12345678"</li>
                  </ul>
                <li><span class="li-required">limit</span> (Optional) The maximun number of records to get.</li>
                  <ul class="ul-self">
                      <li>Example: 50</li>
                  </ul>
                <li><span class="li-required">offset</span> (Optional) The offset of records to get.</li>
            </ul>
            <li><span class="li-normal">params for <b>incidentmgmt_attachments_count</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">attachtype</span> (Optional) The attachment type.</li>
                  <ul class="ul-self">
                      <li>Enum: ['alertevent', 'log', 'comment', 'logsearchfilter', 'uploadfile', 'report']</li>
                  </ul>
                <li><span class="li-required">incid</span> (Optional) The incident ID.</li>
                  <ul class="ul-self">
                      <li>Example: "IN12345678"</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>incidentmgmt_epeuhistory</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">incid</span> (Optional) The incident ID.</li>
                  <ul class="ul-self">
                      <li>Example: "IN12345678"</li>
                  </ul>
                <li><span class="li-required">limit</span> (Optional) The maximun number of records to get.</li>
                  <ul class="ul-self">
                      <li>Example: 50</li>
                  </ul>
                <li><span class="li-required">offset</span> (Optional) The offset of records to get.</li>
            </ul>
            <li><span class="li-normal">params for <b>incidentmgmt_incident_stats</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">filter</span> (Optional) The query filter.</li>
                <li><span class="li-required">stats-item</span> (Optional) The stats item list.</li>
                <li><span class="li-required">time-range</span> (Optional) </li>
            </ul>
            <li><span class="li-normal">params for <b>incidentmgmt_incidents</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">detail-level</span> (Optional) The detail level of return data, basic, standard(default) or extended.</li>
                <li><span class="li-required">filter</span> (Optional) The query filter.</li>
                <li><span class="li-required">incids</span> (Optional) The incident ID list.</li>
                <li><span class="li-required">limit</span> (Optional) The maximun number of records to get.</li>
                  <ul class="ul-self">
                      <li>Example: 50</li>
                  </ul>
                <li><span class="li-required">offset</span> (Optional) The offset of records to get.</li>
                <li><span class="li-required">sort-by</span> (Optional) Sort by field.</li>
            </ul>
            <li><span class="li-normal">params for <b>incidentmgmt_incidents_count</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">filter</span> (Optional) The query filter.</li>
                <li><span class="li-required">incids</span> (Optional) The incident ID list.</li>
            </ul>
            <li><span class="li-normal">params for <b>ioc_license_state</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>ioc_rescan_history</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>ioc_rescan_run</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>logview_logfields</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">devtype</span> (Optional) Device type name, such as FortiGate, FortiClient, FortiMail, FortiWeb, FortiSandbox, FortiDDos, FortiDeceptor</li>
                <li><span class="li-required">logtype</span> (Optional) Logtype names</li>
                  <ul class="ul-self">
                      <li>Enum: ['traffic', 'app-ctrl', 'attack', 'content', 'dlp', 'emailfilter', 'event', 'history', 'virus', 'voip', 'webfilter', 'netscan', 'fct-event', 'fct-traffic', 'waf', 'gtp', 'ztna', 'security']</li>
                  </ul>
                <li><span class="li-required">subtype</span> (Optional) Subtype names.</li>
            </ul>
            <li><span class="li-normal">params for <b>logview_logfiles_data</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">data-type</span> (Optional) The type of return data, e.g. 'text/gzip/base64'.</li>
                  <ul class="ul-self">
                      <li>Enum: ['base64', 'csv/gzip/base64', 'text/gzip/base64']</li>
                      <li>Example: "base64"</li>
                  </ul>
                <li><span class="li-required">devid</span> (Optional) ID of the device hosting the logfile.</li>
                  <ul class="ul-self">
                      <li>Enum: ['device-id', 'All_FortiGate', 'All_FortiMail', 'All_FortiWeb', 'All_FortiManager', 'All_Syslog', 'All_FortiClient', 'All_FortiCache', 'All_FortiProxy', 'All_FortiAnalyzer', 'All_FortiSandbox', 'All_FortiAuthenticator', 'All_FortiDDoS']</li>
                  </ul>
                <li><span class="li-required">filename</span> (Optional) Name of the file.</li>
                  <ul class="ul-self">
                      <li>Example: "filename"</li>
                  </ul>
                <li><span class="li-required">length</span> (Optional) Length in byte of the file content to return. Default is 1MB, the maximum is 50MB.</li>
                  <ul class="ul-self">
                      <li>Example: 1048576</li>
                  </ul>
                <li><span class="li-required">offset</span> (Optional) Offset bytes from the beginning of the file.</li>
                <li><span class="li-required">vdom</span> (Optional) Name of the VDOM. If left empty, all VDOM under the <devid> will be considered.</li>
                  <ul class="ul-self">
                      <li>Example: "root"</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>logview_logfiles_search</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">case-sensitive</span> (Optional) Case sensitivty.</li>
                  <ul class="ul-self">
                      <li>Example: True</li>
                  </ul>
                <li><span class="li-required">devid</span> (Optional) ID of the device hosting the logfile.</li>
                  <ul class="ul-self">
                      <li>Enum: ['device-id', 'All_FortiGate', 'All_FortiMail', 'All_FortiWeb', 'All_FortiManager', 'All_Syslog', 'All_FortiClient', 'All_FortiCache', 'All_FortiProxy', 'All_FortiAnalyzer', 'All_FortiSandbox', 'All_FortiAuthenticator', 'All_FortiDDoS']</li>
                  </ul>
                <li><span class="li-required">filename</span> (Optional) File name to search.</li>
                <li><span class="li-required">filter</span> (Optional) Filter to apply.</li>
                <li><span class="li-required">limit</span> (Optional) Maximum number of log records to fetch.</li>
                  <ul class="ul-self">
                      <li>Example: 50</li>
                  </ul>
                <li><span class="li-required">logtype</span> (Optional) Name of the logtype.</li>
                  <ul class="ul-self">
                      <li>Enum: ['traffic', 'app-ctrl', 'attack', 'content', 'dlp', 'emailfilter', 'event', 'history', 'virus', 'voip', 'webfilter', 'netscan', 'fct-event', 'fct-traffic', 'waf', 'gtp']</li>
                  </ul>
                <li><span class="li-required">offset</span> (Optional) Offset number of log records from the beginning of the log file.</li>
                <li><span class="li-required">vdom</span> (Optional) Name of the VDOM hosting the logfile.</li>
            </ul>
            <li><span class="li-normal">params for <b>logview_logfiles_state</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">devid</span> (Optional) ID of the device. If left empty, all devices under the <adom-name> will be considered. See Appendix for available options</li>
                  <ul class="ul-self">
                      <li>Enum: ['device-id', 'All_FortiGate', 'All_FortiMail', 'All_FortiWeb', 'All_FortiManager', 'All_Syslog', 'All_FortiClient', 'All_FortiCache', 'All_FortiProxy', 'All_FortiAnalyzer', 'All_FortiSandbox', 'All_FortiAuthenticator', 'All_FortiDDoS']</li>
                  </ul>
                <li><span class="li-required">filename</span> (Optional) name of the file. If left empty, all files under the <vdom> will be considered</li>
                <li><span class="li-required">time-range</span> (Optional) Time range for data selection.</li>
                <li><span class="li-required">timezone</span> (Optional) The timezone index or name. Time range in request and date/time if any in response will follow this timezone. See Appendix</li>
                <li><span class="li-required">vdom</span> (Optional) Name of the VDOM. If left empty, all VDOM under the <devid> will be considered.</li>
                  <ul class="ul-self">
                      <li>Example: "root"</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>logview_logsearch</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">tid</span> (Required)</li>
                <li><span class="li-required">limit</span> (Optional) Number of records to return.</li>
                  <ul class="ul-self">
                      <li>Example: 50</li>
                  </ul>
                <li><span class="li-required">offset</span> (Optional) Number of records to offset.</li>
            </ul>
            <li><span class="li-normal">params for <b>logview_logsearch_count</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">tid</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>logview_logstats</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">device</span> (Optional) Device filter. For all devices in some type please use the All-Device ID. <b><i>See Appendix</i></b></li>
            </ul>
            <li><span class="li-normal">params for <b>logview_pcapfile</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">key-data</span> (Optional) The key for searching pcapfile. It supports three type of data: 1) JSON format log , 2) txt format log and 3) pcapurl. A pcapurl can be found in the logsearch result if the log does have an associated pcap file. e.g. 'pcapfile?ZGV2aWQ9IkZHMjAwRTRRMTc5MTYwNTkiIHZkPSJyb290IiBzdWJ0eXBlPSJhcHAtY3RybCIgY2hlY2tzdW09IiIgZXBvY2g9MCBpbmNpZGVudHNlcmlhbG5vPTM4NjE4Mzg5OSBzZXJ2aWNlPSJTU0wiIHR5cGU9InV0bSIgZXZlbnRpZD0wIGluZGVudGlkeD0wIGZpbGVwYXRoPSIvaXBzX2ZpbGVzL0ZHMjAwRTRRMTc5MTYwNTkvcm9vdC8xNjM0ODUxNTU0LzM4NjE4Mzg5OTowIg==\'. For more details, please click 'Show examples...' .</li>
                <li><span class="li-required">key-type</span> (Optional) The type of the given key-data.</li>
                  <ul class="ul-self">
                      <li>Enum: ['log-data', 'pcapurl']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>report_config_chart</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_chart_drilldowntable</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">chart_name</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_chart_tablecolumns</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">chart_name</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_chart_variabletemplate</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">chart_name</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_dataset</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_dataset_variable</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">dataset_name</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_layout</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_layout_component</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">layout-id</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_layout_component_variable</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">component-id</span> (Required)</li>
                <li><span class="li-required">layout-id</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_layout_footer</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">layout-id</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_layout_header</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">layout-id</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_layoutfolder</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_macro</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_output</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_output_emailrecipients</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">output-name</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_schedule</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_schedule_addressfilter</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">schedule_name</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_schedule_devices</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">schedule_name</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_schedule_filter</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">schedule_name</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_config_schedule_reportlayout</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">schedule_name</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_graphfile</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">file-name</span> (Optional) Graph file name.</li>
            </ul>
            <li><span class="li-normal">params for <b>report_graphfile_data</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">file-name</span> (Optional) Graph file name.</li>
            </ul>
            <li><span class="li-normal">params for <b>report_graphfile_list</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">file-name</span> (Optional) Names of the graph files that will be listed. Without this param, all files in the folder will be listed.</li>
            </ul>
            <li><span class="li-normal">params for <b>report_reports_data</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">tid</span> (Required)</li>
                <li><span class="li-required">data-type</span> (Optional) One option to download the text format of XML or CSV reports, e.g. 'text'.</li>
                  <ul class="ul-self">
                      <li>Example: "text"</li>
                  </ul>
                <li><span class="li-required">format</span> (Optional) One format got by /report/adom/&lt;adom-name&gt;/reports/state. Such as HTML, PDF, XML, CSV.</li>
                  <ul class="ul-self">
                      <li>Example: "PDF"</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>report_reports_state</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">sort-by</span> (Optional) Sort by fields. Only support <b>one field</b> for this API.</li>
                <li><span class="li-required">state</span> (Optional) pending-running, or generated.</li>
                <li><span class="li-required">time-range</span> (Optional) Time range for source data selection.</li>
                <li><span class="li-required">timezone</span> (Optional) The timezone index or name. Time range in request and date/time if any in response will follow this timezone. See Appendix</li>
                <li><span class="li-required">title</span> (Optional) Title of a report.</li>
            </ul>
            <li><span class="li-normal">params for <b>report_run</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">tid</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_template_export</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">dev-type</span> (Optional) Device type abbreviation, e.g. 'fgt', 'fml' etc.</li>
                  <ul class="ul-self">
                      <li>Example: "fgt"</li>
                  </ul>
                <li><span class="li-required">language</span> (Optional) Language name, e.g. 'en', 'zh', 'ja' etc, filter for exporting report template.</li>
                  <ul class="ul-self">
                      <li>Example: "en"</li>
                  </ul>
                <li><span class="li-required">title</span> (Optional) Template title, filter for exporting report template.</li>
            </ul>
            <li><span class="li-normal">params for <b>report_template_language</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>report_template_list</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">dev-type</span> (Optional) Device type abbreviation, e.g. 'fgt', 'fml' etc.</li>
                  <ul class="ul-self">
                      <li>Example: "fgt"</li>
                  </ul>
                <li><span class="li-required">language</span> (Optional) Language name, 'en', 'zh', 'ja' etc, filter for listing report template.</li>
                  <ul class="ul-self">
                      <li>Example: "en"</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>soar_alert_indicator</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">alert-id</span> (Optional) The alert ID.</li>
                <li><span class="li-required">filter</span> (Optional) Filter expression. 'indicator-uuid', 'type', 'value', 'status', 'enrichment-uuid', 'enrichment-status' and 'enrichment-reputation' are supported. i.e.: indicator-uuid='8a409a0f-e4b7-4c71-8e42-a03748496b13' and value = '8.8.8.8'</li>
            </ul>
            <li><span class="li-normal">params for <b>soar_config_connectors</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">connector-uuid</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>soar_config_playbooks</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">playbook-uuid</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>soar_fosconnector_automationrules</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
            </ul>
            <li><span class="li-normal">params for <b>soar_incident_indicator</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">filter</span> (Optional) Filter expression. 'indicator-uuid', 'type', 'value', 'status', 'enrichment-uuid', 'enrichment-status' and 'enrichment-reputation' are supported. i.e.: indicator-uuid='8a409a0f-e4b7-4c71-8e42-a03748496b13' and value = '8.8.8.8'</li>
                <li><span class="li-required">incident-id</span> (Optional) The incident ID.</li>
            </ul>
            <li><span class="li-normal">params for <b>soar_indicator</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">filter</span> (Optional) Filter expression. 'indicator-uuid', 'type', 'value', 'status', 'enrichment-uuid', 'enrichment-status' and 'enrichment-reputation' are supported. i.e.: indicator-uuid='8a409a0f-e4b7-4c71-8e42-a03748496b13,2828ad45-82a7-4173-844e-40b2259ab556' and value = '8.8.8.8'</li>
                <li><span class="li-required">limit</span> (Optional) The max number of records to get.</li>
                  <ul class="ul-self">
                      <li>Example: 100</li>
                  </ul>
                <li><span class="li-required">offset</span> (Optional) offset of records to get.</li>
                <li><span class="li-required">option</span> (Optional) This option defines whether the response should include a array of incident_ids and alert_ids associated with the indicator. Leaving this option empty or omitting it entirely will exclude incident and alert ID data from the response.</li>
                <li><span class="li-required">time-range</span> (Optional) Time range for data selection. If not exist, default time-range is 7 days from current time.</li>
            </ul>
            <li><span class="li-normal">params for <b>soar_indicator_enrichment</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">enrichment_uuid</span> (Required)</li>
                <li><span class="li-required">detail-level</span> (Optional) Specify whether include enrichment-detail in response data. 'standard' not included, 'extended' included. Leaving this parameter empty or omitting it entirely will default to 'standard' details.</li>
                  <ul class="ul-self">
                      <li>Enum: ['standard', 'extended']</li>
                  </ul>
                <li><span class="li-required">indicator-type</span> (Optional) The indicator type.</li>
                  <ul class="ul-self">
                      <li>Enum: ['IP', 'URL', 'Domain']</li>
                  </ul>
                <li><span class="li-required">indicator-uuid</span> (Optional) The indicator UUID.</li>
                <li><span class="li-required">indicator-value</span> (Optional) The indicator value.</li>
            </ul>
            <li><span class="li-normal">params for <b>soar_playbook_export</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">attachment</span> (Optional) Objects that will be exported with event handlers.</li>
                <li><span class="li-required">data-format</span> (Optional) The format of the exporting data.</li>
                  <ul class="ul-self">
                      <li>Enum: ['zip', 'txt']</li>
                      <li>Example: "zip"</li>
                  </ul>
                <li><span class="li-required">filter</span> (Optional) A filter for selecting exporting playbooks. <a href="objects.htm#filter">Filter Refrence</a></li>
                  <ul class="ul-self">
                      <li>Example: ['uuid', 'in', '941a1c06-2841-47c5-b45b-ca429d23a332', '2b36d3c6-537f-4671-8280-44549f824e6a']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>soar_playbook_monitor</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">filter</span> (Optional) Filtering expresion.</li>
                  <ul class="ul-self">
                      <li>Example: "trigger-source-id<>'IN00019917' playbook-name~'Shawn - Event trigger-LocalHostConnector'"</li>
                  </ul>
                <li><span class="li-required">instance-id</span> (Optional) Instance ID to get.</li>
                <li><span class="li-required">playbook-uuid</span> (Optional) Playbook UUID to get. An unique identifier of a playbook. 32 hexadecimal digits is displayed in five groups separated by hyphens, in the form 8-4-4-4-12 for a total of 36 characters</li>
                <li><span class="li-required">sort-by</span> (Optional) Sort by field.</li>
                <li><span class="li-required">time-range</span> (Optional) Time range for source data selection.</li>
                <li><span class="li-required">timezone</span> (Optional) The timezone index or name. Time range in request and date/time if any in response will follow this timezone. See Appendix</li>
            </ul>
            <li><span class="li-normal">params for <b>soar_playbook_run</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">filter</span> (Optional) Filtering expresion.</li>
                  <ul class="ul-self">
                      <li>Example: "trigger-source-id<>'IN00019917' playbook-name~'Shawn - Event trigger-LocalHostConnector'"</li>
                  </ul>
                <li><span class="li-required">instance-id</span> (Optional) Instance ID to get.</li>
                <li><span class="li-required">playbook-uuid</span> (Optional) An unique identifier of a playbook. 32 hexadecimal digits is displayed in five groups separated by hyphens, in the form 8-4-4-4-12 for a total of 36 characters.</li>
                  <ul class="ul-self">
                      <li>Example: "2b36d3c6-537f-4671-8280-44549f824e6a"</li>
                  </ul>
                <li><span class="li-required">sort-by</span> (Optional) Sort by field.</li>
                <li><span class="li-required">time-range</span> (Optional) Time range for source data selection.</li>
                <li><span class="li-required">timezone</span> (Optional) The timezone index or name. Time range in request and date/time if any in response will follow this timezone. See Appendix</li>
            </ul>
            <li><span class="li-normal">params for <b>soar_playbook_runlog</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">run-id</span> (Required)</li>
                <li><span class="li-required">detail-on-error</span> (Optional) Specify whether include detail in log if error happened. missing or empty is 'true'</li>
                  <ul class="ul-self">
                      <li>Enum: ['true', 'false']</li>
                  </ul>
            </ul>
            <li><span class="li-normal">params for <b>soar_subnet_export</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">data-format</span> (Optional) The format of the exporting data.</li>
                  <ul class="ul-self">
                      <li>Enum: ['zip', 'txt']</li>
                      <li>Example: "txt"</li>
                  </ul>
                <li><span class="li-required">filter</span> (Optional) A filter for selecting exporting subnets and subnet groups</li>
            </ul>
            <li><span class="li-normal">params for <b>soar_task_monitor</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">filter</span> (Optional) Filtering expresion.</li>
                  <ul class="ul-self">
                      <li>Example: "state<>'success'"</li>
                  </ul>
                <li><span class="li-required">instance-id</span> (Optional) Instance ID to get.</li>
                <li><span class="li-required">playbook-uuid</span> (Optional) Playbook UUID to get. An unique identifier of a playbook. 32 hexadecimal digits is displayed in five groups separated by hyphens, in the form 8-4-4-4-12 for a total of 36 characters</li>
                <li><span class="li-required">run-id</span> (Optional) Run ID to track specific playbook run</li>
                <li><span class="li-required">sort-by</span> (Optional) Sort by field.</li>
                <li><span class="li-required">time-range</span> (Optional) Time range for source data selection.</li>
                <li><span class="li-required">timezone</span> (Optional) The timezone index or name. Time range in request and date/time if any in response will follow this timezone. See Appendix</li>
            </ul>
            <li><span class="li-normal">params for <b>sys_ha_status</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>sys_status</b>:</span> None</li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for <b>task_task</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">task</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
                <li><span class="li-required">range</span> (Optional) Limit the number of output. For a range of [a, n], the output will contain <i>n</i> elements, starting from the <i>a<sup>th</sup></i> matching result.</li>
                <li><span class="li-required">sortings</span> (Optional) Specify the sorting of the returned result.</li>
            </ul>
            <li><span class="li-normal">params for <b>task_task_history</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">history</span> (Required)</li>
                <li><span class="li-required">task</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
                <li><span class="li-required">range</span> (Optional) Limit the number of output. For a range of [a, n], the output will contain <i>n</i> elements, starting from the <i>a<sup>th</sup></i> matching result.</li>
                <li><span class="li-required">sortings</span> (Optional) Specify the sorting of the returned result.</li>
            </ul>
            <li><span class="li-normal">params for <b>task_task_line</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">line</span> (Required)</li>
                <li><span class="li-required">task</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
                <li><span class="li-required">range</span> (Optional) Limit the number of output. For a range of [a, n], the output will contain <i>n</i> elements, starting from the <i>a<sup>th</sup></i> matching result.</li>
                <li><span class="li-required">sortings</span> (Optional) Specify the sorting of the returned result.</li>
            </ul>
            <li><span class="li-normal">params for <b>task_task_line_history</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">history</span> (Required)</li>
                <li><span class="li-required">line</span> (Required)</li>
                <li><span class="li-required">task</span> (Required)</li>
                <li><span class="li-required">fields</span> (Optional) Limit the output by returning only the attributes specified in the string array. If none specified, all attributes will be returned.</li>
                <li><span class="li-required">filter</span> (Optional) Filter the result according to a set of criteria.</li>
                <li><span class="li-required">loadsub</span> (Optional) Enable or disable the return of any sub-objects. If not specified, the default is to return all sub-objects.</li>
                <li><span class="li-required">option</span> (Optional) Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. <b>count</b> - Return the number of matching entries instead of the actual entry data. <b>syntax</b> - Return the attribute syntax of a table or an object, instead of the actual entry data. All filter parameters will be ignored.</li>
                  <ul class="ul-self">
                      <li>Enum: ['count', 'syntax']</li>
                  </ul>
                <li><span class="li-required">range</span> (Optional) Limit the number of output. For a range of [a, n], the output will contain <i>n</i> elements, starting from the <i>a<sup>th</sup></i> matching result.</li>
                <li><span class="li-required">sortings</span> (Optional) Specify the sorting of the returned result.</li>
            </ul>
            <li><span class="li-normal">params for <b>ueba_endpoints</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">detail-level</span> (Optional) The level of details to get.</li>
                  <ul class="ul-self">
                      <li>Enum: ['basic', 'standard', 'simple']</li>
                      <li>Example: "basic"</li>
                  </ul>
                <li><span class="li-required">epids</span> (Optional) The endpoint ID list.</li>
                <li><span class="li-required">filter</span> (Optional) The query filter.</li>
                  <ul class="ul-self">
                      <li>Example: "epname='VAN-201437-PC'"</li>
                  </ul>
                <li><span class="li-required">limit</span> (Optional) The maximun number of records to get.</li>
                  <ul class="ul-self">
                      <li>Example: 100000</li>
                  </ul>
                <li><span class="li-required">offset</span> (Optional) The offset of records to get.</li>
                <li><span class="li-required">sort-by</span> (Optional) Sort by field.</li>
                <li><span class="li-required">time-range</span> (Optional) Time range for endpoints. (required if the epids field is not provided)</li>
            </ul>
            <li><span class="li-normal">params for <b>ueba_endpoints_stats</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">filter</span> (Optional) The query filter.</li>
                  <ul class="ul-self">
                      <li>Example: "category=IOT"</li>
                  </ul>
                <li><span class="li-required">stats-item</span> (Optional) an array of strings that holds the requested stats type.</li>
                <li><span class="li-required">time-range</span> (Optional) Time range for endpoint stats.</li>
                <li><span class="li-required">timezone</span> (Optional) The timezone index or name. Time range in request and date/time if any in response will follow this timezone. See Appendix</li>
            </ul>
            <li><span class="li-normal">params for <b>ueba_endpoints_vuln</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">detectby</span> (Optional) The vulnerabilities detection source. 'FortiGate' by default.</li>
                  <ul class="ul-self">
                      <li>Enum: ['FortiClient', 'FortiGate']</li>
                  </ul>
                <li><span class="li-required">epids</span> (Optional) The endpoint ID list.</li>
                <li><span class="li-required">filter</span> (Optional) The query filter.</li>
                <li><span class="li-required">limit</span> (Optional) The maximun number of records to get.</li>
                  <ul class="ul-self">
                      <li>Example: 100000</li>
                  </ul>
                <li><span class="li-required">offset</span> (Optional) The offset of records to get.</li>
                <li><span class="li-required">sort-by</span> (Optional) Sort by field.</li>
            </ul>
            <li><span class="li-normal">params for <b>ueba_endusers</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">detail-level</span> (Optional) The level of details to get.</li>
                  <ul class="ul-self">
                      <li>Enum: ['basic', 'standard', 'extended']</li>
                      <li>Example: "standard"</li>
                  </ul>
                <li><span class="li-required">euids</span> (Optional) The enduser ID list.</li>
                <li><span class="li-required">filter</span> (Optional) The query filter.</li>
                  <ul class="ul-self">
                      <li>Example: "euname='localhost'"</li>
                  </ul>
                <li><span class="li-required">limit</span> (Optional) The maximun number of records to get.</li>
                  <ul class="ul-self">
                      <li>Example: 100000</li>
                  </ul>
                <li><span class="li-required">offset</span> (Optional) The offset of records to get.</li>
                <li><span class="li-required">sort-by</span> (Optional) Sort by field.</li>
            </ul>
            <li><span class="li-normal">params for <b>ueba_endusers_stats</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">stats-item</span> (Optional) an array of strings that holds the requested stats type.</li>
                <li><span class="li-required">time-range</span> (Optional) Time range for enduser stats.</li>
                <li><span class="li-required">timezone</span> (Optional) The timezone index or name. Time range in request and date/time if any in response will follow this timezone. See Appendix</li>
            </ul>
            <li><span class="li-normal">params for <b>ueba_otview</b>:</span> </li>
            <ul class="ul-self">
                <li><span class="li-required">adom</span> (Required)</li>
                <li><span class="li-required">filter</span> (Optional) The query filter. (only support devid filtering now)</li>
                  <ul class="ul-self">
                      <li>Example: "devid=FGVM02TM23001113"</li>
                  </ul>
                <li><span class="li-required">group-by</span> (Optional) Group by field.</li>
            </ul>
        </ul>
        </div>
      </section>
    </ul>
  </ul>



Notes
-----
.. note::

   - Selector is a mandatory parameter for the module, and the params is varying depending on the selector.
   - Parameter ``adom`` can be ``null`` or ``''`` for all administrative domains,  ``global`` for global domain and any other custom domain strings. and a particular fact may not support all kinds of domains.
   - In parameters section, ``null`` and ``''`` are identical if you are fetching all objects under that selector category.
   - Normally, running one module can fail when a non-zero rc is returned. you can also override the conditions to fail or succeed with parameters ``rc_failed`` and ``rc_succeeded``

Examples
--------

.. code-block:: yaml+jinja

  - name: Gathering fortianalyzer facts
    hosts: fortianalyzers
    gather_facts: false
    connection: httpapi
    vars:
      ansible_httpapi_use_ssl: true
      ansible_httpapi_validate_certs: false
      ansible_httpapi_port: 443
    tasks:
      - name: Fetch adom
        fortinet.fortianalyzer.faz_fact:
          facts:
            selector: "dvmdb_adom"
            filter: [["os_ver", "==", "7.0"], "&&", [["state", "==", "1"]]]
            fields:
              - "name"
              - "restricted_prds"
            # option: "object member" # "count", "object member" or "syntax"
            sortings:
              - "restricted_prds": -1 # sort based on restricted_prds first (-1, descending)
              - "oid": 1 # if restricted_prds are same, then, sort based on oid (1, ascending)


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