---
layout: post
title: PostgreSQL 每周新闻 2021-10-27
---
### PostgreSQL每周新闻#428 - 2021年10月27日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/428)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/qof2ehbmhz94mugqyg4o.jpg)
## [字符串、数组、递归和解析 JSON：探索 PL/pgSQL](https://postgresweekly.com/link/115383/web)
如果您还没有使用过 Postgres 的内置过程语言 PL/pgSQL，这是一本简洁的入门书，从基本操作到递归操作，甚至一点点解析。目标是让 PL/pgSQL “对你来说不那么可怕”，我认为它有效。


`Phil Eaton `
## [StackGres 1.0.0：Kubernetes 的开源“Postgres-aaS”](https://postgresweekly.com/link/115384/web)
StackGres 提供了一种在 Kubernetes 上运行 Postgres 的方法，目标是使其成为在生产中部署 Postgres 的最简单方法之一。这还需要以一种可以动态加载的方式打包扩展，并且已经有100 多个扩展可用。


`Álvaro Hernández `
## [为 Postgres 数据库编制索引的更好方法：Pgganalyze Index Advisor](https://postgresweekly.com/link/115386/web)
我们都喜欢Explain.depesz.com分享 EXPLAIN 计划。所以我们想：为什么不制作一个类似的免费工具，专门用于获取查询的索引建议？查看我们的免费 pganalyze 索引顾问并了解最适合您查询的索引。


`pganalyze `
## [CCockroachDB 推出新的无服务器数据库平台](https://postgresweekly.com/link/115387/web)
CockroachDB 是一个历史悠久、分布式、面向弹性的基于 SQL 的数据库系统，其母公司推出了CockroachDB Serverless，这是一种托管产品，其定价完全围绕存储的总数据和查询的工作量进行。拥有Postgres 工具和客户端兼容性，这是值得一看的。


`Nate Stewart (CockroachDB) `
## [如何使用 Citus 为时间序列数据扩展 Postgres](https://postgresweekly.com/link/115389/web)
TimescaleDB 在与 Postgres 上的时间序列工作负载相关联方面做得很好，但这不是唯一的方法！Citus 通过提供分布式时间分区表提供了一种有趣的方法 - 以下是使其工作的方法。 


`Burak Velioglu `
## [为什么很难自动建议要创建的索引](https://postgresweekly.com/link/115390/web)
永远有用的Explain.depesz.comEXPLAIN ANALYZE工具的创建者解释了为什么他没有向该工具添加索引建议，以及他如何感觉索引建议工具通常只能提供帮助您还需要在组合中添加经验。


`Hubert depesz Lubaczewski `
## [通过迁移到 Amazon Aurora 和 RDS 上的分区表来提高大型表的性能和可管理性](https://postgresweekly.com/link/115392/web)
这个标题有点啰嗦，但这是在 AWS 上使用托管 Postgres 服务时使用分区来提高性能的系列文章中的最新一篇。


`Peter Celentano and Chirag Dave (AWS) `
## [Azure 上 PostgreSQL 灵活服务器中工作负载的内存调整](https://postgresweekly.com/link/115393/web)
以 Azure 为重点的介绍，用于调整 Postgres 服务器配置选项。


`Gennady Kostinsky `
## [中等大小文本对性能的惊人影响](https://postgresweekly.com/link/115394/web)
🏆我本周再次看到的“黄金老歌”:-) 你有你的小文本（用户名、电子邮件）、大文本（整个文档），和您的“中等”文本（评论、描述），虽然TOAST提高了存储较大文档的效率，但中等大小的文本列可能会使行变得非常宽，并对性能产生不成比例的影响。


`Haki Benita `
## [pg_statement_rollback v1.3：语句级别的服务器端回滚](https://postgresweekly.com/link/115397/web)
在语句级别添加服务器端事务回滚，就像在 Oracle 或 DB2 中一样。此版本增加了 Postgres 14 支持。


`Gilles Darold `
## [为什么客户选择 Percona for PostgreSQL？马上去查](https://postgresweekly.com/link/115398/web)
l,null,"en


`Percona `
## [postguard：根据类似 CORS 的规则测试 Postgres 查询的 Rust 库](https://postgresweekly.com/link/115399/web)
旨在通过在将它们发送到您的数据库之前对其进行测试来保护您的数据库免受恶意或无效查询的侵害。


`Alex Pearson `
# 💡本周提示


**🗓即将举办的Postgres活动**
