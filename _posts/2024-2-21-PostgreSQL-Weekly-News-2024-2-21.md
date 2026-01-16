---
layout: post
title: PostgreSQL 每周新闻 2024-2-21
---
### PostgreSQL每周新闻#543 - 2024年2月21日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/543)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/zcbeoxdnt3q3lcaylod7.jpg)
## [SQL 查询优化：综合开发人员指南](https://postgresweekly.com/link/151622/web)
一篇内容丰富的文章，深入探讨了 SELECT、INSERT 和 DELETE 查询的优化，涵盖了使用索引、对结果分页、避免联接以及窗口函数如何提供帮助（或没有帮助）等领域。 它不只是 Postgres，而是明确考虑到 Postgres 而编写的。


`Francesco Tisiot / Aiven `
## [什么更快？ COUNT(*) 或 COUNT(*) with LIMIT](https://postgresweekly.com/link/151623/web)
SQL 大师 Lukas Eder 查看执行计划并运行基准测试，以了解在检查 SQL 中是否存在 N 值时使用 LIMIT 子句是否有用。 剧透：是的。


`Lukas Eder `
## [使用 Hasura 在 PostgreSQL 上提供即时实时 GraphQL API](https://postgresweekly.com/link/151621/web)
将 Hasura 连接到您的 PostgreSQL 数据库并获得安全且高性能的 GraphQL API。 通过过滤、排序、分页、聚合等查询表和视图。 通过订阅立即提取对数据的任何实时更改。


`Hasura `
## [迁移到 AWS RDS 取得巨大成功的故事](https://postgresweekly.com/link/151624/web)
由于已经基于 EC2，这不是典型的本地到云迁移故事，但有趣的是，了解将覆盖 54 个应用程序和 TB 级实时数据的 5 个集群迁移到云上会发生什么情况 到 RDS 所涉及的。


`Karol Galanciak (BookingSync SAS) `

**本周摘要：**

*   📅 Microsoft 的 POSETTE Postgres 活动正在寻找[演讲者](https://postgresweekly.com/link/151625/web) - 您必须在 4 月 7 日之前提交提案。

*   如果您在 Amazon RDS 上运行 Postgres 11，请注意，您的数据库将在本月底[自动注册](https://postgresweekly.com/link/151626/web)到 Amazon RDS 扩展支持。 由于这可能会产生额外费用，请尽快考虑升级。

*   提醒如何在 psql 中[使用变量](https://postgresweekly.com/link/151627/web)。


*   Jimmy Angelakos 分享了他关于 Postgres 如何帮助您实施最佳实践（包括视频和幻灯片）的[演讲](https://postgresweekly.com/link/151628/web)。


## [在 Postgres 中创建“最后更新”列](https://postgresweekly.com/link/151630/web)
如果您希望在表中自动更新 Updated_at 时间戳列，则不必使用触发器（尽管您可能应该......）


`Gunnar Morling `
## [解读 Postgres 加密：初学者指南](https://postgresweekly.com/link/151631/web)
（非常）随意地了解可与 Postgres 一起使用的六级加密，从密码散列等基本内容到磁盘级加密和数据库本身内的数据加密。


`Tristen Raab `

## [使用 Debezium 和 Upstash Redis 从 Postgres 扇出并捕获更改数据](https://postgresweekly.com/link/151632/web)


`EVAN SHORTISS (NEON)`
## [Amazon Aurora 与 RDS：了解差异](https://postgresweekly.com/link/151633/web)


`CARLO MENCARELLI (TIMESCALE)`


**📰 机密**

📢 免费分布式 Postgres DB，具有 3 个节点集群，并可从 pgEdge Cloud 跨 3 个区域进行一键配置。 [报名并获得一件很酷的 T 恤](https://postgresweekly.com/link/151634/web)。

⚡了解如何在 PgBouncer 1.22.0 上使用 [prepared 语句来提高吞吐量](https://postgresweekly.com/link/151635/web)并使用 Neon 优化 Postgres 中的查询。

📢 使用 Redis 作为 Postgres 缓存？ [Readyset](https://postgresweekly.com/link/151636/web) Cloud 使查询缓存变得更容易，无需查询优化或应用程序重写。 今天[免费试用](https://postgresweekly.com/link/151636/web)。


## [PostgreSQL Anonymizer：Postgres 的数据屏蔽](https://postgresweekly.com/link/151637/web)
该扩展不是简单地对转储进行匿名化，而是让您直接针对您的模式声明屏蔽规则，从而直接对您的数据库进行匿名化。


`Dalibo `
## [libpqxx 7.9：Postgres 的官方 C++ 客户端 API](https://postgresweekly.com/link/151640/web)
维护者说，这是一个相当大的版本，也是最后一个支持 C++17 的版本，libpqxx 8.0 设置为要求 C++20。


`Jeroen Vermeulen `
## [Schemalint 1.1：Postgres 模式的 Linter](https://postgresweekly.com/link/151642/web)
一个允许您在大小写或列类型等问题上引发错误的 linter（因此更像 ESLint，而不是基本格式化程序）。


`Kristian Dupont `
## [pgexporter 0.5：Postgres 的 Prometheus Exporter](https://postgresweekly.com/link/151643/web)
从 v0.5 开始，它的目标是 Postgres 12 及更高版本，现在支持 TLS 的客户端证书。


`Red Hat `


* [pgmoneta 0.9](https://postgresweekly.com/link/151645/web) – 备份/恢复工具进行更新以改进 TLS 支持，与上面的 pgexporter 一样。

* [ruby-pg 1.5.5](https://postgresweekly.com/link/151646/web) – Ruby 的 Postgres 客户端库。
