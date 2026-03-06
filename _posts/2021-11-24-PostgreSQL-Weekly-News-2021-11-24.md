---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-11-24
---
### PostgreSQL每周新闻#432 - 2021年11月24日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/432)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/yxosxwkiuidkr8ilup3j.jpg)
## [Postgres 中的实体-属性-值 (EAV) 设计以及为什么不这样做](https://postgresweekly.com/link/116665/web)
EAV 提供了一种获得关键价值灵活性的方法，可以动态地向对象添加属性，但以结构化的关系方式适用于任何标准关系数据库。现在我们有了 JSONB，这是一个值得的想法吗？我不这么认为，作者也不这么认为。


`Laurenz Albe `
## [我应该在外键上创建索引吗？](https://postgresweekly.com/link/116666/web)
剧透： “这里的要点是，我们不应该在所有 FK 上不加选择地创建索引，因为其中许多不会被使用或很少使用，以至于不值得付出代价。”


`Charly Batista (Percona) `
## [遇到您会喜欢的唯一错误：CockroachDB Serverless](https://postgresweekly.com/link/116667/web)
弹性扩展并不意味着牺牲一致性或熟悉度。使用世界上最先进的 SQL 数据库 CockroachDB Serverless 获得轻松的扩展、自动化操作和有保证的事务一致性。


`CockroachDB Serverless `
## [是否VARCHAR(n)使用比VARCHAR()或更少的磁盘空间TEXT？](https://postgresweekly.com/link/116668/web)
曾几何时，在某些数据库上，将VARCHAR列限制为特定长度可能具有空间优势，但对于 Postgres 及其 TOAST 系统，情况并非如此。


`Hubert depesz Lubaczewski `
## [Postgres 14 中 JSON 的新功能](https://postgresweekly.com/link/116669/web)
没有巨大的飞跃，但 Postgres 14 提供了一些以下标形式处理 JSON 文档的优点。


`Sarah Chima Atuonwu `
## [在 Django 中使用 Postgres 视图](https://postgresweekly.com/link/116670/web)
Python 和 Django 用户？你会想看看这个。它表明的观点是如何从不同的物化和意见，使用视图如何使查询汇总数据更容易和（与物化视图）更快。


`Josh Alletto `
## [⚡提高 PostgreSQL 插入性能的 13 个技巧](https://postgresweekly.com/link/116671/web)
l,null,"en


`Timescale `
## [将 TimescaleDB 与 PGO Postgres 运算符一起使用](https://postgresweekly.com/link/116672/web)
有兴趣尝试使用用于 Kubernetes 的 Crunchy Postgres 运算符的 TimescaleDB？这是设置它的快速指南。


`Jonathan S. Katz `
## [📊企业 Postgres 在日本的增长](https://postgresweekly.com/link/116673/web)
EDB 的 Bruce Momjian 为日本 PostgreSQL 用户组做了一个关于日本用户如何成为 Postgres 的早期采用者以及日本开发人员如何推动 Postgres 向前发展的演讲。还没有视频。


`Bruce Momjian slidedeck`
## [隔离 Postgresrepmgr](https://postgresweekly.com/link/116674/web)
repmgr用于提升 Postgres 高可用性游戏的高级用例。


`Shaun Thomas `
## [pg_dirtyread：从关系中读取死但未清空的元组](https://postgresweekly.com/link/116675/web)
因此，如果一行已被删除，例如，您可能仍然可以读取它。


`Christoph Berg `
## [Sqitch 1.2：数据库变更管理工具](https://postgresweekly.com/link/116676/web)
一个独立于数据库和框架（支持 Postgres 8.4+）的系统，用于通过 SQL 脚本管理数据库和架构变更。这是它与 Postgres 的工作方式。


`Sqitch `
# 💡本周提示


**🗓即将举办的Postgres活动**
