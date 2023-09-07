---
layout: post
title: PostgreSQL 每周新闻 2023-9-6
---
### PostgreSQL每周新闻#520 - 2023年9月6日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/520)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/yz5fhludoc40exl2p9qu.jpg)
## [pgvector 0.5 发布：亮点](https://postgresweekly.com/link/144386/web)
pgvector 是一个提供向量相似性搜索功能的扩展，并且越来越多地用于 LLM/ML 用例。 v0.5 引入了新的索引类型（Christopher Winslett 在 HNSW Indexes with Postgres and pgvector 中详细展示了）、ivfflat 索引构建的并行化以及改进的距离函数性能。 [变更日志](https://postgresweekly.com/link/144389/web)和 [GitHub 存储库](https://postgresweekly.com/link/144387/web)。


`Jonathan Katz `
## [Postgres 16 候选版本 1 已发布](https://postgresweekly.com/link/144390/web)
除了最近的测试版之外，没有太多可添加的内容，但最终版本将于下周发布，在此之前您可以仔细阅读发行说明草案以获取完整的摘要。


`PostgreSQL Global Development Group `
## [使用 EXPLAIN 查找 Postgres 查询缓慢的根本原因](https://postgresweekly.com/link/144385/web)
在本深入指南中，您将了解我们使用 Postgres EXPLAIN 查找和改进有问题的查询计划的方法，如何分析和改进这些查询计划，以及如何使用 auto_explain 自动 开始收集 EXPLAIN 计划。


`pganalyze `
## [优化高变动表的 Autovacuum](https://postgresweekly.com/link/144392/web)
由于 Postgres 的数据存储方法，Auto Vacuum 过程对于清理和优化表存储是必要的。 表经历的 UPDATE 和 DELETE 次数越多，此清理过程就变得越重要，因此调整其工作方式可以产生显着的结果。


`Adam Hendel `
## [2023 年 Microsoft Postgres 的新增功能](https://postgresweekly.com/link/144393/web)
无论是通过 Citus、Azure 还是其他方式，Microsoft 在 Postgres 领域都占有重要地位，并维护着各种众所周知的工具、扩展和服务。 Claire 出色地介绍了今年迄今为止 Microsoft 在 Postgres 领域所做的各种事情。


`Claire Giordano (Microsoft) `


**本周摘要：**
*   AWS 推出了 Amazon RDS 扩展支持，这是一项付费计划，在旧版本标准支持结束后的三年内提供安全性和错误修复。 例如，这会将 Postgres 11 支持延长至 2026 年底，将 Postgres 15 支持延长至 2030 年代。


*   📗 Andrew Atkinson 所著的 《High Performance PostgreSQL for Rails》 一书目前处于测试阶段，预计于 10 月份最终发布，目标对象是使用 Postgres 的 Ruby 和 Rails 开发人员。


*   Steven Vaughan-Nichols 谈到最近针对热门开源项目提交的一系列看似伪造的漏洞报告之一时表示，现在轮到 Postgres 拥有伪造的 CVE 了。 在这种情况下，具体来说是 CVE-2020-21469。


*   Amazon RDS for PostgreSQL 增加了对 h3-pg 扩展的支持，这是一种源自 Uber 的六边形分层地理空间索引和查询方法。


*   Amazon RDS 现在在 Postgres 13 和 14 部署中支持 PL/Rust（Postgres 15 中已支持）。


*   最后，Postgres 16 RC1 现已在 Amazon RDS 数据库预览环境中推出。


*   Joshua D. Drake 针对加拿大 PostgreSQL 社区协会和 Fundacion PostgreSQL 之间正在进行的商标/法律纠纷提供了一些急需的额外视角。 我们希望此事能尽快得到友好解决。


## [▶ UPDATE 被认为是有害的](https://postgresweekly.com/link/144403/web)
Jeremy 说，“这是一个标题诱饵”，但它有助于表明 UPDATE 并不像看上去的那样，并且假设它只是“更新”数据可能会导致问题。 （实际上，更新会插入新数据并删除旧数据 - 或将其标记为过时 - 而不是在物理层面上“更新”任何内容。）


`Jeremy Taylor `

## [博客 保护您的 PostgreSQL 数据库](https://postgresweekly.com/link/144404/web)

`TELEPORT | GOTELEPORT․COM`

## [通过 EBS 快照和 pgBackRest 使 Postgres 备份速度提高 100 倍](https://postgresweekly.com/link/144405/web)
pgBackrest 是处理备份的便捷工具，但对于大型数据库来说它可能会变慢。 以下是 Timescale 如何通过合并 EBS 快照来缓解该问题。


`Godeke and Blackwood-Sewell (Timescale) `


**代码和工具：**
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/tnnnn8zaclwq8t2pncjx.jpg)
## [介绍 pg_later：Postgres 的异步查询](https://postgresweekly.com/link/144408/web)
现在执行 SQL，稍后获取结果。 构建在 pgmq Postgres 消息队列扩展之上。 GitHub 存储库。


`Adam Hendel `
## [pg_ivm 1.6：增量视图维护扩展](https://postgresweekly.com/link/144411/web)
当视图的一小部分发生变化时，IVM 可以比重新计算更有效地更新物化视图。 v1.6 添加了对 EXISTS 子句的支持。


`SRA OSS LLC `
## [FerretDB 1.9](https://postgresweekly.com/link/144413/web)
 - 它前端像 MongoDB，但后面是 Postgres（或者可选的 SQLite）。


## [pg_cron 1.6](https://postgresweekly.com/link/144414/web)
↳在 Postgres 中运行定期任务。


## [PGXMOCK 2.12](https://postgresweekly.com/link/144415/web)
↳pgx 模拟驱动程序用于测试 Go 中的数据库交互。


## [pg-anonymizer 0.8](https://postgresweekly.com/link/144417/web)
↳从 Postgres 输出匿名数据工具。


## [Nano ID for PostgreSQL 2.0](https://postgresweekly.com/link/144418/web)
↳Nano ID 生成扩展。


## [Ruby-PG 1.5.4](https://postgresweekly.com/link/144419/web)
↳Ruby Postgres 客户端库。
