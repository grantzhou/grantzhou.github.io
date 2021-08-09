---
layout: post
title: PostgreSQL 每周新闻 2021-8-4
---
### PostgreSQL每周新闻#417 - 2021年8月4日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/417)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/kwib7zmkbkluky9km0bs.jpg)

## [分析一个Postgres Planner“不是很聪明”的案例？](https://postgresweekly.com/link/111882/web)
Postgres的查询规划器通常非常出色，但多年来我遇到了一些特殊案例，因此这里提供了一个解决方案，可以使性能提高2倍。

`Matt DuPress `

## [使用pg_stat_monitor提高查询性能](https://postgresweekly.com/link/111883/web)
pg_stat_monitor是Percona构建的一个扩展，它试图成为通用的pg_stat_statements的更高级替代品。

`Ibrar Ahmed (Percona) `

## [免费电子书：Postgres中有效的索引](https://postgresweekly.com/link/111885/web)
了解如何为查询创建最佳Postgres索引。我们提供了对索引类型、运算符、数据类型等的深入研究。创建正确的索引通常可以将查询性能提高10倍甚至100倍。


`pganalyze `
## [pg_timetable 4.0发布：Postgres上的高级作业调度](https://postgresweekly.com/link/111886/web)
4.0版本向后不兼容，因此需要构建新的timetable表。还有很多新的文档可以参考。

`CYBERTEC PostgreSQL International GmbH `

## [TimescaleDB 2.4引入了“实验模式”](https://postgresweekly.com/link/111897/web)
针对Postgres日益流行的时间序列扩展的新版本。这一次最大的特点是添加了一个特定的“实验性”模式，您可以使用它来尝试一下即将出现的内容中比较前卫的部分。


`Timescale, Inc. `
## [Postgres的Citus 10.1扩展有什么新功能](https://postgresweekly.com/link/111889/web)
作为一个增强清单，10.1中没有什么突出的地方，但总的来说，对于流行的“将Postgres转变为分布式数据库”扩展来说，这仍然是一个强有力的进步。


`Claire Giordano (Microsoft) `
## [Postgres应避免的安全问题](https://postgresweekly.com/link/111890/web)
12条建议涵盖以下领域：不监听所有网络设备、不使用MD5哈希密码、避免SQL注入问题（包括PL/pgSQL函数中的问题）等等。


`Hans-Jürgen Schönig `
## [Postgres 14解释了两阶段提交的逻辑解码](https://postgresweekly.com/link/111891/web)
两阶段提交没有得到逻辑复制的正确支持，但在PG14这一点正在改变。这篇文章巧妙地解释了它们是什么，为什么这很重要，以及PG14将如何改变事情(总的来说是一个很好的解释器，尽管您可能认为不需要该功能。）

`Ajin Cherian `

## [在AWS Lambda中使用SQL触发器](https://postgresweekly.com/link/111892/web)
您知道Postgres触发器可以直接与Lambda托管的函数交互吗？这里展示了一个Python特有的将所有这些结合在一起的示例。


`Liav Yona `
## [Hasura现在支持Citus/Hyperscale，在30秒内对数据进行即时实时图形处理](https://postgresweekly.com/link/111893/web)


`Hasura `
## [查看内存锁](https://postgresweekly.com/link/111894/web)
Egor研究了自旋锁、轻量级锁和缓冲销，所有这些都以某种方式锁定内存。


`Egor Rogov `
## [GoodJob:一个多线程的、基于Postgres的、在Ruby on Rail上的ActiveJob后端](https://postgresweekly.com/link/111895/web)
一个给的Ruby爱好者的功能！完全支持异步、队列、延迟、优先级、超时和接近零配置的重试。最近添加的一些功能包括对重复作业的cron式替换和改进的并发控制。

`Ben Sheldon `

# 💡本周提示


**🗓即将举办的Postgres活动**
