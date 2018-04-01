# プラグインとテーマのセキュリティ

プラグインとテーマは、WordPressコアによって提供される優れた追加機能です。
WordPressの成功はこれらの要素が基盤にあります。
新しい機能をテーマを開発したり、新しい機能をプラグインで追加することは簡単です。
しかし、容易な開発は、セキュリティの欠点につながります。
機能性を追求するあまり、開発者はたびたびセキュリティを忘れてしまいます。
[WorpPressのCVEリスト](https://cve.mitre.org/cgi-bin/cvekey.cgi?keyword=wordpress)を見てみると、セキュリティ上の欠陥のほとんどが、WordPress本体ではなく、プラグインやテーマが影響を与えていることに注意する必要があります。

WordPressでの開発は、正規な開発作業として、標準的なセキュア開発のライフサイクルに沿って行うべきです。
ここでの具体的な手法には、テーマやプラグインのソースコードレビューやペネトレーションテストを取り入れています。

サードパーティーによって開発されたプラグインを利用する場合は、セキュリティ監査を行うべきです。
利用できるプラグインの優れた見極めは以下の通りです。

+ 公式プラグインストア[https://wordpress.org/plugins/](https://wordpress.org/plugins/)での発表
+ ユーザの評価とコメント
+ 最終更新
+ 更新周期
+ 現行バージョンのWordPress本体との互換性

ソースコード監査を行うには、次のツールが使用できます。

* [RIPS](http://rips-scanner.sourceforge.net/)
* [PHP-sat](http://www.program-transformation.org/PHP/PhpSat) 
* [Yasca](http://www.scovetta.com/yasca.html) [現状のURL] https://linuxsecurity.expert/tools/yasca/ 
* [Manual analysis using grep](http://resources.infosecinstitute.com/finding-bugs-in-php-using-grep/) , [GrepBugs](https://grepbugs.com/) 

ソースコード監査において、特別に注意すべき箇所は以下の通りです。

* 難読化されたソースコード
* BASE64エンコード部分
* システムコール (exec, passthru, system, shell_exec, など)
* PHPコードの実行 (eval, assert, preg_replace, など)
* 情報の開示機能 (phpinfo, getenv, getmygid/pid/uid, など)
* ファイルシステムの操作 (fopen, bz/gzopen, chgrp/own/mod, など)
