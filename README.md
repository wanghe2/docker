# docker
1.进入docker-layui文件夹
2.执行命令 docker build layui:v1 .    (layui:v1是自己定义的镜像名，v1是版本号)
3.创建并运行容器 docker run -d -p 8080:8098  layui:v1  
4.此时访问 http://192.168.137.128:8080/page/lay1.html （192.168.137.128是你的ip）
5.还可以对容器进行其他操作，如传到远程仓库，等等，不再赘述


---------------------------------------------------------------
              docker常用命令
---------------------------------------------------------------
1.docker pull java:8   		拉取镜像

2.docker build -t layui:v1 .  		在当前目录构建镜像

3.docker-machine ip default 	 	查看docker虚拟机的ip

4.docker run -d -p 8098:8098 layui:v1  	创建容器 （映射本地端口）   (-d 表示 后台启动方式运行)

5.docker images 			查看所有镜像

6.docker ps                                               查看运行中的容器

7.docker ps -a 			查看所有容器

8.docker stop xxx			停止容器

9.docker start xxx			启动容器

10. sudo docker attach xxx		进入运行的容器

11.docker rm xxx			删除容器

12.docker rmi xxx 			删除镜像

13.docker exec -i -t xxx bash   进入运行的容器，比较常用的方式
