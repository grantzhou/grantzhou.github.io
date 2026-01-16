---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: 数据库每周新闻 2019-6-21
---

## 数据库每周新闻 #259 - 2019年6月21日
![config.yml]({{ site.baseurl }}/images/DBWeekly.png)
备注：[英文原文地址](https://dbweekly.com/issues/259)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/ueqppzrncljvnkuxrgwu.jpg)

## [谷歌发布了“Private Join and Compute”，以改善多方计算体验](https://security.googleblog.com/2019/06/helping-organizations-do-more-without-collecting-more-data.html)
如果两个用户都有一个数据集合，Private Join and Compute为他们提供了一种在不影响任何数据的情况下私下计算共同记录的相关值总和的方法。

`GOOGLE`

## [我们如何在零停机的情况下将数据库迁移到Amazon Aurora](https://www.revenuecat.com/2019/06/19/aurora-migration-zero-downtime)
SaaS公司的CTO分享了从Amazon RDS迁移到Aurora（Amazon的高性能数据库系统，可以将自己呈现为Postgres或MySQL兼容）的故事。避免停机是关键，他们设法做到了。

`MIGUEL CARRANZA (REVENUECAT)`

## [编写高效可维护的SQL的建议](https://github.com/mattm/sql-style-guide)

也被称为Matt Mazur的SQL风格指南，这是一个潜在的有用的关于部署SQL的强烈意见和最佳实践的来源。（只是我更喜欢所有大写的SQL格式吗…）

`MATT MAZUR` 

## [studio 3t使SQL迁移到mongodb变得非常简单](https://studio3t.com/knowledge-base/articles/import-sql-database-to-mongodb/?utm_source=cooper&utm_medium=newsletter&utm_campaign=june13)
现在，您可以使用Studio3T及其新的SQL迁移功能将整个SQL数据库导入MongoDB。

`STUDIO 3T`

## [你可能认识的人：LinkedIn如何根据海量数据快速提出社交建议](https://www.infoq.com/presentations/recommendation-massive-data/)
LinkedIn有一个“你可能认识的人”系统，用于将人们联系在一起。本文将深入探讨它在数据级如何工作的实用性。

`INFOQ`

## [一个Redis实例的速度有多快？](https://docs.keydb.dev/blog/2019/06/17/blog-post/)

keydb是redis数据结构存储的一个多线程分支，它的开发人员试图演示其扩展方法可以带来的性能提升。

`EQ ALPHA`



## [时间刻度揭示时间刻度云：托管时间序列数据库服务](https://blog.timescale.com/timescale-cloud-first-fully-managed-time-series-database-service-runs-on-aws-gcp-azure/)

TimescaleDB是一个开源的Postgres扩展，用于大规模处理时间序列数据，现在它也是第一个托管的多云时间序列数据库系统的一部分。

`JEFF SPOSETTI AND AJAY KULKARNI`



## [bigcache 2.0：一个千兆数据的高效缓存](https://github.com/allegro/bigcache)

一个并发的内存中的高速缓存，内置Go。如果您想将HTTP服务器包作为服务提供，也可以使用它。

`ALLEGRO TECH`



**简介**

- MapR的未来最近一直悬而未决，他表示，[出售这家公司的交易已经接近尾声](https://www.datanami.com/2019/06/18/mapr-says-its-close-to-deal-to-sell-company/)。
- 想快速回顾一下存储在凹口卡上的[计算机前数据库吗](https://hackaday.com/2019/06/18/before-computers-notched-card-databases/)？

- 谁不喜欢一个大承诺？[惠普正在保证其新的高端存储阵列100%的可靠性](https://www.datanami.com/2019/06/18/hpe-guarantees-100-uptime-with-primera-storage/)。



### 💻招聘
[招聘有求知欲的负责的开发者](https://www.keyvalues.com/carbon-five)--个人技术水平遇到瓶颈？新项目、技术和挑战与善良、支持和优秀的人完美结合。
`CARBON FIVE`

[在Vettery上寻找数据库有关的工作](https://www.vettery.com/tech?utm_source=newsletter&utm_medium=cooper-dbweekly&utm_term=tech&utm_content=grouped&utm_campaign=ad-88878) – Vettery专门为科技领域的求职者提供相关工作并完全免费。
`VETTERY`

### 📒 教程和故事

[重新思考数据库物化视图作为索引](https://blog.timescale.com/rethinking-the-database-materialized-view-as-an-index/) -- 通过利用时间序列数据的属性，我们能使物化视图的维护足够有效，使它们像索引一样工作吗？

`MATVEY ARYE`

[无损压缩的最低限度指南](https://tech.marksblogg.com/minimalist-guide-compression.html) -- 无损压缩的简要历史，然后简要介绍它在Hadoop场景中的使用。

`MARK LITWINTSCHIK`



[在5分钟内启动GoCD连续传送服务器](https://www.gocd.org/test-drive-gocd.html?utm_campaign=gocd_test_drive&utm_medium=email&utm_source=cooperpress_db&utm_content=go_website&utm_term=)-- 使用新的gocd试驾，了解如何使用一流的管道、可视化等解决您的CI/CD挑战。

`GOCD`



[SQL线性插值](https://bytefish.de/blog/postgresql_interpolation/) -- 如果您有一个缺少值的按时间顺序排列的数据集，那么您可以做些什么。如何找到差距，然后如何尝试填补这些差距？

`PHILIPP WAGNER`



[OLTP和OLAP：它们之间有什么区别？](https://www.imaginarycloud.com/blog/oltp-vs-olap/)--如果您对这些术语感到困惑，本文将使其保持简单。

`TIAGO FRANCO`



[为企业带来可扩展的实时分析]( https://www.oreilly.com/ideas/bringing-scalable-real-time-analytics-to-the-enterprise)--一次35分钟的播客访谈，采访了Rockset公司的两名员工，Rockset是一家致力于低延迟大数据分析的公司。

`O'REILLY DATA SHOW`