# TEST

## httpサーバ起動

### 必要なもの

[Node.js](https://nodejs.org/ja/) 最新版(>= 9.10.1)をインストール。

`CTRL + @` を押すと、ターミナルが起動されるので、以下のコマンドで必要なモジュールをインストールする。

```bash
> npm install
```

これで `node_modules` というフォルダが作成され、 `package.json` に記述されているパッケージを自動的にインストールしてくれるぞ。

### 起動コマンド

起動コマンドは `package.json` の `scripts` フィールドに書かれているぞと。

```
  "scripts": {
    "server": "http-server -o -a localhost -p 80"
  },
```

以下のコマンドをターミナルから実行し、HTTPサーバを起動する。

```bash
> npm run server
```

もし `80` 番ポートを使っていたら起動できないので、その場合は起動スクリプトのポート番号を修正すればOK.
よく使われるのが、 `8000` とか `8080` とか。
`-p` オプションの後ろの数字ね。

`http-server -o -a localhost -p 80`



