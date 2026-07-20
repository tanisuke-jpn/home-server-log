# Cockpit


## 概要

ブラウザからLinuxサーバを管理するための
Web管理ツール。


## 目的

SSHコマンドだけでは確認しにくい、

- CPU使用率
- メモリ使用量
- ディスク状態
- サービス状態

などをブラウザで確認する。


## インストール

```bash
sudo apt install cockpit
```


## 起動設定

```bash
sudo systemctl enable --now cockpit.socket
```


## アクセス

ブラウザ：

```
https://サーバIP:9090
```


例：

```
https://192.168.0.8:9090
```


## 使用予定

管理用途：

- システム監視
- サービス確認
- ログ確認
- アップデート管理


## メモ

Dockerコンテナ管理はPortainer、
OS管理はCockpitという役割分担にする。