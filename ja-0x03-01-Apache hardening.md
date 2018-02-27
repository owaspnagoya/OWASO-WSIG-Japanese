
== Apache堅牢化 ==
* 定期的にアップデートする
* ディレクトリのリスト化を無効にする
* SSL証明を生成、その証明書を使用することでサーバの通信をセキュアにする。
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


