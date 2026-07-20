# Tanis Home Server Log

自宅サーバ構築記録


## サーバ概要

ThinkStation P330 Tinyをベースに、
家庭内向けサーバを構築しています。


## 目的

- 家庭内ファイル共有
- 音楽サーバ
- 動画サーバ
- スマートフォンとの同期
- 広告ブロック
- 録画サーバ


## 構成

```text
Internet
   |
Router
   |
Switch
   |
ThinkStation P330 Tiny

 ├ Ubuntu Server
 │
 ├ Cockpit
 │
 ├ Docker
 │   ├ Portainer
 │   ├ Homarr
 │   ├ Jellyfin
 │   ├ Navidrome
 │   ├ Syncthing
 │   ├ Pi-hole
 │   └ EPGStation
 │
 └ NAS Storage
```


## 現在の状態

|項目|状態|
|-|-|
|Ubuntu Server|導入済み|
|SSH|設定済み|
|Docker|導入予定|
|Cockpit|導入予定|
|NAS|構築予定|
|録画サーバ|構築予定|


## 更新履歴

詳細は `maintenance/changelog.md` を参照してください。