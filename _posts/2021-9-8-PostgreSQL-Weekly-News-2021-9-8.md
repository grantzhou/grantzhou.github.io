---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-9-8
---
### PostgreSQL每周新闻#421 - 2021年9月8日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/421)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/gc503yrhgvy9lfybar8x.jpg)
## [少即是多：数据库连接扩展](https://postgresweekly.com/link/113407/web)
Postgres 服务器可以处理的连接越多越好……对吗？ 不总是。 如果 max_connections 设置为不切实际的数字，即使没有使用这些连接，也会产生负面影响。


`Richard Yen `
## [使用 PostGIS 和 ogr_fdw 查询空间数据](https://postgresweekly.com/link/113408/web)
ogr_fdw 是一个外部数据包装器，用于处理各种基于矢量的 GIS 数据格式，而无需将数据拉入普通的 Postgres 表。


`Kat Batuigas `
## [🎆什么是时间加权平均值以及您为什么应该关注](https://postgresweekly.com/link/113410/web)
了解时间加权平均值的基础知识、为什么它们对数据分析如此强大，以及如何使用 TimescaleDB 超函数来更快地计算它们——所有这些都使用 SQL。 获取提示和 5+ 个查询以帮助您入门🔥


`Timescale `
## [Aurora PostgreSQL db.r6g 与 db.r5 与 YBIO 的比较](https://postgresweekly.com/link/113411/web)
在 Amazon RDS Aurora 实例方面对 Intel Xeon 与 AWS Graviton 2 性能进行基准测试的实验。 Graviton 因其更便宜的价格而表现良好，但一如既往，以基准测试运行您自己的实验，因为上下文很重要。


`Franck Pachot `
## [使用 Postgres 分区用例](https://postgresweekly.com/link/113412/web)
考虑您可能想要使用本机分区的各种原因。


`Adrien Nayrat `
## [Psycopg3 的初步回顾](https://postgresweekly.com/link/113413/web)
Psycopg3 是 Psycopg2 的继承者，Psycopg2 是一种非常流行的从 Python 使用 Postgres 的方法。 以下是迄今为止它的一些好处。 请注意，如果您需要更多上下文，我们在第 390 期采访了 psycopg3 的创建者 Daniele Varrazzo。


`Ryan Lambert `
## [Postgres 14 的索引膨胀减少](https://postgresweekly.com/link/113415/web)
看看 Postgres 14（仍处于测试阶段）如何通过快速命名的“自底向上索引元组删除”来减少 B 树索引膨胀。 测试用例显示了与 Postgres 13 的差异。


`Laurenz Albe `
## [识别 Datadog 备忘单中的关键指标和有用的 PostgreSQL 命令](https://postgresweekly.com/link/113417/web)


`Datadog `
## [为什么你应该主要在 Kubernetes 上部署 Postgres](https://postgresweekly.com/link/113418/web)
一个可能有争议的演讲 :-) 一个 20 分钟的演讲，涵盖了“堆栈问题”，Kubernetes 如何解决它，以及在 Kubernetes 上运行 Postgres 的一些利弊。


`Álvaro Hernández opinion`
## [Citus 10.1 Postgres 扩展中的分片重新平衡](https://postgresweekly.com/link/113419/web)
“无论您使用 Citus 开源扩展 Postgres，还是在云中使用 Citus，这篇文章都是您了解 Citus 10.1 中分片重新平衡器新功能的指南。”


`Jelte Fennema (Citus Data) `
