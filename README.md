# Tanis Home Server Log

ThinkStation P330 Tinyを使用した
自宅サーバ構築記録です。


## Server Hardware

|項目|内容|
|-|-|
|PC|ThinkStation P330 Tiny|
|CPU|Intel Core i7-8700T|
|Memory|32GB|
|GPU|NVIDIA Quadro P620|
|Storage|NVMe SSD|
|OS|Ubuntu Server 24.04|


## Software

- Cockpit
- Docker
- Portainer
- CasaOS
- Homarr
- Jellyfin
- Navidrome
- Syncthing
- Pi-hole
- EPGStation


## 目的

このサイトは以下を目的に作成しています。

- サーバ構築手順の記録
- 設定変更履歴の保存
- トラブル対応記録
- 再構築時の手順書
- AIへの情報提供用ドキュメント


## MkDocs起動

インストール：

```bash
pip install mkdocs
```

起動：

```bash
mkdocs serve
```

ブラウザ：

```
http://127.0.0.1:8000
```