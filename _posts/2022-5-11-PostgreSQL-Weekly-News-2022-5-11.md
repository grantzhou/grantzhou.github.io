---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-5-11
---
### PostgreSQL每周新闻#454 - 2022年5月11日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/454)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/dh2tn8ozojeohirqxl7g.jpg)
## [数据湖中的 Parquet 和 Postgres](https://postgresweekly.com/link/123324/web)
分区提供了一种方法来将巨大的静态数据集分解成更易于管理的部分（并在不再需要时丢弃它们）但是如果你想保留这些东西而不阻塞你的“主”数据库怎么办？将其放入“数据湖”并在需要时使用 FDW 进行查询！保罗在这里向我们展示了一种方法。


`Paul Ramsey `
## [🔎使用 pg_stat_statements 进行数据库和查询监控](https://postgresweekly.com/link/123325/web)
了解如何定期存储指标快照，以及如何从静态、累积信息转移到时间序列数据，以实现更高效的数据库监控——并附上代码示例。


`Timescale `
## [使用 Postgres 更快地计数](https://postgresweekly.com/link/123326/web)
计数是一项基本的数据操作，但如果您以错误的方式进行操作，它的扩展性可能会很差。Zach 向我们展示了 Postgres 如何处理计数、如何加速计数以及一些替代方法的一些基础知识。


`Zach Naimon `
## [pg_stat_monitor使用pg_stat_monitor更好地了解您的工作负载](https://postgresweekly.com/link/123327/web)
（上周发布了 v1.0 并发布了 GA）是一个收集查询指标的扩展，例如pg_stat_statements，它通过额外的规范进行了更深入的短期分析。


`Matt Yonkovit `
## [▶ 与 Ant Wilson 讨论 Supabase](https://postgresweekly.com/link/123329/web)
Supabase是基于 Postgres 构建的开源 Firebase 替代方案，也是一家以云为基础的 Postgres 即服务提供它的同名公司（他们刚刚筹集了 8000 万美元）。在这个播客中，Supabase 的联合创始人兼首席技术官不仅深入研究了 Supabase，而且更广泛地深入研究了 Postgres。


`Software Engineering Radio podcast`
## [Postgres 中的时区管理](https://postgresweekly.com/link/123332/web)
当 Laurenz 建议开发人员和时区不是好朋友时，他并没有错。数据库是时区出现的常见场所，Postgres 提供了一些类型和便利性，以减少使用它们的痛苦。


`Laurenz Albe `
## [以 100 英里/小时的速度更换轮胎：零停机时间迁移指南](https://postgresweekly.com/link/123333/web)
如果你从未见过人们在开车时更换汽车轮胎，请前往 YouTube 并搜索它——它很简洁——然后回到这篇关于类似编排模式的快速文章改变。就像轮胎一样，这是一种方法，但肯定不是唯一的:-D


`Kiran Rao `
## [使用证书、2FA 和堡垒的 SSH 最佳实践](https://postgresweekly.com/link/123334/web)
l,null,"en


`Teleport `
## [现在是 PostgreSQL 的庆祝时刻](https://postgresweekly.com/link/123335/web)
我情不自禁地喜欢一个被一些愚蠢包裹起来的教育时刻。


`Andreas Scherbaum `
## [Pigsty：“包含电池”的 Postgres 发行版](https://postgresweekly.com/link/123337/web)
一个奇怪的尝试，将 Postgres 与各种有用的扩展、可观察性和管理工具整合到一个更易于管理的发行版中，您可以在沙盒中本地运行或部署到云中地形。


`Feng Ruohang `
## [FerretDB 0.2：一个正在进行的、由 Go 驱动的 MongoDB 替代品](https://postgresweekly.com/link/123339/web)
你说是 MongoDB 吗？是的。这是在 Go 中重新创建 MongoDB 的基本要素的尝试，因此它可以作为替代品工作，并且它使用 Postgres 作为底层数据库引擎。


`FerretDB `
# 💡本周提示


**🗓即将举办的Postgres活动**
