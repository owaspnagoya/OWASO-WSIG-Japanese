# コメント機能の制限　※画面と確認が必要

WordPressは最初はブログのプラットフォームでコメント登録ができることが成功のひとつでした。
WordPressがCMSとして変化するに従い、コメントが不要な場合もでてきました。
考慮する必要としては

* コメントは必要ですか？ 

不要であれば機能を無効化します。

管理者でログインし、
新規の投稿は
［設定］→［ディスカッション］"Allow people to post comments on new articles"のチェックを外す
For new posts go to Settings -> Discussion and uncheck "Allow people to post comments on new articles".
For existing posts, 
go to Posts, select all of them, Bulk Actions -> Edit and choose “do not allow” near Comments before hitting Update posts.

* コメントが必要な場合、だれが投稿できますか？

登録されたユーザだけにコメント登録を許可する場合

［設定］→［ディスカッション］ “Users must be registered and logged in to comment” をチェックします。

* コメントの公開前に確認しますか？

チェックボックスにチェックをします。

コメントを公開前に確認しない場合、初期にインストールされている'Akismet'のような、アンチスパムプラグインの利用をお勧めします。

［設定］→［ディスカッション］の全ての設定を慎重に検討する必要があります。

