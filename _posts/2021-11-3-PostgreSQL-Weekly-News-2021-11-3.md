---
layout: post
title: PostgreSQL 每周新闻 2021-11-3
---
### PostgreSQL每周新闻#429 - 2021年11月3日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/429)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,e_tint:60:cyan/gcv61wtf7ujmndjahtlw.jpg)
## [再见微软 SQL Server，你好 Babelfish](https://postgresweekly.com/link/115657/web)
大约一年前，在第 384 期，我们报道了亚马逊推出 Babelfish，一个 SQL Server 到 Postgres 的“翻译层”——它现在普遍可用于 Aurora，但也已作为开源发布 在 GitHub 上，尽管在这方面还处于早期阶段。


`Sébastien Stormacq (AWS) `
## [部分索引、覆盖索引和多列索引如何减慢 UPDATE](https://postgresweekly.com/link/115662/web)
尽管有这些发现，但它也取决于您的 SELECT 与 UPDATE 命令的比率，以及您是否会权衡两者的性能。


`Nikolay Samokhvalov `
## [免费电子书：Postgres 中的有效索引](https://postgresweekly.com/link/115663/web)
了解如何为您的查询创建最佳 Postgres 索引。 我们深入探讨了索引类型、运算符、数据类型等。 创建正确的索引通常可以提高查询性能。


`pganalyze `
## [我们如何解构 Postgres 规划器以寻找索引机会](https://postgresweekly.com/link/115664/web)
为了构建新的 pganalyze 索引顾问，pganalyze 的团队着手将 Postgres 的查询规划器提取到一个独立的库中，以便他们可以更精确地查询它。 这篇文章深入探讨了他们是如何做到的以及指数顾问如何使用它。


`Lukas Fittl `
## [使用 PL/pgSQL 实现 Forth-Like 解释器](https://postgresweekly.com/link/115666/web)
上周 Phil 介绍了 PL/pgSQL 的基础知识，但本周进入了更奇怪的地方。


`Phil Eaton `
## [配置 TCP Keepalive 以获得更好的 Postgres 体验](https://postgresweekly.com/link/115669/web)
这个想法是为了更好地保持空闲数据库连接打开以及检测断开的连接。


`Laurenz Albe `
## [使用 Amazon Aurora 进行车辆路由优化](https://postgresweekly.com/link/115670/web)
使用 Aurora 的 Postgres 风格变体存储地图和拓扑数据以提供大规模地理空间路由功能的演练。 如果你有很多车辆在固定的时间内去很多地方，这就是你要做的工作。


`Nicola Pietroluongo (AWS) `
## [使用 Postgres 和 TimescaleDB 在 OpenSea 上分析数百万的 NFT 销售额](https://postgresweekly.com/link/115671/web)
我还没有真正进入 NFT 之类的领域，但如果这是一个你感兴趣的领域，Timescale 的人已经创建了一个教程和“工具包”来分析来自一个的 NFT 数据 最大的 NFT 市场之一。


`Sewrathan and Toth (Timescale) `
## [再也不用担心您的数据库](https://postgresweekly.com/link/115672/web)


`CockroachDB Serverless `
## [斯堪的纳维亚航空公司 (SAS) 在 Azure 上过渡到 Postgres](https://postgresweekly.com/link/115673/web)
来自 Microsoft 的一项新案例研究，斯堪的纳维亚领先的航空公司现在在 Azure Kubernetes 服务 (AKS) 上运行他们的预订应用程序，该服务由 Azure Database for PostgreSQL - 灵活服务器提供支持。


`Microsoft `
## [ScalikeJDBC：面向 Scala 开发人员的整洁的 SQL 数据库访问库](https://postgresweekly.com/link/115674/web)
不仅适用于 Postgres，但如果您是 Scala 开发人员，这是一个有吸引力的选择。


`ScalikeJDBC `

## [SQL GROUP BY 中的函数依赖](https://blog.jooq.org/functional-dependencies-in-sql-group-by/)

`LUKAS EDER`

