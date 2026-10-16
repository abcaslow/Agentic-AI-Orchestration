# WS-Federation

Source: ITPIE:OPS Documentation — WS-Federation
Source URL: https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/ws-federation.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | WS-Federation | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/ws-federation.html] WS-Federation
[ITPIE:OPS Documentation | WS-Federation | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/ws-federation.html] The application may be configured to authenticate with an identity provider that implements WS-Federation, commonly Microsoft Active Directory .
[ITPIE:OPS Documentation | WS-Federation | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/ws-federation.html] Settings
[ITPIE:OPS Documentation | WS-Federation | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/ws-federation.html] Display Name: The unique display name for this provider.
[ITPIE:OPS Documentation | WS-Federation | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/ws-federation.html] Enabled: Whether the provider is enabled for log in.
[ITPIE:OPS Documentation | WS-Federation | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/ws-federation.html] Connection
[ITPIE:OPS Documentation | WS-Federation | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/ws-federation.html] Metadata Address: The URL of the federation metadata document. This is different for every environment and should be provided by your organization's system adminstrator. For example:
[ITPIE:OPS Documentation | WS-Federation | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/ws-federation.html] https://adfs.corp.example.com/FederationMetadata/2007-06/FederationMetadata.xml
[ITPIE:OPS Documentation | WS-Federation | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/ws-federation.html] Realm: Often the application's URL, called the "relaying party" by ADFS. This is different for every environment and should be provided by your organization's system administrator. For example:
[ITPIE:OPS Documentation | WS-Federation | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/ws-federation.html] https://itpie.corp.example.com
[ITPIE:OPS Documentation | WS-Federation | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/ws-federation.html] Requirements
[ITPIE:OPS Documentation | WS-Federation | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/ws-federation.html] The application requires the following claims to be configured. Note: this is just an example, your organization's configuration may be different. For a typical environment, this configuration should work.
[ITPIE:OPS Documentation | WS-Federation | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/ws-federation.html] A unique identifier for Name ID in your WS-Federation Transform Rules. UPN is preferred but sAMAAccountName for single-domain forests is acceptable.
[ITPIE:OPS Documentation | WS-Federation | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/ws-federation.html] An email address for email in your LDAP Attribute Mapping