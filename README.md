使用说明
一、需要安装与配置环境
  该示例在Java中实现，需要编译示例，因此需要安装JDK（Java Development Kit）。JRE（Java运行时环境）是不够的。安装完毕后，确保能够执行 java，并在命令行上成功执行javac；
  安装Maven，确保能执行Maven命令；
  该示例在Docker容器中运行，需要安装Docker Community Edition，确保能够docker在安装后运行；
  安装Docker后，确保能够运行 docker-compose。
二、运行说明
1.建立项目
  切换目录到microservice-demo，运行命令mvn clean package，
2.运行容器
  切换目录到docker，运行命令sudo docker-compose build，
  运行命令sudo docker-compose up –d，
  运行命令docker ps，查看所以服务是否开启；
3.Web应用访问
  打开浏览器，输入http://localhost:8080/即可访问。
4.终止所有容器
  运行命令docker-compose down；
