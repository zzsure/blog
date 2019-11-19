# How install mysql with docker-compose on ubuntu

## QA
1. github: https://github.com/zzsure
2. blog: https://blog.azbit.cn
3. wx: zhzosh

## Prerequisites
1. ubuntu: 18.04
2. git: 2.17.1
2. docker-compose: 1.23.2

[How install Docker-Compose](https://blog.azbit.cn/2019/11/15/how-install-docker-and-docker-compose-on-ubuntu/)

## Installing Mysql
1. git clone git@github.com:zzsure/deploy.git
2. create .env in mysql floder, and set PORT, ROOT_PASSWORD, DATA_PATH
3. sh start.sh;
4. mysql -h127.0.0.1 -uroot -p{MYSQL_ROOT_PASSWORD} -P{DEV_PORT}
