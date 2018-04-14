## ブランクindex.phpファイルの追加

特に、WEBサーバー設定がWordPress実装者の制御範囲外である共有ホスティング環境において、、ディレクトリ一覧表示が有効になっていることがあります。
セキュリティレイヤー追加として、ファイルリソースのブラウザ表示防止のために、インデックスを持たないフォルダとしてブランクindex.phpファイルの追加を行うべきです。

ブランクindex.phpの配置検討が必要な主なフォルダ:

+ wp-includes
+ wp-content
+ wp-content/plugins
+ wp-content/themes
+ wp-content/uploads
