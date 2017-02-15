zarafa-webapp-passwd
====================

The Passwd plugin allows the user to change the current user password inside of WebApp.

This plugin is largely based on the Passwd plugin by Andreas Brodowski.
For his original work check this [link](https://community.zarafa.com/pg/plugins/project/157/developer/dw2412/passwd-plugin)

## How to install
1.  If you want to use this plugin with production / debug version of webapp then unzip ./builds/passwd-1.3.zip in <webapp_path>/plugins directory
2.  [ATTENTION NOT TESTED on Kopano] If you are using LDAP plugin then change PLUGIN_PASSWD_LDAP to true and also set proper values for PLUGIN_PASSWD_LDAP_BASEDN and PLUGIN_PASSWD_LDAP_URI configurations
2a. If you are using DB plugin then no need to change anything, default configurations should be fine
4.  Restart apache, reload webapp after clearing cache
5.  If you want to enable this plugin by default for all users then edit config.php file and change PLUGIN_PASSWD_USER_DEFAULT_ENABLE setting to true

## How to enable
1. Go to settings section
2. Go to Plugins tab
3. Enable password change plugin and reload webapp

## How to use
1. Go to Change Password tab of settings section
2. Provide current password and new password
3. Click on apply
4. If password change is success you will be logged out

## How to disable
1. Go to settings section
2. Go to Plugins tab
3. Disable password change plugin and reload webapp

## Notes
- Feedback/Bug Reports are welcome
- thanks to h44z for adding password meter and icon for the plugin
