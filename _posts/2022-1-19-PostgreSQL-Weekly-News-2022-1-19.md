---
layout: post
title: PostgreSQL 每周新闻 2022-1-19
---
### PostgreSQL每周新闻#438 - 2022年1月19日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/438)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/hoz3hob05svsid73aajt.jpg)
## [五个容易错过的 Postgres 查询性能瓶颈](https://postgresweekly.com/link/118575/web)
Postgres 的查询计划器通常做得非常出色，但有时会引发奇怪的惊喜或奇怪的策略，因此您编写的常识或明显的查询可能并不总是按计划进行！这篇文章介绍了如何借助 EXPLAIN ANALYZE 和元数据分析来优化这些看似显而易见的查询。


`Paweł Urbanek `
## [更多的 SQL，更少的代码，使用 PostgreSQL](https://postgresweekly.com/link/118576/web)
与查询它的应用程序相比，数据库系统应该做多少工作有很多不同的观点。这篇文章展示了一些实用的基于 SQL 的方法，您可以倾向于让 Postgres 处理您的应用程序当前可能正在处理的更多小工作。


`pgDash `
## [透明数据加密：加密整个数据库](https://postgresweekly.com/link/118577/web)
TDE 是 PostgreSQL 的 CYBERTEC 补丁。它是目前唯一支持透明和密码安全的数据（集群）级加密的实现，独立于操作系统或文件系统加密。


`CYBERTEC `
## [关于 Postgres 查询的进度条.. 让我们深入了解一下](https://postgresweekly.com/link/118578/web)
上周我们发布了一篇关于监控长时间运行查询的进度的有趣文章，这篇文章更深入地挖掘了一些涉及的机制，并包括一些用于实际监控冗长查询的秘诀在生产中。


`Nikolay Samokhvalov `
## [使用 pglogical 的双向复制](https://postgresweekly.com/link/118580/web)
虽然 Postgres 现在具有本机复制功能，但pglogical扩展仍然有一些额外的技巧，包括双向复制。


`Yaser Raja and Peter Celentano (AWS) `
## [为什么我喜欢 PostgreSQL：基础架构工程师的观点](https://postgresweekly.com/link/118582/web)
主要是因为模式更改（相对）令人愉快。


`Shayon Mukherjee `
## [Temboard 7.9：Postgres遥控器/仪表板](https://postgresweekly.com/link/118595/web)
Python 构建的 Postgres Web 仪表板和监控系统。你在有问题的 Postgres 服务器上安装一个代理，然后 temBoard webapp 在你想要的任何地方运行。


`Dalibo `
## [使用Buildkite的测试分析✅识别，跟踪和解问题测试](https://postgresweekly.com/link/118596/web)
l,null,"en


`Buildkite `
## [redix：一个快速持久的纯key/Value存储](https://postgresweekly.com/link/118597/web)
一个使用 Redis 协议但使用 Postgres 作为其存储引擎的键值存储。三年前作为一种学习体验首次亮相，它经常更新并变成一个简洁的项目 - 用 Go 编写。


`Mohammed Al Ashaal `
# 💡本周提示


**🗓即将举办的Postgres活动**
