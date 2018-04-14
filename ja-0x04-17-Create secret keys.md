# 秘密鍵の生成

WordPress 2.6 のリリースで、新しいセキュリティ機能として、パスワードとパスワードハッシュ、Cookieのセキュリティが組み込まれました。
この機能の特徴は、なにも必要としません。しかし、いくつかの追加ステップを行わないと別段強力ではありません。

WordPress環境のセキュリティを強力に向上させるためには、秘密鍵を設定する必要があります。これは、標準インストールのプロセスの一部です。
秘密鍵の漏えいの疑いが発生した都度においても、管理者は秘密鍵を変更しなくてはなりません。
秘密鍵を変更すると、全てのセッションが無効となり、ユーザは再認証が必要になります。

秘密鍵を設定または変更するには、`wp-config.php`ファイルの以下の行を追加、または編集します。（または、他の`define`記述の次に）

    define('AUTH_KEY', 'put your unique phrase here');

    define('SECURE_AUTH_KEY', 'put your unique phrase here');

    define('LOGGED_IN_KEY', 'put your unique phrase here');

    define('NONCE_KEY', 'put your unique phrase here');


秘密鍵を記憶しておく必要はなく、長く、ランダム、そして複雑に作成するか、[オンラインジェネレータ](https://api.wordpress.org/secret-key/1.1/salt/)を利用します。
