---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-4-26
---
### PostgreSQL每周新闻#503 - 2023年4月26日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/503)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_350,h_100/e_make_transparent/co_white,e_outline:7/lhwcvgc1asd4fzaahty4.png)
## [Postgres 使用的九大失误](https://postgresweekly.com/link/138733/web)
快速浏览您在使用我们最喜欢的数据库时可能遇到的一些常见错误或陷阱。 它引起了很多人的共鸣，并在 Reddit 和 Hacker News 上引发了广泛的讨论。 要点包括忘记为外键添加索引，没有调整 work_mem，以及过于依赖 CTE。


`Phil Booth `
## [优化 Postgres 查询性能的最佳实践（电子书）](https://postgresweekly.com/link/138732/web)
了解如何将 Postgres 数据库的性能提高 3 倍，并将从磁盘加载的数据减少 500 倍。 我们分享帮助 Atlassian、CounterPath 等公司加快查询速度的经验教训。


`pganalyze `
## [使用 Rust 和 PGRX 构建 Postgres 扩展](https://postgresweekly.com/link/138736/web)
由于“各种原因”，流行的 PGX 框架已重命名为 PGRX，但仍然是在 Rust 中构建 Postgres 扩展的好方法。 原因没有解释，但我确实注意到一家公司拥有 PGX 作为数据库用途的商标，所以这可能是一个很好的举措。


`Technology Concepts & Design, Inc. `
## [解决 Ruby on Rails 应用程序的 N+1 Postgres 查询](https://postgresweekly.com/link/138743/web)
使用 Ruby on Rails 的 ActiveRecord 和使用更好的 SQL 来提高性能和避免 N+1 查询的技巧。


`Christopher Winslett `
## [从 Heroku 迁移 Postgres：Crunchy Bridge 的客户研究](https://postgresweekly.com/link/138744/web)


`Crunchy Bridge `
## [Postgres 触发器如何简化您的后端开发](https://postgresweekly.com/link/138745/web)
触发器让您可以自动执行函数以响应特定的数据库事件，该事件提供了将某些逻辑卸载到数据库本身的途径。


`The Mythical Engineer `
## [索引可能会伤害您的几种方式](https://postgresweekly.com/link/138742/web)
索引会在性能和资源消耗方面产生成本。


`Jobin Augustine (Percona) `
## [将批量操作从 Oracle 迁移到 Postgres 时的主要注意事项](https://postgresweekly.com/link/138747/web)
特别是使用 Amazon Database Migration Accelerator (Amazon DMA)。


`Karimi and Gopalappa (AWS) `
## [使用 AWS DMS 从 Postgres 中的分区表迁移数据](https://postgresweekly.com/link/138748/web)


`AYYAKKANNU, JOY, AND HEGDE (AWS)`
## [pgddl：DDL 提取器函数 (ddlx)](https://postgresweekly.com/link/138749/web)
将 PostgreSQL 系统目录转换为格式良好的 SQL DDL 片段的 SQL 函数，例如 CREATE TABLE。 一个有趣的用例是执行导致调用事件触发器的实际 DDL SQL。


`Alexi Theodore `
## [问 HN：Postgres 比 MySQL 好吗？](https://postgresweekly.com/link/138757/web)
Hacker News 解决了一个经典的、长期存在的争论点。 两个最流行的开源数据库如何相互竞争？


`Hacker News `
