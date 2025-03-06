:source: faz_rename.py

:orphan:

.. _faz_rename:

faz_rename -- Rename An Object.
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
 <li><span class="li-head">rename</span> Rename An Object. <span class="li-normal">type: dict</span></li>
 <ul class="ul-self">
 <li><span class="li-head">target</span> Attribute to override for target object. <span class="li-normal">type: dict</span> <span class="li-required">required: true</span></li>
   <li style="list-style: none;"><section class="accordion">
   <input type="checkbox" name="collapse" id="handle1">
   <h2 class="handle">
        <label for="handle1"><u>More details about parameter: <b>target</b>...</u></label>
    </h2>
    <div class="content">
    <ul class="ul-self">
        <li><span class="li-normal">params for cli_fmupdate_fdssetting_pushoverridetoclient_announceip:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_fmupdate_fdssetting_pushoverridetoclient_announceip.html#parameters">faz_cli_fmupdate_fdssetting_pushoverridetoclient_announceip</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_fmupdate_fdssetting_serveroverride_servlist:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_fmupdate_fdssetting_serveroverride_servlist.html#parameters">faz_cli_fmupdate_fdssetting_serveroverride_servlist</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_fmupdate_serveraccesspriorities_privateserver:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_fmupdate_serveraccesspriorities_privateserver.html#parameters">faz_cli_fmupdate_serveraccesspriorities_privateserver</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_fmupdate_webspam_fgdsetting_serveroverride_servlist:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_fmupdate_webspam_fgdsetting_serveroverride_servlist.html#parameters">faz_cli_fmupdate_webspam_fgdsetting_serveroverride_servlist</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_group:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_group.html#parameters">faz_cli_system_admin_group</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_group_member:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_group_member.html#parameters">faz_cli_system_admin_group_member</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_ldap:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_ldap.html#parameters">faz_cli_system_admin_ldap</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_ldap_adom:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>adom-name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_ldap_adom.html#parameters">faz_cli_system_admin_ldap_adom</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_profile:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>profileid</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_profile.html#parameters">faz_cli_system_admin_profile</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_profile_datamaskcustomfields:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>field-name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_profile_datamaskcustomfields.html#parameters">faz_cli_system_admin_profile_datamaskcustomfields</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_profile_writepasswdprofiles:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>profileid</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_profile_writepasswdprofiles.html#parameters">faz_cli_system_admin_profile_writepasswdprofiles</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_profile_writepasswduserlist:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>userid</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_profile_writepasswduserlist.html#parameters">faz_cli_system_admin_profile_writepasswduserlist</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_radius:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_radius.html#parameters">faz_cli_system_admin_radius</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_tacacs:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_tacacs.html#parameters">faz_cli_system_admin_tacacs</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_user:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>userid</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_user.html#parameters">faz_cli_system_admin_user</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_user_adom:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>adom-name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_user_adom.html#parameters">faz_cli_system_admin_user_adom</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_user_adomexclude:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>adom-name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_user_adomexclude.html#parameters">faz_cli_system_admin_user_adomexclude</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_user_dashboard:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>tabid</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_user_dashboard.html#parameters">faz_cli_system_admin_user_dashboard</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_user_dashboardtabs:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_user_dashboardtabs.html#parameters">faz_cli_system_admin_user_dashboardtabs</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_user_metadata:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>fieldname</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_user_metadata.html#parameters">faz_cli_system_admin_user_metadata</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_user_policyblock:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>policy_block_name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_user_policyblock.html#parameters">faz_cli_system_admin_user_policyblock</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_user_policypackage:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>policy-package-name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_user_policypackage.html#parameters">faz_cli_system_admin_user_policypackage</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_admin_user_restrictdevvdom:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>dev-vdom</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_admin_user_restrictdevvdom.html#parameters">faz_cli_system_admin_user_restrictdevvdom</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_alertevent:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_alertevent.html#parameters">faz_cli_system_alertevent</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_certificate_ca:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_certificate_ca.html#parameters">faz_cli_system_certificate_ca</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_certificate_crl:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_certificate_crl.html#parameters">faz_cli_system_certificate_crl</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_certificate_local:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_certificate_local.html#parameters">faz_cli_system_certificate_local</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_certificate_remote:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_certificate_remote.html#parameters">faz_cli_system_certificate_remote</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_certificate_ssh:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_certificate_ssh.html#parameters">faz_cli_system_certificate_ssh</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_csf_fabricconnector:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>serial</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_csf_fabricconnector.html#parameters">faz_cli_system_csf_fabricconnector</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_csf_trustedlist:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_csf_trustedlist.html#parameters">faz_cli_system_csf_trustedlist</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_ha_peer:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_ha_peer.html#parameters">faz_cli_system_ha_peer</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_ha_privatepeer:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_ha_privatepeer.html#parameters">faz_cli_system_ha_privatepeer</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_ha_vip:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_ha_vip.html#parameters">faz_cli_system_ha_vip</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_interface:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_interface.html#parameters">faz_cli_system_interface</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_interface_member:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>interface-name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_interface_member.html#parameters">faz_cli_system_interface_member</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_localinpolicy:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_localinpolicy.html#parameters">faz_cli_system_localinpolicy</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_localinpolicy6:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_localinpolicy6.html#parameters">faz_cli_system_localinpolicy6</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_log_devicedisable:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_log_devicedisable.html#parameters">faz_cli_system_log_devicedisable</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_log_maildomain:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_log_maildomain.html#parameters">faz_cli_system_log_maildomain</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_log_ratelimit_device:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_log_ratelimit_device.html#parameters">faz_cli_system_log_ratelimit_device</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_log_ratelimit_ratelimits:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_log_ratelimit_ratelimits.html#parameters">faz_cli_system_log_ratelimit_ratelimits</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_logfetch_clientprofile:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_logfetch_clientprofile.html#parameters">faz_cli_system_logfetch_clientprofile</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_logfetch_clientprofile_devicefilter:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_logfetch_clientprofile_devicefilter.html#parameters">faz_cli_system_logfetch_clientprofile_devicefilter</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_logfetch_clientprofile_logfilter:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_logfetch_clientprofile_logfilter.html#parameters">faz_cli_system_logfetch_clientprofile_logfilter</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_logforward:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_logforward.html#parameters">faz_cli_system_logforward</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_logforward_devicefilter:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_logforward_devicefilter.html#parameters">faz_cli_system_logforward_devicefilter</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_logforward_logfieldexclusion:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_logforward_logfieldexclusion.html#parameters">faz_cli_system_logforward_logfieldexclusion</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_logforward_logfilter:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_logforward_logfilter.html#parameters">faz_cli_system_logforward_logfilter</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_logforward_logmaskingcustom:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_logforward_logmaskingcustom.html#parameters">faz_cli_system_logforward_logmaskingcustom</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_mail:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_mail.html#parameters">faz_cli_system_mail</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_metadata_admins:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>fieldname</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_metadata_admins.html#parameters">faz_cli_system_metadata_admins</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_ntp_ntpserver:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_ntp_ntpserver.html#parameters">faz_cli_system_ntp_ntpserver</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_report_group:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>group-id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_report_group.html#parameters">faz_cli_system_report_group</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_report_group_chartalternative:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>chart-name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_report_group_chartalternative.html#parameters">faz_cli_system_report_group_chartalternative</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_report_group_groupby:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>var-name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_report_group_groupby.html#parameters">faz_cli_system_report_group_groupby</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_route:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>seq_num</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_route.html#parameters">faz_cli_system_route</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_route6:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>prio</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_route6.html#parameters">faz_cli_system_route6</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_saml_fabricidp:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>dev-id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_saml_fabricidp.html#parameters">faz_cli_system_saml_fabricidp</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_saml_serviceproviders:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_saml_serviceproviders.html#parameters">faz_cli_system_saml_serviceproviders</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_sniffer:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_sniffer.html#parameters">faz_cli_system_sniffer</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_snmp_community:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_snmp_community.html#parameters">faz_cli_system_snmp_community</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_snmp_community_hosts:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_snmp_community_hosts.html#parameters">faz_cli_system_snmp_community_hosts</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_snmp_community_hosts6:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_snmp_community_hosts6.html#parameters">faz_cli_system_snmp_community_hosts6</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_snmp_user:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_snmp_user.html#parameters">faz_cli_system_snmp_user</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_socfabric_trustedlist:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_socfabric_trustedlist.html#parameters">faz_cli_system_socfabric_trustedlist</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_sql_customindex:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_sql_customindex.html#parameters">faz_cli_system_sql_customindex</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_sql_customskipidx:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_sql_customskipidx.html#parameters">faz_cli_system_sql_customskipidx</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_sql_tsindexfield:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>category</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_sql_tsindexfield.html#parameters">faz_cli_system_sql_tsindexfield</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_sslciphersuites:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>priority</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_sslciphersuites.html#parameters">faz_cli_system_sslciphersuites</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_syslog:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_syslog.html#parameters">faz_cli_system_syslog</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_workflow_approvalmatrix:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>adom-name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_workflow_approvalmatrix.html#parameters">faz_cli_system_workflow_approvalmatrix</a> </span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_workflow_approvalmatrix_approver:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>seq_num</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_cli_system_workflow_approvalmatrix_approver.html#parameters">faz_cli_system_workflow_approvalmatrix_approver</a> </span></li>
        </ul>
        <li><span class="li-normal">params for dvmdb_adom:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_dvmdb_adom.html#parameters">faz_dvmdb_adom</a> </span></li>
        </ul>
        <li><span class="li-normal">params for dvmdb_device_vdom:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_dvmdb_device_vdom.html#parameters">faz_dvmdb_device_vdom</a> </span></li>
        </ul>
        <li><span class="li-normal">params for dvmdb_folder:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_dvmdb_folder.html#parameters">faz_dvmdb_folder</a> </span></li>
        </ul>
        <li><span class="li-normal">params for dvmdb_group:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_dvmdb_group.html#parameters">faz_dvmdb_group</a> </span></li>
        </ul>
        <li><span class="li-normal">params for eventmgmt_config_basichandler:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>handler_id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_eventmgmt_config_basichandler.html#parameters">faz_eventmgmt_config_basichandler</a> </span></li>
        </ul>
        <li><span class="li-normal">params for eventmgmt_config_correlationhandler:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>handler_id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_eventmgmt_config_correlationhandler.html#parameters">faz_eventmgmt_config_correlationhandler</a> </span></li>
        </ul>
        <li><span class="li-normal">params for eventmgmt_config_dataselector:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>selector_id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_eventmgmt_config_dataselector.html#parameters">faz_eventmgmt_config_dataselector</a> </span></li>
        </ul>
        <li><span class="li-normal">params for eventmgmt_config_notificationprofile:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>profile_id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_eventmgmt_config_notificationprofile.html#parameters">faz_eventmgmt_config_notificationprofile</a> </span></li>
        </ul>
        <li><span class="li-normal">params for eventmgmt_config_trigger:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_eventmgmt_config_trigger.html#parameters">faz_eventmgmt_config_trigger</a> </span></li>
        </ul>
        <li><span class="li-normal">params for eventmgmt_config_trigger_device:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_eventmgmt_config_trigger_device.html#parameters">faz_eventmgmt_config_trigger_device</a> </span></li>
        </ul>
        <li><span class="li-normal">params for eventmgmt_config_trigger_filter:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_eventmgmt_config_trigger_filter.html#parameters">faz_eventmgmt_config_trigger_filter</a> </span></li>
        </ul>
        <li><span class="li-normal">params for eventmgmt_config_trigger_filter_rule:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_eventmgmt_config_trigger_filter_rule.html#parameters">faz_eventmgmt_config_trigger_filter_rule</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_chart:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_chart.html#parameters">faz_report_config_chart</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_chart_drilldowntable:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>table_id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_chart_drilldowntable.html#parameters">faz_report_config_chart_drilldowntable</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_chart_tablecolumns:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_chart_tablecolumns.html#parameters">faz_report_config_chart_tablecolumns</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_chart_variabletemplate:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>var</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_chart_variabletemplate.html#parameters">faz_report_config_chart_variabletemplate</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_dataset:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_dataset.html#parameters">faz_report_config_dataset</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_dataset_variable:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>var</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_dataset_variable.html#parameters">faz_report_config_dataset_variable</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_layout:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>layout_id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_layout.html#parameters">faz_report_config_layout</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_layout_component:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>component_id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_layout_component.html#parameters">faz_report_config_layout_component</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_layout_component_variable:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>var</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_layout_component_variable.html#parameters">faz_report_config_layout_component_variable</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_layout_footer:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>footer_id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_layout_footer.html#parameters">faz_report_config_layout_footer</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_layout_header:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>header_id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_layout_header.html#parameters">faz_report_config_layout_header</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_layoutfolder:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>folder_id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_layoutfolder.html#parameters">faz_report_config_layoutfolder</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_macro:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_macro.html#parameters">faz_report_config_macro</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_output:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_output.html#parameters">faz_report_config_output</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_output_emailrecipients:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>address</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_output_emailrecipients.html#parameters">faz_report_config_output_emailrecipients</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_schedule:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_schedule.html#parameters">faz_report_config_schedule</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_schedule_addressfilter:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_schedule_addressfilter.html#parameters">faz_report_config_schedule_addressfilter</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_schedule_devices:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>devices_name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_schedule_devices.html#parameters">faz_report_config_schedule_devices</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_schedule_filter:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>name</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_schedule_filter.html#parameters">faz_report_config_schedule_filter</a> </span></li>
        </ul>
        <li><span class="li-normal">params for report_config_schedule_reportlayout:</span></li>
        <ul class="ul-self">
            
            <li><span class="li-normal">required primary key: <b>layout_id</b> </span></li>
            <li><span class="li-normal">optional params list: <a href="docgen/faz_report_config_schedule_reportlayout.html#parameters">faz_report_config_schedule_reportlayout</a> </span></li>
        </ul>
    </ul>
    </div>
    </section>

 <li><span class="li-head">selector</span> selector of the renamed object <span class="li-normal">type: str</span> <span class="li-required">choices:</span></li>
    <li style="list-style: none;"><section class="accordion">
    <input type="checkbox" name="collapse" id="handle2">
    <h2 class="handle">
        <label for="handle2"><u>Show full selector list...</u></label>
    </h2>
    <div class="content">
    <ul class="ul-self">
        <li><span class="li-required">cli_fmupdate_fdssetting_pushoverridetoclient_announceip</span> - available versions:
            <span class="li-normal">>= 6.2.1</span>
        </li>
        <li><span class="li-required">cli_fmupdate_fdssetting_serveroverride_servlist</span> - available versions:
            <span class="li-normal">>= 6.2.1</span>
        </li>
        <li><span class="li-required">cli_fmupdate_serveraccesspriorities_privateserver</span> - available versions:
            <span class="li-normal">>= 6.2.1</span>
        </li>
        <li><span class="li-required">cli_fmupdate_webspam_fgdsetting_serveroverride_servlist</span> - available versions:
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
        <li><span class="li-required">cli_system_alertevent</span> - available versions:
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
        <li><span class="li-required">cli_system_certificate_remote</span> - available versions:
            <span class="li-normal">>= 6.2.1</span>
        </li>
        <li><span class="li-required">cli_system_certificate_ssh</span> - available versions:
            <span class="li-normal">>= 6.2.1</span>
        </li>
        <li><span class="li-required">cli_system_csf_fabricconnector</span> - available versions:
            <span class="li-normal">>= 7.4.1</span>
        </li>
        <li><span class="li-required">cli_system_csf_trustedlist</span> - available versions:
            <span class="li-normal">>= 7.4.1</span>
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
        <li><span class="li-required">cli_system_interface_member</span> - available versions:
            <span class="li-normal">>= 6.4.9</span>
        </li>
        <li><span class="li-required">cli_system_localinpolicy</span> - available versions:
            <span class="li-normal">>= 7.2.0</span>
        </li>
        <li><span class="li-required">cli_system_localinpolicy6</span> - available versions:
            <span class="li-normal">>= 7.2.0</span>
        </li>
        <li><span class="li-required">cli_system_log_devicedisable</span> - available versions:
            <span class="li-normal">>= 6.4.4</span>
        </li>
        <li><span class="li-required">cli_system_log_maildomain</span> - available versions:
            <span class="li-normal">>= 6.2.1</span>
        </li>
        <li><span class="li-required">cli_system_log_ratelimit_device</span> - available versions:
            <span class="li-normal">6.4.8-7.0.2</span>
        </li>
        <li><span class="li-required">cli_system_log_ratelimit_ratelimits</span> - available versions:
            <span class="li-normal">>= 7.0.3</span>
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
        <li><span class="li-required">cli_system_mail</span> - available versions:
            <span class="li-normal">>= 6.2.1</span>
        </li>
        <li><span class="li-required">cli_system_metadata_admins</span> - available versions:
            <span class="li-normal">>= 6.2.1</span>
        </li>
        <li><span class="li-required">cli_system_ntp_ntpserver</span> - available versions:
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
        <li><span class="li-required">cli_system_route</span> - available versions:
            <span class="li-normal">>= 6.2.1</span>
        </li>
        <li><span class="li-required">cli_system_route6</span> - available versions:
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
        <li><span class="li-required">cli_system_snmp_user</span> - available versions:
            <span class="li-normal">>= 6.2.1</span>
        </li>
        <li><span class="li-required">cli_system_socfabric_trustedlist</span> - available versions:
            <span class="li-normal">>= 7.4.0</span>
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
        <li><span class="li-required">cli_system_syslog</span> - available versions:
            <span class="li-normal">>= 6.2.1</span>
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
        <li><span class="li-required">dvmdb_device_vdom</span> - available versions:
            <span class="li-normal">>= 6.2.1</span>
        </li>
        <li><span class="li-required">dvmdb_folder</span> - available versions:
            <span class="li-normal">>= 6.4.2</span>
        </li>
        <li><span class="li-required">dvmdb_group</span> - available versions:
            <span class="li-normal">>= 6.2.1</span>
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
    </ul>
    </div>
    </section>

 <li><span class="li-head">self</span> The parameter for each selector <span class="li-normal">type: dict</span> <span class="li-required">choices:</span></li>
   <li style="list-style: none;"><section class="accordion">
   <input type="checkbox" name="collapse" id="handle3">
    <h2 class="handle">
        <label for="handle3"><u>More details about parameter: <b>self</b>...</u></label>
    </h2>
    <div class="content">
    <ul class="ul-self">
        <li><span class="li-normal">params for cli_fmupdate_fdssetting_pushoverridetoclient_announceip:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">announce-ip</span></li>
        </ul>
        <li><span class="li-normal">params for cli_fmupdate_fdssetting_serveroverride_servlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">servlist</span></li>
        </ul>
        <li><span class="li-normal">params for cli_fmupdate_serveraccesspriorities_privateserver:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">private-server</span></li>
        </ul>
        <li><span class="li-normal">params for cli_fmupdate_webspam_fgdsetting_serveroverride_servlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">servlist</span></li>
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
        <li><span class="li-normal">params for cli_system_admin_user_policyblock:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">policy-block</span></li>
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
        <li><span class="li-normal">params for cli_system_alertevent:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">alert-event</span></li>
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
        <li><span class="li-normal">params for cli_system_certificate_remote:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">remote</span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_certificate_ssh:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">ssh</span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_csf_fabricconnector:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">fabric-connector</span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_csf_trustedlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">trusted-list</span></li>
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
        <li><span class="li-normal">params for cli_system_log_devicedisable:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device-disable</span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_log_maildomain:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">mail-domain</span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_log_ratelimit_device:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_log_ratelimit_ratelimits:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">ratelimits</span></li>
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
        <li><span class="li-normal">params for cli_system_mail:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">mail</span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_metadata_admins:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">admins</span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_ntp_ntpserver:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">ntpserver</span></li>
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
        <li><span class="li-normal">params for cli_system_route:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">route</span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_route6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">route6</span></li>
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
        <li><span class="li-normal">params for cli_system_snmp_user:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">user</span></li>
        </ul>
        <li><span class="li-normal">params for cli_system_socfabric_trustedlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">trusted-list</span></li>
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
        <li><span class="li-normal">params for cli_system_syslog:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">syslog</span></li>
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
        <li><span class="li-normal">params for eventmgmt_config_basichandler:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">basic-handler</span></li>
        </ul>
        <li><span class="li-normal">params for eventmgmt_config_correlationhandler:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">correlation-handler</span></li>
        </ul>
        <li><span class="li-normal">params for eventmgmt_config_dataselector:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">data-selector</span></li>
        </ul>
        <li><span class="li-normal">params for eventmgmt_config_notificationprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">notification-profile</span></li>
        </ul>
        <li><span class="li-normal">params for eventmgmt_config_trigger:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">trigger</span></li>
        </ul>
        <li><span class="li-normal">params for eventmgmt_config_trigger_device:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">trigger_id</span></li>
        </ul>
        <li><span class="li-normal">params for eventmgmt_config_trigger_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">filter</span></li>
            <li><span class="li-normal">trigger_id</span></li>
        </ul>
        <li><span class="li-normal">params for eventmgmt_config_trigger_filter_rule:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">filter_id</span></li>
            <li><span class="li-normal">rule</span></li>
            <li><span class="li-normal">trigger_id</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_chart:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">chart</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_chart_drilldowntable:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">chart_name</span></li>
            <li><span class="li-normal">drill-down-table</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_chart_tablecolumns:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">chart_name</span></li>
            <li><span class="li-normal">table-columns</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_chart_variabletemplate:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">chart_name</span></li>
            <li><span class="li-normal">variable-template</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_dataset:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">dataset</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_dataset_variable:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">dataset_name</span></li>
            <li><span class="li-normal">variable</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_layout:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">layout</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_layout_component:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">component</span></li>
            <li><span class="li-normal">layout-id</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_layout_component_variable:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">component-id</span></li>
            <li><span class="li-normal">layout-id</span></li>
            <li><span class="li-normal">variable</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_layout_footer:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">footer</span></li>
            <li><span class="li-normal">layout-id</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_layout_header:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">header</span></li>
            <li><span class="li-normal">layout-id</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_layoutfolder:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">layout-folder</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_macro:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">macro</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_output:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">output</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_output_emailrecipients:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">email-recipients</span></li>
            <li><span class="li-normal">output-name</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_schedule:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">schedule</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_schedule_addressfilter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">address-filter</span></li>
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">schedule_name</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_schedule_devices:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">devices</span></li>
            <li><span class="li-normal">schedule_name</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_schedule_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">filter</span></li>
            <li><span class="li-normal">schedule_name</span></li>
        </ul>
        <li><span class="li-normal">params for report_config_schedule_reportlayout:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">adom</span></li>
            <li><span class="li-normal">report-layout</span></li>
            <li><span class="li-normal">schedule_name</span></li>
        </ul>
    </ul>
    </div>
    </section>
 </ul>
 </ul>
 </ul>


Notes
-----
.. note::

   - Selector is a mandatory parameter for the module, and the params is varying depending on the selector.
   - Semantic description for the module: rename ``self`` as new ``target``
   - Normally, running one module can fail when a non-zero rc is returned. you can also override the conditions to fail or succeed with parameters rc_failed and rc_succeeded


Examples
--------

.. code-block:: yaml+jinja

  - name: Rename a resource.
    connection: httpapi
    hosts: fortianalyzers
    vars:
      ansible_httpapi_port: 443
      ansible_httpapi_use_ssl: true
      ansible_httpapi_validate_certs: false
    tasks:
      - name: Create device group table.
        fortinet.fortianalyzer.faz_dvmdb_group:
          adom: root
          dvmdb_group:
            name: foogroup
            os_type: unknown
            type: normal
          state: present
      - name: Rename device group table.
        fortinet.fortianalyzer.faz_rename:
          rename:
            selector: dvmdb_group
            self:
              adom: root
              group: foogroup
            target:
              name: "foogroup_renamed"
      - name: Get device group table information.
        fortinet.fortianalyzer.faz_fact:
          facts:
            selector: dvmdb_group
            params:
              adom: root
              group: foogroup
        register: info
        failed_when: info.rc == 0
      - name: Delete device group table.
        fortinet.fortianalyzer.faz_dvmdb_group:
          adom: root
          state: absent
          dvmdb_group:
            name: foogroup_renamed



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