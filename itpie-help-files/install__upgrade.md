# Upgrade

Source: ITPIE:OPS Documentation — Upgrade
Source URL: https://itpie-hostname/documentation/content/install/upgrade.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] Upgrade
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] Important
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] Always back up the application database before upgrading.
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] Package Verification
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] Verify the RPM signature before proceeding. If you have not already imported the GPG key, see Install — Package Verification . Otherwise, verify the package directly:
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] rpm --checksig itpie-server-<new-version>.rpm
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] A successful verification will print itpie-server-<new-version>.rpm: digests signatures OK . If verification fails, contact support before proceeding.
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] ITPIE:OPS Upgrade
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] Stop the service:
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] systemctl stop itpie-server
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] Install the new RPM:
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] sudo dnf upgrade itpie-server-<new-version>.rpm
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] Your existing /etc/itpie/itpie.conf is preserved. Compare it against the updated example to pick up any new or changed options:
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] diff /etc/itpie/itpie.conf /usr/share/itpie-server/examples/itpie.conf
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] Perform database migrations:
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] pushd /var/lib/itpie sudo -u itpie /opt/itpie/itpie-server/itpie-server migrate popd
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] Enable and start the service:
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] systemctl enable --now itpie-server
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] Verify that the application is working as expected. Confirm that the device-support catalog reloads successfully by visiting the /device-support page or checking the service logs:
[ITPIE:OPS Documentation | Upgrade | https://itpie-hostname/documentation/content/install/upgrade.html] journalctl -u itpie-server -f