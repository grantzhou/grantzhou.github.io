---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-9-11
---
### PostgreSQL每周新闻#569 - 2024年9月11日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/569)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/xa03n16p8xueitspvzyv.jpg)
## [Tetris-SQL：使用 SQL 的图灵完备性构建俄罗斯方块](https://postgresweekly.com/link/159621/web)
只需在 Postgres 上执行几个 SQL 查询即可实现俄罗斯方块！这不仅是一份令人印象深刻的工作，而且也具有教育意义，因为 Nuno 花时间在 README 中详细介绍了实现细节。

`Nuno Faria `

## [Postgres 17 候选版本 1 已发布](https://postgresweekly.com/link/159623/web)
如果您不确定是否要运行任何测试版，那么现在正是试用的好时机，因为候选版本往往与最终版本基本相同。最终版本预计于 9 月 26 日发布（因此，我们可能会在那一周推迟 Postgres Weekly）。


`PostgreSQL Global Development Group `
## [以一半的成本将 GitHub Actions 运行速度提高 2 倍](https://postgresweekly.com/link/159620/web)
Blacksmith 通过在现代游戏 CPU 上运行 GitHub Actions 来显著提高运行速度。集成 Blacksmith 只需更改一行代码。Ashby、Superblocks 和 Slope 等 100 多家公司使用 Blacksmith 帮助开发人员更快地合并代码。


`Blacksmith `
## [缩小大型 Postgres 表：复制-交换-删除](https://postgresweekly.com/link/159624/web)
如果您有一个庞大而笨重的表，并且只有一部分数据在活动使用，但您不想对该表进行分区或执行大量的 DELETE 操作，则可以将您想要保留的行复制到新表中，重命名新表，然后删除原始表。


`Andrew Atkinson  `

### 本周摘要：

* Aaron Francis 和 xata 将于下个月发布一个名为 [Mastering Postgres](https://postgresweekly.com/link/159625/web) 的视频课程，但值得注意的是 [X 上相当有冲击力的宣传视频](https://postgresweekly.com/link/159626/web)。😁

* [ParadeDB 的 Philippe Noël](https://postgresweekly.com/link/159627/web) 是本周 PostgreSQL 人物的受访者。


## [Neon 如何动态估计 Postgres 的工作集大小](https://postgresweekly.com/link/159628/web) 
“工作集”是指系统在特定时间段内使用/读取/写入的数据。弄清楚 Postgres 服务器当前的“工作集”实际上相当困难，但如果您想要实现自动扩展，这一点至关重要，因为无服务器平台 Neon 现在可以做到这一点。


`Em Sharnoff (Neon)`
## [了解 Postgres Hackers 邮件列表](https://postgresweekly.com/link/159629/web)
如果您想参与 Postgres 开发或对跟进开发有浓厚兴趣，那么 pgsql-hackers 邮件列表就是您的不二之选。作为一个繁忙且技术含量极高的邮件列表，这里有很多内部术语，Greg 在此处对此进行了解释。


`Greg Sabino Mullane`
## [为什么 SELECT * FROM Table 不仅仅是一个“读取”操作](https://postgresweekly.com/link/159631/web)
从表中选择所有内容肯定是一个可以安全负载平衡的读取操作吗？别急，Hans 举了一个反例。


`Hans-Jürgen Schönig`

📄 [使用 pgvector 和 JavaScript 实现过滤语义搜索](https://postgresweekly.com/link/159632/web) - Team Timescale

📄 [撰写一份好的演讲提案](https://postgresweekly.com/link/159633/web) – 来自一位为 Postgres 活动撰写过大量提案的人 - Tomas Vondra

📄 [如何获取有关系统表之间关系的信息](https://postgresweekly.com/link/159634/web) - Pavel Stěhule


### 🛠 代码和工具

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ce19jlksglrpqd99jo4h.jpg)

## [PG Back Web 0.3：带有 Web 界面的 Postgres 备份系统](https://postgresweekly.com/link/159635/web)
一款基于 Go 的应用程序，为 Postgres 备份以及计划备份、备份监控和 webhook 带来更友好的用户界面。它也可以作为 Docker 映像使用。


`Luis Eduardo `


📰 分类广告
* [Redgate Software](https://postgresweekly.com/link/159636/web) 正在研究 Postgres 用户如何使用数据库工具。[请完成我们的简短调查以分享您的观点](https://postgresweekly.com/link/159636/web)。

* [Dragonfly（25k GitHub 星）](https://postgresweekly.com/link/159637/web) 是现代 Redis 替代品。改用 Dragonfly 的组织可以看到 25 倍的性能提升。

* 今年 11 月，PASS 数据社区峰会和西雅图 Postgres 会议宣布建立新的 [PostgreSQL 合作伙伴关系](https://postgresweekly.com/link/159638/web)。


## [pgcopydb 0.17：将 Postgres 数据库复制到目标 Postgres 服务器](https://postgresweekly.com/link/159639/web)
自动化并提供在两个正在运行的 Postgres 服务器之间运行 pg_dump | pg_restore 的一些结构。


`Dimitri Fontaine`
## [PL/Haskell 4.0：在您的 SQL 函数中使用 Haskell](https://postgresweekly.com/link/159640/web)
Haskell 是一种函数式语言，但是您仍然可以使用它以 Postgres 可以使用的方式定义过程。


`Edward F. Behn, Jr.`


[PLV8 3.2.3](https://postgresweekly.com/link/159641/web) – 在 Postgres 中使用 V8 JavaScript 引擎。此版本升级引入了对 Postgres 17 的支持。

[pgrx 0.12.3](https://postgresweekly.com/link/159642/web) – 一种使用 Rust 构建 Postgres 扩展的方法。现在支持 Postgres 17 RC1。

[pgxmock 4.3](https://postgresweekly.com/link/159643/web) – 模拟驱动程序，用于在 Go 中测试数据库交互。

[ruby-pg 1.5.8](https://postgresweekly.com/link/159644/web) – Ruby 的 Postgres 客户端库