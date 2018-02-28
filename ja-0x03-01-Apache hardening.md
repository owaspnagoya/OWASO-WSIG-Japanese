
# Apache堅牢化
* 定期的にアップデートする
* ディレクトリのリスト化を無効にする
* SSL証明を生成、その証明書を使用することでサーバの通信をセキュアにする
* 不必要なモジュールの無効化にする
  * 次のような設定は有効的である: 'userdir', 'suexec', 'cgi/cgid', 'include', 'autoindex'
* ユーザとグループを分離してデーモンを実行する
* ディレクトリへのアクセスを制限するために'Allow'と'Deny'を使用する

* Use ''mod_security'' module to secure Apache
* Disable following of ''symbolic links''
* Turn off server sides includes and CGI execution
* Limit request size
* Configure other settings like ''TimeOut'', ''MaxClients'', ''KeepAliveTimeout'', ''LimitRequestFields'', ''LimitRequestFieldSize'' in order to prevent DoS attacks
* Enable and configure proper logging
* Modify server banner


