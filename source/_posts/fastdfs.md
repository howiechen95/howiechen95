---
title: Fastdfs 文件系统
date: 2021-06-23 01:04:34
updated:
tags: 中间件,文件系统  
categories: 中间件 
keywords: 分布式 中间件 文件系统 fastdfs
description: Fastdfs 介绍
cover: http://howiechen95.com:8888/group1/M00/00/00/CgAMB2DSxb6AI3KPAA4v7j_0ybc88.jpeg  
---
### 介绍
FastDFS是一个开源的轻量级分布式文件系统，它对文件进行管理，功能包括：文件存储、文件同步、文件访问（文件上传、文件下载）等，解决了大容量存储和负载均衡的问题。 特别适合以文件为载体的在线服务，如相册网站、视频网站等等。

### 文档
[源码 wiki](https://github.com/happyfish100/fastdfs/wiki)

fastdfs 如果要使用http下载，需要配置nginx代理

启动成功后会有 fdfs_storaged 和 fdfs_storaged 两个进程

```
/usr/bin/fdfs_trackerd /etc/fdfs/tracker.conf
/usr/bin/fdfs_storaged /etc/fdfs/storage.conf
```

// 配置完成后可以使用下面命令测试上传
```
fdfs_upload_file /etc/fdfs/client.conf [文件名]
```

fastdfs 限制上传下载安全，在/etc/fdfs/storage.conf 配置参数allow_hosts=[ip]

存储路径
```
/data/fastdfs
```


