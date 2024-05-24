---
layout: post
title: PostgreSQL 每周新闻 2024-5-22
---
### PostgreSQL每周新闻#556 - 2024年5月22日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/556)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/jq618vrw8lqcuxlkqocu.jpg)
## [pg_timeseries 简介：一种新的时间序列扩展](https://postgresweekly.com/link/155406/web)
被誉为一种在 Postgres 中管理时间序列数据的简单开源方式，它主要是用 SQL 实现的。他们还需要时间来回答“为什么不使用 Timescale？”这个问题。主要是license。然而，就 pg_timeseries 功能而言，现在还处于早期阶段。

`SHARMA AND PETERSEN (TEMBO) `
## [从慢速查询到快速 - 通过统计](https://postgresweekly.com/link/155409/web)
我们之前链接到 Render 的“有大问题的简单查询” - 以下是深入探讨为什么他们的简单查询需要这么长时间才能运行以及他们深入研究和解决问题的方法。这里有一些有用的指导。


`ERIC FRITZ (RENDER) `
## [Redgate 的 PostgreSQL 学习中心](https://postgresweekly.com/link/155405/web)
探索 PostgreSQL 内容，了解即将举办的活动，加入社区讨论，并了解 Redgate 工具如何帮助您解决数据库挑战。


`REDGATE SOFTWARE `
## [Heroku 推出 Heroku Postgres Essentials](https://postgresweekly.com/link/155411/web)
作为扩展大型 Postgres 平台的先驱，Heroku 仍在继续改进。这些新计划建立在 Amazon Aurora 之上，专注于低端（取代其 Mini 和 Basic 级别），同时仍然提供比以前更高的性能（此外，它们支持 pgvector）。


`HEROKU `

**本周摘要：**

* 📊 核心贡献者 Peter Eisentraut 喜欢测试 Postgres 的编译速度（可能是因为他必须做很多事情），并研究了最新的 [Clang 18 和 GCC 14 的性能](https://postgresweekly.com/link/155412/web)。尽管 GCC 速度越来越慢，但 Clang 已经恢复了状态。


* Gabriele Bartolini 向最近[去世](https://postgresweekly.com/link/155415/web)的 2ndQuadrant 创始人西蒙·里格斯 (Simon Riggs) 致以[感人至深的敬意](https://postgresweekly.com/link/155413/web)，并介绍了 2ndQuadrant 在意大利的发展历史。

* 今年的 [Stack Overflow 开发者调查](https://postgresweekly.com/link/155417/web)刚刚开始 – 记得表达你对 Postgres 的热爱.. 😄

* 🇬🇷 PGConf.EU 2024 今年 10 月在希腊雅典举行，目前正在[寻找赞助商](https://postgresweekly.com/link/155419/web)。


## [当 Postgres 说“不，谢谢，我不需要你的索引”时](https://postgresweekly.com/link/155421/web)
故事时间到了！ Jean-Mark 在遇到优化查询问题后讲述了一个“胜利的故事”。让谈判开始吧..


`JEAN-MARK WRIGHT `
## [使用内存磁盘存储 Postgres 的临时文件](https://postgresweekly.com/link/155423/web)
Postgres 在各种情况下都会生成临时文件，包括执行并行查询时，Stefan 想看看使用基于 RAM 的文件系统是否会带来改进。确实有...有一点。

`STEFAN FERCOT `


**📰 机密：**


[POSETTE](https://postgresweekly.com/link/155425/web)做好准备！ Postgres 的免费虚拟开发者活动（6 月 11 日至 13 日）。收听 4 个直播中的 42 场演讲中的一场或多场

📅 [Moar Serverless 2024](https://postgresweekly.com/link/155427/web) 是一项免费的、为期一天的在线活动，将于 5 月 23 日（明天）举行，多位演讲者分享了构建无服务器应用程序的最新信息。


## [如何使用 Postgres 来崩溃你的 stack 内存。。。所有](https://postgresweekly.com/link/155428/web)
如果 stack 蔓延对你或你的公司来说是一个问题，为什么不将更多的工作转移到你已经了解和喜爱的值得信赖的数据库上呢？

`JAMES BLACKWOOD-SEWELL (TIMESCALE)`

📄 [Postgres 17 TIMESCALE](https://postgresweekly.com/link/155429/web) 让我们兴奋的事情 - TIMESCALE

📺 使用 Postgres 在 6 个月内将 Clubhouse 的用户数量[从 1 万扩大到 1,000 万](https://postgresweekly.com/link/155431/web) - HARRY TORMEY 和 LUKE DEMI

📄 [优化 SQL 查询：一些 Postgres 最佳实践](https://postgresweekly.com/link/155433/web) – 一些基础知识的总结 - MARKUS WIREKAT

📄 使用 Lua [在 Postgres CDC 中进行行级转换](https://postgresweekly.com/link/155435/web) - SAI SRIRAMPUR (PEERDB) 


**🛠 代码和工具：**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/v8y4aivdk8jebp5p65pb.jpg)

## [SQLFrame：基于 PySpark 的 SQL 生成器](https://postgresweekly.com/link/155437/web)
一个数据框架库，可以在 BigQuery、DuckDB 和 Postgres 上运行 PySpark 代码。它将 DataFrame 操作直接转换为 SQL。这里有更长的解释和理由。


`RYAN EAKMAN `

## [PgHero 3.5：Postgres 的性能仪表板](https://postgresweekly.com/link/155441/web)
作为（Ruby on）Rails 引擎构建的仪表板，用于查看基本性能统计数据，包括实时查询、维护状态和连接。


`ANDREW KANE`

[Pgpool-II 4.5.2](https://postgresweekly.com/link/155443/web),[4.4.7](https://postgresweekly.com/link/155443/web),[4.3.10](https://postgresweekly.com/link/155443/web),[4.2.17](https://postgresweekly.com/link/155443/web) 和 [4.1.20](https://postgresweekly.com/link/155443/web)

[pgRoll 0.6](https://postgresweekly.com/link/155445/web) – Postgres 的零停机、可逆模式迁移。 v0.6 添加了一些新功能。

[Pigsty 2.7](https://postgresweekly.com/link/155449/web) – “包含电池”的 Postgres 发行版获得了 20 多个新包含的扩展。

[DBMate 2.16](https://postgresweekly.com/link/155451/web) – 轻量级、与框架无关的数据库迁移工具。

[Bytebase 2.17](https://postgresweekly.com/link/155453/web) – 团队的数据库开发和 CI/CD 系统。

[Bob 0.26](https://postgresweekly.com/link/155455/web) – Go 的 SQL 查询构建器和 ORM/Factory 生成器。

[pg_dumpbinary v2.17](https://postgresweekly.com/link/155457/web) – 将数据库转储为二进制格式。