## LAMP環境構築(docker)
少し古い開発環境が必要になりdockerで構築

## 環境
Docker Community Edition Version 17.09.1-ce-mac42 (21090) Channel: stbale 3176a6af01
Docker version 17.09.1-ce, build 19e2cf6
docker-compose version 1.17.1, build 6d101fb

## 構築手順


```
git clone https://github.com/s-fukumoto/docker-lamp.git
cd docker-lamp/
```

.envを環境に合わせて修正
```
cp .env_sample .env
vi .env
```

Dockerfileを環境に合わせて修正
```
cp -r web_sample web
vi /web/Dockerfile
vi /web/php.ini
```

環境構築
```
docker-compose up -d
```

確認
```
docker ps
```
