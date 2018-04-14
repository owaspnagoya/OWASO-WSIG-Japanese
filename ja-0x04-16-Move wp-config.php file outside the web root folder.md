## wp-config.phpファイルのwebルートフォルダー（ドキュメントルート）外への移動

wp-config.phpファイルは、非常に重要な（WordPress）設定ファイルです。例として、データベース情報など、あなたのWordPressサイトについて多くの機密情報を含んでいます。

WordPressは、WordPressルートフォルダーにwp-config.phpファイルが存在しない場合、自動的に上層フォルダでwp-config.phpファイルを探します。public_htmlフォルダーの外部へwp-config.phpファイルを移動することは、インターネットから接続させないを意味します。
