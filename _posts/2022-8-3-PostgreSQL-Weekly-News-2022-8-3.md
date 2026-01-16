---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-8-3
---
### PostgreSQL每周新闻#466 - 2022年8月3日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/466)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/vbgd6szk5vaodilgnpxn.jpg)
## [调试 Postgres Autovacuum 问题：13 条提示](https://postgresweekly.com/link/127027/web)
Samay 要求我们想象看到我们的数据库比预期的大，I/O 负载高且性能低下。 我们在我们的表中发现了很多膨胀并运行 VACUUM。 但是我们可能会问“为什么 Postgres autovacuum 不首先清理膨胀......？” — 这是一个很好的问题，如果您值得信赖的VACUUM没有像以前那样清理干净，这篇文章涵盖了各种绊脚石和要做的事情。


`Samay Sharma (Citus Data) `
## [📊 Postgres 2022 完整状态](https://postgresweekly.com/link/127028/web)
最近几周他们一直在用零碎的东西取笑我们，但现在我们可以看到完整的结果（或下载结果的转储以自己分析）。 不过，这并不令人惊讶。 PostGIS 是最流行的扩展。 Python 作为最流行的非 SQL 语言。


`Timescale `
## [从边缘访问 Postgres](https://postgresweekly.com/link/127029/web)
在几分钟内在全球范围内扩展 PostgreSQL 数据库以实现低延迟边缘访问。 PolyScale 自动缓存数据并在更靠近用户的位置执行查询，以在边缘实现低延迟、无服务器功能。


`PolyScale.ai `
## [改进了 ORDER BY / DISTINCT 聚合的性能](https://postgresweekly.com/link/127030/web)
来自 Postgres 存储库的技术项目传入！ “在 Postgres 中，ORDER BY / DISTINCT 聚合的性能已经糟糕太久了，”David Rowley 说，但是在实施了理论上听起来很简单但在实践中很难正确实现的优化之后，情况将不再如此 .


`David Rowley `
## [用 C 扩展 Postgres：一个简单的例子](https://postgresweekly.com/link/127034/web)
我最近看到一些公开讨论，有人评论说为 Postgres 构建扩展是多么令人愉快。 现在有很多选项可以做到这一点（例如将 Rust 与 pgx 一起使用），但使用良好的老式 C 可以很好地工作，并且没有您想象的那么困难。 （本教程也有助于建立必要的部分。）


`Eric Radman `
## [在 Amazon Aurora 上管理长时间运行的读取查询](https://postgresweekly.com/link/127037/web)
讨论“潜在冲突”并分享“在 Aurora PostgreSQL 上管理长时间运行的读取查询的最佳实践”。


`Wanda He and Avi Jain (AWS) `
## [使用 citus_stat_activity 和 citus_lock_waits 监控分布式 Postgres 活动](https://postgresweekly.com/link/127038/web)
仅适用于 Citus 用户：“.. Citus 11 中引入的一些新监控工具将帮助您跟踪和控制分布式查询”


`Halil Ozan Akgul (Citus Data) `
## [g-boss 8.0: Postgres + Node.js 作业排队系统](https://postgresweekly.com/link/127039/web)
用于后台处理和可靠异步执行的作业队列。 它使用 Postgres 的特定功能（如 SKIP LOCKED）来保证安全。 v8 使 Node 14 成为支持的最低版本，并允许在某些操作上重用现有的数据库连接。

`Tim Jones `
## [简化数据库管理。 释放您的团队。 控制您的数据](https://postgresweekly.com/link/127040/web)


`EDB BigAnimal `
## [Dexter：Postgres 的自动索引器](https://postgresweekly.com/link/127041/web)
收集您的查询并生成适合它们的索引。 这是一篇介绍这个想法的文章。


`Andrew Kane `

