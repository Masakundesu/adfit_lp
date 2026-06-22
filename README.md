# Adfit LP

AI広告運用チーム「Adfit」のランディングページ（静的HTML・1ファイル完結）。

## 構成
- `index.html` … 全アセット同梱の自己完結ページ（これ1枚で動作）

## Vercelへデプロイ（GitHub連携）
1. このフォルダをGitリポジトリにする
   ```bash
   git init
   git add .
   git commit -m "init: Adfit LP"
   git branch -M main
   git remote add origin https://github.com/<あなたのユーザー名>/<リポジトリ名>.git
   git push -u origin main
   ```
2. [vercel.com/new](https://vercel.com/new) を開く
3. 上記リポジトリを **Import**
4. Framework Preset は **Other**（ビルド設定なし／Static）でそのまま **Deploy**
5. 以降は `git push` するたびに自動デプロイされます

## 補足
- フォーム（formrun）／ Xタイムライン ／ Webフォントは外部読み込みです。公開サイト（通常のネット環境）では正常に表示されます。
- 独自ドメインは Vercel の Project → Settings → Domains から接続できます。
- 内容を更新する場合は、デザイン側で再ビルドした `index.html` を差し替えてコミットしてください。
