# How install wordpress multiple https sites on ubuntu using docker

## Prerequisites
1. ubuntu: 18.04
2. docker-compose: 1.23.2
3. mysql: 5.7
4. nginx: latest
5. certbot: latest

[Installing Docker-Compose](https://blog.azbit.cn/2019/11/15/how-install-docker-and-docker-compose-on-ubuntu/)
[Installing Mysql](https://blog.azbit.cn/2019/11/15/how-install-mysql-with-docker-compose-on-ubuntu/)
[Installing nginx](https://blog.azbit.cn/2019/11/15/how-install-nginx-with-docker-compose-on-ubuntu/)
[Installing certbot](https://blog.azbit.cn/2019/11/15/how-install-certbot-with-docker-compose-on-ubuntu/)

## Installing Wordpress
1. git clone git@github.com:zzsure/deploy.git
2. cd wordpress
3. create .env in wordpress floder, and set WORDPRESS_DB_HOST, WORDPRESS_DB_USER, WORDPRESS_DB_PASSWORD, WORDPRESS_DB_NAME
4. create wordpress db in mysql
5. sh start.sh
6. you can visit wordpress by http://{IP}:{Port} to install
7. login in management site: http://{IP}:{Port}/wp-admin.php/
8. Settings->WordPress Address and Site Address, fill your domain and Save Changes
9. you can visit your blog by domain name now.
