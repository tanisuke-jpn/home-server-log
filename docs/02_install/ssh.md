# SSH設定


## 概要

別PCからサーバを管理するため、
OpenSSH Serverを利用する。


## インストール確認

状態確認：

```bash
systemctl status ssh
```


正常時：

```
active (running)
```


## 起動設定

自動起動：

```bash
sudo systemctl enable ssh
```


起動：

```bash
sudo systemctl start ssh
```


## Windowsから接続

PowerShell：

```powershell
ssh ユーザー名@192.168.0.8
```


## 接続確認

接続後：

```bash
hostname
```

結果：

```
tanisv-p330
```


## 注意

サーバ管理は基本的にSSH経由で実施。

モニター・キーボードなし運用を目指す。