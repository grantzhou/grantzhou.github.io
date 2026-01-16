---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-9-20
---
### PostgreSQL每周新闻#522 - 2023年9月20日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/522)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ndome6zuagflo2fejljb.jpg)
## [Postgres 16发布](https://postgresweekly.com/link/145143/web)
Postgres 的最新主要版本在我们上周发送Postgres Weekly的第二天就发布了，但好处是我们可以在下面的代码和工具中链接到过去一周添加了 PG16 支持的许多扩展😆 尽管如此，这里有一些新增内容：

- 在 x86 和 ARM 上支持 SIMD 的 CPU 加速
- 查询规划器现在可以并行化FULL和RIGHT连接。
- 聚合函数性能改进。
- 批量数据加载的巨大性能改进COPY
- 允许从备用服务器进行逻辑复制。
- 扩展的 SQL/JSON 语法，例如JSON_ARRAY()&JSON_ARRAYAGG()
- pg_stat_io用于精细 I/O 指标。
有关新增功能的完整列表，请查看发行说明，或者...

`PostgreSQL Global Development Group `
## [Postgres 16 中的变化、我们如何做到这一点以及 Postgres 17+ 中的预期](https://postgresweekly.com/link/145146/web)
Amit Kapila 以比官方发布帖子（上面）更容易浏览的形式列出了 Postgres 16 中引入的新功能，包括新功能的代码示例SQL/JSON 函数正在发挥作用。


`Amit Kapila `
## [对任何数据库进行安全、合规且轻松的数据库访问](https://postgresweekly.com/link/145142/web)
通过将数据库访问权限整合到一处，打破访问孤岛并减少开销。持续保持合规性并以最小的努力通过 SOC 2、FedRAMP、HIPAA、ISO 27001、PCI 等审核


`Teleport | goteleport․com `
## [Hydra 1.0：开源、面向列的 Postgres](https://postgresweekly.com/link/145147/web)
一种开源扩展，可将柱状表添加到 Postgres 中，以实现高效的分析报告，而无需更改数据库。Hydra 的 Owen Ou 录制了一段▶️ 五分钟的截屏视频来展示。


`Simon Wijckmans `
**本周摘要：**
*   如果您想在 AWS 上评估Postgres 16，则它已在 Amazon RDS 的数据库预览环境中可用。


*   🇬🇧 2023 年首届英国 PGDay上周在伦敦举行，组织者 Dave Page 分享了该活动如何取得巨大成功的最新消息。迎接 2024 年英国 PgDay！


*   ✅如果您想参与的话，数据库工具公司 Redgate Software 的人员正在对数据库状况进行一项调查。


*   FOR在 PL/pgSQL 中使用循环内定义的变量时要小心，因为它们的范围是有限的。


*   Bruce Momjian 解释了他选择参加哪些 Postgres 会议的标准。


*   关于为什么在 Postgres 会议上发表演讲很重要的讨论。


## [活跃在Postgres 16](https://postgresweekly.com/link/145156/web)
实用的演练使Postgres 16的逻辑复制改进通过其步伐进行了改进。


`Brian Pace `
## [Lantern：用于 AI 用例的 Postgres 矢量扩展](https://postgresweekly.com/link/145158/web)
pgvector可能非常流行，但 Lantern 提供了一个替代选项（幸运的是，它可以与 pgvector 互操作）。它希望超越 pgvector 和类似的扩展，并支持并行索引创建，使索引创建保持在实时数据库之外。它在底层依赖于usearch 。


`Jeung Park and Narek Galstyan `


`Adab Biranimal`
## [PeerDB：用于 Postgres 的更简单、更快的 ETL](https://postgresweekly.com/link/145162/web)
来自 Microsoft 和 Citus Data 的校友推出了一个新平台，专门用于将数据移入和移出 Postgres 的任务。有一个快速入门指南，但其想法是无缝集成多个数据存储，包括 Postgres、Snowflake 和 BigQuery，并提供实时同步、定制 ETL 以及跨所述存储进行联合查询的方法。


`PeerDB `
## [pgtt 3.0：管理和使用 Oracle 风格的全局临时表](https://postgresweekly.com/link/145164/web)
适用于您想要重现 Oracle 行为而不是重写代码以使用标准 Postgres 临时表的情况。v3 支持 Postgres 12+。


`Gilles Darold `
## [Ppg_hint_plan 1.6：在执行计划中手动强制决策](https://postgresweekly.com/link/145165/web)
与往常一样，修复了错误，但 Postgres 16 支持是这里的标题。


`NTT OSS Center DBMS Development and Support Team `
## [Pigsty 4.0：“包含电池”的 Postgres 发行版](https://postgresweekly.com/link/145166/web)
Postgres 的发行版，将自己标榜为“RDS PG 替代品”，包含许多开箱即用的功能，例如扩展、可观察性、自我修复 HA 和监控仪表板。v4.0 引入了 Postgres 16 支持和各种新的捆绑扩展，包括 Apache AGE 和 pgsql-http。


`Feng Ruohang `
## [pgrx 0.10.1](https://postgresweekly.com/link/145167/web)
 - 用生锈构建邮政扩展。现在，自然而然地获得了Postgres 16的支持。


## [pg_qualstats 2.1](https://postgresweekly.com/link/145168/web)
 - 保存和分析所使用谓词的统计信息


## [Good Job 3.19.0](https://postgresweekly.com/link/145169/web)
 - Postgres 支持的 Ruby on Rails 作业队列。


## [pgxmock 3.0](https://postgresweekly.com/link/145170/web)
 - 用于测试 Go 中数据库交互的模拟驱动程序。


## [pg_ivm 1.7](https://postgresweekly.com/link/145171/web)
 - 增量视图维护 (IVM) 扩展。


# 💡本周提示


**🗓即将举办的Postgres活动**
