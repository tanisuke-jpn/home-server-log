# Docker


## 概要

Dockerはアプリケーションをコンテナ単位で動作させる仕組み。

自宅サーバでは、各サービスを分離して管理するために利用する。


## 利用目的

このサーバでは以下のサービスをDocker上で動作させる予定。

- Portainer
- Homarr
- Jellyfin
- Navidrome
- Syncthing
- Pi-hole
- EPGStation


## インストール

Ubuntu Serverへインストール：

```bash
sudo apt update

sudo apt install docker.io
```


## サービス起動

Dockerを自動起動：

```bash
sudo systemctl enable docker
```


起動：

```bash
sudo systemctl start docker
```


## 動作確認

バージョン確認：

```bash
docker --version
```


コンテナ一覧：

```bash
docker ps
```


## ユーザー設定

sudoなしでdockerを利用する場合：

```bash
sudo usermod -aG docker $USER
```


設定反映後、ログアウト・ログインする。


## 管理方針

基本的に以下の構成で管理する。

```
Docker
 |
 ├ コンテナ
 |
 ├ ボリューム
 |
 └ composeファイル
```


## 注意

重要なデータはコンテナ内ではなく、
ホスト側ディレクトリへ保存する。

例：

```
/opt/docker/
```