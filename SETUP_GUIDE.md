# 🚀 Receipt Maker Privacy Policy - GitHub Pages セットアップガイド

このガイドでは、プライバシーポリシーをGitHub Pagesで公開する手順を説明します。

## 📋 前提条件

- GitHubアカウント（cochobo-info-byte）
- Gitコマンドラインツール
- このリポジトリのローカルコピー

## 🔧 セットアップ手順

### ステップ1: GitHubで新規リポジトリ作成

1. **GitHubにログイン**
   - https://github.com にアクセス
   - アカウント: `cochobo-info-byte` でログイン

2. **新規リポジトリを作成**
   - 右上の「+」→「New repository」をクリック
   - または直接: https://github.com/new

3. **リポジトリ設定**
   ```
   Repository name: receipt-maker-privacy
   Description: Privacy Policy for Receipt Maker Android App
   Visibility: ✅ Public (GitHub Pagesには必須)
   ❌ Initialize this repository with:
      - README (チェックしない)
      - .gitignore (チェックしない)
      - License (チェックしない)
   ```

4. **「Create repository」をクリック**

### ステップ2: ローカルリポジトリをプッシュ

GitHubリポジトリ作成後、以下のコマンドを実行：

```bash
cd /home/user/receipt-maker-privacy

# リモートリポジトリを追加
git remote add origin https://github.com/cochobo-info-byte/receipt-maker-privacy.git

# メインブランチをプッシュ
git branch -M main
git push -u origin main
```

### ステップ3: GitHub Pagesを有効化

1. **リポジトリのSettingsへ移動**
   - https://github.com/cochobo-info-byte/receipt-maker-privacy/settings

2. **左サイドバーの「Pages」をクリック**

3. **GitHub Pages設定**
   ```
   Source: Deploy from a branch
   Branch: main
   Folder: / (root)
   ```

4. **「Save」をクリック**

5. **公開完了を待つ**
   - 通常1-2分で公開されます
   - ページ上部に緑色のチェックマークと公開URLが表示されます

### ステップ4: 公開URLを確認

**公開URL:**
```
https://cochobo-info-byte.github.io/receipt-maker-privacy/
```

ブラウザでアクセスして、プライバシーポリシーが正しく表示されることを確認してください。

## 📝 Google Play Consoleでの設定

1. **Play Consoleにアクセス**
   - https://play.google.com/console

2. **アプリを選択** → **ポリシー** → **アプリのコンテンツ**

3. **プライバシーポリシー欄に以下のURLを入力:**
   ```
   https://cochobo-info-byte.github.io/receipt-maker-privacy/
   ```

4. **保存**

## 🔄 プライバシーポリシーの更新方法

プライバシーポリシーを更新する場合：

```bash
cd /home/user/receipt-maker-privacy

# index.htmlを編集
nano index.html

# 変更をコミット
git add index.html
git commit -m "プライバシーポリシー更新: [変更内容]"

# GitHubへプッシュ
git push origin main
```

GitHub Pagesは自動的に更新されます（1-2分後）。

## 🎯 カスタムドメインの設定（オプション）

独自ドメイン（例: privacy.receiptmaker.com）を使用したい場合：

1. **DNS設定**
   - ドメインのDNS設定でCNAMEレコードを追加
   ```
   privacy.receiptmaker.com → cochobo-info-byte.github.io
   ```

2. **GitHub Pages設定**
   - Settings → Pages → Custom domain
   - ドメイン名を入力: `privacy.receiptmaker.com`
   - 「Save」をクリック

3. **HTTPS強制を有効化**
   - 「Enforce HTTPS」にチェック

## ✅ 確認事項チェックリスト

- [ ] GitHubリポジトリ作成完了
- [ ] ローカルリポジトリをプッシュ完了
- [ ] GitHub Pages有効化完了
- [ ] 公開URLでアクセス可能
- [ ] プライバシーポリシーが正しく表示される
- [ ] Google Play ConsoleにURL登録

## 🆘 トラブルシューティング

### GitHub Pagesが公開されない

- リポジトリが **Public** に設定されているか確認
- Settings → Pages で設定が正しいか確認
- 1-2分待ってから再度アクセス

### 404エラーが表示される

- `index.html` ファイルがルートディレクトリにあるか確認
- ファイル名が正確に `index.html` か確認（大文字小文字区別）

### プッシュ時に認証エラー

- Personal Access Token (PAT) を使用
- https://github.com/settings/tokens で生成
- `repo` スコープを有効化

## 📞 サポート

問題が発生した場合は、GitHubのIssuesで報告してください：
https://github.com/cochobo-info-byte/receipt-maker-privacy/issues

---

**最終更新:** 2024年2月16日  
**バージョン:** 1.0.0
