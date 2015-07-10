# Moduleについて

Node.js界隈で使われるようになったモジュール概念を[Browserify](http://browserify.org/)というツールがクライアントサイドサイドでも使えるようにした。

JSでのモジュールは、`var hoge = require 'hoge'`のような感じで使い、`module.exports`でExportされたものが返ってくる仕組み。
これにより、1モジュール1ファイルという、きれいな仕組みが保たれる。

## 参考

* [Node.jsのモジュールの説明](http://nodejs.jp/nodejs.org_ja/api/modules.html)
* [Browserify: それはrequire()を使うための魔法の杖 - Qiita](http://qiita.com/cognitom/items/4c63969b5085c90639d4)
