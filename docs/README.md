# カナウサギのんびり日より PWA版

まっさら初期状態の GitHub Pages + PWA 版です。
予定、Sunoお気に入り、画像・動画、時計デザインをブラウザ内に保存できます。

## 公開するファイル

GitHub Pages に公開するときは、このフォルダ全体をリポジトリへ置きます。

```text
kanawusagi-nonbiri-pwa/
├─ index.html
├─ app/
│  ├─ index.html
│  ├─ style.css
│  ├─ script.js
│  ├─ manifest.json
│  ├─ sw.js
│  └─ assets/
└─ docs/
   └─ README.md
```

## GitHub Pages 設定

1. GitHubで新規リポジトリを作成
2. このZIPの中身をアップロード
3. Settings → Pages
4. Source: `Deploy from a branch`
5. Branch: `main` / `/ (root)`
6. Save

公開URL例：

```text
https://ユーザー名.github.io/リポジトリ名/
```

## スマホ・PCへの追加

- iPhone: Safariで開く → 共有 → ホーム画面に追加
- Android: Chromeで開く → メニュー → アプリをインストール / ホーム画面に追加
- PC: Chrome / Edgeで開く → アドレスバー右側のインストールボタン

## 保存仕様

このPWA版は、予定やお気に入りをサーバーに送信しません。
ブラウザ内に保存します。

保存されるもの：

- 予定
- Sunoお気に入り
- タイトル
- 画像・動画
- 時計設定

バックアップしたい場合は、アプリ内の `JSONバックアップ` を使ってください。

## 注意

ブラウザのデータ削除をすると、保存済みの予定や画像が消える場合があります。
大事な予定は `予定CSV出力` と `JSONバックアップ` を定期的に使うのがおすすめです。
