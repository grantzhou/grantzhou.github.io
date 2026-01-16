---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-3-29
---
### PostgreSQL每周新闻#499 - 2023年3月29日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/499)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_350,h_100/e_make_transparent/co_white,e_outline:7/lhwcvgc1asd4fzaahty4.png)
## [您的 Postgres 准备好投入生产了吗？](https://postgresweekly.com/link/137517/web)
Craig 通过一份快速的生产要点清单让您做好生产准备，从备份和日志记录到语句超时和连接池。


`Craig Kerstiens `
## [max_wal_size 的重要性](https://postgresweekly.com/link/137518/web)
work_mem 和 max_wal_size 是两个可以对性能产生巨大影响的参数。 这是适当设置 max_wal_size 的基本技术。 （如果您对 work_mem 更感兴趣，Christophe 就此发表了一篇单独的文章 ;-)）


`Christophe Pettus `
## [了解如何为您的查询创建最佳 Postgres 索引（电子书）](https://postgresweekly.com/link/137516/web)
创建正确的索引可以显着提高查询性能。 在这本 PDF 电子书中，我们提供了有关索引类型、运算符、数据类型等的详细信息。 阅读本书后，您将能够为您的查询创建最佳索引。


`pganalyze `
## [Postgres：您不知道自己拥有的图形数据库？](https://postgresweekly.com/link/137520/web)
Postgres 足够灵活，可以为您提供开箱即用的类似图形数据库的功能，如果您准备为其建模正确的模式。 但是，如果您需要更高级的东西，Apache AGE 将提供更完整的支持，包括 OpenCypher 查询。


`Dylan Paulus `
## [在 Postgres 11–15 中搜索性能回归](https://postgresweekly.com/link/137527/web)
如果您使用 sysbench 在 Postgres v11 到 v15.2 中搜索性能回归，您会发现什么？ 主要是好消息。 从广义上讲，Postgres 继续变得稍微快一点，没有严重的性能失误。


`Mark Callaghan `
## [使用 Amazon S3 扩展 Postgres（在 Timescale 云上）](https://postgresweekly.com/link/137528/web)
这是 Timescale 的云平台特有的，但这是一个有趣的发展，其中 Postgres 可以正常使用，数据无缝“分层”并在适当的情况下存储在成本较低的 S3 存储中。 对于您可能很少想访问旧数据的时间序列数据库，从长远来看，这可能是一个巨大的胜利。


`Mike Freedman (Timescale) `
## [Postgres 16 中的新旧 debug_parallel_query 设置](https://postgresweekly.com/link/137529/web)
force_parallel_mode 在 Postgres 16 中将被称为 debug_parallel_query。为什么？ 加强它是为了调试目的，而不是获得并行查询执行的神奇方法。


`Pavlo Golub `
## [问我任何有关 Postgres 点播网络研讨会的高可用性的问题](https://postgresweekly.com/link/137530/web)


`Percona `
## [Postgres 16 亮点：pg_ident.conf 的更多模式](https://postgresweekly.com/link/137531/web)
Postgres 16 对 pg_ident.conf 进行了身份验证配置改进，允许使用 pg-user 条目的模式，如 pg_hba.conf 中的模式。


`Michael Paquier `
## [PgCat 1.0：现代 Postgres 池和代理](https://postgresweekly.com/link/137532/web)
内置于 Rust 中，PgCat 提供对分片的支持（包括实验性的基于 SQL 语法的分片）、负载平衡和故障转移支持。


`PostgresML `
## [pg_gpt：用自然语言进行查询的实验性扩展](https://postgresweekly.com/link/137533/web)
是的，想象一下“实验性”这个词周围巨大的闪光灯，但看到 OpenAI 的 ChatGPT 进行 SQL 查询生成总是很有趣。 也是使用 Rust 和 PGX 构建的简单扩展的简洁示例。


`CloudQuery `
## [Neon 的 Postgres 边缘兼容无服务器驱动程序](https://postgresweekly.com/link/137535/web)
Neon 是一个多云“无服务器 Postgres”平台，但某些无服务器功能平台的一个问题是无法与 Postgres 等系统建立直接 TCP 连接。 该怎么办？ 请改用 HTTP。 Neon 现在以使用 WebSockets 的 node-postgres 替代品的形式为 V8/Node 用户提供此功能。


`George MacKerron (Neon) `
