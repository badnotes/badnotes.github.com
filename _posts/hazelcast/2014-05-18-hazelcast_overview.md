---
layout: mypost
title: "Hazelcast 概述"
tagline: "Hazelcast 概述"
description: "badnotes,萬軍的个人网站，记录生活旅行代码。Hazelcast 概述."
category: Hazelcast
tags: [Hazelcast]
---




Hazelcast 是一个高度可扩展的数据聚类的Java分发平台,Hazelcast 帮助构架师和开发者更容易设计和快速开发出高扩展性的实时应用。

* 分布式实现 java.util.{Queue, Set, List, Map}
* 分布式实现 java.util.concurrent.ExecutorService
* 分布式实现 java.util.concurrency.locks.Lock
* 分布式主题用于发布/订阅消息
* 事务支持和用JCA集成J2EE容器
* 分布式监听和事件
* 支持集群信息和节点间事件传递
* 动态 HTTP session 集群
* 动态集群
* 动态扩展到数百台服务器
* 动态分区备份
* 动态故障移除
* 仅一个很小的JAR文件
* 超级易用,仅引入一个 jar
* 超级快，每秒可处理成千上万次操作
* 超级高效，高效使用CPU和RAM

Hazelcast是纯Java写的，运行在 JVM　上的　Hazelcast 可以动态集群。虽然在默认情况下 Hazelcast 节点间将用多路广播(multicast)用于相互识别，不过在多路广播不适合或者不想用时也可以通过配置只用 TCP/IP。集群成员间是用TCP/IP与高效的Java NIO完成通信的。默认配置带有1个备份，所以如果一个节点失败,也不会有数据丢失。它就像使用 java.util.{Queue, Set, List, Map}一样简单。仅仅在你的 classpath 增加一个 hazelcast.jar 文件然后启动你的程序就可以了。

