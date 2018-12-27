# lemp
nginx+DB+PHPなどの環境を用意していきます

## テスト環境
### conohaのVPS
* メモリ：512MB
* CPU：1コア
* SSD：20GB

### さくらののVPS
* メモリ：512MB
* CPU：1コア
* SSD：20GB

### 実行方法
SFTPなどでアップロードをして、rootユーザーもしくはsudo権限で実行
wgetを使用する場合は[環境構築スクリプトを公開してます](https://www.logw.jp/cloudserver/8886.html)を閲覧してください。
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

## [nginx_php72_mariadb103_drn.sh](https://github.com/site-lab/lemp/blob/master/nginx_php72_mariadb103_drn.sh)
nginx+PHP7.2+MariaDB10.3をインストールします。
PHP7は **FastCGI版** となります

## [nginx_php73_mariadb103_drn.sh](https://github.com/site-lab/lemp/blob/master/nginx_php73_mariadb103_drn.sh)
nginx+PHP7.3+MariaDB10.3をインストールします。
PHP7は **FastCGI版** となります

## [nginx_php72_mysql57_drn.sh](https://github.com/site-lab/lemp/blob/master/nginx_php72_mysql57_drn.sh)
nginx+PHP7.2+MySQL5.7をインストールします。
PHP7は **FastCGI版** となります

## [nginx_php73_mysql57_drn.sh](https://github.com/site-lab/lemp/blob/master/nginx_php72_mysql57_drn.sh)
nginx+PHP7.3+MySQL5.7をインストールします。
PHP7は **FastCGI版** となります
