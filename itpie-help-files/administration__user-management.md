# User Management

Source: ITPIE:OPS Documentation — User Management
Source URL: https://itpie-hostname/documentation/content/administration/user-management.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] User Management
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] A user management command-line interface is provided for automated bootstrapping and emergency situations.
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] Auditing
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] INFO
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] User account modifications are auditable events .
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] When the application service is running as a Systemd unit, auditable event messages should be logged to the same Syslog source. For example:
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] Command-line interface
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] You should execute the command-line interface as a local user with access to application configuration. This is typically the itpie account created by the application package (RPM) during installation. The current working directory should also be owned by or accessible to that account, such as: /var/lib/itpie or /opt/itpie/itpie-server .
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] $ cd /opt/itpie/itpie-server $ sudo -u itpie ./itpie-server user-management --help
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] Usage
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] Command Description
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] list Lists user accounts
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] create <username> Creates a new user account
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] enable <username> Enables a user account
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] disable <username> Disables a user account
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] unlock <username> Unlocks an user account
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] reset-password <username> Resets the password on a user account
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] reactivate <username> Reactivates an inactive user account
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] superuser list Lists superusers
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] superuser create <username> Creates a new superuser
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] superuser add <username> Adds superuser permissions
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] superuser remove <username> Removes superuser permissions
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] emergency-account list Lists emergency accounts
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] emergency-account create <username> Creates a new emergency account
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] emergency-account add <username> Adds emergency account permissions
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] emergency-account remove <username> Removes emergency account permissions
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] Scenarios
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] Emergency account access
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] If you need to recover access to the system due to an outage of an external identity provider, create an emergency account with a one-time use password.
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] $ sudo -u itpie /opt/itpie/itpie-server/itpie-server user-management emergency-account create 'emergency-account@example.com'
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] Automated bootstrap
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] If you need to automate the boostrapping of a system install including an initial superuser account creation.
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/administration/user-management.html] $ sudo -u itpie /opt/itpie/itpie-server/itpie-server user-management superuser create $ITPIE_BOOTSTRAP_USERNAME --password $ITPIE_BOOTSTRAP_PASSWORD