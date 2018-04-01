# ユーザの役割と正しい使い方

権限を理解しユーザへの正しい割当をすることは、業務権限の分離に重要です。

WordPressの権限は

* 特権管理者(Super Admin) – サイトのネットワーク管理機能へのアクセスおよび他のすべての機能を持つ管理者
* 管理者(Administrator) – 1つのサイト内のすべての管理機能にアクセスできるユーザー
* 編集者(Editor) – 他のユーザーの投稿を含む投稿を公開し管理できるユーザー
* 投稿者(Author) – 自分の投稿を公開し管理できるユーザ
* 寄稿者(Contributor) – 自分の投稿を書いて管理することはできるが、投稿することができないユーザ
* 購読者(Subscriber) – 自分のプロフィールのみを管理できるユーザ

権限割当には、原則最小特権を考えることが必要です。

役割ごとの全権限一覧の比較は、http://codex.wordpress.org/Roles_and_Capabilities

サポートするプラグイン

* [https://wordpress.org/plugins/members/ Members Plugin]
* [https://wordpress.org/plugins/role-scoper/ Role Scoper Plugin]
* [http://wordpress.org/extend/plugins/user-access-manager/ User Access Manager]
* [http://wordpress.org/extend/plugins/advanced-access-manager/ Advanced Access Manager]
* [http://wordpress.org/extend/plugins/user-role-editor/ User Role Editor]

