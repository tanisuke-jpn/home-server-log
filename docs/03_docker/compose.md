# Docker Compose


## 概要

複数のコンテナ設定を
YAMLファイルで管理する仕組み。


## 利点

- 設定をファイル化できる
- 再構築が容易
- バックアップしやすい
- Git管理できる


## 基本構成

例：

```
service/
 |
 ├ docker-compose.yml
 |
 └ data/
```


## 起動

composeファイルがある場所で実行：

```bash
docker compose up -d
```


## 停止

```bash
docker compose down
```


## 更新

イメージ更新：

```bash
docker compose pull
```


再起動：

```bash
docker compose up -d
```


## 管理方針

各サービスごとにディレクトリを分ける。

例：

```
/opt/docker/

├ jellyfin/
├ navidrome/
├ syncthing/
└ pihole/
```


## メモ

設定ファイルはGit管理対象にする。

ただし、

- パスワード
- APIキー
- 個人情報

は除外する。