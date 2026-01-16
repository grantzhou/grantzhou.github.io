---
layout: post
title: PostgreSQL 每周新闻 2023-5-10
---
### PostgreSQL每周新闻#505 - 2023年5月10日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/505)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,w_430,h_100/e_make_transparent/co_white,e_outline:7/xyflkz7n00elwtgja9ne.png)
## [Citus Con 2023会谈](https://postgresweekly.com/link/139379/web)
▶微软最近举行了他们的第二届年度虚拟 Postgres 会议，虽然我还没有时间观看其中的许多内容（所以请留意接下来几期的更直接的建议），但还有很多内容享受 YouTube 上现在提供的 37 个演讲。


`Citus Con 2023 `
## [如何在Postgres中强制执行联接顺序](https://postgresweekly.com/link/139380/web)
尽管 Postgres 没有固有的“查询提示”功能（这就是原因），但在某些情况下连接表时仍然可以强制查询优化器使用特定的连接顺序。


`Laurenz Albe `
## [Postgres能做到吗？](https://postgresweekly.com/link/139378/web)
 答案通常是肯定的。仅仅 Postgres 就可以做很多事情。不是“Postgres”兼容的模仿，实际的 Postgres。想要一个可以帮助您的供应商吗？我们是来帮忙的。


`Crunchy Data `
## [如何使用pg_stat_statements跟踪性能差异](https://postgresweekly.com/link/139382/web)
如何使用古老的pg_stat_statements 模块跟踪配置更改对特定工作负载的影响。


`Ryan Lambert `
## [使用Amazon SageMaker和pgvector构建人工智能搜索](https://postgresweekly.com/link/139390/web)
正如 AI 领域现在大肆宣传一样，有一些有趣的方法可以利用最近的发展，包括在 Postgres 中。使用复杂的向量和嵌入作为执行相似性搜索的方法现在相当简单。在这种情况下，AWS 占据中心位置，SageMaker 提供嵌入。


`Krishna Sarabu (AWS) `
## [使用时间点恢复的各种恢复技术](https://postgresweekly.com/link/139392/web)
这不是你想做的事情，但值得运行这个过程，以防有一天你需要它。


`Tristen Raab `
## [如何通过电子邮件提交补丁，2023版](https://postgresweekly.com/link/139393/web)
14 年前类似帖子 的更新，但符合现代“现在我们使用”的标准。git


`Peter Eisentraut `
## [优化Postgres查询性能的最佳实践（电子书）](https://postgresweekly.com/link/139395/web)


`pganalyze `
## [让我们聚会，一起升级Postgres和PostGIS](https://postgresweekly.com/link/139396/web)
Florian 的聚会想法与我的有点不同，但尽管如此，这是将 Postgres 13 + PostGIS 2.5.5 升级到 15/3.3.2 的一种方法。


`Florian Nadler `
## [使用DOMAIN规则验证数据列](https://postgresweekly.com/link/139397/web)
域是一种具有可选约束的数据类型。


`Francesco Tisiot `
## [在两个端口上运行Postgres？](https://postgresweekly.com/link/139399/web)
不要。或者，如果必须的话，使用第三方工具。


`Christophe Pettus `
## [Citus 11.3针对多租户SaaS工作负载的新增功能](https://postgresweekly.com/link/139400/web)
Citus是一种将分布式表添加到 Postgres 的良好方式。一个常见的用例是使用由租户分发的表构建多租户应用程序。Citus 11.3 引入了租户监控功能，可以在可配置的时间段内查看每个租户的查询计数和 CPU 使用情况。


`Marco Slot (Citus Data) `
## [HeidiSQL 12.5:用于数据库工作的本机Windows应用程序](https://postgresweekly.com/link/139402/web)
如果您使用的是 Windows，HeidiSQL 是一款方便的开源数据库管理工具。支持 Postgres、MySQL、SQL Server 和 SQLite。用 Delphi 编写并且是开源的。


`Ansgar Becker `
# 💡本周提示


**🗓即将举办的Postgres活动**
