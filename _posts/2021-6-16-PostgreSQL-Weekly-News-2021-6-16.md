---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-6-16
---
### PostgreSQL每周新闻#410 - 2021年6月16日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/410)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/zeaaliqt2rrnamgrjdfi.jpg)
## [关于 Postgres 的优化器方法论](https://postgresweekly.com/link/109661/web)
▶EDB 的 Robert Haas，Postgres 的长期主要贡献者，就查询优化的两个关键部分进行了一个小时的演讲：连接计划和统计。这是技术性的东西，但 Robert 在使相当不透明的过程变得可访问方面做得很好，并且了解这些东西会提升你的 Postgres 游戏。


`Robert Haas `
## [Postgres 中的交叉联接：问题和用例](https://postgresweekly.com/link/109662/web)
两个表之间的交叉联接或交叉乘积本质上是它们的笛卡尔积，即一个表的每一行与另一个表的每一行的组合。


`Laurenz Albe `
## [无需操作、可扩展且灵活的 Postgres 替代方案](https://postgresweekly.com/link/109663/web)
Fauna 将Postgres的操作完整性和关系建模与更适合云中现代应用程序开发的界面和架构相结合。没有操作瓶颈的 Postgres 的优点 -了解有关 Fauna 的更多信息。


`Fauna `
## [Postgres 中的“忽略空值”](https://postgresweekly.com/link/109664/web)
尽管缺少特定的“忽略空值”语法，但您可以通过定义自定义聚合来模拟此类行为。


`Jędrzej Biedrzycki `
## [在 Linux 上计算已提交的内存](https://postgresweekly.com/link/109665/web)
Linux 的内存管理器可以“过度使用”内存，这意味着将虚拟内存分配给进程，而不能保证内存具有任何底层物理存储。在查看 Postgres 正在使用的“已提交”内存时，这具有一定的相关性。


`Greg Smith `
## [从哪里获得 Postgres 在线帮助？](https://postgresweekly.com/link/109666/web)
Robert 概述了一些有用的地方，如果您有特定的 Postgres 问题，您可能想要尝试，包括在最近的 Freenode 惨败之后IRC（聊天）频道的结束位置。


`Robert Treat `
## [你需要Redis吗？Postgres 执行排队、锁定和 Pub/Sub ..](https://postgresweekly.com/link/109668/web)
我是Redis 的超级粉丝，虽然主流数据库（如 Postgres）和Redis 并排运行是很常见的，但您可能只将 Postgres 用于诸如工作之类的事情队列或锁。然而，到目前为止，这只能扩展..（我确实说过我是 Redis 的粉丝！


`Chris Farber `
## [HA with Patroni：轮到您测试失败场景](https://postgresweekly.com/link/109670/web)
了解由 Patroni 管理的 Postgres 高可用性环境在实践中是如何工作的。


`Camargos and Augustine (Percona) `
## [在 Go中加速Postgres 集成测试](https://postgresweekly.com/link/109671/web)
使用模板数据库和迁移进行更快的测试。


`Markus Wüstenberg `
## [实时监控 Postgres 性能](https://postgresweekly.com/link/109672/web)
收集 OOTB 和自定义 PostgreSQL 指标，并将它们与来自分布式基础架构、应用程序和日志的数据相关联。


`Datadog `
## [PostgREST：从 Postgres 数据库提供 RESTful API](https://postgresweekly.com/link/109673/web)
我们已经多次介绍过这个流行的工具。这是一个流行的独立应用程序，可将 Postgres 数据库转换为 RESTful API。


`Joe Nelson and Steve Chavez `
## [dadbod.vim：Vim 的现代数据库接口](https://postgresweekly.com/link/109675/web)
用于与包括 Postgres 在内的众多数据库交互的 Vim 插件。


`Tim Pope `
## [什么是 Postgres 贡献者？](https://postgresweekly.com/link/109676/web)
除了频繁的本周人物采访之外，聚光灯通常不会集中在 Postgres 的众多贡献者身上。感谢他们所有人的工作。


`Joshua D. Drake `
# 💡本周提示


**🗓即将举办的Postgres活动**
