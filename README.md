# Vagrant + Ansibleのlemp環境

## 構成
- Centos 7.1
- Nginx 1.12
- MySQL 5.6
- PHP 7.1

## 必要ツール
- VirtualBox 5.0
- Vagrant 1.8
(当方上記バージョンにて確認)

## 開発ディレクトリ
デフォルトのドキュメントルートは`repository/your-app/public/`になっています。  
もし変更が必要であれば`ansible/group_vars/local`ファイルの`default_docroot`を修正し`vagrant up`を実行してください。  
一度`vagrant up`をした後に修正した場合は、`vagrant provision`を実行してください。

## 利用方法
cloneした`Vagrantfile`があるディレクトリで`vagrant up`コマンドを実行してください。  

## URL
- アプリ：[http://192.168.111.222](http://192.168.111.222)
- phpMyAdmin：[http://192.168.111.222:8080](http://192.168.111.222:8080) (id/pw root/vagrant)