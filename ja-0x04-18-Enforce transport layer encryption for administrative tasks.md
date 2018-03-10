# 管理作業は暗号通信を実施する

通常、サイトは80又は443ポートを通じて利用できます。これは、平文テキストか、暗号接続経路か、利用者が自由に選べることを意味します。

機微な作業のためにSSL（最低でも）を強制するには、wp-config.phpファイルに以下の行を追加します。

define('FORCE_SSL_ADMIN', true);

注意: FORCE_SSL_LOGIN は Version 4.0 で廃止されました。FORCE_SSL_ADMIN を使用してください。
