# Adfit LP

AI広告運用チーム「Adfit」のランディングページ（静的サイト）。

## 構成
```
index.html        … ページ本体
support.js        … 描画ランタイム（必須）
image-slot.js     … ヒーロー背景の表示用（必須）
assets/           … 画像一式（WebP / PNG）
```
※ `index.html` 単体では動きません。上記をすべて同じ階層のまま配置してください。

## Vercelへデプロイ（GitHub連携）
1. このフォルダの中身をリポジトリ直下に置く
   ```bash
   git init
   git add .
   git commit -m "init: Adfit LP"
   git branch -M main
   git remote add origin https://github.com/<ユーザー名>/<リポジトリ名>.git
   git push -u origin main
   ```
2. [vercel.com/new](https://vercel.com/new) で Import
3. Framework Preset = **Other**（Static／ビルド設定なし）→ **Deploy**
4. 以降は `git push` で自動デプロイ

## 補足
- 「無料で相談する」は formrun の問い合わせフォームへ遷移します。
- フォーム／Xタイムライン／Webフォントは外部読み込みのため、公開サイトでは正常表示されます。
- 1ファイル版で出ていた「building…」スプラッシュは、この複数ファイル構成では表示されません。
- 独自ドメインは Vercel の Project → Settings → Domains から接続できます。
