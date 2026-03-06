---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-5-29
---
### PostgreSQL每周新闻#602 - 2025年5月29日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/602)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/q3plmo60gxww7dzvldpy.jpg)
## [OpenAI 如何将 Postgres 扩展至更高水平](https://postgresweekly.com/link/169815/web)
OpenAI 工程师 Bohan Zhang 在 PGConf.dev 上的演讲记录，讲述了 OpenAI 如何通过非分片方法（仅使用一个写入器和多个读取器）实现扩展，尽管 Postgres 是“OpenAI 最关键系统的骨干”。如果这对他们来说足够好……

`PixelsTech / Lao Feng`

## [不要错过 POSETTE 2025：6 月 10 日至 6 月 12 日](https://postgresweekly.com/link/169814/webb)
45 位 Postgres 生态系统专家将通过 4 场直播和 Discord 在线聊天，带来 42 场精彩纷呈的演讲，与你一起学习。POSETTE：Postgres 盛会是由微软 Postgres 团队组织的免费线上开发者活动。快来参与吧！


`Microsoft `

## [PostgresqlCO.NF：面向人类的 Postgres 配置设置](https://postgresweekly.com/link/169817/webb)
一份有用的在线参考指南，介绍 Postgres 的各种参数，从 log_statement 和 application_name 等基础知识到最新版本（包括 v18，目前处于测试阶段）中添加的内容。

`OnGres, Inc.`

## [使用 pg_test_fsync 测试低延迟写入](https://postgresweekly.com/link/169820/web)
pg_test_fsync 是 Postgres 附带的工具，用于确定硬件上最快的 wal_sync_method 选项。

`Tanel Poder`


### **本周摘要**

* [Amazon Aurora DSQL 现已正式发布。](https://postgresweekly.com/link/169823/web)

* Karen Jex 分享了她[最近在 PostgreSQL 欧洲多样性工作组演讲的幻灯片和文字记录，介绍了该工作组的用途及其目标](https://postgresweekly.com/link/169824/web)。

* ✅ 不知何故，我[从未注意到 Postgres 有一个官方的“功能矩阵”](https://postgresweekly.com/link/169825/web)，用于比较各主要版本的功能。

* [IBM COBOL](https://postgresweekly.com/link/169826/web) for Linux 现已支持 Postgres。

* 🇧🇪 [法国 PGDay](https://postgresweekly.com/link/169827/web) 将于下周（6 月 3 日至 4 日）在比利时举行！

* Dirk Krautschick 是最新一位 [PostgreSQL 本周人物](https://postgresweekly.com/link/169828/web)的受访者。

## [通过 Heaptrack 调试 Postgres 中的内存泄漏](https://postgresweekly.com/link/169829/web)
一个仅限 Linux 的演示，通过一个人工示例将内存泄漏引入 Postgres，然后使用 heaptrack 内存分析器对其进行调试。

`Phil Eaton`

## [如何在没有额外基础设施的情况下在 Postgres 中运行 Cron 作业](https://postgresweekly.com/link/169831/web)
如果您想将所有内容都保留在 Postgres 本身中，pg_cron 可能是您的首选，但如果您正在构建 Node 应用程序（例如使用 Wasp，如本教程中所示），那么 pg-boss 作业队列提供了另一种选择。

`Andrei Gaspar`

* 📄 [使用 PostgREST 在 Postgres 中重建 S3](https://postgresweekly.com/link/169834/web)——一种从数据库提供任意二进制文件的有趣方法。Sam Harrison (Neon)

* 📄 [如何使用 Zig 构建 Postgres](https://postgresweekly.com/link/169835/web)：一个 GCC/Clang 的嵌入式替代方案 Alvaro Hernandez

* 📄 [理解 Postgres 中的逻辑复制](https://postgresweekly.com/link/169836/web) Garth Goodson

* 📄 [对随机 (v4) 和基于时间 (v7) 的 UUID 进行基准测试](https://postgresweekly.com/link/169837/web) Umang Sinha

* 📄 [在 Debezium 数据变更事件中回填 Postgres TOAST 列](https://postgresweekly.com/link/169838/web) Gunnar Morling


### **代码和工具**

## [从源代码构建 Postgres 18 Beta 的 Dockerfile](https://postgresweekly.com/link/169839/web)
一种快速使用 Postgres 18 beta 1 的便捷方法，因为测试版没有获得官方容器镜像。

`Michael Crawford`

## [📊 PG Exporter 1.0：适用于 Prometheus 的高级 Postgres + Pgbouncer 指标导出器](https://postgresweekly.com/link/169840/web)
通过一个完全可定制的导出器，公开 600 多个涵盖核心内部结构和流行扩展的指标。v1.0 也提供了一些初始的 Postgres 18 支持。

`Ruohang Feng`

[pgfdb：使用 FoundationDB 使 Postgres 分布式](https://postgresweekly.com/link/169841/web) 
pgfdb 是一个实验性的扩展，它将 Postgres 转变为位于分布式多模型数据存储 FoundationDB 之上的无状态层。

`Fabian Lindfors`

📰 分类广告
Notion 工程团队如何利用 pganalyze 在 [Amazon RDS 上大规模运行 PostgreSQL](https://postgresweekly.com/link/169844/web)，应对病毒式增长的用户增长。

Ryan Booz 和 Grant Fritchey 合著的[《面向数据专业人士的 PostgreSQL 入门》](https://postgresweekly.com/link/169845/web)将帮助您掌握 PostgreSQL，这是一本面向希望提升数据库技能的数据专业人士的全面指南。

* [无状态 Postgres 查询路由器 (SPQR) 2.6](https://postgresweekly.com/link/169846/web) – 一种水平分片方法，最初由 Yandex Cloud 构建。

* [PgHero 3.7](https://postgresweekly.com/link/169847/web) – 作为 (Ruby on) Rails 引擎的 Postgres 性能仪表板。

* [pgmoneta 0.16.1](https://postgresweekly.com/link/169848/web) – 备份/恢复解决方案 – 现已支持 PG18。

* [pg_ivm 1.11](https://postgresweekly.com/link/169849/web) – 增量视图维护扩展。

* [pgroll 0.13.0](https://postgresweekly.com/link/169850/web) – 强大的模式迁移工具。

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/zskinvfjymtb9ti3kfe3.jpg)

[为什么要升级 Postgres？原因如下](https://postgresweekly.com/link/169851/web) 
一个永久实用的资源，可让您选择“原”版本和“升级”版本，并查看 Postgres 在此期间获得了哪些改进。即使是这个从 17.4 到 17.5 的示例也包含了大量详细信息。

`Hubert depesz Lubaczewski`