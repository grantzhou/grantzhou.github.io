---
layout: post
title: PostgreSQL 每周新闻 2021-9-15
---
### PostgreSQL每周新闻#422 - 2021年9月15日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/422)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/pslzvoamdiae0nmrbgow.jpg)
## [2021年Postgres GUI 综述](https://postgresweekly.com/link/113637/web)
2020 年的一篇文章，针对 2021 年进行了一些更新，涵盖了一些常见的数据库客户端，如 pgAdmin、Navicat、DBeaver、HeidiSQL、Datagrip 等。


`Angel D'az (Retool) `
## [Boundless TEXT再次回来](https://postgresweekly.com/link/113638/web)
使用 Postgres，VARCHAR(n)列和无限列之间没有性能差异TEXT，但是如果您想限制长度呢？Brandur 分享了来自 Stripe 的一个稍微混乱的故事，关于如果没有限制会发生什么，以及他目前使用的基本原理VARCHAR。


`Brandur Leach `
## [Postgres 聚合如何启发我们的超函数设计](https://postgresweekly.com/link/113639/web)
我们的工程师分解了 PostgreSQL 聚合的工作原理，它如何启发了 TimescaleDB 的超函数的设计，以及它如何与连续聚合和其他高级功能交互——并附有示例和图片。🚀


`Timescale `
## [针对 PostgreSQL 社区的商标诉讼](https://postgresweekly.com/link/113640/web)
如果跨境商标纠纷不是你的事，请继续——长话短说，Postgres 核心团队和社区协会管理着 Postgres 的商标（以及我们从谁那里获得了本时事通讯名称的许可） ) 在名称的使用上与Fundación PostgreSQL发生冲突。如果你想看到故事的另一面， Fundación PostgreSQL 的Álvaro Hernández有更多.. 标题强烈的“Postgres 核心团队对 Postgres 社区发起前所未有的攻击”。


`PostgreSQL News `
## [在批量加载之前还是之后创建索引？](https://postgresweekly.com/link/113642/web)
在大量数据摄取之前或之后创建索引是否重要？Hans-Jürgen 执行他的特征基准之一来找出答案。（简而言之：after 更快，但它可能不适合您的工作流程。）


`Hans-Jürgen Schönig `
## [使用JQ获取“PGBACKREST”的信息](https://postgresweekly.com/link/113643/web)
pgBackRest是一种流行的备份和恢复工具，它可以在JSON格式返回它的输出，因此非常适合与更受欢迎解析JQ JSON命令行处理器。


`Luca Ferrari `
## [我们如何sqlc/pgx全力支持Go 中的Postgres](https://postgresweekly.com/link/113646/web)
sqlc从 SQL 查询文件生成 Go，它提供了许多与 ORM 相同的好处，而没有一些缺点。不过，这不是一个适合所有场景的尺寸，这在很大程度上是一个偏好问题。


`Brandur Leach `
## [使用 Retool 在几分钟内构建内部工具，让可视化编程与真实代码的力量相遇](https://postgresweekly.com/link/113648/web)
l,null,"en


`Retool `
## [AWS RDS 和 Aurora 的不同 Postgres 版本的发布日期](https://postgresweekly.com/link/113649/web)
我不确定这有多大用处，但我喜欢它的呈现方式:-)


`Brian Likes Postgres `
## [Bun 1.0：用于 Go 的简单且高性能的数据库客户端库](https://postgresweekly.com/link/113650/web)
支持 Postgres、MySQL 和 SQLite，Bun 是面向 Go 开发人员的现代 SQL 优先数据库客户端库，具有内置迁移和夹具支持。为什么不改用 GORM、Ent 或 go-pg？他们对这个问题有一些答案。


`Vladimir Mihailenco `
## [PostGIS 3.2.0 Alpha 1 发布](https://postgresweekly.com/link/113652/web)
即将发布的 PostGIS 3.2.0 的第一个预览版本在这里，目标是 Postgres 14 beta 3。


`Regina Obe `
# 💡本周提示


**🗓即将举办的Postgres活动**
