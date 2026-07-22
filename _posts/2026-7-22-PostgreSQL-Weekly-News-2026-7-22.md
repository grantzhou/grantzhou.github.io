---
layout: post
title: PostgreSQL 每周新闻 2026-7-22
---
### PostgreSQL每周新闻#658 - 2026年7月22日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/658)

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/c4md7advis5kslx7uxhj.jpg)

## [让768台服务器看起来像1台](https://postgresweekly.com/link/188236/rss)

一篇有趣且具有教育意义的动画讲解文章，介绍了如何将分布在256个分片（每个分片有一个主节点和两个副本）上的PB级Postgres数据库呈现为单一数据库，涵盖了副本的局限性、查询解析路由器以及负载均衡等内容。

`Ben Dicken (PlanetScale)`


## [VACUUM 并非为仅追加的时序数据而设计](https://postgresweekly.com/link/188235/rss)

TimescaleDB 通过超表扩展 Postgres，随着数据增长自动分区，列式压缩可减少高达95%的存储空间，连续聚合保持汇总数据的新鲜度。同样的 Postgres，同样的 SQL。[获取$1000积分开始使用](https://postgresweekly.com/link/188235/rss)。

`Tiger Data (creators of TimescaleDB)` **赞助商**


## [在添加只读副本之前先读这篇文章](https://postgresweekly.com/link/188237/rss)

只读副本的一个常见问题是陈旧读取，这可能会在意想不到的地方出现。[incident.io](https://postgresweekly.com/link/188238/rss) 解释了他们在将大部分读取操作从主库迁移出去时使用的方法，包括LSN标记和查询路由策略。

`Johanna Larsson`


**简讯：**

- ⭐ [Postgres 19 Beta 2 已发布](https://postgresweekly.com/link/188239/rss)，专注于修复第一个测试版中发现的bug。请继续测试和报告，以便9月/10月的最终v19版本更加稳定。

- [Supabase Pipelines 现已进入公开alpha阶段](https://postgresweekly.com/link/188242/rss)。它旨在近实时地将Supabase数据库复制到外部分析系统。

- [Neon](https://postgresweekly.com/link/188240/rss) 正在扩展，超越Postgres，提供[完整的后端平台](https://postgresweekly.com/link/188241/rss)，包括对象存储、函数和AI网关，现处于beta阶段。


## [Postgres 19 压缩：从pglz到LZ4](https://postgresweekly.com/link/188243/rss)

在v19中，TOAST压缩默认从pglz切换到LZ4（自Postgres 14起作为选项）。Christopher介绍了历史，但也涵盖了有趣的内容：什么内容被压缩或TOAST的决策树，以及索引如何压缩超大键。

`Christopher Winslett`


## [Turso: '我们正在用Rust构建Postgres'](https://postgresweekly.com/link/188244/rss)

我们最近介绍了[pgrust](https://postgresweekly.com/link/188245/rss)，但现在以用Rust重写SQLite而闻名的Turso也在尝试，采用了LLVM启发的方法：一个单一的数据库核心，通过多个前端呈现，其中Postgres是第二个。

`Costa and Enberg (Turso)`


## [▶ 在SQL Server工作13年后转向Postgres](https://postgresweekly.com/link/188246/rss)

Microsoft的Panagiotis Antonopoulos讨论了他从SQL Server工作13年转向Postgres的经历，为什么Postgres已成为许多工作负载的默认选择，以及Azure HorizonDB的共享存储架构。

`Talking Postgres` **podcast**


📺 [让Iceberg像Postgres一样行走和说话](https://postgresweekly.com/link/188247/rss) — 在DuckCon上关于[pg_lake](https://postgresweekly.com/link/188248/rss)的5分钟闪电演讲。`Marco Slot`

📄 [你真的需要了解多少数据库知识？](https://postgresweekly.com/link/188249/rss) `Karen Jex`

📄 [构建OAPE PostgreSQL认证](https://postgresweekly.com/link/188250/rss) `Cornelia Biacsics`


📰 **分类广告：**

查看Oracle迁移中真正出现的问题，从存储过程到边缘案例，以及AI代理如何处理它。[在浏览器中运行](https://postgresweekly.com/link/188251/rss)。

[MyDBA](https://postgresweekly.com/link/188252/rss)：为您的Postgres数据库提供全面监控。从免费的一周健康检查开始，然后继续免费监控。


## 🛠 代码和工具

## [pgBackRest 2.59.0 发布，支持Postgres 19](https://postgresweekly.com/link/188253/rss)

这款流行的备份和恢复工具自项目[短暂停滞后重获新生](https://postgresweekly.com/link/188254/rss)以来的首次发布。为Postgres 19做准备是重点，但也添加了一些便捷的S3和Azure增强功能。

`David Steele`


## [pg_timetable 7.0：Postgres的高级作业调度](https://postgresweekly.com/link/188255/rss)

一个成熟的独立作业调度器，将其状态存储在数据库中，让您可以调度任务并将它们串联起来。v7添加了OpenTelemetry跟踪、Docker镜像的`arm64`支持，以及[启用/禁用任务](https://postgresweekly.com/link/188256/rss)的方法。

`CYBERTEC PostgreSQL International GmbH`

💡 [pgAdmin](https://postgresweekly.com/link/188257/rss) 正在开发[用于处理pg_timetable任务的UI](https://postgresweekly.com/link/188258/rss)。


## [Puffgres：保持Postgres实体与Turbopuffer同步](https://postgresweekly.com/link/188259/rss)

听说过[A24](https://postgresweekly.com/link/188260/rss)吗，这是《Backrooms》和《Uncut Gems》等电影的发行商？他们的首个开源版本是一个Rust工具，使用逻辑复制将Postgres实体镜像到[Turbopuffer](https://postgresweekly.com/link/188261/rss)，这是一个云端向量/全文搜索服务。

`A24 Films`


- [Nano ID for Postgres 3.0](https://postgresweekly.com/link/188262/rss) — 作为Postgres函数的微小、安全、URL友好的唯一字符串ID生成器。[v3.0](https://postgresweekly.com/link/188263/rss)有破坏性更改并支持可选前缀。

- [PGSync 7.2](https://postgresweekly.com/link/188264/rss) — Postgres到Elasticsearch/OpenSearch同步的中间件。

- [pgstream 1.2](https://postgresweekly.com/link/188265/rss) — 支持DDL更改的Postgres复制。v1.2添加了用于飞行前验证的`check`命令。

- [node-pg-migrate 9.0](https://postgresweekly.com/link/188266/rss) — Node.js应用程序的模式迁移管理。

- 🌐 [PostGIS 3.7.0 Beta 1](https://postgresweekly.com/link/188267/rss) — 支持Postgres 14到19 beta 2。