---
layout: post
title: PostgreSQL 每周新闻 2021-7-21
---
### PostgreSQL每周新闻#415 - 2021年7月21日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/415)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/lrftbpdom7zs8imcuii3.jpg)
## [切切出中间层：直接从 Postgres 生成 JSON](https://postgresweekly.com/link/111292/web)
除了能够存储 JSON 数据结构，Postgres 长期以来一直能够生成 JSON，它可以直接返回以在您的应用程序中使用（或者直接传递给用户，如果 你有信心）


`Paul Ramsey `
## [在 Amazon RDS 或 Aurora 数据库上使用 pg_cron 调度作业](https://postgresweekly.com/link/111293/web)
RDS 在 12.5 及更高版本中支持 pg_cron 扩展，Aurora 在 12.6 及更高版本中支持它。 您可以使用它来自动执行日常维护任务。


`Sukhpreet Kaur Bedi (AWS) `
## [使用 Datadog 可视化关键 Postgres 性能指标](https://postgresweekly.com/link/111295/web)
使用粒度 Postgres 分析和开箱即用的仪表板快速识别运行缓慢的查询、瓶颈和错误。 将数据与跟踪和日志相关联以实时优化 Postgres 性能。 立即开始 Datadog 试用。


`Datadog `
## [Postgres 在生成顺序 ID 时意外跳过？](https://postgresweekly.com/link/111296/web)
原标题:“一个，两个，跳过一些……” 听起来很有趣，但我想更好地解释这是关于什么的:-) 本质上，Postgres 可以在崩溃或以其他方式重新启动时传递序列中的预分配值。。。用你意想不到的方式。


`Pineapple Technology `
## [正在进行的事务的逻辑复制](https://postgresweekly.com/link/111297/web)
Postgres 14 正在开发拥有复制正在进行的大型事务的能力，这篇文章详细介绍了所涉及的问题以及它是如何结合在一起的。


`Amit Kapila `
## [如何从列表范围中获取元素列表？](https://postgresweekly.com/link/111298/web)
与 Postgres 即将推出的多范围数据类型合作的另一种看法。


`Hubert depesz Lubaczewski `
## [使用语句超时控制“失控”查询](https://postgresweekly.com/link/111300/web)
一个经过良好调整的生产数据库是一件美妙的事情，可以看到处理成千上万的查询，直到……一个查询使一切都崩溃了。 为您的数据库设置默认语句超时有助于避免一些棘手的时刻。


`Craig Kerstiens `
## [使用 Postgres 对 CentOS 与 Rocky Linux 进行基准测试](https://postgresweekly.com/link/111301/web)
我发现，基准测试总是很难解释，但了解 Rocky Linux 很有趣，它与之前的 CentOS 一样，是一个红帽企业兼容的 Linux 发行版。


`Dinesh Kumar `
## [💻如何在 Mac、Ubuntu、Debian 和 Windows 上安装 psql](https://postgresweekly.com/link/111303/web)

`Timescale `
## [pgAdmin 4 v5.5 发布](https://postgresweekly.com/link/111304/web)
流行的基于 Web 的 Postgres 管理工具又向前迈进了一步。 5.5 获得 OAuth 2 支持并引入了在仪表板上突出显示长时间运行的查询的功能。


`pgAdmin Development Team `
## [Noisia：Postgres 的“有害工作负载生成器”](https://postgresweekly.com/link/111305/web)
创建诸如死锁、不做任何事情的事务和生成磁盘临时文件的查询之类的事情。 为什么？ 用于测试、压力测试您的设置等。小心谨慎地使用。


`Lesovsky Alexey `
## [PGX：使用 Rust 构建 Postgres 扩展](https://postgresweekly.com/link/111306/web)
使用 Rust 构建 Postgres 扩展的框架，而不是您可能更习惯的 C 或 C++。 它现在也支持 Postgres 13。


`ZomboDB `
