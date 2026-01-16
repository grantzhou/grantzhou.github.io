---
layout: post
title: PostgreSQL 每周新闻 2023-11-29
---
### PostgreSQL每周新闻#532 - 2023年11月29日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/532)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ztkesfltdc5sxeuwao9c.jpg)
## [📊 PDF：扩展塑造未来](https://postgresweekly.com/link/148315/web)
一个精彩的幻灯片，专为 2023 年 PASS 数据社区峰会的演讲而制作，它本身就很好地充实了扩展在 Postgres 生态系统中的位置，以及最近的一些发展 空间。


`Ryan Lambert `
## [AWS 预览 Amazon Aurora Limitless 数据库](https://postgresweekly.com/link/148316/web)
在本周的 re:Invent 上，Amazon 宣布预览一项新功能，支持在单个 Aurora PostgreSQL 数据库上自动水平扩展至每秒数百万个写入事务。 因此，不仅您的数据库可以无限，您的 AWS 账单也可以无限。


`Channy Yun (AWS) `
## [使用约束编程自动为 Postgres 选择索引](https://postgresweekly.com/link/148314/web)
选择索引有什么困难？ 在写入开销、热更新影响和更快的查询之间进行权衡。 了解有关新模型的更多信息，该模型基于分层优化和 CP-SAT，可让您控制自动选择索引的方式。

`pganalyze `
## [索引时间戳](https://postgresweekly.com/link/148317/web)
有几种方法可以做到这一点，在粒度和时区方面需要进行各种权衡。


`Bruce Momjian `

**本周摘要：**
*   Microsoft 向 Azure Database for PostgreSQL 引入了 azure_ai 扩展，以向托管在那里的数据库开放 Azure 的各种 AI 服务。


*   AWS Amplify 添加了一项新功能，可以为任何现有 Postgres 数据库创建 GraphQL API，即使是在 AWS 外部托管时也是如此。


*   AWS 的 Jonathan Katz 在使用 HNSW 索引时非常深入地研究了加速 RDS 上基于向量的查询。


## [为什么 DoorDash 从 Aurora Postgres 迁移到 CockroachDB](https://postgresweekly.com/link/148321/web)
您最初会有“案例研究”的感觉，但这篇文章是基于 ▶️ DoorDash 工程师关于迁移过程及其动机的详细技术演讲。


`Charlie Custer (Cockroach Labs) `
## [提高 Postgres 性能并降低云支出](https://postgresweekly.com/link/148323/web)


`EDB Postgres`
## [循环函数和线性级数的乐趣](https://postgresweekly.com/link/148324/web)
Greg 继续他的 Postgres 代码冒险，将 PL/pgSQL 推向其美丽的极限。
```
💡 如果您想和 Greg 一起参加今年的 Advent of Code，活动将于本周五开始！ 不过你不必使用 PL/pgSQL.. 😅
```

`Greg Sabino Mullane `
## [Django 和 Postgres 中的数据库生成列](https://postgresweekly.com/link/148326/web)
Pythonistas 的一个！ 介绍数据库生成列，使用 Postgres 和 Django 5.0 中添加的新生成字段。


`Paolo Melchiorre `
## [Timescale 在 Aurora PostgreSQL Serverless 基准测试中学到了什么](https://postgresweekly.com/link/148327/web)
当供应商进行基准测试时，如果他们推广结果，他们通常会做得很好。 尽管如此，一些结论很难被否认：“Amazon Aurora Serverless 很昂贵。” 😅


`James Blackwood-Sewell (Timescale) `
## [我弄清楚了为什么 pg_dump 在 Postgres 15-16 上失败了](https://postgresweekly.com/link/148328/web)
Postgres v15 及更高版本更改了确定 .pgpass 文件可能所在位置的方法顺序。


`Dan Langille `
## [解锁安全连接：Postgres 身份验证方法指南](https://postgresweekly.com/link/148329/web)


`SEMAB TARIQ`
## [▶ 在 Postgres 中取消数组的嵌套](https://postgresweekly.com/link/148330/web)


`CODING WITH MISSAK`

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/vy8j2u2qlglahrpw2jug.jpg)

## [TimescaleDB 2.13.0：Postgres 的时间序列扩展](https://postgresweekly.com/link/148331/web)
Timescale 作为一个业务和托管平台越来越为人所知，但其产品的核心仍然是开源扩展。 v2.13.0 引入了完整的 Postgres 16 支持，但不再发布 AMI 映像 - 这也是包含多节点支持的最终版本。


`Timescale `
## [PgHero 3.4：Postgres 的性能仪表板](https://postgresweekly.com/link/148333/web)
用 Ruby 构建的仪表板（并在 Instacart 中使用），可让您查看基本的性能统计数据，包括实时查询、维护状态和连接。 v3.4 添加了对解释 Postgres 16 中规范化查询的支持，以及适用于 linux/arm64 的 Docker 映像。


`Andrew Kane `
## [pgAdmin 4 v8.0](https://postgresweekly.com/link/148334/web)
领先的 Postgres 图形管理工具。


## [pg_auto_failover 2.1](https://postgresweekly.com/link/148335/web)
监视和管理 Postgres 集群中的自动故障转移。 现在支持 Postgres 16。

## [postgres_exporter 0.15.0](https://postgresweekly.com/link/148336/web)
服务器指标的 Prometheus 导出器。

## [SQL Formatter 14.0](https://postgresweekly.com/link/148337/web)
用于漂亮打印 SQL 查询的 JavaScript 库。

## [pgBadger 12.3](https://postgresweekly.com/link/148338/web)
快速 Postgres 日志分析器。