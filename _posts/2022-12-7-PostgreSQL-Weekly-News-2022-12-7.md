---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-12-7
---
### PostgreSQL每周新闻#485 - 2022年12月7日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/484)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/qoqb9smpem7n1pk6fqzc.jpg)
## [Amazon's Trusted Language Extensions for Postgres](https://postgresweekly.com/link/132635/web)
Amazon 的 Aurora 和 RDS Postgres 平台都运行着大约 85 个流行的 Postgres 扩展，但除此之外你就不走运了。考虑到扩展的强大功能，Amazon 不希望用户任意安装扩展，因此提出了一种围绕 RDS 或 Aurora 等平台可以满意pg_tle的权限模型构建安全扩展的解决方案这个想法能否在 Postgres 领域更普遍地流行起来？我们将会看到


`CHANNY YUN (AWS)`
## [Amazon RDS 上更快、更便宜的 Postgres](https://postgresweekly.com/link/132634/web)
了解如何在 RDS 上运行 Postgres 时显着提高查询性能并降低成本。PolyScale 是一种智能的无服务器数据库缓存，无需编写代码即可在几分钟内连接。


`POLYSCALE.AI`
## [Neon 的无服务器 Postgres 平台现已面向所有人开放](https://postgresweekly.com/link/132637/web)
邀请门消失了！Neon是 Postgres 平台世界的一个有趣的新成员（于 6 月首次亮相），它采用分离存储和计算方法，允许它们提供“无服务器”弹性扩展体验。与面向 MySQL 的PlanetScale 一样，分支也是一个主要功能。一个值得关注。


`NEON`
## [Instacart on Dropping Postgres for Amazon DynamoDB](https://postgresweekly.com/link/132640/web)
这篇文章给人一种奇怪的感觉，但有趣的是在幕后观察了 Instacart从Postgres 到 DynamoDB 的以扩展为动机的转变。工程团队共享架构设计，将每次事务的计费写入次数减少了一半以上。


`JESSICA WACHTEL`
## [选择一个带有权重的随机元素](https://postgresweekly.com/link/132646/web)
假设您需要生成一个充满样本数据的大表，并希望该数据的分布符合某些要求？休伯特有weighted_random适合你的功能。


`HUBERT 'DEPESZ' LUBACZEWSKI `
## [DB Fiddle：一个 SQL 数据库游乐场](https://postgresweekly.com/link/132650/web)
我经常发现这个工具对于测试少量 SQL 很有用，它现在也支持 Postgres 15（除了各种版本的 MySQL 和 SQLite）。


`STATUS200 `
## [pg_stat_monitor 1.1.1：查询性能监控工具](https://postgresweekly.com/link/132651/web)
如果你在 Postgres 15 上运行它时遇到问题，1.1.1 修复了这个问题。


`PERCONA`
## [PostgreSQL 的身份本地基础设施访问？](https://postgresweekly.com/link/132652/web)


`TELEPORT | GOTELEPORT․COM`
## [pg_hint_plan：在执行计划中手动强制决策](https://postgresweekly.com/link/132653/web)
Postgres 15 支持刚刚提交


`NTT OSS CENTER DBMS DEVELOPMENT AND SUPPORT TEAM `


# 💡本周提示


**🗓即将举办的Postgres活动**
