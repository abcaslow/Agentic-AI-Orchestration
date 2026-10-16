# OpenID Connect (OIDC)

Source: ITPIE:OPS Documentation — OpenID Connect (OIDC)
Source URL: https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/oidc.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | OpenID Connect (OIDC) | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/oidc.html] OpenID Connect (OIDC)
[ITPIE:OPS Documentation | OpenID Connect (OIDC) | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/oidc.html] The application may be configured to authenticate with an identity provider that implements OpenID Connect (OIDC), like Keycloak.
[ITPIE:OPS Documentation | OpenID Connect (OIDC) | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/oidc.html] Settings
[ITPIE:OPS Documentation | OpenID Connect (OIDC) | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/oidc.html] Display Name: The unique display name for this provider.
[ITPIE:OPS Documentation | OpenID Connect (OIDC) | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/oidc.html] Enabled: Whether the provider is enabled for log in.
[ITPIE:OPS Documentation | OpenID Connect (OIDC) | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/oidc.html] Connection
[ITPIE:OPS Documentation | OpenID Connect (OIDC) | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/oidc.html] Authority: The URL of the Authority to connect to for OIDC calls. This is sometimes referred to as the Server Realm.
[ITPIE:OPS Documentation | OpenID Connect (OIDC) | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/oidc.html] https://keycloak.example.com/auth/realms/master
[ITPIE:OPS Documentation | OpenID Connect (OIDC) | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/oidc.html] Metadata Address: The URL of the discovery endpoint for obtaining metadata. This can usually be inferred from the Authority URL. Optional.
[ITPIE:OPS Documentation | OpenID Connect (OIDC) | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/oidc.html] https://keycloak.example.com/auth/realms/master/.well-known/openid-configuration
[ITPIE:OPS Documentation | OpenID Connect (OIDC) | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/oidc.html] Client ID: The OIDC client ID.
[ITPIE:OPS Documentation | OpenID Connect (OIDC) | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/oidc.html] Client Secret: The OIDC client secret.
[ITPIE:OPS Documentation | OpenID Connect (OIDC) | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/oidc.html] Requirements
[ITPIE:OPS Documentation | OpenID Connect (OIDC) | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/oidc.html] See the OIDC provider's documentation for creating a client application, for example:
[ITPIE:OPS Documentation | OpenID Connect (OIDC) | https://itpie-hostname/documentation/content/features/settings/configuration/external-identity-providers/oidc.html] https://www.keycloak.org/docs/latest/authorization_services/index.html#_resource_server_create_client