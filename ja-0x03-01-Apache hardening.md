
# Apache堅牢化
* 定期的にアップデートする
* ディレクトリリスティングを無効にする
* SSL証明書を生成して使用することでサーバとの通信をセキュアにする
* 不必要なモジュールを無効化する
  * 次のような設定は有効的である: *userdir*, *suexec*, *cgi/cgid*, *include*, *autoindex*
* ユーザとグループを分離してデーモンを実行する
* ディレクトリへのアクセスを制限するために'Allow'と'Deny'を使用する
* Apacheをセキュアにする*mod_security*を使用する
* *symbolic links*の追跡を無効にする
* サーバサイドのincludeとCGI実行を使用不可にする
* リクエストサイズを制限する
* DoS攻撃を防ぐために*Timeout*, *MaxClients*, *KeepAliveTimeout*, *LimitRequestFields*, *LimitRequestFieldSize*等の項目を設定する
* 適切なロギングを設定し有効にする
* サーバのバナー情報を変更する


