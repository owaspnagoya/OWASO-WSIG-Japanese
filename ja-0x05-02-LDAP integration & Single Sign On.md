# LDAP統合とシングルサインオン

大規模なWordPressサイトのユーザ管理には、悩まされることになります。
企業環境において、ユーザは一元的に管理され、異なったグループに割り当てられます。
WordPressは、このすでにある仕組みを利用することができます。
アクティブディレクトリもしくは、LDAP互換サービスにおいて、この方法は、すでにWordPressへの導入を試みる組織で実施されています。
セットアップは簡単、必要なアクセスレベルに基づき、WordPress権限毎のグループを作成し、個々のユーザを割り当てます。
一元統合を果たすと、シングルサインオンにより、更に洗練されたソリューションとなります。

サポートしているプラグインは

* [Active Directory Integration](https://wordpress.org/plugins/active-directory-integration/)
* [Active Directory SSO](https://wordpress.org/support/plugin/active-directory-sso)
* [Simple LDAP Login](https://wordpress.org/plugins/simple-ldap-login/)

