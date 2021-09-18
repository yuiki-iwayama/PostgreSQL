# PostgreSQL

## Overview
- PostgreSQL:alpine13.4の環境
- JupyterLab接続確認用に作成

## 動作環境（確認済）
- macOS BigSur 11.5.1
- Docker Desktop(macOS) 20.10.7

## Install
```
$ git clone https://github.com/yuiki-iwayama/PostgreSQL-Docker
$ cd PostgreSQL-Docker
$ docker-compose up -d --build
```

## Usage
```
$ docker-compose exec db bash
$ psql -U admin
```

## Document
- データベースを永続化するために./db-dataを配置
