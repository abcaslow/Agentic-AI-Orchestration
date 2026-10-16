# External Services

Source: ITPIE:OPS Documentation — External Services
Source URL: https://itpie-hostname/documentation/content/administration/external-services.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] External Services
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] INFO
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] External service connection attempts are auditable events .
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] The application server may be configured to connect to external services in order to provide optional functionality.
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] Settings
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] Following are a general pattern for external service settings, specific settings should be documented on feature configuration pages. Services connected via an API or SDK may require completely different settings.
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] Host: An external service should be reachable by its host name or IP address (IPv4 or IPv6).
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] Security: The external service connection security protocol should be configurable, to allow for onboarding security infrastructure.
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] Certificates: If an SSL certificate-based security protocol is configured, certificates may be validated on connection. One such validation is of the chain of trust, including anchors or root certificates. See the server configuration section for more information.
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] Authentication: The application does not yet support mutual TLS (also known as client certificates). Some form of Basic or Bearer authentication should be used, depending on the technology and/or protocol of the external service.
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] Server configuration
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] The implementation details of SSL certificate trust and stores is platform dependent. Always consult operating system documentation and organizational policies. The information provided below is only an example.
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] Linux
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] Trusted certificates should be installed to the following location according to 4.14. Using Shared System Certificates . Don't forget to run update-ca-trust after installing certificates.
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] /etc/pki/ca-trust/source/anchors
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] Catalog
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] Some of the configurable external services include:
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] Directory server : A directory server may be configured as an external identity provider for authentication.
[ITPIE:OPS Documentation | External Services | https://itpie-hostname/documentation/content/administration/external-services.html] Mail server : A mail server may be configured for sending mail messages by one or more features, including reports.