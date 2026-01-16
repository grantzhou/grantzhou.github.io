---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-2-1
---
### PostgreSQL每周新闻#491 - 2023年2月1日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/491)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_350,h_100/e_make_transparent/co_white,e_outline:7/egbfiqexzspzz9grnyef.png)
## [transaction ID 环绕：野外漫步](https://postgresweekly.com/link/134714/web)
“对于大多数人来说，这是一个抽象的概念，一个潜伏在角落黑暗中的怪物。许多人都知道关于反环绕自动真空罐性能或数据库停止工作的恐怖故事，但是 谁见过真正的数据丢失？我决定直面野兽……”与 Laurenz 一起旅行，您也可以看到数据来自“死者”。


`Laurenz Albe `
## [问 HN：您如何测试 SQL？](https://postgresweekly.com/link/134715/web)
广泛讨论人们使用或不使用（！）测试他们的 SQL 查询的无数种方式。 “尝试将任何复杂的 SQL 编写为一系列具有语义意义的 CTE”引起了人们的共鸣。


`Hacker News `
## [你的 PostgreSQL 能保证 99.9% 的 HA 级别吗？](https://postgresweekly.com/link/134716/web)
Percona HA PostgreSQL 架构将开源工具和组件结合在一起，以增强和强化互操作性，确保您的应用程序始终可以访问所需的数据。 联系我们以了解更多关于我们架构的信息。


`Percona `
## [来到 v16：在没有超级用户的情况下生存](https://postgresweekly.com/link/134717/web)
Postgres 中的超级用户可以获得最高权限并且可以访问任何东西，包括在某种程度上，操作系统。 如果你想要 Postgres 中的超级用户而不是操作系统，这很棘手，但由于这次更新，在 Postgres 16 中变得容易得多。 罗伯特在这篇文章中进行了详细介绍。


`Robert Haas `
## [Postgres 的“供应链”](https://postgresweekly.com/link/134723/web)
每个重要项目都依赖于许多其他项目。 Peter 指出，Postgres 的一些依赖项非常脆弱，尽管这些问题似乎都不是 Postgres 独有的。


`Peter Eisentraut `
## [tbls：用于记录数据库的 CI 友好工具](https://postgresweekly.com/link/134725/web)
以 Markdown 格式自动记录数据库，并使用通过 DOT、PlantUML、Mermaid 或直接图像呈现的模式。 默认情况下，您会获得涵盖列、索引、关系和其他模式详细信息的文档（这里是示例文档）。 用 GO 写的。


`Ken’ichiro Oyama `
## [pg-lock-tracer: 基于 BPF 的锁跟踪器](https://postgresweekly.com/link/134727/web)
一种有趣的方式来挖掘在 Linux 上运行时 Postgres 中与锁相关的瓶颈。 它通过使用 eBPF 检测来观察 Postgres 进程的锁定活动。


`Jan Nidzwetzki `
## [您一直在寻找的 Postgres 服务](https://postgresweekly.com/link/134728/web)


`Crunchy Bridge `
## [Patroni 3.0：Postgres 高可用性模板](https://postgresweekly.com/link/134729/web)
使用 Python 和 ZooKeeper、etcd、Consul 或 Kubernetes 创建您自己的定制高可用性解决方案的模板。 v3.0 特别增加了对 Citus 的支持。


`Zalando SE `
## [pgslice：Postgres 分区“像馅饼一样简单”](https://postgresweekly.com/link/134732/web)
一种工具，可以生成或生成并执行所需的 SQL 语句来对新表或现有表进行分区，无需在服务器端安装任何内容。 用Ruby写的。


`Andrew Kane `
## [pg-mem：用于测试的实验性内存中 Postgres 实例](https://postgresweekly.com/link/134733/web)
由于是用 TypeScript 编写的，因此针对 Node.js 和基于浏览器的用例。 如果您想试验它可以处理的内容，可以使用 playground。


`Olivier Guimbal `
