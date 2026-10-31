# PayNote

大学生向けのおこづかい帳 PWA。次の入金日まで、1日あといくら使えるかを表示します。

## GitHub Pages で公開する手順

1. GitHub で新しいリポジトリを作る（例: `paynote`、Public）
2. このフォルダの中身（index.html, manifest.webmanifest, sw.js, icon-*.png）をリポジトリ直下にアップロード
3. リポジトリの Settings → Pages → Branch を `main` / `/(root)` にして Save
4. 数分後、`https://<ユーザー名>.github.io/paynote/` で開けるようになる

## iPhone のホーム画面に追加

1. Safari で上の URL を開く
2. 共有ボタン → 「ホーム画面に追加」
3. ホーム画面のアイコンから起動すると、アプリのように全画面で動き、オフラインでも使える

## データについて

- 記録は iPhone 内（ブラウザの localStorage）だけに保存され、どこにも送信されません
- Safari のタブで使うより、ホーム画面に追加して使うほうがデータが消えにくいです
- アプリを更新したときは sw.js の `CACHE` の名前（paynote-v3 → paynote-v4 など）を変えると、新しい版が反映されます
- 旧名（あと何円・ペイノート）のときに記録したデータも、同じURLで開けばそのまま引き継がれます
