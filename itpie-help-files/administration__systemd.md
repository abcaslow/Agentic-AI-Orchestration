# Service Management

Source: ITPIE:OPS Documentation — Service Management
Source URL: https://itpie-hostname/documentation/content/administration/systemd.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Service Management
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] ITPIE:OPS installed via RPM or Debian package files now runs on the host and relies on systemd for service management.
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Here is a quick reference guide for working with systemd as it relates to ITPIE:OPS.
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Operation Command
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Starting the service. systemctl start itpie
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Stopping the service. systemctl stop itpie
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Configure ITPIE:OPS to start at boot. systemctl enable itpie
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Configure ITPIE:OPS NOT to start at boot. systemctl disable itpie
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Configure ITPIE:OPS to start at boot and starting the service immediately. systemctl enable --now itpie
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Inspecting the health of the ITPIE:OPS service. systemctl status itpie
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] The status command above will output similar to the following shown below as well as some logs. Use q to exit.
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] ● itpie.service - ITPIE: Operations Suite Loaded: loaded (/usr/lib/systemd/system/itpie.service; enabled; vendor preset: disabled) Active: active (running) since Mon 2023-09-25 13:15:32 UTC; 7h ago Main PID: 1183 (itpie-server) Tasks: 20 (limit: 49004) Memory: 451.5M CGroup: /system.slice/itpie.service └─1183 /opt/itpie/itpie-server/itpie-server
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Service Logs
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] ITPIE:OPS relies on journald for log management. Use the following commands to view the logs:
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Operation Command
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] View entire ITPIE log. journalctl -u itpie.service
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Follow the ITPIE log. journalctl -fu itpie.service
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] View the logs for the last 15 minutes. journalctl -u itpie.service --since=-15m
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] View the logs between two specific timeframes. journalctl -u itpie.service --since="2023-09-25 20:00:00" --until="2023-09-25 20:15:40"
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] View the logs before a specific timeframe. journalctl -u itpie.service --until="2023-09-25 20:15:40"
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Notes on journald time:
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] --since and --until accept a wide range of time formats
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] for relative time, such "15 minutes ago" -15m the m indicates minutes. Other suffixes include: s for seconds, h for hours, d for days.
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] see: https://man7.org/linux/man-pages/man1/journalctl.1.html (or man 1 journalctl on a Linux server) for complete information
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Notes on journald paging:
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] journald uses its own pager to assist the administrator is viewing logs with minimal hassle
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] reading a log is intuitive (allowing one to use the arrow keys) for up/down a single line at a time, or left/right to move approximately half a screen horizontally
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] journalctl's pager will display arrows on the side of the screen to indicate that text is being cut off.
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] scrolling to the top of the log (oldest messages) is performed by typing 1G (note G is case sensitive)
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] scrolling to the bottom of the log (newest messages) is performed by typing 0G
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] page up/down work as expected
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] exit the pager with q
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] If the logs need to be copy/pasted to another program, the pager will cause problems. In these situations, simply re-run your command with --no-pager added to the command line arguments. This will allow it to behave non-interactively. journalctl can also detect when it is being piped and will automatically behave non-interactively. This is useful for dumping logs to files.
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] For example:
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] journalctl --no-pager -u itpie.service
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] journalctl -u itpie.service >currentlogs.txt
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Database Logs
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] The database logs are accessed in different ways depending on the kind of ITPIE:OPS deployment.
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] RPM installations
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] The exact name of this service depends on the system, so, to locate which name to use, run the following command:
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] systemctl list-units | grep sql
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] If nothing is returned, try systemctl list-units | grep post (which may return multiple results, such as postgresql and postfix ).
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Example output:
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] [root@itpie-ops ~]# systemctl list-units | grep sql postgresql.service loaded active running PostgreSQL database server [root@itpie-ops ~]# systemctl list-units | grep post postgresql.service loaded active running PostgreSQL database server
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Once the database service name is determined, the above journactl commands work as one would expect. Simply replace itpie.service with the name determined by the previous command. In the following examples, we will use postgresql.service .
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] journalctl -u postgresql.service --since=-5m
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] Additionally, multiple services can be viewed at the same time. For example, to view both ITPIE:OPS & pgsql logs at the same time, the following command would work:
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] journalctl -u postgresql.service -u itpie.service --since=-5m
[ITPIE:OPS Documentation | Service Management | https://itpie-hostname/documentation/content/administration/systemd.html] All the previous journalctl command advice applies (timestamps, paging, redirecting to a file for diagnosis by our support team, etc).