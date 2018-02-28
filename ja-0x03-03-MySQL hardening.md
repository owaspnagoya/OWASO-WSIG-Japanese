
== MySQL hardening ==
There is an entire [https://www.owasp.org/index.php/OWASP_Backend_Security_Project_MySQL_Hardening OWASP project dedicated to MySQL hardening]. The main action items are:

* Update regularly
* Disable or restrict remote access
* Filesystem access restrictions and ACLs
* Designing a chroot-jail
* Encrypting network traffic (this is a must if the database layer is physically separated from the application layer)
* Encrypting raw databases on filesystem level
** Redundant if disk encryption is in place at the OS layer
** However, by using ''dmcrypt'', one can generate an extra layer of encryption
* Backup encryption
* Configuration
** Connectivity: maximum number of concurrent connections and related settings
** Logging
** Access control and privilege management
** Set up root password
** Rename root account
** Delete unused users and databases
** Remove installation history

A PHP security checker is available [https://github.com/sektioneins/pcc here]. This is a one-page php file designed to analyze PHP configuration and rank the findings based on severity.
