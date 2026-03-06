---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-7-31
---
### PostgreSQL每周新闻#565 - 2024年7月31日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/565)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/uyzd9ns4dadbvyccch1t.jpg)
## [pg_statviz：Postgres 统计数据的时间序列分析和可视化](https://postgresweekly.com/link/158227/web)
扩展和实用程序对，用于执行时间序列分析和各种统计数据的可视化，例如 I/O、锁、WAL 和缓冲区使用情况。新的 v0.7 版本增加了 Postgres 17 支持、新的 I/O 统计数据和收集数据的 Pandas 重采样。

`Jimmy Angelakos `

## [在 Postgres 表之间复制数据的最快方法](https://postgresweekly.com/link/158229/web)
Anthony 比较了几种方法，既使用本机 SQL，也使用扩展。剧透是 pg_bulkload 以相当大的优势胜出，尽管有一些权衡。


`Anthony Sotolongo `
## [找到 Postgres 性能问题的根本原因](https://postgresweekly.com/link/158226/web)
查询速度慢导致应用程序运行缓慢？膨胀的表导致意外 I/O？使用 pganalyze 通过智能调优顾问和深入监控提供一致的数据库性能和可用性。


`pganalyze `
## [ClickHouse 收购 PeerDB 以实现本机 Postgres CDC 集成](https://postgresweekly.com/link/158231/web)
[PeerDB](https://postgresweekly.com/link/158232/web) 是由前 Microsoft 和 Citus Data 员工构建的数据复制工具，用于将数据从 Postgres 流式传输到数据仓库、队列和其他存储引擎。数据仓库公司 [ClickHouse](https://postgresweekly.com/link/158233/web) 似乎已经看到了将这种技术引入内部的战略价值。


`Sai Srirampur `
## [设计原型：Postgres 计划冻结](https://postgresweekly.com/link/158234/web)
计划冻结是指为参数化查询保存特定计划，以便将来可以按原样再次使用。Andrei 解释了实现他的扩展（您也可以试用）的技术细节。


`Andrei Lepikhov `

### 本周摘要：

* Stack Overflow 广受欢迎的年度开发者调查结果于上周出炉，Postgres 已连续第二年位居[数据库排行榜榜首](https://postgresweekly.com/link/158235/web)，目前有 48.7% 的受访者在使用。

* Robert Haas 宣布将举办[虚拟 PostgreSQL 黑客研讨会](https://postgresweekly.com/link/158236/web)，8 月和 9 月将以小组形式讨论不同的 Postgres 技术讲座。

## [关于 Linux 内存过量使用 Postgres 的知识](https://postgresweekly.com/link/158237/web)
Linux 的过量使用功能可以允许分配比实际可用内存更多的内存。在某些情况下，这有好处，但对 Postgres 来说却是个坏消息。


`Laurenz Albe `
## [如何保持 Postgres 社区的活力](https://postgresweekly.com/link/158238/web)
在法国 PG Day 的兴奋中，作者分享了他对建立本地 Postgres 用户组和召开会议的想法。


`Florent Jardin `

### 机密：

[Blacksmith](https://postgresweekly.com/link/158240/web) 只需更改一行代码，即可将 GitHub Actions 的运行速度提高 2 倍，成本降低一半。受到 GitBook 和 Slope 等 100 多家公司的信赖。

通过 [Redgate 的 101 系列网络研讨会](https://postgresweekly.com/link/158241/web)（简单易懂、由专家主持的课程）提升您的 PostgreSQL 技能。这就是简化版的 PostgreSQL。


## [使用递归 CTE 进行图形检索](https://postgresweekly.com/link/158242/web)
Postgres 不是“图形数据库”，但它肯定可以处理与图形相关的概念。


`Sheshbabu Chinnakonda`

📄 [连接池基础知识](https://postgresweekly.com/link/158243/web) - Stefanie Janine Stölting

📄 [在 Postgres 17 中拆分和合并分区](https://postgresweekly.com/link/158244/web) - pgDash



### 🛠 代码和工具
[QuestDB 8.1](https://postgresweekly.com/link/158245/web) – Java 驱动的时间序列数据库，兼容 Postgres 有线协议。v8.1 现在可以读取 Parquet 文件。

[Pongo 0.8](https://postgresweekly.com/link/158247/web) – Node.js 的 Postgres 驱动程序，提供 MongoDB 样式的 API。

[FerretDB 1.23](https://postgresweekly.com/link/158248/web) – 类似于 MongoDB 的数据库，但使用 Postgres 进行存储。

[pgxmock 4.2](https://postgresweekly.com/link/158249/web) – 模拟驱动程序，用于在 Go 中测试数据库交互。

[Bytebase 2.22](https://postgresweekly.com/link/158250/web) – 面向团队的数据库 devops 和 CI/CD 系统。

[RisingWave 1.10](https://postgresweekly.com/link/158251/web) – 与 Postgres 兼容的流式数据库。

[pgAdmin 4 8.10](https://postgresweekly.com/link/158252/web) – 流行的 Postgres 管理工具。