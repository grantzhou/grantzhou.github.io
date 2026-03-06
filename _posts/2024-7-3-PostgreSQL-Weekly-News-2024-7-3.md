---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-7-3
---
### PostgreSQL每周新闻#556 - 2024年7月3日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/560)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/xhtzylhdtbjhlgly9xga.jpg)
## [PostgreSQL 17 Beta 2 发布](https://postgresweekly.com/link/157053/web)
Beta 1 发布一个月后，Postgres 17 的最终版本即将发布，距离发布还有很长的路要走，预计今年 9 月或 10 月。草稿版本说明仍然是了解最新动态的最佳方式。

`POSTGRESQL GLOBAL DEVELOPMENT GROUP `

## [构建和扩展 Notion 的数据湖](https://postgresweekly.com/link/157056/web)
Notion 是一款流行的基于 Web 的笔记和 Wiki 应用程序，因此，它控制着大量数据。从纯粹基于 Postgres 的方法开始（他们在此处撰写了有关扩展的文章），他们已经取得了长足的发展，并且必须与许多其他技术集成才能采用数据湖方法。


`TIE, LOUIE, CHOW, ET AL. (NOTION) `
## [优化 PostgreSQL：基本调优策略](https://postgresweekly.com/link/157052/web)
从 Percona 专家支持工程师那里了解经过验证的 PostgreSQL 性能调优策略。免费电子书包含实际示例和有关查询优化、索引、分区、架构设计等方面的建议。立即获取您的副本。


`PERCONA  `
## [查看 Postgres 17 中的新内置排序规则提供程序](https://postgresweekly.com/link/157059/web)
Postgres 17 beta 版中有一个内置的 UTF-8 语言环境和排序规则提供程序，带有二进制字符串比较功能。下面介绍它为什么有趣、如何使用它以及它的性能。


`DANIEL VÉRITÉ  `
## [PGExtensions：跨云扩展支持的比较](https://postgresweekly.com/link/157059/web)
在您自己的 Postgres 服务器上运行扩展是一回事，但是当涉及到使用托管的 Postgres 服务或云提供商时，您通常会受到提供商所提供内容的限制。


`DATACLOUDGAZE CONSULTING `

### 本周摘要：

🇬🇷 [PGConf.EU 2024 的注册已开放](https://postgresweekly.com/link/157061/web)。它将于今年 10 月在希腊举行，如果我没记错的话，截至本文发布时，只剩下三张早鸟票。

Postgres 平台 [Tembo.io](https://postgresweekly.com/link/157062/web) 宣布已[筹集 1400 万美元资金](https://postgresweekly.com/link/157063/web)。

[EDB 的 Dilip Kumar](https://postgresweekly.com/link/157064/web) 是本周的 PostgreSQL 人物。

📄 在 Hyperdrive 中[支持 Postgres 命名准备语句](https://postgresweekly.com/link/157065/web) – Hyperdrive 是 Cloudflare 的全球分布式 SQL 连接池和缓存 - ANDREW REPP (CLOUDFLARE)

📄 [使用 SELECT FOR UPDATE 确保安全的数据修改](https://postgresweekly.com/link/157066/web) -  SEMAB TARIQ

📄 [使用事务链减少服务器往返](https://postgresweekly.com/link/157067/web) - CHRISTOPH SCHIESSL

📄 [Kubernetes 刚满十岁：Postgres 处于什么位置？](https://postgresweekly.com/link/157068/web) - GABRIELE BARTOLINI

📄 [使用短寿命 Postgres 服务器进行测试](https://postgresweekly.com/link/157069/web) - ROBIN KÅVELAND

📄 [生产 Postgres 中的 ORM：朋友还是敌人？](https://postgresweekly.com/link/157070/web) - TIMESCALE



### 🛠 代码和工具

## [Psycopg 3.2 发布](https://postgresweekly.com/link/157071/web)
Psycopg 是 Python 最受欢迎的 Postgres 适配器。（顺便说一句，我们在[第 390 期](https://postgresweekly.com/link/157072/web)采访了 Psycopg 的创建者 — 三年前！ — 当时他已经开始开发 Psycopg 3。）


`DANIELE VARRAZZO `

## [pg_dirtyread：从关系中读取已死但未清理的元组](https://postgresweekly.com/link/157073/web)
因此，如果某一行已被删除，您仍然可以读取它。

`CHRISTOPH BERG `

## [pg_back 2.4：一个简单、全面的 Postgres 备份工具](https://postgresweekly.com/link/157074/web)
一个由 Go 提供支持的工具，用于以您选择的格式将您的数据库转储到文件（包括角色、服务器参数等）。


`NICOLAS THAUVIN `


[pgAdmin4 8.9](https://postgresweekly.com/link/157075/web) – 流行的 Postgres 管理仪表板。

[Hasql 1.8](https://postgresweekly.com/link/157076/web) – 高效的 Haskell Postgres 驱动程序，具有类型安全映射 API。

[postgres-meta 0.83.1](https://postgresweekly.com/link/157077/web) – 用于管理 Postgres 的 RESTful API。

[FerretDB 1.22](https://postgresweekly.com/link/157078/web) – 与 MongoDB 类似，但基于 Postgres 。

