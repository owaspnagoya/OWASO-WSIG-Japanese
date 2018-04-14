##readme.html と install.phpの削除

readme.htmlは、機密情報をサイトの外部に漏らしうることになり、機能的に不要です。
install.phpは、WordPressインストール用のファイルが残ったものですが、（WordPressインストール後）再度、使われるべきではありません。install.phpは、（WordPressインストール後）不要であり、削除すべきです。
license.txtはWordPressの最終更新年をサイトの外部に漏らします。　－　実際、攻撃者は、更新されていない多くのWordPressに脆弱性スキャンを行う事ができます。

削除対象ファイル:

/WordPressドキュメントルート/readme.html　/WordPressドキュメントルート/license.txt　/WordPressドキュメントルート/wp-admin/install.php files
