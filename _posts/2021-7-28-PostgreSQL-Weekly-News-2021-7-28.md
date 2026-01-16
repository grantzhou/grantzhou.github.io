---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-7-28
---
### PostgreSQL每周新闻#416 - 2021年7月28日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/416)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/nexjx5akxihjgsyzls6t.jpg)
## [使用继承执行ETL](https://postgresweekly.com/link/111587/web)
如果您需要以接近零的停机时间更新多 TB 的表，Postgres 对表继承的支持可能会派上用场。


`Robert Bernier `
## [使用 Postgres、TimescaleDB和SQL处理NFL数据](https://postgresweekly.com/link/111590/web)
NFL训练营现已开放，在这里您可以看到如何使用 NFL 提供的时间序列数据从 Postgres 中发现对许多球员表现指标的宝贵见解。当然，还需要大量的Timescale（Postgres 的时间序列扩展）才能使其全部工作


`Timescale `
## [无需操作、可扩展且灵活的Postgres替代方案](https://postgresweekly.com/link/111594/web)
Fauna 将Postgres的操作完整性和关系建模与更适合云中现代应用程序开发的界面和架构相结合。没有操作瓶颈的 Postgres 的优点 -了解有关 Fauna 的更多信息。


`Fauna `
## [语法指南ClickHouse Postgres的用户](https://postgresweekly.com/link/111596/web)
ClickHouse是一种越来越流行的基于列的OLAP数据库系统和本指南介绍如何许多类型的Postgres的查询的适应ClickHouse风格。


`Tinybird `
## [从 Go(lang) 访问 Postgres 数据库](https://postgresweekly.com/link/111600/web)
这里没有 ORM，它回顾了从 Go 访问 Postgres 数据库的低级方法，包括pq驱动程序pgx和sqlx.


`Eli Bendersky `
## [使用 Postgres 进行现代数据分析 - JSONB 与窗口函数](https://postgresweekly.com/link/111601/web)
了解经典数据布局范例以及事务数据库功能（例如快速更新和 JSON/JSONB 类型）如何使分析更容易。


`Thomas Richter `
## [增加每次收集的最大并行工作线程数](https://postgresweekly.com/link/111602/web)
每个版本 Postgres 并行运行操作的能力都在不断提高，但默认设置可能有点保守。“如果你认为你的工作负载可以从更多的并行性中受益，那么这篇文章适合你”。


`Michael Christofides `
## [逻辑副本和快照：谨慎进行](https://postgresweekly.com/link/111604/web)
反思“从 RDS Postgres 中的快照创建逻辑副本”中演示的技术，其中使事情更快地工作通常意味着需要掌舵的专家来确保事情顺利进行。总结： “捷径是危险的，如果你不理解它们就会带来危险”。


`Jeremy Schneider `
## [查看 Postgres 扩展目录](https://postgresweekly.com/link/111606/web)
您可以查看三个主要目录，以查看哪些扩展处于活动状态，哪些可用，以及各种扩展的哪些版本可用。


`Luca Ferrari `
## [使用 Datadog 实时跟踪关键的 PostgreSQL 指标](https://postgresweekly.com/link/111607/web)
l,null,"en


`Datadog `
## [使用Django 和 Postgres进行数据分页](https://postgresweekly.com/link/111608/web)
使用 Django 和 Postgres 进行数据分页的三种不同方法以及每种方法的优缺点。


`Ryan Westerberg `
## [使用 AWS DMS 将 Postgres 集群复制到 Redshift](https://postgresweekly.com/link/111609/web)
RevenueCat 的团队使用 Postgres 作为他们的主数据库，然后使用Redshift（AWS 的托管数据仓库服务）进行分析 — 以下是他们如何使用数据库迁移服务大规模复制数据。


`Jesús Sánchez `
## [Postgres 中巧妙的“缓冲区标签”](https://postgresweekly.com/link/111612/web)
Postgres 在内部使用缓冲区标签来优化连接缓冲区和数据文件的过程。这是非常底层的东西，并不适合所有人。几乎没有 Postgres 用户需要知道这些内部部分，但您可能会发现它仍然很有趣。


`David Zhang `
## [pg_validate_extupgrade：验证 Postgres 扩展升级脚本的工具](https://postgresweekly.com/link/111613/web)
这是非常小众的，但如果您开发和分发自己的 Postgres 扩展并想验证您的扩展的升级脚本是否会产生正确的结果，这很方便。


`Julien Rouhaud `
# 💡本周提示


**🗓即将举办的Postgres活动**
