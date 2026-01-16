---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-5-25
---
### PostgreSQL每周新闻#456 - 2022年5月25日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/456)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/dxpjerumowllwolram7f.jpg)
## [PostgreSQL Anonymizer 1.0：Postgres 的隐私设计](https://postgresweekly.com/link/123868/web)
使用三种不同策略之一隐藏或替换数据库中的个人身份信息 (PII) 或商业敏感数据的扩展。 有了这个 1.0 版本，它现在被认为可以投入生产了。


`Dalibo `
## [Postgres 15 Beta 1 发布](https://postgresweekly.com/link/123870/web)
上周我们链接到了草稿发行说明，但现在实际的 beta 版本在这里。 不要指望将其推出到生产环境中，但您可以使用刚刚发布的 Docker 映像 15beta1 快速使用它。 如果您不熟悉这个想法，我已经写了一篇关于使用 Docker 启动 Postgres 15 的快速教程。


`PostgreSQL Global Development Group `
## [网络研讨会：如何推理为您的 Postgres 数据库编制索引](https://postgresweekly.com/link/123874/web)
我们深入探讨 Postgres 如何确定性地选择用于特定查询的索引，并介绍分析查询以及创建和优化索引的方法。 立即注册并参加我们在太平洋夏令时间 6 月 16 日上午 9:30 举行的网络研讨会。


`pganalyze `
## [加快 Postgres 15 中的排序性能](https://postgresweekly.com/link/123887/web)
对在 Postgres 中更快地进行排序（与数据库中的基本操作一样）所做的工作结果进行了精彩的观察。 您的查询会在 Postgres 15 上运行得更快吗？ 最有可能的。


`David Rowley `
## [与 Postgres 未完成的事情](https://postgresweekly.com/link/123875/web)
Craig（现在在 Crunchy Data 工作）是 Heroku 托管 Postgres 服务的关键参与者，在这篇文章中，他讲述了它是如何组合在一起的一些故事，围绕其操作的一些技术考虑，以及， 好吧，让它运行良好的大量护理。


`Craig Kerstiens `
## [查询优化：LEFT JOIN vs UNION ALL](https://postgresweekly.com/link/123876/web)
作者遇到了一个看起来很简单的查询，它运行的时间不成比例，在这篇文章中，它通过一个更复杂但更快的替代方法来工作。


`David Christensen `
## [WAL-G 2.0 发布：存档和恢复工具](https://postgresweekly.com/link/123877/web)
WAL-G 是一种用于创建加密和压缩 Postgres（以及 MySQL 或 SQL Server）备份的工具，支持多种压缩方法，如 LZ4、LZMA 和 Brotli。


`Citus Data `
## [带有 pg_featureserv 的即时热图](https://postgresweekly.com/link/123880/web)
尽管名称如此，pg_featureserv 不是 Postgres 扩展，而是一个基于 Go 的微服务，它提供对 PostGIS 的 RESTful 访问——这个快速教程展示了如何将各个部分组合在一起以使用它来制作动态热图 .


`Paul Ramsey `
## [使用 Datadog 数据库监控优化](https://postgresweekly.com/link/123882/web)


`Datadog Database Monitoring `
## [让我们用 Go(lang) 构建一个分布式 Postgres 概念证明](https://postgresweekly.com/link/123883/web)
你能用 600 行代码组合一个迷你 Postgres 吗？ 一个简单的例子，你可以在 Go 中用一点点代码完成一些复杂的事情（即使第三方包在这里做了很多工作。）


`Phil Eaton `
## [如何在 Red Hat Enterprise Linux 9 上安装 Postgres 10 到 14](https://postgresweekly.com/link/123884/web)
上周发布了 RHEL 9。


`Devrim Gündüz `
## [使用 Azure 数据工厂将 Postgres 数据移动速度提高 26 倍](https://postgresweekly.com/link/123886/web)
如果您在 Azure 上使用 Postgres，并且需要将数据大量输入或输出数据库，Azure 数据工厂必须引起您的注意，尤其是现在它甚至比之前还快出许多


`Halil Ozan Akgul `

