# docker-lamp
[![Build Status](https://travis-ci.org/sooch/docker-lamp.svg?branch=master)](https://travis-ci.org/sooch/docker-lamp)

Lightweight LAMP environment on docker


## Features
Based on [Alpine Linux](https://alpinelinux.org/) images.

|Container|Based Image|Host Port|
|:--|:--|:--|
|Apache|[httpd:2.4.28-alpine](https://github.com/docker-library/httpd/blob/5b3b87b10907617b0d69af4308ae1dfa21ccf703/2.4/alpine/Dockerfile)|8000|
|PHP|[php:7.1-fpm-alpine](https://github.com/docker-library/php/blob/0bb4068bd639ba98631bc2999e0d20cae583ec00/7.1/alpine3.4/fpm/Dockerfile)|-|
|MySQL|[mysql:5.7](https://github.com/docker-library/mysql/blob/0590e4efd2b31ec794383f084d419dea9bc752c4/5.7/Dockerfile)|13306|


## Requiements
- [`docker`](https://www.docker.com/
) 
```bash
$ docker --version
Docker version ...
```
- [`docker-compose`](https://docs.docker.com/compose/)
```bash
$ docker-compose --version
docker-compose version ...
```


## Setup
1. Clone
```bash
git clone https://github.com/sooch/docker-lamp.git
```

2. Copy .env file
```bash
$ cp .env.example .env
```

3. up !!
```bash
$ docker-compose up -d
```


## [The .env file](https://docs.docker.com/compose/environment-variables/#the-env-file)
You can set default values for any environment variables referenced in the Compose file, or used to configure Compose, in an environment file named .env:

**Example**
```.env
APP_NAME=app_name
TZ=Asia/Tokyo
```
