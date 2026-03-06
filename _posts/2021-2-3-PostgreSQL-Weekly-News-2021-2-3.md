---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-2-3
---
### PostgreSQL每周新闻#391 - 2021年2月3日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/391)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/wusf4vkgx3c1m1ctfnks.jpg)
## [意外发现释放了20GB未使用索引空间](https://postgresweekly.com/link/102307/web)
有趣（并且相当彻底）的研究了释放空间而不删除索引或删除数据的方法，包括清理未使用的索引占用的空间，尤其是替换了包含大量数字的索引 具有部分索引的空值。 这篇文有很多有趣的东西！


`Haki Benita `
## [Amazon Aurora现在支持Postgres 12](https://postgresweekly.com/link/102308/web)
是的，是的，最新版本是Postgres 13，但是Aurora并不是完全标准的Postgres服务，并且Aurora团队必须重新实现新的Postgres功能，因为它不是纯粹Postgres。 在相关新闻中，您现在也可以“就地”将Aurora数据库从Postgres 11升级到12。


`Amazon Web Services `
## [对云进行基准测试：AWS vs. GCP vs. Azure](https://postgresweekly.com/link/102310/web)
AWS通常“赢得”云报告。 今年他们没有。 了解每个云的当前性能，它们的权衡因素以及哪些机器测试得很好（或不好），以便为服务选择最佳的云配置。


`Cockroach Labs `
## [使用pg_stat_replication监视复制](https://postgresweekly.com/link/102311/web)
如果使用复制，则必须确保正确监视的集群。 一种方法是使用pg_stat_replication。


`Hans-Jürgen Schönig `
## [pg_timetable 3.2的异步链执行](https://postgresweekly.com/link/102312/web)
pg_timetable是Postgres的高级作业调度程序，我们之前已经介绍过几次。 这篇文章深入探讨了最新版本对作业执行的额外控制。


`Pavlo Golub `
## [如何完全卸载和重新安装基于Homebrew的Postgres](https://postgresweekly.com/link/102314/web)
Postgres是否出错并显示“无法读取块39”或“错误地址”？ 如果您是在Mac上通过Homebrew安装Postgres的，则这篇文是是解决的最快方法


`Justin Searls `
## [如何创建自定义Postgres构建和Debian软件包](https://postgresweekly.com/link/102315/web)
幸运的是，如果您只想要最受欢迎的发行版的最新软件包，则永远不需要这样做，但是如果您确实需要构建自己的软件包，则Ibrar的经验可能会有用。


`Ibrar Ahmed `
## [Fauna - Postgres的所有优点，没有操作瓶颈](https://postgresweekly.com/link/102472/web)
Fauna将Postgres的安全性与架构灵活性，现代功能和无限规模结合在一起。 [了解更多...](https://postgresweekly.com/link/102472/web)


`Fauna `
## [即将出版的Postgres查询优化书的预审](https://postgresweekly.com/link/102317/web)
即将出版的Postgres查询优化书的预审-“ Postgres查询优化：构建有效查询的终极指南”是一本将于3月出版的新书，Tom作为其技术审阅者之一，对此非常热情。 图书上市后，我们将为您提供更多相关信息。


`Tom Kincaid (EDB) `

## [使用`psql`元命令快速记录您的Postgres数据库](https://postgresweekly.com/link/102318/web)

`MARK LANE`
## [使用适用于PostgreSQL的Azure数据库构建应用的最佳实践](https://postgresweekly.com/link/102319/web)

`SUNITHA MUTHUKRISHNA (MICROSOFT)`
## [如何在Linux Mint 20上使用pgAdmin4安装PostgreSQL](https://postgresweekly.com/link/102320/web)

`WINNIE ONDARA`

## 🔧工具和代码

## [pgAdmin 4 v4.30发布](https://postgresweekly.com/link/102321/web)
pgAdmin是Postgres的流行开源管理系统，此最新版本添加了新的ERD（实体关系图）工具，以最直观的方式布置架构以及Kerberos支持。


`PostgreSQL News `
## [Logidze 1.0：基于Ruby on Rails的Postgres支持的数据审核](https://postgresweekly.com/link/102323/web)
Logidze通过Postgres触发器和JSONB跟踪对Active Record管理的表所做的更改。 它自豪地声称是“ Rails生态系统中审核模型最快的gem”。


`Vladimir Dementyev `
## [pg-anonymizer：Postgres的匿名数据转储](https://postgresweekly.com/link/102324/web)
一种由Node.js支持的工具，用于匿名导出数据库。 敏感数据将替换为等效类型的伪造数据。


`Raphaël Huchet `

## [deno-postgres 0.5.0：Deno的PostgreSQL驱动程序](https://postgresweekly.com/link/102325/web)

`DENO DRIVERS`