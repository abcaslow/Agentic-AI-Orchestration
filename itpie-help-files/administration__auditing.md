# Auditing

Source: ITPIE:OPS Documentation — Auditing
Source URL: https://itpie-hostname/documentation/content/administration/auditing.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Auditing
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] The application implements several categories of auditable events.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Logging
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Auditable event messages are written to the service log at the "Information" level using an event ID in the 1000-1999 range. The message should include identification of the component performing the auditable activity, beginning with "ITPIE". Except for application lifecycle events, which should be logged by the Microsoft hosting subsystem.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Example configuration enabling all categories of audit event messages:
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] { "Logging": { "LogLevel": { "Default": "Information", "Microsoft": "Warning", "Microsoft.Hosting.Lifetime": "Information" } } }
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Log format
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Event messages use statically defined message templates, with the template being filled out by the calling component using local context. The message template includes, generally, the following fields.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Other fields are specific to the auditable event and/or feature context, while the certain parts are provided by the logging subsystem.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Remote Address: The IP address (IPv4 or IPv6) of the connection to the application server that initiated or caused the auditable event. This is usually a user's client/machine address and may be associated with their username.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Username: The authenticated username, in the case of an authenticated event; or, the anonymous username, if available from local context, in the case of an authentication attempt or an allowed anonymous event.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Reason: A human-readable reason for a failure, in the case of a failed auditable event.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Example of an auditable event message template:
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': User log in.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Example of a complete auditable event message template:
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] {Timestamp} {LogLevel}: {LogCategory}[{EventId}] {Timestamp} [{RemoteAddress}] '{AuthenticatedUserName}': User log in.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Example of the complete auditable event message, as written in the log:
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 2024-01-01 10:00:00 info: ITPIE.API.Identity.Controllers.IdentityController[1000] 2024-01-01 10:00:00 [::1] 'user@example.com': User log in.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Event categories
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Auditable events include activities in the following categories.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Application lifecycle
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Application lifecycle events are auditable. These are logged automatically by the Microsoft ASP.NET Core hosting subsystem. We do not have control over these message tempates or event IDs. We reproduce them here completely for reference.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Example application started:
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] info: Microsoft.Hosting.Lifetime[14] Microsoft.Hosting.Lifetime: Information: Now listening on: https://[::]:443 info: Microsoft.Hosting.Lifetime[0] Microsoft.Hosting.Lifetime: Information: Application started. Press Ctrl+C to shut down. info: Microsoft.Hosting.Lifetime[0] Microsoft.Hosting.Lifetime: Information: Hosting environment: Production info: Microsoft.Hosting.Lifetime[0] Microsoft.Hosting.Lifetime: Information: Content root path: /opt/itpie/itpie-server/
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Example application shut down:
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] info: Microsoft.Hosting.Lifetime[0] Microsoft.Hosting.Lifetime: Information: Application is shutting down...
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] User log in
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] User log in attempts via local user account and/or external identity provider, if configured, are auditable, including some self-service workflows, like password changes.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1000: User log in.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': User log in.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1001: User log in failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AnonymousUserName}': User log in. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1002: User log out.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': User log out.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1003: User log out failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': User log out. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1004: User change password.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AnonymousOrAuthenticatedUserName}': User change password.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1005: User change password failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AnonymousOrAuthenticatedUserName}': User change password. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1006: User external log in.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': User external log in with '{ExternalIdentityProviderDisplayName}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1007: User external log in failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AnonymousUserName}': User external log in with '{ExternalIdentityProviderDisplayName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Sessions
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] The user session lifecycle is auditable.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1100: Create user session.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Create user session for '{UserName}': '{SessionKeyHash}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1101: Create user session failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Create user session for '{UserName}': '{SessionKeyHash}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1102: Renew user session.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Renew user session for '{UserName}': Expires on '{SessionExpires}': '{SessionKeyHash}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1103: Renew user session failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Renew user session for '{UserName}': '{SessionKeyHash}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1104: Remove user session.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Remove user session for '{UserName}': '{SessionKeyHash}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1105: Remove user session failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Remove user session for '{UserName}': '{SessionKeyHash}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1106: Remove expired user session.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Remove expired user session for '{UserName}': Last activity on '{SessionLastActivity}': Expires on '{SessionExpires}': '{SessionKeyHash}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1107: Remove expired user session failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Remove expired user session for '{UserName}': Last activity on '{SessionLastActivity}': Expires on '{SessionExpires}': '{SessionKeyHash}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1108: Remove max-age user session.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Remove max-age user session for '{UserName}': Created on '{SessionCreated}': '{SessionKeyHash}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1109: Remove max-age user session failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Remove max-age user session for '{UserName}': Created on '{SessionCreated}': '{SessionKeyHash}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] User management
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] All user management activities are auditable, including changes to security levels .
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1200: Create user.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Create user: '{TargetUserName}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1201: Create user failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Create user: '{TargetUserName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1202: Reset user password.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Reset user password: '{TargetUserName}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1203: Reset user password failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Reset user password: '{TargetUserName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1204: Enable user.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Enable user: '{TargetUserName}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1205: Enable user failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Enable user: '{TargetUserName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1206: Disable user.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Disable user: '{TargetUserName}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1207: Disable user failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Disable user: '{TargetUserName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1208: Unlock user.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Unlock user: '{TargetUserName}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1209: Unlock user failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Unlock user: '{TargetUserName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1210: Reactivate user.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Reactivate user: '{TargetUserName}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1211: Reactivate user failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Reactivate user: '{TargetUserName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1212: Assign feature access.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Assign feature access: '{TargetUserName}': {FeatureName}={AccessLevel}.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1213: Assign feature access failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Assign feature access: '{TargetUserName}': {FeatureName}={AccessLevel}. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1214: Assign superuser.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Assign superuser: '{TargetUserName}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1215: Assign superuser failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Assign superuser: '{TargetUserName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1216: Remove superuser.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Remove superuser: '{TargetUserName}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1217: Remove superuser failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Remove superuser: '{TargetUserName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1218: Remove user session.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Remove user session: '{TargetUserName}': '{SessionKeyHash}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1219: Remove user session failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Remove user session: '{TargetUserName}': '{SessionKeyHash}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1220: Remove user external login.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Remove user external login: '{TargetUserName}': '{LoginProvider} ({ProviderKey})'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1221: Remove user external login failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Remove user external login: '{TargetUserName}': '{LoginProvider} ({ProviderKey})'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1222: Associate OUs.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Associate OUs: '{TargetUserName}': '{OuNames}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1223: Associate OUs failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Associate OUs: '{TargetUserName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1224: Delete user.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Delete user: '{TargetUserName}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1225: Delete user failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Delete user: '{TargetUserName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1226: Add emergency account permission.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Add emergency account permission: '{TargetUserName}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1227: Add emergency account permission failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Add emergency account permission: '{TargetUserName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1228: Remove emergency account permission.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Remove emergency account permission: '{TargetUserName}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1229: Remove emergency account permission failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Remove emergency account permission: '{TargetUserName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1230: Unassign feature access.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Unassign feature access: '{TargetUserName}': {FeatureName}.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1231: Unassign feature access failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Unassign feature access: '{TargetUserName}': {FeatureName}. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] OU management
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] All OU management activities are auditable, as OUs are currently the only implementation of security objects .
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1300: Create OU.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Create OU: '{OuName}' (Parent: '{ParentOuName}').
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1301: Create OU failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Create OU: '{OuName}' (Parent: '{ParentOuName}'). FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1302: Rename OU.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Rename OU: '{OuNameBefore}' to '{OuNameAfter}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1303: Rename OU failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Rename OU: '{OuNameBefore}' to '{OuNameAfter}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1304: Move OU.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Move OU: '{OuName}' from '{ParentOuNameBefore}' to '{ParentOuNameAfter}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1305: Move OU failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Move OU: '{OuName}' from '{ParentOuNameBefore}' to '{ParentOuNameAfter}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1306: Remove OU.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Remove OU: '{OuName}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1307: Remove OU failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Remove OU: '{OuName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1308: Associate OU.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Associate OU: '{OuName}' to '{TargetUserName}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1309: Associate OU failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Associate OU: '{OuName}' to '{TargetUserName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1310: Disassociate OU.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Disassociate OU: '{OuName}' from '{TargetUserName}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1311: Disassociate OU failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Disassociate OU: '{OuName}' from '{TargetUserName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Authentication
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Tip
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Some application settings require the service to be restarted to make the change effective. If the change is reverted, the restart is not required, but should be recorded nonetheless.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Configuring authenticators and setting the authentication profile are auditable events.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1400: Set authentication profile.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Set authentication profile: '{ProfileName}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1401: Set authentication profile failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Set authentication profile: '{ProfileName}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1402: Create external identity provider.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Create external identity provider: {DisplayName}.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1403: Create external identity provider failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Create external identity provider: {DisplayName}. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1404: Delete external identity provider.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Delete external identity provider: {DisplayName}.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1406: Enable external identity provider.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Enable external identity provider: {DisplayName}.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1408: Disable external identity provider.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Disable external identity provider: {DisplayName}.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1410: Configure external identity provider.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Configure external identity provider: {DisplayName}. Settings: {Settings}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1412: Rename external identity provider.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Rename external identity provider. From: {FromDisplayName}. To: {ToDisplayName}.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1413: Rename external identity provider failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Rename external identity provider. From: {FromDisplayName}. To: {ToDisplayName}. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1414: Reorder external identity providers.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Reorder external identity providers: {DisplayNames}.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] External services
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] All external services connection attempts are auditable events. A configured host name should be resolved to one or more IP addresses, for the purposes of logging, although we cannot tell which IP address was resolved for the actual connection.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1500: Connect to external service by address.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Connect to external service: [{ServiceAddress}].
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1501: Connect to external service by address failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Connect to external service: [{ServiceAddress}]. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1502: Connect to external service by hostname.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Connect to external service: {ServiceName} ([{ServiceAddresses}]).
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1503: Connect to external service by hostname failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Connect to external service: {ServiceName} ([{ServiceAddresses}]). FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Categories of sensitive information
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Changes to categories of sensitive information including configuring the data classification feature is an auditable event.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1600: Enable data classification.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Enable data classification.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1601: Enable data classification failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Enable data classification. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1602: Disable data classification.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Disable data classification.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1603: Disable data classification failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Disable data classification. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1604: Set data classification level.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Set data classification level: '{ClassificationLevel}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1605: Set data classification level failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Set data classification level: '{ClassificationLevel}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Access tokens
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1700: Create access token.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Create access token: '{TokenKeyHash}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1701: Create access token failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Create access token: '{TokenKeyHash}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1702: Delete access token.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Delete access token: '{TokenKeyHash}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1703: Delete access token failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Delete access token: '{TokenKeyHash}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Remote agents
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1800: Seen agent.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}]: Seen agent: '{IdentifierHash}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1801: Seen agent failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}]: Seen agent: '{IdentifierHash}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1802: Authorize agent.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Authorize agent: '{IdentifierHash}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1803: Authorize agent failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Authorize agent: '{IdentifierHash}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1804: Deauthorize agent.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Deauthorize agent: '{IdentifierHash}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1805: Deauthorize agent failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Deauthorize agent: '{IdentifierHash}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1806: Connect agent.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}]: Connect agent: '{IdentifierHash}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1807: Connect agent failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}]: Connect agent: '{IdentifierHash}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1808: Disconnect agent.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Disconnect agent: '{IdentifierHash}'.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1809: Disconnect agent failed.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Disconnect agent: '{IdentifierHash}'. FAILED: {Reason}
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] Authorization
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1900: Assign default feature access.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Assign default feature access: {FeatureName}={AccessLevel}.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] 1901: Assign default OU access.
[ITPIE:OPS Documentation | Auditing | https://itpie-hostname/documentation/content/administration/auditing.html] [{RemoteAddress}] '{AuthenticatedUserName}': Assign default OU access: OuId={ouId}.