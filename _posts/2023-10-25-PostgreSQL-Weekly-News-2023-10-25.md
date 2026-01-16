---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-10-25
---
### PostgreSQL每周新闻#527 - 2023年10月25日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/527)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/j8vxxgc7so046ubvmylp.jpg)
## [介绍 pg_timetable v5.6](https://postgresweekly.com/link/146807/web)
pg_timetable ([GitHub 存储库](https://postgresweekly.com/link/146808/web)) 是一个强大的 Postgres 独立作业调度程序。 v5.6 添加了延迟异步启动任务链的功能。


`Pavlo Golub `
## [Citus 的分布式 Postgres 新技术自述文件](https://postgresweekly.com/link/146809/web)
Microsoft 的 Citus 团队制作了一份 Citus 技术自述文件，深入探讨了 Citus 如何将 Postgres 转换为分布式数据库的技术细节，详细介绍了底层机制和优化 — 这些细节对其他 Postgres 扩展的开发人员可能会很有价值。


`Onder Kalaci (Microsoft) `
## [在任何云上运行 Postgres DBaaS 的灵活性和强大功能。从 300 美元的积分开始免费](https://postgresweekly.com/link/146806/web)
利用现在具有高可用性和分布式功能的完全托管 Postgres 加快创新 — 可以在需要时随时联系顶级 Postgres 专家。


`EDB BIgAnimal `
## [Postgres 中的版本数据：测试类似 git 的方法](https://postgresweekly.com/link/146811/web)
Sam 探索了一种在 Postgres 中手动建模 git 式数据版本控制的方法。 然而，这是一个足够常见的要求，如果您需要的话，有很多开箱即用的解决方案，包括 Neon 的分支功能等解决方案、temporal_tables、Postgres.ai 等扩展或 PL/pgSQL- 基于时态表的方法。


`Samuel Bodin`

**本周摘要：**
*   Amazon 显然不想错过所有这些新的 LLM 和 RAG 相关工作负载，因此 Amazon Aurora 现在支持带有 HNSW 索引的 pgvector v0.5.0。 更多关于这意味着什么在这里。


*   在 Aurora 的其他新闻中，Aurora 现在支持 Postgres 15.4、14.9、13.12、12.16 和 11.21。


*   最后，关于 Amazon Postgres 的消息，pgactive（RDS 的主动-主动复制扩展）现已全面推出。 这是有关其使用的教程。


*   当经验丰富但很少接触 Postgres 的人进入 Postgres 世界并分享他们的观察结果时，这总是很有趣的，VC Zain Rizavi 就做到了这一点。 这是对空间的合理的高层分析。


*   📅 2023 年欧洲 PostgreSQL 会议日程已发布。 会议于今年 12 月在布拉格举行，Simon Riggs 发表了题为“PostgreSQL 的下一个 20 年”的开幕主题演讲。


## [PgBouncer 事务模式下的 PREPARE 语句](https://postgresweekly.com/link/146823/web)
上周，我们提到 PgBouncer 现在支持 PREPARE 语句。 这篇文章进一步深入探讨，详细分析了 PREPARE STATEMENT 的性能收益以及它们传统上构成挑战的原因。


`Greg Sabino Mullane `
## [如何使用 Psycopg2：Python 的 Postgres 适配器](https://postgresweekly.com/link/146825/web)
在重点介绍长期存在且非常流行的 psycopg2 之前，快速回顾一些最流行的 Python Postgres 库。 （值得记住的是，psycopg3 也提供了 asyncio 支持。）


`Anber Arif (Tailscale) `
## [简单的查询优化：避免顺序扫描](https://postgresweekly.com/link/146828/web)
“优化 Postgres 查询可能看起来很复杂，让我们把它变得简单。”


`Jason Zucchetto `

## [Postgres 101 网络研讨会 – 针对 Postgres 新用户的一系列关键主题](https://postgresweekly.com/link/146829/web)

`Redgate`
## [您不需要专用的缓存服务：使用 Postgres 作为缓存](https://postgresweekly.com/link/146831/web)

`MARTIN HEINZ`
## [在多区域集群中部署适用于 Kubernetes 的 Crunchy Postgres](https://postgresweekly.com/link/146830/web)

`BOB PACHECO (CRUNCHY DATA)`
## [Postgres 中的高 CPU 使用率：如何检测和修复它](https://postgresweekly.com/link/146832/web)

`CHARLIE CUSTER (COCKROACH LABS)`

**代码和工具：**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ozyuvbmyyotf5qdr3wmw.jpg)

## [pglift：大规模部署 Postgres 的新方法](https://postgresweekly.com/link/146833/web)
pglift 是一个 CLI 工具和 Ansible 集合，用于部署生产就绪的 Postgres 集群，并提供用于备份和监控的可选辅助服务。


`DALIBO `
## [对 Postgres 数据进行匿名 dump](https://postgresweekly.com/link/146835/web)
这种方法不是在生产数据库中安装扩展，而是在本地数据库中创建副本，然后使用其中的 PostgreSQL Anonymizer。


`Steven Miller `
## [FerretDB 1.13](https://postgresweekly.com/link/146837/web)
 - 使用 Postgres 进行存储的 MongoDB 替代方案。 （现在还有一个在线 FerretDB 游乐场可供使用。）

## [Pigsty 2.5](https://postgresweekly.com/link/146839/web)
 - 类似于 RDS 的开源 Postgres 发行版，捆绑了许多扩展。 现在使用 Postgres 16 并支持 Ubuntu/Debian。

## [Piccolo 1.0](https://postgresweekly.com/link/146840/web)
 - 用户友好的 Python ORM 和查询生成器。

## [pgAdmin 4 v7.8](https://postgresweekly.com/link/146841/web)
 - 流行的基于 Web 的 Postgres 管理工具。

## [pg_cron 1.6.2](https://postgresweekly.com/link/146842/web)
 - 运行定期作业。 比 pg_timetable 更简单。

## [Prisma 5.5](https://postgresweekly.com/link/146843/web)
 - 适用于 Node.js 和 TypeScript 的下一代 ORM。

## [sqlc 1.23](https://postgresweekly.com/link/146844/web)
 - 从 SQL 生成类型安全的 Go 代码。

## [pg-parquet-py](https://postgresweekly.com/link/146845/web)
 - 将 Postgres 数据写入 Parquet 的 Python 脚本。
