# lemp
nginx+PHP+Databaseなどの環境を用意していきます

## テスト環境
### conohaのVPS
* メモリ：512MB
* CPU：1コア
* SSD：20GB

### さくらののVPS
* メモリ：512MB
* CPU：1コア
* SSD：20GB

### さくらのクラウド
* メモリ：1GB
* CPU：1コア
* SSD：20GB

### IDCFクラウド
* メモリ：1GB
* CPU：1コア
* SSD：15GB

### 実行方法
SFTPなどでアップロードをして、rootユーザーもしくはsudo権限で実行
wgetを使用する場合は[Buildree](https://buildree.com/)を閲覧してください。
wgetがない場合は **yum -y install wget** でインストールしてください

**sh ファイル名.sh** ←同じ階層にある場合

**sh /home/ユーザー名/ファイル名.sh** ユーザー階層にある場合（rootユーザー実行時）

## 共通内容
* epelインストール
* gitのインストール
* システム更新
* mod_sslのインストール
* HTTP2の有効化
* firewallのポート許可(80番、443番)
* gzip圧縮の設定
* centosユーザーの作成
* スロークエリ有効化

## [nginx_php_mariadb103_drn.sh](https://github.com/site-lab/lemp/blob/master/nginx_php_mariadb103_drn.sh)
nginx+PHP7.x+MariaDB10.3をインストールします。
**PHP**
- 7.2系：2020年中に削除予定
- 7.3系
- 7.4系

## [nginx_php_mysql.sh](https://github.com/site-lab/lemp/blob/master/nginx_php_mysql.sh)
nginx+PHP7.x+MySQLをインストールします。
**PHP**
- 7.2系：2020年中に削除予定
- 7.3系
- 7.4系

**MySQL**
- 5.7
- 8.0
