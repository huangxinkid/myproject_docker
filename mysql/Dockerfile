FROM mysql:5.7

# 设置环境变量，用户名以及秘密
ENV MYSQL_USER root
ENV MYSQL_PASS 123456
ENV MYSQL_DATABASE=mysite_db
ENV MYSQL_ROOT_PASSWORD=123456

# 添加文件夹下的 MYSQL 配置文件
ADD ./conf/my.cnf /etc/mysql/conf.d/my.cnf
ADD ./init/init.sql /docker-entrypoint-initdb.d/

# 设置可以映射的端口
EXPOSE 3306
