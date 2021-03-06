# PHP堅牢化
* 定期的にアップデートする
* CGI BinaryのPHPをインストールしない
* 不要なPHPモジュールを無効にする
* 未使用の危険なPHP関数を無効にする（良い例： '' exec ''、 '' passthru ''、 '' shell_exec ''、 '' system ''など）
* 内部エラーを記録する
* クライアント側で冗長なエラー報告を無効にする
* リモートコードの実行を無効にする（必要がない場合、WordPressのコアにはこの機能は必要ありません）
* マジック引用符を無効にする
* ファイルシステムへのPHPアクセスを制限する
* DoSから防御する
  * POST size を制御する
  * スクリプtの実行時間を制限する
  * メモリ使用量を制限する
* [Suhoshinのセキュリティ拡張機能](http://www.suhosin.org/stories/index.html)を実装することを検討する
* Consider implementing the Suhoshin security extension
* 使用しているPHPバージョンを隠す
* .php拡張子を隠す

phpセキュリティチェッカーを使う事ができます [https://github.com/sektioneins/pcc here]. これはphpの解析を行い、緊急度の高さに応じた（脆弱性の）ランク付けを行うために作られた1枚のphpファイルです。
