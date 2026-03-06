---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-3-27
---
### PostgreSQL每周新闻#594 - 2025年3月27日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/594)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/whmicx3cy8lfssghbvql.jpg)
## [改变生活的 Postgres 模式](https://postgresweekly.com/link/167370/web)
作者承诺标题不仅仅是点击诱饵，还提供了十二种不同的简短、来之不易的技巧和见解，涉及从使用 UUID 作为主键和表命名到使用模式和视图等领域。

`Ethan McCue`

## [驯服 Postgres 隔离异常的实用指南](https://postgresweekly.com/link/167096/web)
基于 Ruby（尽管 SQL 繁重）的 Postgres 并发控制实用指南，详细介绍了现实世界中的问题，例如丢失更新、写入偏差和其他隔离异常。即使您很少遇到冲突，您也会获得有关管理事务的宝贵见解。


`Dan Svetlov`
## [使用 AI 驱动的审查功能在编写代码时学习 PostgreSQL 最佳实践](https://postgresweekly.com/link/167369/web)
CodeRabbit 在代码审查期间发现 PostgreSQL 性能问题。我们的 AI 标记慢查询、缺少索引和 ORM 陷阱 — 用通俗易懂的语言解释每个修复。我们免费提供开源，并且已经帮助流行的 Postgres 工具提供更好的代码。开始吧！


`CodeRabbit   `
## [为什么 Postgres 需要更好的替代表引擎 API？](https://postgresweekly.com/link/167372/web)
Postgres 具有允许扩展提供自己的索引类型和表访问方法的机制，但推出强大的替代表引擎仍然不那么容易。OrioleDB 的 Alexander 解释了局限性和一些潜在的发展方向。


`Alexander Korotkov `
## [Postgres 中的语义搜索：概述](https://postgresweekly.com/link/167373/web)
全文搜索很棒，但如果您想根据其含义而不是文字数据来查询数据，则需要引入 pgvector 等扩展。Hans-Jürgen 在这里解释了它的工作原理。


`Hans-Jürgen Schönig`
## [🔒 Postgres 安全检查表](https://postgresweekly.com/link/167374/web)
互联网安全中心 (CIS) 发布了针对互联网基础设施中使用的各种流行工具和服务的安全基准，现在有了一套 Postgres 指南（尽管可惜的是，它被置于具有商业使用限制的电子邮件墙后面）。


`Elizabeth Christensen`
## [使用存储在 Gopass 中的密码创建 Postgres 角色](https://postgresweekly.com/link/167376/web)
Gopass 是一款基于 Go 的基于 CLI 的团队密码管理器。


`homas Klausner`
## [减少云支出：使用 Postgres 将日志从 CloudWatch 迁移到 Iceberg](https://postgresweekly.com/link/167378/web)
Postgres 提供商 Crunchy Data 有大量日志需要存储，而将这些日志存储在 AWS CloudWatch 中也需要花费很多钱。Craig 解释了 Crunchy Data 如何实施新的工作流程，将日志存储在 S3 上的 Iceberg 表中，同时仍允许通过 Crunchy Data Warehouse 进行 SQL 查询。


`Craig Kerstiens`
### 本周摘要：

* 📄 [以简单的方式在只读模式下启动](https://postgresweekly.com/link/167379/web) – 如何以更安全的只读模式启动 psql。Kaarel Moppel

* 📺 [Autovacuum 是如何出错的：我们能让它停止这样做吗？](https://postgresweekly.com/link/167380/web)Robert Haas

* 📄 [关于分片 pgvector 的想法](https://postgresweekly.com/link/167381/web) Leo Kokotov (PgDog)

### 代码和工具：

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ekl8zdyxyhf9z4mjfbyp.jpg)

## [Teable：Postgres 上的开源 Airtable 替代品](https://postgresweekly.com/link/167382/web)
Airtable 是一种流行的数据表数据库 SaaS，但这里有一个类似的开源替代品，它位于 Postgres 之上，允许使用 SQL 直接查询数据。GitHub 仓库。

`Teable Team`
## [⭐ Electric 1.0：Postgres 同步引擎](https://postgresweekly.com/link/167389/web)
“Electric 解决同步问题”。这个想法是，如果您在 Postgres 中有数据，而您需要在其他地方同步，那么 Electric 可以为您解决同步的难题，包括部分复制、扇出和数据传输，无论您的数据模型或 Web 框架如何。更多信息请点击此处。

`James Arthur (Electric DB)`
## [Rainfrog 0.3：Postgres 的数据库管理 TUI](https://postgresweekly.com/link/167384/web)
比 psql 更结构化，具有 vim 风格的查询、历史记录、架构等导航。

`Carl Liu`

[@neondatabase/serverless 1.0](https://postgresweekly.com/link/167385/web) – Neon 的适用于 JavaScript 和 TypeScript 的 Postgres 驱动程序。

[Addax 5.0](https://postgresweekly.com/link/167386/web) – 一款快速且多功能的 ETL 工具，支持超过 20 个 SQL/NoSQL 数据源。

[BemiDB 0.43](https://postgresweekly.com/link/167387/web) – 针对分析优化的单一二进制 Postgres 读取副本。

[Procrastinate 3.1](https://postgresweekly.com/link/167388/web) – 基于 Postgres 的 Python 任务队列。