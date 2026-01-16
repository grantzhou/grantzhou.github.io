---
layout: post
title: PostgreSQL 每周新闻 2022-4-20
---
### PostgreSQL每周新闻#451 - 2022年4月20日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/451)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/yrwb1ikowjn298kv96jx.jpg)
## [Retool 如何将其 4TB Postgres 数据库升级到 v13](https://postgresweekly.com/link/122484/web)
4TB 可能不是“大数据”，但它位于 SaaS 主数据库大小的共同区域，因此 Retool 在从 Postgres 9.6 升级到 13 的过程中学到的故事和技巧可能证明了这一点 兴趣。


`Peter Johnston (Retool) `
## [更快的地理空间丰富：Postgres 与 ..](https://postgresweekly.com/link/122485/web)
马克多年来以发表一些出色的数据分析帖子而闻名（例如他的 11 亿次出租车乘车系列），现在他将 Postgres 与 ClickHouse 和 BigQuery 放在一起转换大量坐标 到 H3 标识符中。 Postgres 没有赢，但也没有输。


`Mark Litwintschik `
## [具有时间序列超能力的 Postgres 你最喜爱的。。。](https://postgresweekly.com/link/122488/web)
TimescaleDB 是用于时间序列和分析的开源关系数据库，由开发人员为开发人员构建。 它将 PostgreSQL 的熟悉程度与速度和 PB 级规模结合在一起。 免费试用（无需信用卡）。


`Timescale `
## [查找并修复缺失的 Postgres 索引](https://postgresweekly.com/link/122489/web)
如果你正在寻找一个完美的方法来以最有效的方式破坏性能，那么缺失的索引是一个关键因素，”Hans-Jürgen 说，但幸运的是，这里的任务是如何 避免该问题，修复丢失的索引并提高性能。


`Hans-Jürgen Schönig `
## [▶ 高级 INT 到 BIGINT 转换](https://postgresweekly.com/link/122490/web)
多年来，整数溢出导致了各种错误、问题和中断，所以我们是否应该将所有事情都转移到 BIGINT 上？ 没那么快，罗伯特说，他在这个 20 分钟的演讲中深入探讨了这个困境。


`Robert Treat `
## [那一种最合适：Postgres 和 ClickHouse？](https://postgresweekly.com/link/122493/web)
GitLab 首席执行官的一篇观点文章认为 Postgres 和 Clickhouse 涵盖了企业所需的大部分 OLAP 和 OLTP 基础（尽管可以说 Postgres 正在以 HTAP 的形式更多地进入 OLAP 世界）。


`Sid Sijbrandij `
## [在 Emacs 中使用 pgFormatter 格式化 SQL 代码](https://postgresweekly.com/link/122495/web)
如果 Emacs 是您选择的操作系统编辑器，这可能会很有用，尽管 pgFormatter 是一个基于 Perl 的 SQL 美化器，也可以在命令行（甚至在 Web 上）使用。


`Luca Ferrari `
## [保护您的 PostgreSQL 数据库：最佳实践概述](https://postgresweekly.com/link/122498/web)


`Teleport `
## [使用自签名证书在 Rust 中通过 SSL 连接到 Postgres](https://postgresweekly.com/link/122499/web)
这确实适用于 YugabyteDB，但它与 Postgres 是有线兼容的，因此我们承诺它可以在两者上工作。


`Fits Hoogland `
## [“我们在 ZFS 上使用 Postgres 的经验”](https://postgresweekly.com/link/122500/web)
ZFS 是一个文件系统，具有许多有用的高级特性（但也有更高的硬件要求），包括快照和透明压缩——这两者对于数据库用例都非常有用。


`Aycan Gulez `
## [一个 SQLite 到 PostgreSQL 的迁移故事](https://postgresweekly.com/link/122502/web)
你不经常听说 SQLite 到 Postgres 的迁移，但我自己在将小型 Rails 应用程序迁移到云平台时做了一些（SQLite 和容器造成了悲伤的时刻）。 这个特别的故事没有太多内容，但很高兴看到人们的推理。


`Danny Xu `
## [Orafce：适用于 PostgreSQL 的 Oracle 兼容性函数](https://postgresweekly.com/link/122504/web)
Orafce 实现了 Oracle 数据库中的一些函数，这些函数可能对迁移到 Postgres 的用户有用。 v3.21.0 从未来的 Postgres 15 向后移植 regexp_replace 和 regexp_instr。


`Orafce `
## [PostgresML：仅使用 SQL 训练模型和进行预测](https://postgresweekly.com/link/122506/web)
“您使用简单的 SQL 命令训练模型，并通过您已经在使用的机制在您的应用程序中获得预测：通过标准 Postgres 连接进行查询。”


`Lev Kokotov and Montana Low `

