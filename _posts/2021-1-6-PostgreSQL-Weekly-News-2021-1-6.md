---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-1-6
---
### PostgreSQL每周新闻#387 - 2021年1月6日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/387)
![img](https://res.cloudinary.com/cpress/image/upload/e_grayscale,w_150,h_170,c_pad,g_south/xrupigpv8kyjqotfdgy8.jpg)
## [闲置的Postgres连接对性能的影响](https://postgresweekly.com/link/100711/web)
与Postgres数据库的连接即使处于空闲状态也要消耗资源，因此本帖子深入探讨了原因以及一些基准测试。 如果需要减少连接数，请考虑使用Pgpool-II，PgBouncer或RDS代理（如果适用）之类的连接池工具。


`Yaser Raja `
## [Postgres是DB-Engines的“2020年度DBMS”](https://postgresweekly.com/link/100715/web)
DB-Engines是受欢迎的DBMS知识库，并且根据受欢迎程度的增长，每年都有“年度DBMS”。 Postgres曾经赢过，但在2020年从MySQL夺回了冠军。


`Paul Andlinger and Matthias Gelbmann `
## [PostgreSQL的安全最佳实践](https://postgresweekly.com/link/100717/web)
这是一个框架和一系列的数据库安全建议，用于保护PostgreSQL数据库。 点击下载白皮书。


`EDB `
## [“PostgreSQL”的Shibboleth](https://postgresweekly.com/link/100718/web)
shibboleth是一种习俗或传统（可以像一个单词的发音一样简单），可以将一个群体与另一个群体区分开– PostgreSQL？还是Postgres One？


`Laurenz Albe `
## [不再担心Rails迁移中的Postgres锁定](https://postgresweekly.com/link/100719/web)
迁移数据库时最常见的陷阱，以及在Doctolib上如何减轻它们。


`Thomas Hareau `
## [将数据加载到PostGIS中：概述](https://postgresweekly.com/link/100720/web)
当您需要处理地理空间对象和数据时，PostGIS是Postgres的流行插件。 这里是一些用于将此类数据加载到PostGIS支持的数据库中的工具。


`Kat Batuigas `
## [使用Amazon Aurora PostgreSQL查询计划管理在版本升级后确保一致的性能](https://postgresweekly.com/link/100721/web)
如果您使用的是Aurora或对它们在工具方面的工作很感兴趣，则仅需要阅读此内容。 查询计划管理（QPM）是Aurora比较和监视查询计划（例如在整个升级过程中）的功能，如此处所示。


`Lanre Showunmi (AWS) `
## [将查询结果从psql重定向到LibreOffice Calc](https://postgresweekly.com/link/100723/web)
假设您已经在psql中获得了查询结果，并且希望将其放入电子表格（在这种情况下为LibreOffice Calc）–这是一种（Linux风格）的做法。


`Pavel Stěhule `
## [Postgres 13基准测试：内存速度与TPS](https://postgresweekly.com/link/100724/web)
在计算机上运行2133MHz vs 3200MHz RAM这样简单的事情会影响Postgres基准测试吗？ 结果当然不如您所想！

#### 🔧工具和代码

`Greg Smith `
## [Postgres-deno：Deno Postgres扩展](https://postgresweekly.com/link/100725/web)
在Postgres函数和触发器中运行TypeScript。 仍然是概念上的证明，但是一个简洁的主意，是plv8的替代品。


`Supabase `
## [多合一以及自动的网站和数据库备份](https://postgresweekly.com/link/100726/web)
在2分钟内从待办事务列表中删除备份。 自动执行所有服务器和数据库备份，并将它们存储在所需的位置。


`SimpleBackups `
## [Database Lab Engine 2.1：适用于开发环境的大型Postgres数据库的即时克隆](https://postgresweekly.com/link/100727/web)
在几秒钟内为独立的非生产环境提供数TB的Postgres数据库，而无需支付额外费用。


`Postgres.ai `
## [ActiveRecordExtended：向Ruby和Rails Apps添加扩展的Postgres功能](https://postgresweekly.com/link/100728/web)
在以前流行的postgres_ext库上完成的工作的延续。 这将对ANY，ALL和一些JSON和HSTORE运算符的支持添加到Active Record中，Active Record是一种正流行的基于Ruby的ORM，在Rails应用程序中著名。


`George Protacio-Karaszi `
## [不支持的PostgreSQL版本的RPM存储库](https://postgresweekly.com/link/100734/web)
如果出于某种原因，如果您使用不支持的PostgreSQL版本或Red Hat / CentOS / Scientific Linux / Oracle Linux版本，并且需要这些版本的RPM，我们将为它们提供存档。”


`Devrim Gunduz `
## [pgHoard 2.2：Postgres备份和还原工具](https://postgresweekly.com/link/100731/web)


`Aiven `
## [pgagroal 1.1.0：高性能Postgres连接池](https://postgresweekly.com/link/100732/web)


`Red Hat Inc. `

