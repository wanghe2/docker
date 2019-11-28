部署war包，依赖tomcat镜像中，形成新的镜像

war包里其实要连接数据库，只需要在docker中启动一个mysql的容器，
并将端口暴露到宿主机，web项目就可以连接到该数据库

其实为了保险起见，应该使用 docker-compose 或者 --link进行容器互联，这个后面再实现