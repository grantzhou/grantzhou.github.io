---
layout: post
title: PostgreSQL 每周新闻 2023-6-21
---
### PostgreSQL每周新闻#511 - 2023年6月21日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/511)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_380,h_100/e_make_transparent/co_white,e_outline:7/dm8pbpm4svdu3ggeoyqk.png)
## [🥇 Postgres：最受欢迎、最需要和最受推崇的数据库](https://postgresweekly.com/link/141281/web)
🥇Postgres 在 Stack Overflow 的最新开发人员调查中表现出色，成为最“受推崇和最喜爱”的数据库。 MySQL、SQLite、MongoDB 和 Redis 排在第二位。 在流行度方面，Postgres 也首次登上榜首，将 MySQL 推到第二位。


`Stack Overflow `
## [使用prepared statement使 Postgres 快 30%？](https://postgresweekly.com/link/141283/web)
prepared statement比临时查询更快，因为它们已经被解析、计划并准备好执行。 PgCat Postgres pooler 现在支持prepared statement，因此更容易利用。


`Lev Kokotov (PostgresML) `
## [[清单] 每天零到 100 次部署](https://postgresweekly.com/link/141280/web)
没有足够的时间阅读电子书来学习如何更快地部署？ 这是一个快速的里程碑清单，可指导您完成这些步骤，因此您可以从每周部署一次到每天部署 100 次。


`Sleuth `
## [Postgres 重新考虑其基于进程的模型（再次）](https://postgresweekly.com/link/141287/web)
上周，我们重点介绍了关于将 Postgres 从其基于进程的模型转变为基于线程的模型的邮件列表讨论，但这篇 LWN 帖子将这个故事整合到一篇文章中。


`Jonathan Corbet `
## [Postgres 文档和社区的局限性](https://postgresweekly.com/link/141294/web)
当谈到文档时，这是最好的时代，也是最坏的时代，建议 Postgres 的主要贡献者。 虽然该项目的核心是一个强大的文档流程（补丁也需要更新文档），但这些文档有一种混乱的参考手册感觉，并且在整体、任务驱动的意义上并不那么强大。


`Robert Haas `
## [Native Enum 或 CHECK 约束？](https://postgresweekly.com/link/141295/web)
查看使用native enum或 CHECK 约束来强制数据正确性之间的选择，每个的优缺点，以及作者为什么选择 CHECK 约束。


`João Sampaio `
## [Postgres 中的数据倾斜](https://postgresweekly.com/link/141296/web)
倾斜或不均匀的数据很常见，但它会影响索引的工作情况。 这篇文章包括在您自己的数据库中查找此类数据示例的查询，以及对索引问题的部分修复。


`Elizabeth Christensen (CrunchyData) `
## [使用 Postgres 进行快速分析的五个技巧](https://postgresweekly.com/link/141298/web)


`Hydra `
## [Postgres 谜题带来更多乐趣](https://postgresweekly.com/link/141297/web)
今天可能是夏至（在北半球），但 Greg 仍然专注于 2022 年的 Advent of Code 挑战并在 Postgres 中解决它们。 这篇文章深入探讨了第 17 天，其中包含许多您一定会学到一些东西的点点滴滴。


`Greg Mullane (CrunchyData) `
## [UUID 密钥的意外缺点](https://postgresweekly.com/link/141299/web)
如果您想独立于数据库生成密钥或在不发生冲突的情况下在数据库之间混合记录，UUID 会很方便，但默认情况下它们缺乏时间局部性。 不过，顺序 UUID 在 Postgres 的未来计划有被考虑到。


`Ants Aasma `
## [在 Kubernetes 上部署 Pgpool 作为负载均衡器](https://postgresweekly.com/link/141300/web)


`Cary Huang`
## [pgMagic：使用自然语言与 Postgres 聊天](https://postgresweekly.com/link/141301/web)
来自独立开发人员的新 macOS Postgres 客户端（付费，但有试用版）可以使用 OpenAI 生成和执行针对您的数据库的查询。 有一些这样的实验，这里的介绍很好。


`Tom Hill `
## [pg_easy_replicate：以最少的停机时间切换数据库](https://postgresweekly.com/link/141302/web)
一个基于 Ruby 的编排器，用于简化在两个 Postgres 数据库之间设置逻辑复制的任务，然后让您以最少的停机时间切换到较新的数据库。


`Shayon Mukherjee `
## [FerretDB v1.4.0：感觉像 MongoDB，使用 Postgres 进行存储](https://postgresweekly.com/link/141303/web)
为了应对 MongoDB 许可模型的混乱而创建，FerretDB 旨在与 MongoDB 兼容，但本质上充当后端 Postgres 的代理。 它可能会吸引那些需要维护基于 MongoDB 的应用程序但厌倦了在生产中运行 MongoDB 的人。


`Alexander Fashakin `

