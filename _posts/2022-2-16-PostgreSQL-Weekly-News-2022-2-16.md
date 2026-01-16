---
layout: post
title: PostgreSQL 每周新闻 2022-2-16
---
### PostgreSQL每周新闻#442 - 2022年2月16日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/442)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/xsnnlqxgrvhnhq7ka7ne.jpg)
## [一个毛茸茸的 Postgres 事件](https://postgresweekly.com/link/119771/web)
⭐️一个团队在他们的一个地区升级到 Postgres 11，他们的应用程序开始遇到“问题”。作者以相当重要的方式进行了救援。这是一个关于解决问题的奇妙故事，也是一个看似简单的问题可以变得多么复杂的例子。


`Jeremy Schneider `
## [PostgreSQL 14.2、13.6、12.10、11.15 和 10.20 已发布](https://postgresweekly.com/link/119772/web)
更新所有维护的 Postgres 版本，以修复过去几个月报告的超过 55 个错误，涵盖从索引损坏和崩溃到内存泄漏和查询计划程序等领域。


`PostgreSQL Global Development Group `
## [CYBERTEC MIGRATOR - 从 Oracle 到 Postgres 的最简单方式](https://postgresweekly.com/link/119773/web)
如果您的公司被锁定在昂贵的 Oracle 许可证中，您可以通过迁移到 PostgreSQL 来节省成本。您可能想知道，“我怎样才能以最高的安全性和最短的停机时间迁移我们的数据库？” CYBERTEC MIGRATOR 就是答案。


`CYBERTEC `
## [新手的Postgres限制](https://postgresweekly.com/link/119774/web)
一些可以在 Postgres 中放置的各种类型约束的快速解释和示例，包括外键、唯一性、空性、排除和检查约束。还有一个方便的（如果很大的话）查询来找出数据库中已经存在的约束。


`Elizabeth Christensen `
## [TOAST 压缩和toast_tuple_target](https://postgresweekly.com/link/119775/web)
如果表中有行存储大量数据，Postgres 将依靠一种称为 TOAST 的机制将额外数据存储在单独的位置并引用原始表中的数据。这样做的一个好处是 Postgres 可以压缩这些数据，并且您可以自定义发生这种情况的阈值。


`Adrien Nayrat `
## [Postgres 中更安全的应用程序用户](https://postgresweekly.com/link/119776/web)
更改应用程序用户权限的指南，以便他们无法删除您的生产数据库，例如。


`Mike Palmiotto `
## [使用较小的整数可以节省多少磁盘空间？](https://postgresweekly.com/link/119777/web)
挑选用于表示整数的几个字节对我来说感觉太详细了，但在规模上也许它会有所作为？事实证明，不，不是真的，使其工作所需的计划和订购量与任何收益都不成比例。


`Hubert depesz Lubaczewski `
## [Studio 3T 管理您的数据，同时让您的应用程序成形](https://postgresweekly.com/link/119778/web)
l,null,"en


`Studio 3T `
# 💡本周提示


**🗓即将举办的Postgres活动**
