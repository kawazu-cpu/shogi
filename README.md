# 将棋 — 詰将棋と対局

詰将棋100問、無限モード、4段階のコンピューター対局が遊べるWebアプリです。
iPhoneのホーム画面に追加すると、アプリのように全画面で使えます。一度開けばオフラインでも遊べます。

## GitHub Pagesで公開する手順

1. https://github.com にアクセスして無料アカウントを作ります（すでにあれば不要）。
2. 右上の「＋」→「New repository」を選びます。
3. Repository name に `shogi` などの名前を入れ、「Public」を選んで「Create repository」を押します。
4. 次の画面で「uploading an existing file」のリンクを押します。
5. このフォルダの中のファイルを**すべて**ドラッグして入れ、「Commit changes」を押します。
   （フォルダごとではなく、中身のファイルを直接入れてください。index.html が一番上の階層にある必要があります）
6. リポジトリの「Settings」→ 左メニューの「Pages」を開きます。
7. 「Build and deployment」の Source を「Deploy from a branch」、Branch を「main」「/(root)」にして「Save」を押します。
8. 1〜2分待つと、同じ画面に公開URLが表示されます。
   形式は `https://あなたのユーザー名.github.io/shogi/` です。

このURLを送れば、誰でもログインなしで遊べます。

## iPhoneのホーム画面に追加する

1. SafariでURLを開きます。
2. 下の共有ボタン（□に↑）を押します。
3. 「ホーム画面に追加」を押します。

## アプリを更新するとき

1. 新しい index.html をGitHubに上書きアップロードします。
2. sw.js の1行目にある `shogi-v1` を `shogi-v2` のように1つ上げてアップロードします。
   これを忘れると、古い版が表示され続けることがあります。
3. iPhoneでは、アプリを一度開いて閉じ、もう一度開くと新しい版になります。

## ファイル一覧

- index.html … アプリ本体
- manifest.webmanifest … アプリ名やアイコンの設定
- sw.js … オフラインで遊ぶための仕組み
- apple-touch-icon.png, icon-192.png, icon-512.png, icon-maskable-512.png … アイコン
