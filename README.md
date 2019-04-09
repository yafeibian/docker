# docker
学习笔记
查询镜像 docker search nginx
下载镜像 docker pull nginx --镜像名称
查看本机镜像 docker images
创建新镜像 docker commit f9d6ffce5b61 learn/ping 镜像新名称
上传镜像到中央仓库 docker push learn/ping 
查看镜像分层 docker history nginx

创建并启动容器 docker run nginx 
修改容器 docker run learn/tutorial apt-get install -y ping
显示机器上所用容器 docker ps -l
查询正在运行容器 docker ps
查看容器完整id docker ps --no-trunc
查看单个容器 docker inspect f9d6ffce5b61 容器ID
启动容器 docker start redmine_redmine_1 容器NAME
停止容器 docker stop redmine_redmine_1
删除容器 docker rm redmine_redmine_1
查看容器的log日志 docker logs nginx 
查看容器所占系统资源 docker status wordpress_db_1
容器内部命令 docker exec 容器名称 容器内部执行命令（docker exec wordpress_db_1 ps aux）
连续执行加-it docker exec -it WordPress_db_1 /bin/bash





