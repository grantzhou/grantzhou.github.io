---
layout: post
title: PostgreSQL 每周新闻 2023-8-2
---
### PostgreSQL每周新闻#517 - 2023年8月2日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/517)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/xxvuotgyql1uiv57oukr.jpg)
## [PostgreSQL 2023调查现已开放](https://postgresweekly.com/link/143311/web)
从 2019 年开始，Timescale 的年度 Postgres 调查已成为监测更广泛社区感受的流行方式。如果您好奇的话，这是去年的结果。除了共享结果外，Timescale 还提供原始（匿名）数据供第三方分析。


`Timescale `
## [查看Postgres锁定冲突的一种方式](https://postgresweekly.com/link/143313/web)
🔓虽然 Postgres 有两种广泛的锁类型（共享锁和独占锁），但存在不同级别的粒度，不同的命令通过其锁定要求相互影响或冲突。该工具显示所有锁定类型以及它们如何与不同命令交互。


`Hussein Nasser `
## [介绍Pastgres新的 pganalyze VACUUM Advisor](https://postgresweekly.com/link/143310/web)
pganalyze VACUUM Advisor 为每个表提供 autovacuum 设置建议，以优化表膨胀、冻结、VACUUM 性能等。实施其建议以优化空间使用、防止膨胀并提高查询性能。


`pganalyze `
## [表分区简介](https://postgresweekly.com/link/143314/web)
Postgres 支持三种形式的表分区，其中表可以分为多个分区，以获得各种性能、维护或后勤优势。这篇文章提供了三种分区类型的一些基本示例。


`Matteo Crosta `
**本周摘要：**
*   Craig Kerstiens 在Real Python播客上▶️ 讨论如何将 Postgres 与 Python 结合使用。


*   🐦一个有趣的 Twitter 帖子，介绍 PlanetScale、它对 MySQL 的使用，以及为什么很难将 PlanetScale 的 Postgres 等价物整合到一起。PlanetScale 的首席执行官在该帖子中指出： “在 Postgres 的 Vitess 出现之前（至少十年后），为 Postgres 设计 PlanetScale 几乎是不可能的。”


*   在科技界引发争论的最快方法是……运行一些基准测试！Perfect Makanju对AWS，Digitalocean和Google Cloud上的Postgres进行了基准测试，结果相当不同。


*   很少有读者会需要这个，但是看到流行的开发者 YouTuber在 100 秒内处理 ▶️ PostgreSQL 中的 Postgres 真是太棒了。也许是一个视频，当人们问你一整天都在做什么时，可以参考这个视频;-)


*   最新的PGSQL Phriday博客挑战的主题是撰写有关分区与分片的文章。


*   如果您使用 Vercel Edge Functions，现在只需更新软件包，即可在使用 Vercel Postgres 时显着提高性能。@vercel/postgres


## [比较批量加载技术的性能](https://postgresweekly.com/link/143323/web)
快速比较将数据快速批量插入表中的基本方法，无论是通过单个事务还是多个事务，无论是使用INSERTs 还是COPY. 毫不奇怪，COPY速度最快，专为任务而设计，但您可以INSERT以一种意味着它不会落后太远的方式使用。


`Laurenz Albe `
## [澄清事实：商标纠纷的更多更新](https://postgresweekly.com/link/143324/web)
PostgreSQL 社区协会 (PGCA) 和PostgreSQL 基金会目前陷入与 Postgres 相关的欧盟商标纠纷中。这是 PGCA 的看法，但为了平衡，你也可以看看Fundación PostgreSQL 的 Álvaro Hernández 的想法。


`PostgreSQL Community Association `
## [在 PL/PgSQL 中实现 Shift 函数的一种可能方法](https://postgresweekly.com/link/143326/web)
“Shift”意味着一个接受数组并删除并返回第一个/最左边元素的函数。


`Luca Ferrari `
## [PL/PgSQL 简单罗马数字转换器](https://postgresweekly.com/link/143327/web)
更多PL/PGSQL恶作剧。


`Luca Ferrari `
## [PLJS：Postgres的JavaScript语言插件](https://postgresweekly.com/link/143328/web)
PLV8可以说是在 Postgres 中使用 JavaScript 作为过程语言的“首选”方式，但是这个来自同一创建者的基于QuickJS的变体更紧凑，更易于维护，并且可能足以满足您的需求。


`Jerry Sievert `


`Adab Biranimal`
## [“Rusting”一个新的Postgres C扩展名来计算子译用](https://postgresweekly.com/link/143332/web)
子事务或嵌套事务是在另一个事务中开始的事务，虽然有用，但存在性能影响。pg_subxact_counters是用C 和 Rust编写的新扩展，用于对此类子事务进行计数，并且它对于比较两种语言中扩展的实现也很有用。


`Bertrand Drouvot `
## [pgAdmin 4 v7.5](https://postgresweekly.com/link/143335/web)
↳流行的GUI Postgres管理工具。


`Prisma 5.1`
↳ Node.js and TypeScript ORM.


`FerretDB 1.7`
↳想象一下，如果 MongoDB 运行在 Postgres 之上......


`SQLC 1.20`
↳在 Go 中从 SQL 生成类型安全代码。


`PGModeler 1.0.5`
↳开源数据建模工具。


# 💡本周提示


**🗓即将举办的Postgres活动**
