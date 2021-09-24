# PostgreSQL

## Overview
- PostgreSQL:alpine13.4の環境
- GUIはpgAdmin4で接続も可能

## 動作環境（確認済）
- macOS BigSur 11.5.1
- Docker Desktop(macOS) 20.10.7

## Install
```
$ git clone git@github.com:yuiki-iwayama/PostgreSQL-Docker.git
$ cd PostgreSQL-Docker
$ docker-compose up -d --build
```

## Usage
- コンテナでSQLを直接操作
```
$ docker-compose exec db bash
# psql -U admin -h localhost
```

- pgAdmin4アプリで操作
1. http://localhost:8000に接続する
2. **General**でデータベースの任意の名前を入力する
3. **Connection**でdocker-compose.ymlのpostgres側の情報を入力する

※下記を参照する\
https://www.souya.biz/blog2/pinevillage/2021/03/07/post-0/

## Document
- Postgresを永続化するために./volumes/db-dataを配置
- pdAdmin４を永続化するために./volumes/pgadmin4-volumeを配置
