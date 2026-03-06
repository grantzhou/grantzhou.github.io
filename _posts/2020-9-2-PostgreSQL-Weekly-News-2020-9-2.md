---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2020-9-2
---
### PostgreSQL每周新闻#371 - 2020年9月2日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/371)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/v1599042560/f64vevur9prtzfuy37ey.jpg)

## [postgresql13中可信扩展概述](https://postgresweekly.com/link/94414/web)
Postgres支持扩展，以便于动态引入新的特性和功能，但在Postgres 13中，有一个可信扩展的概念，允许任何在当前数据库上具有创建权限的用户引入一个没有超级用户权限的扩展。

`Nidhi Bansal `

## [为Postgres数据库调整Autovacuum](https://postgresweekly.com/link/94415/web)
大多数情况下，您不需要调整autovacuum的设置，因为Postgres通常会做正确的事情，但是有时默认配置是不够的，本文将帮助您了解一些调优方法。


`Laurenz Albe `
## [关于如何加快Postgres查询的最佳实践。免费电子书](https://postgresweekly.com/link/94425/web)
像Robinhood和Atlassian这样的公司能够以数量级的速度加快查询速度。这本电子书分享了我们优化Postgres性能的最佳实践。


`pganalyze `
## [使用Postgres索引的注意点](https://postgresweekly.com/link/94417/web)
如果你不是一个索引专家，那就值得看一下这个博客。索引可以加快速度，但索引并不总是被使用，即使您认为应该使用索引，而且索引会增加您需要准备好管理的维护和存储开销。

`Kat Batuigas `

## [在postgres13中，增加了并行vacuum的特性](https://postgresweekly.com/link/94418/web)
postgres13中值得注意的新特性之一是能够加快索引清空的执行时间。Masahiko提供了一个快速的好处例子。

`Masahiko Sawada `

## [JSON聚合函数是多么酷](https://postgresweekly.com/link/94419/web)
与其用SQL查询提取数据然后将其转换为JSON，不如让Postgres来完成这项繁重的工作，下面是方法。

`Knut Hühne `

## [Postgres对外部压缩方法的需求](https://postgresweekly.com/link/94420/web)
如果您可以为不同的表或列指定不同的压缩系统，基于最适合存储的数据类型的压缩系统，那将是非常好的。。而且，Postgres团队似乎开始讨论Postgres中的这个潜在特性。


`Amit Khandekar `
## [使用PostgreSQL & TCP代理过滤器收集SQL统计信息](https://postgresweekly.com/link/94421/web)
一个新PostgreSQL过滤器使开发人员和操作工程师能够方便地收集SQL统计信息。

`YugabyteDB `

## [Postgres中的基准检查点](https://postgresweekly.com/link/94422/web)
评估从1GB到100GB的不同日志大小的检查点。


`Vadim Tkachenko `
## [全文搜索大战：Postgres vs Elasticsearch](https://postgresweekly.com/link/94423/web)
少了一场战斗，更多的是用一个简单的基准对技术进行基本的比较，但可能会引起兴趣。


`Rocky Warren `
## [postgres12中逻辑复制的陷阱与怪癖](https://postgresweekly.com/link/94424/web)
“在大型ish（1 TB）生产数据库中设置逻辑复制后，我想分享一些想法。”


`Elephant Tamer `
# 💡本周提示


**🗓即将举办的Postgres活动**
