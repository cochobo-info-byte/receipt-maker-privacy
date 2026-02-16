# ⚡ クイックスタートガイド - 5分でGitHub Pages公開

## 🎯 概要

このガイドに従えば、**5分以内**にプライバシーポリシーをGitHub Pagesで公開できます。

## 📦 必要なもの

- ✅ GitHubアカウント（cochobo-info-byte）
- ✅ このバックアップファイル
- ✅ インターネット接続

---

## 🚀 3ステップデプロイメント

### ステップ1️⃣: GitHubリポジトリ作成（1分）

1. https://github.com/new を開く
2. 以下を入力：
   - Repository name: **`receipt-maker-privacy`**
   - Description: **`Privacy Policy for Receipt Maker Android App`**
   - Visibility: **Public** ✅
3. **他のチェックボックスは全てOFF**
4. 「Create repository」をクリック

### ステップ2️⃣: コードをアップロード（2分）

**方法A: GitHubのWebインターフェース（簡単！）**

1. 作成したリポジトリページで「uploading an existing file」をクリック
2. バックアップファイルを展開
3. 以下のファイルをドラッグ&ドロップ:
   - `index.html`
   - `README.md`
   - `SETUP_GUIDE.md`
   - `_config.yml`
   - `.gitignore`
4. コミットメッセージ: `Initial commit: Privacy Policy`
5. 「Commit changes」をクリック

**方法B: コマンドライン**

```bash
# バックアップを展開済みのディレクトリで:
git remote add origin https://github.com/cochobo-info-byte/receipt-maker-privacy.git
git push -u origin main
```

### ステップ3️⃣: GitHub Pages有効化（1分）

1. リポジトリの **Settings** タブをクリック
2. 左サイドバーの **Pages** をクリック
3. **Source** セクション:
   - Branch: **main**
   - Folder: **/ (root)**
4. **Save** をクリック
5. ✅ 完了！1-2分で公開されます

---

## 🎉 公開完了！

### 確認方法

1. Settings → Pages に戻る
2. 上部に緑色のメッセージが表示される：
   ```
   ✅ Your site is live at https://cochobo-info-byte.github.io/receipt-maker-privacy/
   ```
3. URLをクリックして確認

### Google Play Consoleに登録

```
https://cochobo-info-byte.github.io/receipt-maker-privacy/
```

このURLをコピーして、Play Consoleの「プライバシーポリシー」欄に貼り付け。

---

## 🔄 更新方法（1分）

### GitHubで直接編集

1. リポジトリの `index.html` をクリック
2. 鉛筆アイコン（Edit）をクリック
3. 編集して「Commit changes」

✅ 1-2分後に自動反映！

---

## 🆘 よくある問題

### Q: 404エラーが出る
**A:** 1-2分待ってから再度アクセス。初回公開は時間がかかります。

### Q: 認証エラーでプッシュできない
**A:** Personal Access Token (PAT) を使用：
- https://github.com/settings/tokens/new
- Scopes: `repo` を選択

### Q: ページが表示されるが真っ白
**A:** ブラウザキャッシュをクリア (Ctrl+Shift+R)

---

## 📞 サポート

問題が解決しない場合：
- **詳細ガイド:** `SETUP_GUIDE.md` を参照
- **GitHub Issues:** https://github.com/cochobo-info-byte/receipt-maker-privacy/issues

---

**所要時間:** 約5分  
**難易度:** ⭐☆☆☆☆ (初心者向け)  
**最終更新:** 2024-02-16
