## はじめに

ちょっと見ないうちにJavascriptは圧倒的な進化を遂げている。
Node.jsとか言う、何でJavascriptでサーバーを書かなきゃいけないんだ、やってられるかとか思っていたら、そこで進化したツール群や書き方ノウハウみたいな物があって、それがBrowserifyとかでクライアントサイド側に進出してきている。
他にも昔はブラウザの違いとやらで、jQueryなしでは何もできない言語だった気がするけど、ライブラリを使わなくても`document.querySelector`とかで`$`の置き換えが聞くし、`ajax`リクエストとかも普通にできるようになってきている。
class使うならalterJSのCoffeeScriptやTypeScriptとか思っていたらES6とかいう新バージョンで、普通にクラスも使えるようになるときた。
ちょっとコレは勉強しない訳には行かなくなったみたいなので、ゴミのようなコードサンプル群を書きつつ、知っておくと良さそうなJavascriptの知識を増やしていく。
基本的には、クライアントサイドで使える部分を書くつもり。

## 目次

* [モジュール](module) - ファイル単位でモジュール化
 - [Browserify](module/browserify) - クライアントサイドでもrequireを
 - [Watchify](module/watchify) - 変更を監視して差分ビルド
 - [UgrifyJS](module/ugrifyjs) - JSをMinifyしてくれる
 - [Exorcist](module/exorcist) - Source Mapをはいてくれる
 - [Gulp](module/gulp) - これらのモジュールをコマンド実行できるタスクに
