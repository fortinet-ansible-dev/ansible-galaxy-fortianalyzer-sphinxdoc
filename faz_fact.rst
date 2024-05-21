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
              <span class="li-normal">7.0.5-7.0.12, >= 7.2.2</span>
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
              <span class="li-normal">6.4.7-6.4.14, >= 7.0.2</span>
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
              <span class="li-normal">6.4.8-6.4.14, >= 7.0.2</span>
              </li>
              <li><span class="li-required">cli_system_status</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_syslog</span> - available versions:
              <span class="li-normal">>= 6.2.1</span>
              </li>
              <li><span class="li-required">cli_system_webproxy</span> - available versions:
              <span class="li-normal">6.4.8-6.4.14, >= 7.0.3</span>
              </li>
              <li><span class="li-required">cli_system_workflow_approvalmatrix</span> - available versions:
              <span class="li-normal">6.2.1-6.2.9, 6.4.1-6.4.7, 7.0.0-7.0.2</span>
              </li>
              <li><span class="li-required">cli_system_workflow_approvalmatrix_approver</span> - available versions:
              <span class="li-normal">6.2.1-6.2.9, 6.4.1-6.4.7, 7.0.0-7.0.2</span>
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
              <li><span class="li-required">fazsys_monitor_logforwardstatus</span> - available versions:
              <span class="li-normal">>= 7.2.2</span>
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
              <li><span class="li-required">soar_config_connectors</span> - available versions:
              <span class="li-normal">>= 6.4.2</span>
              </li>
              <li><span class="li-required">soar_config_playbooks</span> - available versions:
              <span class="li-normal">>= 6.4.2</span>
              </li>
              <li><span class="li-required">soar_fosconnector_automationrules</span> - available versions:
              <span class="li-normal">>= 6.4.2</span>
              </li>
              <li><span class="li-required">soar_playbook_export</span> - available versions:
              <span class="li-normal">>= 7.0.0</span>
              </li>
              <li><span class="li-required">soar_playbook_monitor</span> - available versions:
              <span class="li-normal">6.4.2-7.2.1</span>
              </li>
              <li><span class="li-required">soar_playbook_run</span> - available versions:
              <span class="li-normal">>= 6.4.2</span>
              </li>
              <li><span class="li-required">soar_subnet_export</span> - available versions:
              <span class="li-normal">>= 7.0.0</span>
              </li>
              <li><span class="li-required">soar_task_monitor</span> - available versions:
              <span class="li-normal">>= 6.4.2</span>
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
              <span class="li-normal">6.2.2-6.2.12</span>
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
      <li><span class="li-head">params</span> The parameter for each selector. You can also add any API specified parameters (E.g., some "get" JSON APIs support "loadsub", "meta field", "range"...). <span class="li-normal">type: dict</span> <span class="li-required">choices:</span></li>
      <li style="list-style: none;">
      <section class="accordion">
        <input type="checkbox" name="collapse" id="handle3">
        <h2 class="handle"><label for="handle3"><u>More details about parameter: <b>params</b>...</u></label></h2>
        <div class="content">          
        <ul class="ul-self">
            <li><span class="li-normal">params for cli_fmupdate_analyzer_virusreport:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_avips_advancedlog:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_avips_webproxy:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_customurllist:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_diskquota:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_fctservices:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_fdssetting:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_fdssetting_pushoverride:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_fdssetting_pushoverridetoclient:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_fdssetting_pushoverridetoclient_announceip:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">announce-ip</span></li>
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_fdssetting_serveroverride:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_fdssetting_serveroverride_servlist:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">servlist</span></li>
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_fdssetting_updateschedule:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_fwmsetting:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_fwmsetting_upgradetimeout:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_multilayer:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_publicnetwork:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_serveraccesspriorities:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_serveraccesspriorities_privateserver:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">private-server</span></li>
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_serveroverridestatus:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_service:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_webspam_fgdsetting:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_webspam_fgdsetting_serveroverride:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_webspam_fgdsetting_serveroverride_servlist:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">servlist</span></li>
            </ul>
            <li><span class="li-normal">params for cli_fmupdate_webspam_webproxy:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_metafields_system_admin_user:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_admin_group:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">group</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_group_member:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">group</span></li>
                <li><span class="li-normal">member</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_ldap:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">ldap</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_ldap_adom:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
                <li><span class="li-normal">ldap</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_profile:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">profile</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_profile_datamaskcustomfields:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">datamask-custom-fields</span></li>
                <li><span class="li-normal">profile</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_profile_writepasswdprofiles:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">profile</span></li>
                <li><span class="li-normal">write-passwd-profiles</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_profile_writepasswduserlist:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">profile</span></li>
                <li><span class="li-normal">write-passwd-user-list</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_radius:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">radius</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_setting:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_admin_tacacs:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">tacacs</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_user:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">user</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_user_adom:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
                <li><span class="li-normal">user</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_user_adomexclude:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom-exclude</span></li>
                <li><span class="li-normal">user</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_user_dashboard:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">dashboard</span></li>
                <li><span class="li-normal">user</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_user_dashboardtabs:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">dashboard-tabs</span></li>
                <li><span class="li-normal">user</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_user_metadata:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">meta-data</span></li>
                <li><span class="li-normal">user</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_user_policypackage:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">policy-package</span></li>
                <li><span class="li-normal">user</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_admin_user_restrictdevvdom:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">restrict-dev-vdom</span></li>
                <li><span class="li-normal">user</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_alertconsole:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_alertemail:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_alertevent:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">alert-event</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_alertevent_alertdestination:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">alert-destination</span></li>
                <li><span class="li-normal">alert-event</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_autodelete:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_autodelete_dlpfilesautodeletion:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_autodelete_logautodeletion:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_autodelete_quarantinefilesautodeletion:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_autodelete_reportautodeletion:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_backup_allsettings:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_centralmanagement:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_certificate_ca:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">ca</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_certificate_crl:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">crl</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_certificate_local:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">local</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_certificate_oftp:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_certificate_remote:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">remote</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_certificate_ssh:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">ssh</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_connector:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_csf:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_csf_fabricconnector:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">fabric-connector</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_csf_trustedlist:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">trusted-list</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_dns:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_docker:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_fips:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_fortiview_autocache:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_fortiview_setting:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_global:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_guiact:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_ha:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_ha_peer:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">peer</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_ha_privatepeer:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">private-peer</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_ha_vip:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">vip</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_interface:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">interface</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_interface_ipv6:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">interface</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_interface_member:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">interface</span></li>
                <li><span class="li-normal">member</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_localinpolicy:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">local-in-policy</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_localinpolicy6:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">local-in-policy6</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_disk_filter:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_disk_setting:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_fortianalyzer2_filter:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_fortianalyzer2_setting:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_fortianalyzer3_filter:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_fortianalyzer3_setting:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_fortianalyzer_filter:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_fortianalyzer_setting:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_memory_filter:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_memory_setting:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_setting:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_syslogd2_filter:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_syslogd2_setting:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_syslogd3_filter:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_syslogd3_setting:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_syslogd_filter:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_locallog_syslogd_setting:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_log_alert:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_log_devicedisable:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">device-disable</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_log_fospolicystats:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_log_interfacestats:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_log_ioc:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_log_maildomain:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">mail-domain</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_log_pcapfile:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_log_ratelimit:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_log_ratelimit_device:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">device</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_log_ratelimit_ratelimits:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">ratelimits</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_log_settings:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_log_settings_rollinganalyzer:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_log_settings_rollinglocal:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_log_settings_rollingregular:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_log_topology:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_logfetch_clientprofile:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">client-profile</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_logfetch_clientprofile_devicefilter:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">client-profile</span></li>
                <li><span class="li-normal">device-filter</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_logfetch_clientprofile_logfilter:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">client-profile</span></li>
                <li><span class="li-normal">log-filter</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_logfetch_serversettings:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_logforward:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">log-forward</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_logforward_devicefilter:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">device-filter</span></li>
                <li><span class="li-normal">log-forward</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_logforward_logfieldexclusion:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">log-field-exclusion</span></li>
                <li><span class="li-normal">log-forward</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_logforward_logfilter:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">log-filter</span></li>
                <li><span class="li-normal">log-forward</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_logforward_logmaskingcustom:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">log-forward</span></li>
                <li><span class="li-normal">log-masking-custom</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_logforwardservice:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_mail:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">mail</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_metadata_admins:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">admins</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_ntp:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_ntp_ntpserver:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">ntpserver</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_passwordpolicy:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_performance:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_report_autocache:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_report_estbrowsetime:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_report_group:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">group</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_report_group_chartalternative:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">chart-alternative</span></li>
                <li><span class="li-normal">group</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_report_group_groupby:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">group</span></li>
                <li><span class="li-normal">group-by</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_report_setting:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_route:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">route</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_route6:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">route6</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_saml:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_saml_fabricidp:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">fabric-idp</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_saml_serviceproviders:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">service-providers</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_sniffer:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">sniffer</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_snmp_community:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">community</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_snmp_community_hosts:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">community</span></li>
                <li><span class="li-normal">hosts</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_snmp_community_hosts6:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">community</span></li>
                <li><span class="li-normal">hosts6</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_snmp_sysinfo:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_snmp_user:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">user</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_socfabric:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_socfabric_trustedlist:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">trusted-list</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_sql:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_sql_customindex:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">custom-index</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_sql_customskipidx:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">custom-skipidx</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_sql_tsindexfield:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">ts-index-field</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_sslciphersuites:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">ssl-cipher-suites</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_status:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_syslog:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">syslog</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_webproxy:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for cli_system_workflow_approvalmatrix:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">approval-matrix</span></li>
            </ul>
            <li><span class="li-normal">params for cli_system_workflow_approvalmatrix_approver:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">approval-matrix</span></li>
                <li><span class="li-normal">approver</span></li>
            </ul>
            <li><span class="li-normal">params for dvmdb_adom:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for dvmdb_device:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
                <li><span class="li-normal">device</span></li>
            </ul>
            <li><span class="li-normal">params for dvmdb_device_haslave:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
                <li><span class="li-normal">device</span></li>
                <li><span class="li-normal">ha_slave</span></li>
            </ul>
            <li><span class="li-normal">params for dvmdb_device_vdom:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
                <li><span class="li-normal">device</span></li>
                <li><span class="li-normal">vdom</span></li>
            </ul>
            <li><span class="li-normal">params for dvmdb_folder:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
                <li><span class="li-normal">folder</span></li>
            </ul>
            <li><span class="li-normal">params for dvmdb_group:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
                <li><span class="li-normal">group</span></li>
            </ul>
            <li><span class="li-normal">params for eventmgmt_alertfilter:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for eventmgmt_alertlogs:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for eventmgmt_alertlogs_count:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for eventmgmt_alerts:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for eventmgmt_alerts_count:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for eventmgmt_alerts_export:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for eventmgmt_alerts_extradetails:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for eventmgmt_basichandlers_export:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for eventmgmt_correlationhandlers_export:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for fazsys_enduseravatar:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for fazsys_forticare_licinfo:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for fazsys_language_fonts_export:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for fazsys_language_fonts_list:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for fazsys_language_translationfile_export:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for fazsys_language_translationfile_list:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for fazsys_monitor_logforwardstatus:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for fortiview_run:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
                <li><span class="li-normal">tid</span></li>
                <li><span class="li-normal">view-name</span></li>
            </ul>
            <li><span class="li-normal">params for incidentmgmt_attachments:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for incidentmgmt_attachments_count:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for incidentmgmt_epeuhistory:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for incidentmgmt_incidents:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for incidentmgmt_incidents_count:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for ioc_license_state:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for ioc_rescan_history:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for ioc_rescan_run:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for logview_logfields:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for logview_logfiles_data:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for logview_logfiles_search:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for logview_logfiles_state:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for logview_logsearch:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
                <li><span class="li-normal">tid</span></li>
            </ul>
            <li><span class="li-normal">params for logview_logsearch_count:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
                <li><span class="li-normal">tid</span></li>
            </ul>
            <li><span class="li-normal">params for logview_logstats:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for logview_pcapfile:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for report_graphfile:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for report_graphfile_data:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for report_graphfile_list:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for report_reports_data:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
                <li><span class="li-normal">tid</span></li>
            </ul>
            <li><span class="li-normal">params for report_reports_state:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for report_run:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
                <li><span class="li-normal">tid</span></li>
            </ul>
            <li><span class="li-normal">params for report_template_export:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for report_template_language:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for report_template_list:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for soar_config_connectors:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
                <li><span class="li-normal">connector-uuid</span></li>
            </ul>
            <li><span class="li-normal">params for soar_config_playbooks:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
                <li><span class="li-normal">playbook-uuid</span></li>
            </ul>
            <li><span class="li-normal">params for soar_fosconnector_automationrules:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for soar_playbook_export:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for soar_playbook_monitor:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for soar_playbook_run:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for soar_subnet_export:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for soar_task_monitor:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for sys_ha_status:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for sys_status:</span></li>
            <ul class="ul-self">
            </ul>
            <li><span class="li-normal">params for task_task:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">task</span></li>
            </ul>
            <li><span class="li-normal">params for task_task_history:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">history</span></li>
                <li><span class="li-normal">task</span></li>
            </ul>
            <li><span class="li-normal">params for task_task_line:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">line</span></li>
                <li><span class="li-normal">task</span></li>
            </ul>
            <li><span class="li-normal">params for task_task_line_history:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">history</span></li>
                <li><span class="li-normal">line</span></li>
                <li><span class="li-normal">task</span></li>
            </ul>
            <li><span class="li-normal">params for ueba_endpoints:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for ueba_endpoints_stats:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for ueba_endpoints_vuln:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for ueba_endusers:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for ueba_endusers_stats:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
            </ul>
            <li><span class="li-normal">params for ueba_otview:</span></li>
            <ul class="ul-self">
                <li><span class="li-normal">adom</span></li>
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