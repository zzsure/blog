# How install certbot with docker-compose on ubuntu

## QA
1. github: https://github.com/zzsure
2. blog: https://blog.azbit.cn
3. wx: zhzosh

## Prerequisites
1. ubuntu: 18.04
2. git: 2.17.1
3. docker-compose: 1.23.2
4. nginx: latest

[How install Docker-Compose](https://blog.azbit.cn/2019/11/15/how-install-docker-and-docker-compose-on-ubuntu/)
[How install nginx](https://blog.azbit.cn/2019/11/15/how-install-nginx-with-docker-compose-on-ubuntu/)

## Installing certbot
1. git clone git@github.com:zzsure/deploy.git
2. cd certbot
3. open renew_cert.sh file and change volume mapping, email, domain name
4. sh renew_cert.sh  it can generate ssl file
5. add "0 0 1 * * cd /root/deploy/certbot; sh renew_cert.sh" to crontab
