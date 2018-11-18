# mysql
## docker-compose.yml
```
version: '2.0'

services:
   db:
     image: mysql:5.7
     volumes:
       - db_data:/sapmnt/HOME/i075883/dockers/mysql/mysqldata
     restart: always
     ports:
       - "3306:3306"
     environment:
       MYSQL_ROOT_PASSWORD: somewordpress
       MYSQL_DATABASE: wordpress
       MYSQL_USER: wordpress
       MYSQL_PASSWORD: wordpress

volumes:
    db_data:
```

## 启动命令
docker-compose up -d

## 参考文件
### https://hub.docker.com/_/mysql/
列出了参数和方法

### https://hub.docker.com/r/mysql/mysql-server/

### https://docs.docker.com/compose/wordpress/
用compose整合mysql和wordpress

# phpmyadmin

## 参考文件
### https://github.com/phpmyadmin/docker
列出列docker phpmyadmin命令，以及怎样整合

### https://docs.phpmyadmin.net/en/latest/setup.html#installing-using-docker
安装

# 其他参考
## https://docs.docker.com/compose/compose-file/compose-file-v2/#platform
## https://hub.docker.com/r/phpmyadmin/phpmyadmin/
## https://docs.docker.com/compose/reference/stop/


