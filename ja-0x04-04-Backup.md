# バックアップ

バックアップは不可欠です。
バックアップによって、クリーンで高速な復旧と、データの損失による長期停止の明暗を分けることになります。

バックアップには何を含める必要がありますか？

* WordPressファイル
  * WordPress 本体(コア)
  * WordPress プラグイン
  * WordPress テーマ
  * イメージ（画像）ファイル
  * JavaScriptと PHP スクリプト, その他のソースコードファイル
  * 追加ファイルと静的Webページ
* データベース

/public_htmlフォルダのフルバックアップが必要だと言うのは簡単です。
しかし、これだけでは十分でない場合もあります。大量のデータ(統計やテンポラリデータなど)が公開フォルダに生成され、バックアップ処理が機能しない場合があります。設定ファイルが公開ディレクトリの外に配置される場合もあります。やはりバックアップが必要です。

バックアップすべきファイルやフォルダを見極め、これらを隔離された場所に保存することです。

データベースのバックアップは、MySQLコマンドの使用やphpMyAdminのような管理インターフェースを使用することができます。

バックアップはどのくらいの間隔で実施すべきですか？それは、コンテンツの更新される頻度に依存します。一日に複数の更新が発生する場合は、毎日バックアップすする方が良いです。新しい記事が数日ごとの場合は、週間または月間でのバックアップをするのも方法です。

複数のバックアップを保持し、日付管理するのは良い習慣です。違反行為にただちに気づかない可能性があり、クリーンバックアップが何世代か前の古いバックアップからしか行えない場合があるためです。

バックアップが動作していることを確認することは、バックアップ作業の一部です。迅速かつ完全復旧ができないバックアップでは役に立ちません。クリーンなサーバにバックアップからフルリカバリーを実行し、全ての機能をチェックし欠陥がないことを確認します。

## 自動化

The steps above are manual and labor intensive. There is a full list of plugins that can help this process: https://wordpress.org/plugins/tags/backup

The one free alternative offering full backup capabilities that stands out of the list is [https://wordpress.org/plugins/backwpup/ BackWPup]. The free version can be used to save your complete installation including /wp-content/ and push it to an external Backup Service, like Dropbox, S3, FTP (not a good idea) and many more. 

From a security perspective, it’s worth noticing that an attacker who compromised the installation may be able to retrieve credentials and access the remote location of the backups, thus being able to manipulate or delete them. As a good precaution, on the remote side where the backups are stored, an independent process should take the backups and move them to a location inaccessible from the WordPress installation.

