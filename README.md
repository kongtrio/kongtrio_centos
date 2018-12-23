#### 基于centos，构建一个属于自己的centos，主要做了以下修改:
- 安装了ssh、vim、less、wget
- 安装了jre1.8
- 修改了时区，变成北京时间

#### 拉取代码后通过以下命令构建镜像，镜像名可以随意更改:
```shell
docker build -t kongtrio_centos:v1 .
``` 

#### 之后启动容器:
```shell
docker run -d -P --name centos_test kongtrio_centos:v1 /usr/local/sbin/run.sh
```
