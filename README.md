# dbcli

![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/ggedde/dbcli) &nbsp; ![GitHub](https://img.shields.io/github/license/ggedde/dbcli?label=license)


### Database CLI tool for Creating, Copying, and Syncing databases quickly. It can create local databases, copy local or remote database or copy remote to local databases. It cannot write to remote databases.  

\* Currently only supports mysql and mariadb  
\* All Databases are collated as utf8mb4_unicode_ci


### db copy [-o] [project_config_file]

&nbsp; &nbsp; Copies Remote Database to Local Database using the project_config_file.  
&nbsp; &nbsp; Local Database will be backup before getting overwritten

&nbsp; &nbsp; -o &nbsp; Omits the backup files. Use only if you are sure you will not need to revert back.


### db backup [-l | -r] [project_config_file]

&nbsp; &nbsp; Backsup databases from both local and remote

&nbsp; &nbsp; -l &nbsp; Backup local database Only  
&nbsp; &nbsp; -r &nbsp; Backup remote database Only


### db add [project_config_file]

&nbsp; &nbsp; Adds a new project_config_file, but does not create a local database


### db create [-a] [project_config_file]

&nbsp; &nbsp; Creates a new database on your localhost

&nbsp; &nbsp; -a &nbsp; Also add a new project_config_file