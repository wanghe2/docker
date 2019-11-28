FROM java:8
MAINTAINER wanghe

COPY spring-valid-0.0.1-SNAPSHOT.jar /properties.jar
ENV URL=jdbc:mysql://192.168.99.100:3306/docker_wh_mysql USER=root PASSWD=123456
EXPOSE 8088
#ENTRYPOINT  ["sh","-c","java $params -D -jar /properties.jar"]
ENTRYPOINT  ["sh","-c","java -jar /properties.jar --url=$URL --username=$USER --passwd=$PASSWD"]

#创建镜像
#docker build -t wh-param .
#运行镜像
#docker run -p 8088:8088 wh-param