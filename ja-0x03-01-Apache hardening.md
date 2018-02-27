
== Apache堅牢化 ==
* Update regularly
* Disable directory listing
* Secure the communication with the server by generating and using SSL certificates
* Disable unnecessary modules
** Good candidates for this are: ''userdir'', ''suexec'', ''cgi/cgid'', ''include'', ''autoindex''
* Run the daemon as a separate user and group
* Use ''Allow'' and ''Deny'' to restrict access to directories
* Use ''mod_security'' module to secure Apache
* Disable following of ''symbolic links''
* Turn off server sides includes and CGI execution
* Limit request size
* Configure other settings like ''TimeOut'', ''MaxClients'', ''KeepAliveTimeout'', ''LimitRequestFields'', ''LimitRequestFieldSize'' in order to prevent DoS attacks
* Enable and configure proper logging
* Modify server banner

