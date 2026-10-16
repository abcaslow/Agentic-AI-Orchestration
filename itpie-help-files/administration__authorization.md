# Authorization

Source: ITPIE:OPS Documentation — Authorization
Source URL: https://itpie-hostname/documentation/content/administration/authorization.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Authorization
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] The application supports several categories of security levels, which provide permissions or authorization capabilities to users.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Security levels
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] A security level denotes a permission or authorization capability within the application.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Emergency account
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] A user with emergency account permission is a kind of "account of last resort" for use in bootstrapping and emergencies. An emergency account is exempt from user inactivity and password max-age checks, but otherwise participates in authentication workflows. A user with the emergency account permission is always allowed to attempt a password login even if external identity providers are configured.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] For all other considerations, a user with emergency account permission also has the superuser permission.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Superuser
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] A user with the superuser permission acts as a kind of "application administrator". A superuser, generally, has the following permissions:
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Configures application server functionality, including authenticators and external services.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Manages local users and local user sessions.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Bypasses feature access, effectively configure permission on every feature.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Bypasses OU associations, viewing data from any and all OUs.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] The following features require superuser access: Export, Collection
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Feature access
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Feature access is a permission scheme for protecting access to certain feature functionality, resources, and pages.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Search and Discovery
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Maps
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Config Backup
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Network Data
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Custom Reports
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] ZoneViz
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Access levels
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Tip
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] A “higher” access level will inherit the “lower” access levels.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] The access levels are defined, in general, as below, but each feature may implement these access levels in different ways (see the feature specific authorization information).
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] None: The user is not allowed to access the feature.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Read: The user is allowed to read feature resources or view feature pages.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Write: The user is allowed to create feature resources.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Configure: The user is allowed to configure the feature.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Security objects
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] A security object is an application object or data element that grants privileges to an associated user.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] Access tokens
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] The user's generated access token(s) can be used externally, as in cURL scripts, to access the application API as the user.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] OU associations
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] The organizational unit (OU) is a method of organizing network targets and data into hierarchies.
[ITPIE:OPS Documentation | Authorization | https://itpie-hostname/documentation/content/administration/authorization.html] A user's view of network targets and data should be filtered through the OU hierarchies with which they are associated. Every feature should take this into account when constructing queries and displaying data.