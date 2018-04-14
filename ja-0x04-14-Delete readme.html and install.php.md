# readme.html と install.php の削除

readme.htmlファイルは、機密情報を漏らすことになり、機能的に必要ありません。

install.phpファイルは、インストールプロセスの残骸で、再び利用することはできず不要なため、削除することが必要です。

license.txtファイルは、WordPressの最終アップデートの時期を漏らすことになります。（攻撃者が古いWordPressを探すために利用されてしまう）


以下のファイルを削除します。

    /<WordPress_root>/readme.html
    /<WordPress_root>/license.txt
    /<WordPress_root>/wp-admin/install.php

