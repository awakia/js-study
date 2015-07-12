## Watchifyとは

Watchifyは、Browserifyによるビルド結果に変更がある場合、それを検知しビルドしなおしてくれる仕組みを提供している

https://github.com/substack/watchify

## やったこと

[Browsorify](/module/browserify)と同じことを差分変更出来るようにする。


まず、Watchifyをグローバルにインストール。

```
npm install -g watchify
```

そして、Browserifyのコマンド

```
browserify main.js -o bundle.js
```

を`watchify`に変えて、

```
watchify main.js -o bundle.js
```

とする。

一応、何が起こっているか知りたければ、`-v --verbose`オプションをつけて、

```
watchify main.js -o bundle.js -v
```

とするとよい。

こうしておくと、`main.js`に変更を加えると

```
$ watchify main.js -o bundle.js -v
1565 bytes written to bundle.js (0.03 seconds)  # 起動時
1573 bytes written to bundle.js (0.01 seconds)  # 変更時
```

となり、変更を検知してbundle.jsを生成しなおしているのを確認できる。
