http://browserify.org/

に書いてあることそのまま。

まず

```
npm install -g browserify
```

でBrowserifyをグローバルにインストール。

その後、

```
var unique = require('uniq');

var data = [1, 2, 2, 3, 4, 5, 5, 5, 6];

console.log(unique(data));
```

としてmain.jsを作り、

```
npm install uniq
```

して、

```
browserify main.js -o bundle.js
```

する。

これで出来た`bundle.js`を読み込んで

```
<script src="bundle.js"></script>
```

とかく。

そうするとconsoleに、

```
[1, 2, 3, 4, 5, 6]
```

と表示されるはず。
