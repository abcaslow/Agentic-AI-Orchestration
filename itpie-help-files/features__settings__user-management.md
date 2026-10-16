# User Management

Source: ITPIE:OPS Documentation — User Management
Source URL: https://itpie-hostname/documentation/content/features/settings/user-management.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] User Management
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Note
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] See Authentication and Authorization for more details on user status, access, and permissions.
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] This page supports creating, viewing, updating, and removing users from the system. This page is only accessible to super users.
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] User List
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] The user list shows all of the users in the system with details to aid in user management tasks. For example:
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Filter the last login column to see who has never logged in.
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Sort the last activity column to see who used the application recently.
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Display statuses that affect a user's ability to log in.
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] A super user can use the action buttons in the edit user drawer to change these statuses.
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Edit User
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Click the "Edit" action button beside a user to open the edit user drawer. This drawer can be used to view user details and to change user permissions, including:
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Super User
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Feature Access
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] OU Access
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Changing super user or feature access will require reauthentication by the changed user (all of their active sessions will be removed).
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Relevant action buttons will be displayed at the bottom of the edit user drawer depending on the user's status.
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] INFO
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Emergency accounts may not be disabled, have their sessions revoked, or their password reset on the User Management | Edit form.
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] INFO
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Users may not disable themselves, remove their own sessions, or reset their own password from the User Management | Edit form. However, they may manage their own session, passwords, and access tokens from the Settings | Profile page.
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Enable / Disable : Enable or disable a user. Disabling a user will remove all of their active sessions (requiring reauthentication if they are subsequently enabled).
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Reactivate : Reactivate an inactive user.
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Unlock : Unlock a locked-out user.
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Log out all sessions : Remove all active sessions from a user (requiring reauthentication).
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Remove Access Tokens : Remove all access tokens from a user (requiring them to create new access tokens for API access).
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Reset password : Reset the user's password with a new one-time use password. The new password will be displayed only once and must be sent securely to the user.
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Add User
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Click the "Add" user button to open the add user drawer. A new user requires a unique email and may be assigned permissions at this time or later using the "Edit" user action. A new user will be assigned a one-time use password, which will be displayed only once and should be sent securely to the user.
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Import Users
[ITPIE:OPS Documentation | User Management | https://itpie-hostname/documentation/content/features/settings/user-management.html] Click the "Import Users" button to show the import users page. Follow the instructions on the page to import any number of users with predefined permissions and OU access.