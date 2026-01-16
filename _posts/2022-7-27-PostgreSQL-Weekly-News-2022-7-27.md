---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-7-27
---
### PostgreSQL每周新闻#465 - 2022年7月27日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/465)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/jmmu5s2w7gpavomzvrtc.jpg)
## [Postgres v14 中更好的 SQL 函数](https://postgresweekly.com/link/126733/web)
Postgres 14 引入了一种定义 SQL 函数的新方法，本周它引起了至少两名开发人员的注意，因为我们有两篇关于它的好帖子。 从本质上讲，“SQL 函数和过程的主体不再需要是字符串常量”，这提供了一些优势，正如我们在 Laurenz 的演示中看到的那样。

`Laurenz Albe `
## [BEGIN ATOMIC：在 Postgres 14 中创建函数的更好方法](https://postgresweekly.com/link/126734/web)
是的，它与上面的故事相同，但更少关注解释，更多关注更大的代码示例。 如果您对这个领域感兴趣，那么两者都值得略读。


`Jonathan Katz `
## [免费电子书：Postgres 中的有效索引](https://postgresweekly.com/link/126735/web)
了解如何为您的查询创建最佳 Postgres 索引。 我们深入探讨了索引类型、运算符、数据类型等。 创建正确的索引通常可以将您的查询性能提高 10 倍甚至 100 倍。


`pganalyze `
## [使用行级安全性交付多租户 SaaS](https://postgresweekly.com/link/126736/web)
对单模式多租户数据库中的数据库级（而不是应用程序级）“默认安全”安全性的探索和思考。 Hacker News 上关于这个话题的广泛讨论也被证明是非常有价值的。


`Miki Pokryvailo (Nile) `
## [使用 Native Postgres 和 pg_partman 进行分区](https://postgresweekly.com/link/126738/web)
有时过早的优化是没有意义的，但是如果你知道你的数据库很可能会迅速进入 TB 的世界（例如，你可能存储了大量的时间序列数据），那么主动进行分区就是 一个明智的想法，这是一个特别温和的介绍。


`Elizabeth Christensen `
## [使用 BUFFERS 进行查询优化](https://postgresweekly.com/link/126746/web)
你知道 EXPLAIN ANALYZE，但是 BUFFERS 呢？ 它提供了有关如何在查询中使用 Postgres 缓冲区的信息，并且可以帮助您缩小与 I/O 相关的问题的范围。

`Michael Christofides `
## [13 个与 psql 无关的 Postgres 相关工具](https://postgresweekly.com/link/126745/web)
Timescale 继续分析其最近的 PostgreSQL 2022 状态调查的结果，这一次着眼于工具。 我们每周都会自己介绍 Postgres 工具，但这篇文章包含了人们实际使用的数字。


`Ryan Booz (Timescale) `
## [从 Heroku 迁移：关于 Crunchy Bridge 的客户研究](https://postgresweekly.com/link/126748/web)


`Crunchy Bridge `
## [AlloyDB 与 Postgres：性能评估](https://postgresweekly.com/link/126749/web)
一如既往，以愤世嫉俗但开放的心态进入基准测试； 基准测试很难！ 尽管如此，看到有人将 Google 的类似 Aurora 的 AlloyDB for PostgreSQL 投入使用，还是很酷的。


`Michael Aboagye `
## [pg_jsonschema：JSON Schema 验证扩展](https://postgresweekly.com/link/126751/web)
Postgres 对 JSON / JSONB 列的支持现在几乎是首屈一指的，但是如果你想验证 JSON 数据的结构怎么办？ JSON Schema 提供了一种定义基于 JSON 的格式的方法，并且此扩展允许您使用此类模式验证 JSON 文档。 （有趣的是代码是多么简单，因为它依赖于不同的 Rust 库来完成艰苦的工作。）


`Supabase `
## [如何在 Rocky Linux 9 上安装 Postgres 和 PostGIS](https://postgresweekly.com/link/126753/web)

`DEVRIM GUNDUZ`