# Database

Source: ITPIE:OPS Documentation — Database
Source URL: https://itpie-hostname/documentation/content/administration/database.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] Database
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] The application server requires a properly installed and configured local PostgreSQL database.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] Requirements
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] PostgreSQL 16
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] An application database (default: itpie )
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] An application role with all privileges on the application database (default: itpie )
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] A superuser role (default: postgres )
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] Trusted extensions:
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] btree_gist
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] citext
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] pgcrypto
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] Connection string
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] Tip
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] You should restart the service after any configuration changes.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] You should provide the database connection string in the application configuration file . Only basic authentication (username and password) is supported at this time. The credential is not encrypted in this file, so ensure appropriate access controls.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] { "ConnectionStrings": { "Database": "Host=localhost;Database=itpie;User ID=itpie" } }
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] For additional security, it is possible to connect to PostgreSQL via a local socket. This prevents any possibility of external database connections to PostgreSQL. ITPIE supports this type of connection. Please consult your database administrator for information on using this configuration.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] Configuration
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] Settings may be modified by a system administrator to ensure correct and efficient operation of the application database. The PostgreSQL configuration file's exact location depends on which installation used to install it on the server.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] Parameters
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] The official docs on server configuration are invaluable. As are community resources on topics such as performance tuning . Following are the settings we know have an immediate impact.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] shared_buffers
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] From the official docs :
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] Sets the amount of memory the database server uses for shared memory buffers. The default is typically 128 megabytes (128MB), but might be less if your kernel settings will not support it (as determined during initdb). This setting must be at least 128 kilobytes. (Non-default values of BLCKSZ change the minimum.) However, settings significantly higher than the minimum are usually needed for good performance. This parameter can only be set at server start.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] Important
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] The size should be set somewhere between 25-40% of server memory, but some sources have pushed that as high as 75%.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] shared_buffers = 128MB
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] max_locks_per_transaction
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] From the official docs
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] The shared lock table tracks locks on max_locks_per_transaction * (max_connections + max_prepared_transactions) objects (e.g., tables); hence, no more than this many distinct objects can be locked at any one time. This parameter controls the average number of object locks allocated for each transaction; individual transactions can lock more objects as long as the locks of all transactions fit in the lock table. This is not the number of rows that can be locked; that value is unlimited. The default, 64, has historically proven sufficient, but you might need to raise this value if you have queries that touch many different tables in a single transaction, e.g., query of a parent table with many children. This parameter can only be set at server start.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] The application is known to have several large queries that require this value to be set much higher than the defualt. We'll provide this default and make changes as necessary in each release.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] max_locks_per_transaction = 1000
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] max_wal_size
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] From the official docs :
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] Maximum size to let the WAL grow during automatic checkpoints. This is a soft limit; WAL size can exceed max_wal_size under special circumstances, like under heavy load, a failing archive_command, or a high wal_keep_segments setting. The default is 1 GB. Increasing this parameter can increase the amount of time needed for crash recovery. This parameter can only be set in the postgresql.conf file or on the server command line.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] The min size should not be modified, but the max size should be set proportionally to shared_buffers size.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] max_wal_size = 1GB min_wal_size = 80MB
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] Take into account any checkpoint warnings produced by the service when running.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] HINT: Consider increasing the configuration parameter "max_wal_size". LOG: checkpoints are occurring too frequently (3 seconds apart)
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] pg_stat_statements
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] From the official docs :
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] The pg_stat_statements module provides a means for tracking execution statistics of all SQL statements executed by a server.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] The module should already be enabled in the default configuration.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] shared_preload_libraries = 'pg_stat_statements'
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] The module is configured by a number of additional settings . An example of typical usage is as follows.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] pg_stat_statements.max = 10000 pg_stat_statements.track = all
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] Also take note of the various statistics collection settings. This application has a lot of user functions, some are very long. These two settings may be used together.
[ITPIE:OPS Documentation | Database | https://itpie-hostname/documentation/content/administration/database.html] track_functions = all track_activity_query_size = 4096