# TweetLauncher

このパックには以下の2つが含まれています：

- `TweetGenerator.exe`  
  → Gemini API を使ってツイート文を自動生成し、`tweet.txt` に保存するツール（初回のみAPIキー入力）

- Chrome拡張機能  
  → `tweet.txt` の内容を読み取り、ボタンひとつでTwitterの投稿画面を開く

---

## ✅ 基本的な使い方

1. `TweetGenerator.exe` を実行（初回のみ Gemini APIキーの入力あり）  
   → `tweet.txt` に最新のツイート文章が自動生成されます

2. `chrome_extension` フォルダを Chrome に読み込む  
   - `chrome://extensions/` にアクセス  
   - 「パッケージ化されていない拡張機能を読み込む」ボタンから `chrome_extension` フォルダを指定

3. ツールバーの拡張アイコンをクリック  
   - `tweet.txt` の内容が表示されます  
   - 「ツイート画面を開く」ボタンを押すと、Twitterの投稿画面が別タブで開きます  
   - ※投稿は自動ではなく、**手動で送信ボタンを押す形式**です

---

## ⏱ 自動化（1時間ごとにツイート文を自動生成）

`TweetGenerator.exe` をWindowsのタスクスケジューラーに登録することで、  
1時間ごとに `tweet.txt` の内容を自動更新できます。

手順については本README内の「自動化」セクションをご確認ください。

---

## 📦 ダウンロード

最新版の配布パッケージ（ZIP形式）は、以下のリリースページからダウンロードできます：

👉 [TweetLauncher リリースページ](https://github.com/DaitaiOK/TweetLauncher/releases/latest)

> ※ ダウンロード後は ZIP を展開し、任意のフォルダに置いてご利用ください。
> ※ prompt.txt を編集することでツイート内容を自由にカスタマイズできます。
