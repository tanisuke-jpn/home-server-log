# SSHトラブル


## SSH接続できない


## 確認項目


### 1. サーバ起動確認

サーバ本体が起動しているか確認する。


### 2. IPアドレス確認

サーバ側：

```bash
ip addr
```


確認例：

```
192.168.0.8
```


### 3. SSHサービス確認

```bash
systemctl status ssh
```


正常：

```
active (running)
```


### 4. ポート確認

SSHは通常22番ポートを使用。

```bash
ss -tlnp | grep ssh
```


## Windows側確認

```powershell
ping 192.168.0.8
```


応答があるか確認する。


## メモ

SSHはサーバ管理の基本となるため、
最初に確認する項目として記録する。