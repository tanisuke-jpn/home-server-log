# GitHub Pages公開


## 目的

MkDocsで作成したサイトを
GitHub Pagesで公開する。


## 必要なもの

- GitHubアカウント
- Gitリポジトリ
- MkDocs


## Materialテーマの場合


インストール：

```bash
pip install mkdocs-material
```


## GitHubへ登録


```bash
git remote add origin リポジトリURL

git push -u origin main
```


## 公開用ビルド


```bash
mkdocs gh-deploy
```


## 公開後


URL例：

```
https://ユーザー名.github.io/home-server-log/
```


## 注意

公開する場合、

- IPアドレス
- パスワード
- 個人情報
- 外部公開したくない設定

は削除する。