---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-9-25
---
### PostgreSQL每周新闻#617 - 2025年9月25日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/617)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/iosout28y26yrnqummvo.jpg)
## [Postgres 18 发布](https://postgresweekly.com/link/174773/web)
Postgres 的最新主要版本如期发布。它并非 Postgres 史上最大的进步之一，但却包含许多显著的改进，可以提升资料库的效能。以下是一些新功能：

* 引进[非同步 I/O 子系统](https://postgresweekly.com/link/174740/web)，实现更有效率的扫描、清理等功能。
* 支援 [UUIDv7](https://postgresweekly.com/link/174741/web)，并新增[多项功能](https://postgresweekly.com/link/174742/web)。
* [UPDATE...RETURING](https://postgresweekly.com/link/174743/web)功能显著改善。
* [支援并行应用大型事务](https://postgresweekly.com/link/174744/web)。
* [OAuth 2.0 授权和身份验证](https://postgresweekly.com/link/174745/web)。

💡 如果您想要所有新功能的完整列表，[发行说明](https://postgresweekly.com/link/174746/web)提供了详尽的要点演练。

## [首期专为产品工程师打造的简报](https://postgresweekly.com/link/174737/web)
《产品工程师》是 PostHog 的简报，致力于帮助工程师提升产品技能。它涵盖了工程师在建立 PostHog 流程中的经验、对顶级新创公司的研究，以及打造优秀产品的精选建议。

`PostHog   `

## [PlanetScale for Postgres 现已正式发布](https://postgresweekly.com/link/174747/web)
今年 7 月，以 MySQL 服务闻名的云端资料库平台 PlanetScale 宣布将进军 PG 领域，并分享了一系列基准测试，以展示其解决方案与其他同类产品相比的优势。此前，该服务一直处于「私人预览」阶段，现已向所有人开放。

`Sam Lambert`

💡 值得注意的是，[Hacker News 上对此消息的评论非常积极](https://postgresweekly.com/link/174749/web)，许多早期用户都对这项服务表示称赞。


### **本周摘要**

* 伊丽莎白·克里斯滕森 (Elizabeth Christensen) 查阅了 [1986 年 Postgres 的原始设计目标论文](https://postgresweekly.com/link/174750/web)，并得出[结论：“PostgreSQL 的创建者完全做到了这一点](https://postgresweekly.com/link/174751/web)。”

* IEEE 发布了 [2025 年顶级程式语言榜单](https://postgresweekly.com/link/174752/web)，SQL 位列第四。

* 本·迪肯 (Ben Dicken) [制作了一个可视化的进程和线程解释器](https://postgresweekly.com/link/174753/web)，对 Postgres 和 MySQL 的方法进行了比较。

* Red Gate 正在进行其[最新的资料库现况调查。更多资讯请点击此处](https://postgresweekly.com/link/174754/web)。


## [Postgres 18 中非同步 I/O (AIO) 的调优](https://postgresweekly.com/link/174756/web)
Postgres 18 最引人注目的变化之一是引入了非同步 I/O（又称 AIO，您可以点击此处了解更多资讯）。 Tomas 将介绍引入的新配置设置，这些设置会影响 AIO 的工作方式和扩展方式。


`Tomas Vondra`

📄 [Redis 速度很快 - 我会用 Postgres 做cache](https://postgresweekly.com/link/174758/web) – 比较 Postgres 和 Redis 的基本快取任务。 Redis 速度更快，但不一定快到值得运行第二个系统，这取决于您的设定。 Viktoras Kuznecovas

📄 [一周只写文件](https://postgresweekly.com/link/174759/web) – PgDog Postgres 连接池和分片器的创建者真的非常重视文件。 Lev Kokotov

📄 [Postgres 分区最佳实践](https://postgresweekly.com/link/174761/web)：Sofia 的故事 Karen Jex

📄 [理解 WAL 并使用专用磁碟对其进行最佳化](https://postgresweekly.com/link/174762/web) Warda Bibi


## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/c2401vxr0z16de9mqvp2.jpg)

## [pgschema：Postgres 的声明式模式迁移](https://postgresweekly.com/link/174763/web)
想像一下类似 Terraform 的东西，但将宣告式模式迁移工作流程引入 Postgres。它提供了许多功能，并支援许多高级功能——GitHub 仓库。

`Tianzhou et al.`

## [pgAudit 18.0：稽核日志扩展](https://postgresweekly.com/link/174766/web)
Postgres 18 支援此扩展，用于产生可能需要遵守政府、财务或 ISO 认证的稽核日志。

`PostgreSQL Global Development Group`

## [pgexporter 0.7：适用于 Postgres 的 Prometheus 导出器](https://postgresweekly.com/link/174767/web)
现已改善核心指标，包括新增的 autovacuum 指标，并新增对 PostGIS、pg_stat_statements、pgvector 和 Timescale 等多个扩充功能的支援。主页。

`pgexporter community`


[DoltgreSQL 0.52](https://postgresweekly.com/link/174769/web) – 类似 Postgres 的版本控制，具有类似 Git 的功能。

[BemiDB 1.6](https://postgresweekly.com/link/174770/web) – 针对分析最佳化的单二进位 Postgres 唯读副本。

[pgFormatter 5.8](https://postgresweekly.com/link/174771/web) – SQL 程式码格式化程式和美化器。

[pgenv 1.4.3](https://postgresweekly.com/link/174772/web) – Postgres 二进位档案管理器。