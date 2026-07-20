# Portainer


## 概要

Dockerコンテナをブラウザから管理するWeb UI。


## 目的

コマンド操作だけでは確認しにくい、

- コンテナ状態
- ログ
- イメージ
- ボリューム

をGUIで管理する。


## 導入

Dockerコンテナとして起動する。


例：

```bash
docker volume create portainer_data
```


```bash
docker run -d \
-p 8000:8000 \
-p 9443:9443 \
--name portainer \
--restart=always \
-v /var/run/docker.sock:/var/run/docker.sock \
-v portainer_data:/data \
portainer/portainer-ce
```


## アクセス

ブラウザ：

```
https://サーバIP:9443
```


例：

```
https://192.168.0.8:9443
```


## 役割分担

|管理対象|使用ソフト|
|-|-|
|Ubuntu本体|Cockpit|
|Docker|Portainer|
|サービス一覧|Homarr|


## メモ

PortainerはDocker管理専用として使用。

アプリの利用画面は各サービスへアクセスする。