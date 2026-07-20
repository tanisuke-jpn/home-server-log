# Ubuntu Server


## インストール概要

P330 TinyへUbuntu Serverをインストール。


## 使用環境

|項目|内容|
|-|-|
|OS|Ubuntu Server 24.04 LTS|
|CPU|Intel Core i7-8700T|
|Memory|32GB|
|Storage|NVMe SSD|


## インストール設定

設定内容：

|項目|設定|
|-|-|
|Boot|UEFI|
|Storage|LVM|
|Filesystem|ext4|
|Encryption|なし|
|SSH|有効|


## インストール時メモ

設定した項目：

- OpenSSH Serverを選択
- サーバ名を設定
- ネットワークはDHCP


## ホスト名

```
tanisv-p330
```


## ネットワーク

インストール時取得IP：

```
192.168.0.8
```


## 初回更新

インストール後：

```bash
sudo apt update

sudo apt upgrade
```


## 確認コマンド

OS確認：

```bash
cat /etc/os-release
```


カーネル確認：

```bash
uname -a
```