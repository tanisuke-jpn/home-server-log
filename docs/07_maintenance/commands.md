# Linuxコマンド集


## システム確認


CPU確認：

```bash
lscpu
```


メモリ確認：

```bash
free -h
```


ディスク確認：

```bash
df -h
```


## サービス管理


状態確認：

```bash
systemctl status サービス名
```


起動：

```bash
sudo systemctl start サービス名
```


停止：

```bash
sudo systemctl stop サービス名
```


再起動：

```bash
sudo systemctl restart サービス名
```


## 更新


```bash
sudo apt update

sudo apt upgrade
```


## Docker


一覧：

```bash
docker ps
```


ログ：

```bash
docker logs コンテナ名
```