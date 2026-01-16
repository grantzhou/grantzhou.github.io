---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-3-20
---
### PostgreSQL每周新闻#547 - 2024年3月20日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/547)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/tjuxk6slt19hp3wuekxx.jpg)
## [Figma 历时九个月对其 Postgres 堆栈进行分片之旅](https://postgresweekly.com/link/152719/web)
为了解锁“（几乎）无限可扩展性”，Figma 的数据库团队在转向水平分片架构方面需要做大量工作（“从头到尾，我们的团队花了 大约九个月的时间来分片我们的第一个表”）。 这篇文章深入探讨了他们如何规划和执行该项目。


`Sammy Steele (Figma) `
## [OtterTune 优化您的 RDS 和 Aurora Postgres 数据库](https://postgresweekly.com/link/152718/web)
没有虚假屏幕截图 — 使用我们的产品导览点击浏览所有 OtterTune，了解如何使用 AI 来优化您的 Postgres 数据库。 然后进行测试：对无限数量的数据库进行 30 天免费试用。


`OtterTune `
## [“看，我为 Postgres 编写了一个新的 JIT 编译器”](https://postgresweekly.com/link/152720/web)
在你兴奋之前，作者的 pg-copyjit 项目是实验性的（仅限 x86-64），但他们确实寻求关于它如何为你工作的反馈——所以 如果您感到勇敢并且正在寻求一些潜在的绩效提升......


`Pinaraf / Pierre Ducroquet `
## [pgvector 的分布式查询](https://postgresweekly.com/link/152722/web)
在多个数据库之间分配工作负载提供了另一种在单个实例达到最大容量后进行扩展的方法。 Jonathan 还研究了如何使用 pgvector 和 Postgres 来水平扩展向量工作负载。


`Jonathan Katz `

**本周摘要：**

*   [Xata](https://postgresweekly.com/link/152723/web) 于 2022 年作为无服务器数据库平台推出，但现在它的作用就像也是[构建在 AWS Aurora 之上的无服务器 Postgres 平台](https://postgresweekly.com/link/152724/web)。


*   Dalibo 的 Florent Jardin 是[本周 PostgreSQL 人物](https://postgresweekly.com/link/152725/web)。


*   Nile 的 Gwen Shapira 在 [TOAST 及其对性能的影响](https://postgresweekly.com/link/152726/web)上写了一篇简洁的 Twitter/X 帖子。


## [Postgres 性能提升：HOT 更新和填充因子](https://postgresweekly.com/link/152727/web)
Postgres 有一种方法可以只更新堆（表），而不必更新所有索引 - 所谓的 HOT 更新，其中 HOT 代表“仅堆元组”。


`Elizabeth Christensen `
## [当 Postgres 不够用时？ Postgres 与分布式 DBMS 的性能评估](https://postgresweekly.com/link/152728/web)
通过 TPC-C 基准对 Postgres、CockroachDB 和 YDB 进行实证研究，并考虑 Postgres 中的可靠性/性能权衡。


`Evgeniy Ivanov `
## [提取数据库元数据以 Excel 格式呈现](https://postgresweekly.com/link/152730/web)


`RAYIS IMAYEV`
## [在一秒钟内创建1TB数据库的副本？](https://postgresweekly.com/link/152731/web)
您可以使用Neon Postgres中的复印件存储模型吗？



**📰 机密：**



* 你能在[一秒钟内创建 1TB 数据库](https://postgresweekly.com/link/152731/web)的副本吗？ 借助 [Neon Postgres](https://postgresweekly.com/link/152731/web) 中的写时复制存储模型，您可以做到。

* 📢 免费的 [pgEdge](https://postgresweekly.com/link/152732/web) 分布式 Postgres DB，具有 3 节点主动-主动集群和跨 3 个区域的一键配置。 [前 500 名免费 T 恤](https://postgresweekly.com/link/152732/web)。



**🛠 代码和工具：**


## [pgzx：使用 Zig 创建 Postgres 扩展](https://postgresweekly.com/link/152733/web)
如果您熟悉 pgrx 作为使用 Rust 构建 Postgres 扩展的方法，那么这与 Zig 类似，Zig 是另一种现代系统语言，比 Rust 更像 C。


`Xata `
## [WAL-G 3.0：数据库存档恢复工具](https://postgresweekly.com/link/152736/web)
用于 Postgres, MySQL/MariaDB、MongoDB 和其他几个 DBMS 的数据库存档和恢复的工具 - v3.0 引入了故障转移存储，特别是针对 Postgres 的 WAL 存档守护进程。


`Citus Data Inc. `
## [transqlate：将 SQL 转换为 PostgreSQL 语言](https://postgresweekly.com/link/152737/web)
这个由 Go 驱动的工具（诚然仍处于早期阶段）专注于 Oracle 风格的 SQL，旨在让您在样式、语法、 和语义。


`DALIBO `

* [pgweb 0.15](https://postgresweekly.com/link/152738/web) – Postgres 的跨平台桌面客户端。
* [pgwire 0.20](https://postgresweekly.com/link/152739/web) – Rust 库中的 Postgres wire协议。