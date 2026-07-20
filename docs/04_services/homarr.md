# Homarr


## 概要

自宅サーバ用ダッシュボード。


## 目的

複数サービスへの入口を一つにまとめる。


## 表示予定

- Cockpit
- Portainer
- CasaOS
- Jellyfin
- Navidrome
- Syncthing
- Pi-hole


## Docker

Docker Composeで管理する。


例：

```yaml
services:
  homarr:
    image: ghcr.io/homarr-labs/homarr
```


## アクセス

例：

```
http://192.168.0.8:7575
```


## メモ

サーバ利用者が最初に開くページとして使用予定。