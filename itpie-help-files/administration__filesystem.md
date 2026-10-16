# Filesystem

Source: ITPIE:OPS Documentation — Filesystem
Source URL: https://itpie-hostname/documentation/content/administration/filesystem.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Filesystem
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Note
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] All filesystem access is mediated through a Microsoft ASP.NET Core file provider , which implements security controls, such as preventing path traversal.
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] The application server uses an installation, configuration, and data directory according to platform standards. More information is provided below and important files are called out.
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Installation directory
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] The application server requires an executable to be targeted by the service infrastructure . Some bundled resources should be loaded at start up from this directory.
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Linux
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] The installation directory file should be created in the standard location .
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] /opt/itpie/itpie-server
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Configuration directory
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Tip
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] You should restart the service after any configuration change.
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Warning
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] If a configuration file is incorrectly formatted, the application should fail to start. You should check the service log for messages like:
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Could not parse the JSON file.
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] The configuration directory should contain only a few specific files required for application server operation.
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Linux
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] The configuration directory should be created in the standard location .
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] /etc/itpie
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Configuration file
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Minimal configuration is required for the application server to start, notably a database connection string . The configuration file supports the configuration of certain Microsoft .NET subsystems used by the application server, for example logging and certain web server settings.
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Linux
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] The configuration file should be found in the standard location .
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] /etc/itpie/itpie.conf
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] The configuration file is a JSON document . It should look something like this when first installed:
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] { "ConnectionStrings": { "Database": "Host=localhost;Database=itpie;User ID=itpie" }, "Logging": { "LogLevel": { "Default": "Information" } } }
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] License file
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Note
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] If you cannot use a license file, you may assign the license key to an environment variable named ITPIE_LICENSE__KEY .
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] The application server should be licensed before it allows access to the website or API. The license file or key should be supplied by VAE, Inc.
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Linux
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] The license file should be found in the standard location .
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] /etc/itpie/itpie.lic
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] The license file is a JSON document . It should look something like this when provided or after submitting the licensing form:
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] { "License": { "Key": "license-key-value" } }
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Data directory
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Some features allow users to upload files from their computer to the application server. Those features should use the data directory to temporarily store those files while they're being imported into the application database as feature-specific data, before being removed.
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] Linux
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] The data directory should be created in the standard location .
[ITPIE:OPS Documentation | Filesystem | https://itpie-hostname/documentation/content/administration/filesystem.html] /var/lib/itpie