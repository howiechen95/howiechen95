---
title: RocketMQ
date: 2021-12-02 23:26:30
tags:
    - MQ
    - RocketMQ
categories:
    - 消息队列
    - RocketMQ
---

### 一、介绍

[Apache RocketMQ](https://github.com/apache/rocketmq)

消息队列作用：
1.异步
2.削峰
3.解耦

### 二、概念

1.Producer 生产者
将消息存进消息队列中的一方，实际是发送给broker，由broker处理。

发送方式：
- 同步发送
- 异步发送
- 顺序发送
- 单向发送

同步和异步方式均需要Broker返回确认信息，单向发送不需要。

2.Consumer 消费者
从消息队列中取出消息的一方

3.Broker 代理
消息中转角色，负责存储消息、转发消息。

4.Topic 消息分类
表示一类消息的集合，每个主题包含若干条消息，每条消息只能属于一个主题，是RocketMQ进行消息订阅的基本单位。
每个Topic的消息也可以分片存储于不同的 Broker


### 三、部署
[5分钟不到！Docker搭建RocketMQ，史上最快教程！](https://cloud.tencent.com/developer/article/1621263)

### 四、使用场景

[特性](https://github.com/apache/rocketmq/blob/master/docs/cn/features.md)
- 1 订阅发布  
- 2 消息顺序
- 3 消息过滤
- 4 消息可靠性
- 5 至少一次
- 6 回溯消费
- 7 事务消息
- 8 定时消息
- 9 消息重试
- 10 消息重投
- 11 流量控制
- 12 死信队列
