---
title: Robot framework 环境配置
date: 2021-06-30 00:43:16
tags:
    - python
    - 自动化测试
categories:
    - 测试
    - 自动化脚本
cover: http://howiechen95.com:8888/group1/M00/00/00/CgAMB2DbUhyAal3gAAL08K4etkA976.jpg
---

### 一、介绍

Robot Famework 是一款python编写的功能自动化测试框架。具备良好的可扩展性，支持关键字驱动，可以同时测试多种类型的客户端或者接口，可以进行分布式测试执行。主要用于轮次很多的验收测试和验收测试驱动开发（ATDD）。

### 二、安装 python 和 pycharm

### 三、pycharm 插件

1. IntelliBot
File—>settings—>Plugins—>搜索 IntelliBot—>install

2. 配置robotframework的文件类型识别 
File—>settings—>Editor—>File Types  -->Robot Feature –>在Registered Patterns 中添加两种类型：*.txt,*.robot

3. 运行配置
File—>settings—>Tools—>External Tools –>添加两个运行配置。

4. suite 运行时配置

```
name: Robot Run TestSuite    
Program: D:\Python\Python37\Scripts\robot.exe     
Arguments: -d results $FileName$    
Working directory: $FileDir$    
```

参考文章：     
* [python3+Robot Framework+PyCharm 环境部署](https://www.cnblogs.com/emma-lucas/p/11231722.html)
