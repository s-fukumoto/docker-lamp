## LAMP環境構築(docker)
少し古い開発環境が必要になりdockerで構築

## 環境
Docker Toolbox version 17.10.0-ce
Docker version 17.10.0-ce, build f4ffd25
docker-compose version 1.16.1, build 6d1ac219

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
