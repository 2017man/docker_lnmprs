# docker_lnmprs
一款基于宝塔打造的lnmp+redis_swoole快速开发环境的docker镜像
- [镜像地址](https://hub.docker.com/repository/docker/dockerbyman/lnmprs)
# 你想
- 快速部署lnmp+redis+swoole界面化服务端环境
- 统一的开发环境
- 和线上环境隔离
- 本地开发环境
# latest
基于centos7.8搭建的php高并发开发快速部署镜像
- centos
- npm(taobao)+yarn+yum(update)+wget
- git
- composer
- lnmp
- bt

# 使用
> docker请自行安装
## 拉取镜像并启动容器
- ### 端口+文件映射用法（快速开发用建议使用）
```
docker run -itd --name bt -p 30:20 -p 31:21 -p 90:80 -p 91:81 -p 92:82 -p 93:83 -p 94:84 -p 95:85 -p 96:86 -p 97:87 -p 98:88 -p 99:89 -p 543:443 -p 988:888 -p 4306:3306 -p 7379:6379 -p 9888:8888 --privileged=true -v E:\phpstudy\WWW:/www dockerbyman/lnmprs
```
- ###  端口映射用法（构建自己镜像建议使用）
```
docker run -it --name bt -p 30:20 -p 31:21 -p 90:80 -p 91:81 -p 92:82 -p 93:83 -p 94:84 -p 95:85 -p 96:86 -p 97:87 -p 98:88 -p 99:89 -p 543:443 -p 988:888 -p 4306:3306 -p 7379:6379 -p 9888:8888 --privileged=true dockerbyman/lnmprs
```

## 进入容器
- `docker exec -it bt /bin/bash`

## 使用面板
-  打开面板：浏览器输入ip：9888即可
