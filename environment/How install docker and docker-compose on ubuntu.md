# How install docker and docker-compose on ubuntu

Please contact me with any questions.    blog: https://blog.azbit.cn     wechat: zhzosh

## Prerequisites
1. ubuntu: 18.04
2. user: root
3. terminal: iterm2

## Steps For Installing Docker
1. sudo yum install -y yum-utils device-mapper-persistent-data lvm2
2. sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
3. sudo yum install docker-ce
4. sudo systemctl start docker
5. sudo systemctl enable docker
6. sudo docker run hello-world

## Steps For Installing Docker-Compose
1. sudo curl -L "https://github.com/docker/compose/releases/download/1.23.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
2. sudo chmod +x /usr/local/bin/docker-compose
3. docker-compose --version

Tips: If you want a different version of Docker Compose, you may [browse the list](https://github.com/docker/compose/releases) and substitute your preferred version for /1.23.2/
