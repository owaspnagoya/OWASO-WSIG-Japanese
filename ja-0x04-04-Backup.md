
== Backup ==
The backup process is essential. The configuration of the backup process can make the distinction between a clean and fast recovery or a loss of data and prolonged downtime.

What needs to be included in the backup?

* The WordPress Files
** WordPress Core Installation
** WordPress Plugins
** WordPress Themes
** Images and Files
** JavaScript and PHP scripts, and other code files
** Additional Files and Static Web Pages
* The Database

It’s easy to say that a full backup of the /public_html folder is needed. However there are situations in which this is not feasible nor enough. There are situations in which large quantities of data is generated in the public folder (statistics, temporary data, etc.) that is useless in the backup process. There’s also the situation in which configuration files are placed outside the public directory. They also need backup.

The plan is to identify the files and folders that must be part of the backup process and save these in a remote location.

For database backup, the mysql command line can be used or administrative interfaces like phpMyAdmin. 

How often should the backup be performed? It all depends on how often the instance is updated from a content perspective. If there are multiple updates a day, it’s a good idea to have a daily backup. If there’s a new article every several days, than a weekly or monthly backup is the way to go.

It’s a good practice to keep multiple backups and have them time stamped. This is because a breach might not be noticed immediately and a clean recovery can only be performed from a backup which is several iterations old. 

Verifying that the backup is functional is part of the process. A backup that does not allow quick and full recovery is useless. The idea is to have a clean server and perform a full recovery from the backup, then check all the functionality and make sure nothing is missing.
