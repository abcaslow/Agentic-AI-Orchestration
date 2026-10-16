# Backup and Restore

Source: ITPIE:OPS Documentation — Backup and Restore
Source URL: https://itpie-hostname/documentation/content/administration/backup-and-restore.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] Backup and Restore
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] Important
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] These instructions assume a local database (running on the application server) and access to the database superuser ( postgres by default). If this does not match your deployment, please contact your database administrator for guidance.
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] Before upgrading the application you should determine which kind of backup is necessary.
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] Export application data— This is feature specific. Not all features support export and import. You should refer to the relevant feature documentation.
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] Dump the application database— This produces a version-specific database "dump" that can be used to restore the previous version in the case of an upgrade failure. This is the process documented below.
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] Backup
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] Dump the application database. This assumes the database is named itpie .
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] sudo su postgres -c 'pg_dump -v -Fc itpie' >itpie.dump
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] Restore
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] Ensure that the application is not running.
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] systemctl stop itpie-server
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] Restore the database from the database dump.
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] Important
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] This command will drop the existing database, even if it is canceled. Ensure that it is performed on a server that can be in a broken state until a successful database restoration completes.
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] sudo su postgres -c 'pg_restore -v -cC -d postgres' <itpie.dump
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] Note: your dump file must be in a location readable by the 'postgres' user. We recommend moving it to /var/lib/itpie or /data depending on your available partition space / layout.
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] If the application server needs to be downgraded, do so at this time. Run the uninstall script, then install the version that matches the database backup:
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] sudo bash /usr/share/itpie-server/uninstall.sh sudo bash itpie-server-<version-matching-the-database-backup>.run systemctl enable itpie-server
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] Start the application server:
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] systemctl start itpie-server
[ITPIE:OPS Documentation | Backup and Restore | https://itpie-hostname/documentation/content/administration/backup-and-restore.html] Refresh the website and/or confirm that the system is working as expected.