# m1 docker install

## 1. 下载安装
Go to https://docs.docker.com/desktop/mac/apple-silicon/ and click [Mac with Apple chip] to install dmg package
![download docker](./markdown_source/pic/note_m1_docker_install_1.png)

> * Here is an optional requirement, to have a best experience for docker, it`s better to install Rosetta2 in your mac, so run below command. But as your macos is Monterey(v12.1), Rosetta2 should be defaultly installed, this step is optional.
> ```bash
> softwareupdate --install-rosetta
> ```

## 2. 配置国内镜像源
科大镜像：https://docker.mirrors.ustc.edu.cn/  
网易：https://hub-mirror.c.163.com/  
阿里云：https://<你的ID>.mirror.aliyuncs.com  
七牛云加速器：https://reg-mirror.qiniu.com  

 
镜像放在那里?


## 3. docker常用命令
[官方参考](https://docs.docker.com/engine/reference/run/)
|用法|作用|常用参数|例子|
|----|----|----|----|
|docker [COMMAND] --help|查看所有/指定命令的用法||docker pull --help|
|docker pull [OPTIONS] NAME[:TAG\|@DIGEST]|下载镜像, 可以指定tag, 默认是latest||docker pull 
|docker images [OPTIONS] [REPOSITORY[:TAG]]|查看本地镜像的信息, 不带参数默认列出所有镜像,参数可指定特定仓库/特定tag的镜像||docker images; docker images java:8
|docker run [OPTIONS] IMAGE [COMMAND] [ARG...]|为镜像运行容器||docker run ubuntu




  


    

    
docker search 
docker images
docker run 
    docker run -d 后台运行容器
    docker run -p <host_port>:<container_expose_port> 指定容器端口映射到宿主机端口
docker ps
docker logs -f <container_id/name> 查看容器内部的标准输出, -f 类似tail -f滚动输出log
docker top <container_id/name> : 查看容器中运行的进程
docker inspect <container_id/name> : 查看容器底层信息
docker stop <container_id/name> : 停止容器
docker start <container_id/name> : 启动已经停止的容器
docker rm <container_id/name> : 删除不需要的已经停止的容器

docker port <container_id/container_name> 查看容器端口情况


