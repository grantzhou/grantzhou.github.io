---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-10-13
---
### PostgreSQL每周新闻#426 - 2021年10月13日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/426)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/o4hdgv48fcfqo5jkxglz.jpg)
## [Google Cloud Spanner 添加与 Postgres 兼容的接口](https://postgresweekly.com/link/114775/web)
Cloud Spanner是一种基于 Google 云的关系数据库服务，拥有无限的可扩展性，现在您可以通过新的 Postgres 接口在更多地方使用它。值得注意的是，Kelsey Hightower在一年前提出，如果 Cloud Spanner 拥有兼容 Postgres 的接口，它就有可能成为“符合 ACID 的数据库中的 Gmail”。嗯，现在有了。


`Justin Makes (Google) `
## [Herding Elephants：从 Notion 分片 Postgres 的经验教训](https://postgresweekly.com/link/114778/web)
Notion 是一种流行的基于云的知识管理系统，它们严重依赖 Postgres。事实上，他们需要从大型 Postgres 单体到更水平分区的方法进行漫长的迁移，以实现扩展。


`Notion `
## [📣收听 10 月 28 日的 Timescale 社区日](https://postgresweekly.com/link/114779/web)
参加直播讲座（充满演示！），主题范围从时间序列数据和 PostgreSQL 技巧到普遍感兴趣的数据库主题。连接与其他社区成员，得到专家的提示，建议和 更多。


`Timescale `
## [如何优化work_mem调整排序操作](https://postgresweekly.com/link/114780/web)
work_mem是一个 Postgres 设置，指定在回退到使用临时文件之前要使用多少内存用于内部排序操作和哈希表。考虑到数据库查询中排序的常见程度以及临时文件的繁重程度，正确设置此设置可以带来一些重大改进。


`Naga Appani (AWS) `
## [Postgres 14 中的多范围类型](https://postgresweekly.com/link/114781/web)
Postgres 14 中的一个新特性是多范围类型，本质上是一组不重叠的范围（例如 1-3和6-8，作为一个单一的概念）。这篇文章展示了它们的（非常）基本用法。


`Leo Hsu and Regina Obe `
## [SHOW TABLES在 Postgres 中：它有什么问题？](https://postgresweekly.com/link/114782/web)
和许多人一样，我在精通 MySQL 之后才开始使用 Postgres，并且SHOW TABLES花了一段时间才弄清楚不使用。当然，Postgres 有自己更高效的方法。


`Pavlo Golub `
## [pspg (Postgres Pager) 5.4.0 发布](https://postgresweekly.com/link/114784/web)
pspg 是我们多年来多次链接的工具。它是一个用于处理来自 Postgres 的表数据的“分页器”工具，但继续添加新功能，这次包括自定义其颜色主题。


`Pavel Stěhule `
## [Psycopg 3.0 发布：Python 的 Postgres 适配器](https://postgresweekly.com/link/114785/web)
早在第 390 期，我们对 Psycopg 的创建者进行了采访，讨论了他对 Psycopg 3（下一代 Python-Postgres 适配器）的目标，该适配器现在以最终形式出现。该文档可能会给你最好的印象，至于为什么要考虑使用它。


`Daniele Varrazzo `
## [使用 Retool 在几分钟内构建内部工具，让可视化编程与真实代码的力量相遇](https://postgresweekly.com/link/114788/web)
l,null,"en


`Retool `
## [pgAdmin 4 v6.0 发布](https://postgresweekly.com/link/114789/web)
流行的基于 Web 的 Postgres 界面得到了重大升级，特别是切换到使用 React 为其前端提供动力。


`pgAdmin Team `
## [pg_partman：分区管理扩展](https://postgresweekly.com/link/114790/web)
提供一种自动创建和维护表分区的方法。


`Crunchy Data `
## [Sequelize 6.7.0：用于 Node.js 的易于使用的多 SQL 方言 ORM](https://postgresweekly.com/link/114791/web)
支持 PG、MySQL、MariaDB、SQLite 和 SQL Server，并且完全基于承诺。


`Sequelize `
# 💡本周提示


**🗓即将举办的Postgres活动**
