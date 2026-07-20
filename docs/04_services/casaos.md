# CasaOS


## 概要

家庭向けサーバ管理用のWeb UI。

Dockerアプリを簡単に管理できる。


## 目的

サーバ管理を簡単にするため、

- アプリ管理
- ストレージ管理
- Dockerコンテナ管理

に利用する。


## 導入方針

現在の構成では、

- OS管理 → Cockpit
- Docker管理 → Portainer
- アプリ管理 → CasaOS

という役割分担を想定。


## インストール例

公式インストールスクリプトを使用。

```bash
curl -fsSL https://get.casaos.io | sudo bash
```


## アクセス

ブラウザ：

```
http://サーバIP
```

例：

```
http://192.168.0.8
```


## 注意

CasaOSはDocker環境を簡単に扱うためのUI。

細かい設定はPortainerやcomposeファイルで管理する。