# Dockerトラブル


## コンテナが起動しない


## 確認


### コンテナ一覧

```bash
docker ps -a
```


### ログ確認

```bash
docker logs コンテナ名
```


## コンテナ再起動

```bash
docker restart コンテナ名
```


## Composeの場合


停止：

```bash
docker compose down
```


起動：

```bash
docker compose up -d
```


## イメージ更新後

```bash
docker compose pull

docker compose up -d
```


## 注意

設定変更前には
composeファイルをバックアップする。