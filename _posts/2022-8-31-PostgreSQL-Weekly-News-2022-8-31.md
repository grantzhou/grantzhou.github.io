---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-8-31
---
### PostgreSQL每周新闻#469 - 2022年8月31日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/469)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/zyauj12kmafhsls6apmh.jpg)
## [Postgres 15 中的 Stats Collector 去了哪里？](https://postgresweekly.com/link/128034/web)
Postgres 的统计收集器密切关注表或索引被扫描的次数、何时发生清理等。这些信息通常存储在临时文件中，但 Postgres 15 已经转向更直接的基于内存的方法——幸运的是， 任何监视 pg_stat_* 视图的东西都将继续按原样工作。

`Jobin Augustine `
## [Postgres 15 中的“public schema”更改](https://postgresweekly.com/link/128036/web)
Andreas 解释了默认情况下如何不再为 public schema 设置 CREATE 权限，以及在您最终的 v14 到 v15 升级期间如何重新抬头。 他总结道：“最好不要依赖可写的public schema。” 更多讨论（从 2020 年开始）在这里。


`Andreas Scherbaum `
## [让您的 Postgres 数据更靠近用户](https://postgresweekly.com/link/128035/web)
PolyScale 自动在边缘缓存 Postgres，使数据驱动的应用程序速度极快。 无需编写代码即可在几分钟内部署它。 通过我们的 Playgroun


`PolyScale.ai `
## [Cloudflare 开源其 PgBouncer 分支](https://postgresweekly.com/link/128038/web)
Cloudflare 一直在维护 PgBouncer（连接池）的内部分支，其中包含身份验证错误修复以及围绕每个用户和连接池隔离的新功能。 现在是公开的。


`Justin Kwan (Cloudflare) `
## [AALTER TABLE ... ADD COLUMN 正确用法](https://postgresweekly.com/link/128047/web)
在生产环境中向表中添加列无疑是一种令人毛骨悚然的体验。Hans-Jürgen 很快就了解了其中的含义。


`Hans-Jürgen Schönig `
## [▶ 如何成为一名 DBA](https://postgresweekly.com/link/128048/web)
初级和高级数据库管理角色所涉及的各种任务、期望和角色是什么？ 迈克尔和尼古拉讨论。


`Postgres FM Podcast podcast`
## [Postgres 15 如何改进逻辑复制中的通信](https://postgresweekly.com/link/128064/web)
你们中很少有人需要知道这一点，但简而言之：WAL 发送者和接收者之间的通信变得更加高效和健壮，因此复制变得稍微快一些。 👍


`Wei Wang `
## [使用 Flyway 和 AWS Lambda 在 Aurora 上自动化架构版本控制和迁移](https://postgresweekly.com/link/128049/web)
Flyway 是一种基于 Java 的版本驱动架构管理工具，支持（大多数）SQL 数据库，并且可以与一些 AWS Lambda 无服务器函数一起设置以部署 SQL 脚本 定期进入 Aurora Postgres 环境。


`Gohil and Lonappan (AWS) `
## [PostGIS 3.3.0 发布：地理空间扩展](https://postgresweekly.com/link/128051/web)
PostGIS 正领先中，最适合与 Postgres 15（仍处于测试阶段）一起使用，但也适用于 11 及更高版本。 NEWS 文件涵盖了相对较小的改进。


`Regina Obe (PostGIS) `
## [您一直想要的 Postgres 开发人员体验](https://postgresweekly.com/link/128100/web)


`Crunchy Bridge `
## [pgagroal 1.5.0：高性能协议原生连接池](https://postgresweekly.com/link/128065/web)
添加了日志格式和轮换支持等。 还有一些新教程，包括这个“入门”指南。


`Red Hat `
