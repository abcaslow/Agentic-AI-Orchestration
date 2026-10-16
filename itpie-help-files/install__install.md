# Install

Source: ITPIE:OPS Documentation — Install
Source URL: https://itpie-hostname/documentation/content/install/install.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] Install
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] Database Installation
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] See Database for details on installing and configuring the application database before proceeding.
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] Package Verification
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] The download package contains the RPM package ( .rpm ) and a GPG-signed digest ( .sha256.asc ). Verifying the package before installation is strongly recommended.
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] Import the GPG public key
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] The GPG public key used to sign the RPM is distributed with the download package. Import it once per server:
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] sudo rpm --import RPM-GPG-KEY-ITPIE-Jun2026-RELEASE-13F1AB91D7CB75C1
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] Our GPG key is also available out-of-band on request if your security procedures require it.
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] Verify the GPG signature on the RPM
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] rpm --checksig itpie-server-<version>.rpm
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] A successful verification will print itpie-server-<version>.rpm: digests signatures OK . If verification fails, contact support before proceeding.
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] ITPIE:OPS Installation
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] Important
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] If your environment requires POSIX users to have a specific UID or GID, create a user and group named itpie following your organization's policies before running the installer. The installer will create an itpie user and group with an automatically assigned UID/GID if they do not already exist.
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] Important
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] The RPM package declares its dependencies. dnf will automatically install required system packages ( libicu , libcap , openssl ) during installation. If you are installing with rpm directly instead of dnf , ensure these dependencies are present beforehand.
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] Install the RPM package:
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] sudo dnf install itpie-server-<version>.rpm
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] Review and edit the configuration file. The installer places a default configuration at /etc/itpie/itpie.conf (copied from the example at /usr/share/itpie-server/examples/itpie.conf ) if one does not already exist.
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] vi /etc/itpie/itpie.conf
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] At a minimum, configure the database connection string.
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] Perform database migrations. This must be run as the itpie service account from its home directory:
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] pushd /var/lib/itpie sudo -u itpie /opt/itpie/itpie-server/itpie-server migrate popd
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] The installer generates a self-signed TLS certificate at /etc/itpie/ssl/itpie.crt and /etc/itpie/ssl/itpie.key if no certificate exists. Replace these with a certificate signed by a trusted authority before deploying to production.
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] Enable and start the service:
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] systemctl enable --now itpie-server
[ITPIE:OPS Documentation | Install | https://itpie-hostname/documentation/content/install/install.html] Visit the web interface, accept or replace the certificate, activate your license, and create the initial administrator account.