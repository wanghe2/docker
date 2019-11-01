# docker
1.进入docker-layui文件夹
2.执行命令 docker build layui:v1 .    (layui:v1是自己定义的镜像名，v1是版本号)
3.创建并运行容器 docker run -d -p 8080:8098  layui:v1  
4.此时访问 http://192.168.137.128:8080/page/lay1.html （192.168.137.128是你的ip）
5.还可以对容器进行其他操作，如传到远程仓库，等等，不再赘述
