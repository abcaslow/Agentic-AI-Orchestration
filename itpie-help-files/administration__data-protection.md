# Data Protection

Source: ITPIE:OPS Documentation — Data Protection
Source URL: https://itpie-hostname/documentation/content/administration/data-protection.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Data Protection | https://itpie-hostname/documentation/content/administration/data-protection.html] Data Protection
[ITPIE:OPS Documentation | Data Protection | https://itpie-hostname/documentation/content/administration/data-protection.html] Note
[ITPIE:OPS Documentation | Data Protection | https://itpie-hostname/documentation/content/administration/data-protection.html] Organizational policy may supercede these controls. For example, full-disk encryption covers the entire filesystem, including files backing the database at rest.
[ITPIE:OPS Documentation | Data Protection | https://itpie-hostname/documentation/content/administration/data-protection.html] The application server may protect certain sensitive information in transit and/or at rest, depending on the context.
[ITPIE:OPS Documentation | Data Protection | https://itpie-hostname/documentation/content/administration/data-protection.html] Categories of sensitive information
[ITPIE:OPS Documentation | Data Protection | https://itpie-hostname/documentation/content/administration/data-protection.html] The application server may be installed in an environment containing sensitive information. It may be configured to connect to and collect information on network targets that are themselves or contain sensitive information.
[ITPIE:OPS Documentation | Data Protection | https://itpie-hostname/documentation/content/administration/data-protection.html] Network credentials
[ITPIE:OPS Documentation | Data Protection | https://itpie-hostname/documentation/content/administration/data-protection.html] Network targets and relationships
[ITPIE:OPS Documentation | Data Protection | https://itpie-hostname/documentation/content/administration/data-protection.html] Network device configuration backups
[ITPIE:OPS Documentation | Data Protection | https://itpie-hostname/documentation/content/administration/data-protection.html] Under these circumstances, organizational policy should be followed for server, network, and connection configuration and security. Additionally, data classification should be enabled and configured.
[ITPIE:OPS Documentation | Data Protection | https://itpie-hostname/documentation/content/administration/data-protection.html] Cryptographic implementation
[ITPIE:OPS Documentation | Data Protection | https://itpie-hostname/documentation/content/administration/data-protection.html] Note
[ITPIE:OPS Documentation | Data Protection | https://itpie-hostname/documentation/content/administration/data-protection.html] See Microsoft .NET cryptography , including notes on FIPS compliance .
[ITPIE:OPS Documentation | Data Protection | https://itpie-hostname/documentation/content/administration/data-protection.html] All cryptography should go through the Microsoft .NET platform, which calls operating system libraries (for example, OpenSSL on Linux). Sensitive information stored on the application server filesystem or in the application database is encrypted using AES (256-bit) with PKCS7 padding in CBC mode.
[ITPIE:OPS Documentation | Data Protection | https://itpie-hostname/documentation/content/administration/data-protection.html] Key materials for cryptographic operations are managed on and by the application server.