---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-6-26
---
### PostgreSQL每周新闻#605 - 2025年6月26日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/605)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/uvbpow6isegiaatrekwx.jpg)
## [Postgres 语法趣闻](https://postgresweekly.com/link/170968/web)
Steve 一直在为 Postgres 迁移构建一个 linter，并且不得不深入研究 Postgres 所支持的语法的一些奇特之处，并结合了标准 SQL 和 Postgres 专用方法。

`Steve Dignam`

## [Notion 如何大规模运行 PostgreSQL](https://postgresweekly.com/link/170967/web)
Notion 通过优化单个 GIN 索引，将关键查询的性能提升了 733%。了解他们如何利用 pganalyze 将 Postgres 扩展到 96 个分片，并更快地解决生产问题。


`pganalyze `

## [PLJS 1.0：Postgres 的 JavaScript 语言插件](https://postgresweekly.com/link/170970/web)
多年来，PLV8 一直是 Postgres 中使用 JavaScript 作为过程语言的首选方式，但这个基于 QuickJS 的变体（来自同一个创建者）占用空间更小，更易于维护，可能足以满足您的需求。

`Jerry Sievert `

### **本周摘要**

* 🎧 Nile 联合创始人 Gwen Shapira 做客 Postgres․fm 播客，探讨[多租户架构](https://postgresweekly.com/link/170974/web)。

* 🎤 说到播客，我（Peter Cooper）做了[一期 Talking Postgres 播客](https://postgresweekly.com/link/170975/web)，与主持人 Claire Giordano 聊了聊内容策展、Postgres 的历史、RSS、发布以及其他一些有趣的话题 :-)

* 🇱🇻 [PGConf.EU 2025](https://postgresweekly.com/link/170976/web) 将于 10 月 21 日至 24 日在拉脱维亚里加举行，现已开放报名。

* 🇬🇧 [PGDay UK](https://postgresweekly.com/link/170977/web) 将于 9 月在伦敦举行，现已开放报名。

* Peter Eisentraut 回顾了下一代 [SQL 标准中对向量数据类型及相关函数的支持](https://postgresweekly.com/link/170978/web)。

* EDB 的 [Suraj Kharage](https://postgresweekly.com/link/170979/web) 是本周 PostgreSQL 人物访谈嘉宾。


## [▶ 性能考古——20 年的改进](https://postgresweekly.com/link/170980/web)
本演讲回顾了 Postgres 多年来的性能变化，从 Postgres 8.0（2005 年发布）至今。尽管自 Postgres 11 以来性能的大幅提升有所放缓，但随着时间的推移，我们取得了惊人的进步。

`Tomas Vondraz`

💡 如果您想了解这项工作，Tomas 有一篇[博客文章介绍他在这里的所作所为](https://postgresweekly.com/link/170981/web)。

📄 [Postgres 内存泄漏调试 – Jemalloc 版](https://postgresweekly.com/link/170982/web) – Phil 继续深入探讨内存泄漏调试。Phil Eaton

📄 [哪种高可用性解决方案更适合您的需求：Pgpool 还是 Patroni？](https://postgresweekly.com/link/170983/web) Semab Tariq

📄 [OrioleDB 和 Neon 的区别](https://postgresweekly.com/link/170984/web) Alexander Korotkov



### **✂︎ 队列深度剪辑**

我们每天都会将有趣的发现添加到潜在的新闻通讯队列中。不过，并非所有内容都能每周入选，因此队列会悄然增长。本周，我们进行了回顾，并挑选出一些我们认为仍然值得分享的亮点：


* 📄 回顾一下 [Postgres 的设计](https://postgresweekly.com/link/170985/web)。这篇论文发表于 1986 年，由 Michael Stonebreaker 和 Lawrence A. Rowe 共同撰写，分享了 Postgres 在 INGRES 时代诞生之初的设计构想。

* VectorChord 的 [Jinjing Zhou 提供了一些提升 Postgres 内置全文搜索 (FTS) 功能速度的技巧](https://postgresweekly.com/link/170986/web)。

* Laurenz Albe [解释了 EXPLAIN 的 GENERIC_PLAN 选项](https://postgresweekly.com/link/170987/web)，该选项自 Postgres 16 版本起就已存在。

* Peter Eisentraut 概述了 [Postgres 的 ICU 排序规则设置](https://postgresweekly.com/link/170988/web)。

* Kirk Laurence Roybal [解释了如何修复事务 ID 回绕耗尽问题](https://postgresweekly.com/link/170989/web)。

* Shaun Thomas [尝试在 Postgres 的语境下定义“极高可用性”](https://postgresweekly.com/link/170990/web)。

* Oskar Dudycz [提供了一个实用教程，教您如何使用 Docker 数据库自动设置 pgAdmin。](https://postgresweekly.com/link/170991/web)