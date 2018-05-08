# MySQL堅牢化

[OWASP ProjectのMySQL堅牢化はこちらです。](https://www.owasp.org/index.php/OWASP_Backend_Security_Project_MySQL_Hardening)
主な実装項目は次の通りです:

- 定期的にアップデートする
- リモートアクセスの無効化、もしくは制限する
- ファイルシステムのアクセス制限とACLs（Access Control Lists）を設定する
- chrootによるrootサービス隠蔽を設計する（指定ディレクトリより上のディレクトリに移動できない様に設計）
- ネットワーク通信を暗号化する (WEBサーバーとDBサーバーの分離を行う場合、必須)
- rawデバイスデータベース（ファイルシステムを入れる前のディスク）暗号化する
  - Redundant if disk encryption is in place at the OS layer
  - However, by using ''dmcrypt'', one can generate an extra layer of encryption
- バックアップデータを暗号化する
- MySQL設定
  - 同時接続数の上限設定
  - ログ設定
  - アクセス権限ユーザー権限管理
  - rootパスワード設定
  - rootアカウントのリネーム
  - 未使用ユーザーやデータベースの削除
  - インストール履歴の削除
