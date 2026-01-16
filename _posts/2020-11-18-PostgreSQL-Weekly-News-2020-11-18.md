---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2020-11-18
---
### PostgreSQL每周新闻#382 - 2020年11月18日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/382)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/ultjzazwfrukgaealxsg.jpg)
## [pg_timetable V3发布](https://postgresweekly.com/link/98721/web)
一个cron与PostgreSQL兼容的高级调度程序，现在具有一些新功能，包括改进的调度（例如“每6小时”），禁止shell任务的选项以及可以重复运行的间隔任务。


`Pavlo Golub `
## [在不停机的情况下将大型Heroku Postgres实例迁移到AWS Aurora](https://postgresweekly.com/link/98722/web)
Heroku可以使操作变得容易，但是当您需要扩展，降低成本或要使用AWS生态系统的其他部分时，RDS的灵活性很有吸引力。这里有很多需要处理和享受的地方，因为有很多活动部件。


`Adam McQuistan `
## [Postgres Build 2020-PostgreSQL在线会议[免费]](https://postgresweekly.com/link/98723/web)
收听25项以上有关PostgreSQL最新内容以及PostgreSQL如何帮助企业的演讲。这次会议还将提供健康会议，以促进健康和恢复活力。12月8日至9日加入我们。立即注册。


`EDB `
## [已发布Postgres 13.1、12.5、11.10、10.15、9.6.20和9.5.24](https://postgresweekly.com/link/98724/web)
更新了所有当前维护的Postgres产品线，以解决三个安全漏洞（以及常见的小错误修复）。特别是由于一个问题，促使升级的原因是：允许用户创建非临时对象，然后在超级用户的身份下执行任意SQL函数。


`PostgreSQL News `
## [Citus 9.5扩展Postgres的新功能](https://postgresweekly.com/link/98725/web)
逐步浏览Citus 9.5开源扩展中的所有新功能，该功能可横向扩展Postgres。从Postgres 13支持到undistribute_table的自适应连接管理COPY，等等


`Claire Giordano (Microsoft) `
## [Google Cloud SQL增加了对Postgres 13的支持](https://postgresweekly.com/link/98726/web)
Google的完全托管的Postgres数据库服务现在可以在最新版本上运行


`Google Cloud `
## [在Postgres中执行此操作10次并停止...](https://postgresweekly.com/link/98727/web)
Postgres拥有全文搜索功能已有一段时间了，并且它会不断完善。这篇文章将回顾其历史，并针对从8.3到13的每个主要版本运行基准测试。


`Robert Treat `
## [全文搜索因为PostgreSQL 8.3](https://postgresweekly.com/link/98728/web)
Postgres有过的全文检索功能，一段时间并继续变得更好。


`Tomas Vondra `
## [⚡️改善PostgreSQL插入的13条小窍门](https://postgresweekly.com/link/98729/web)
从优化磁盘性能到使用并行写入+批量插入insert获取我们加快INSERT速度的主要方法🚀


`Timescale `
## [macOS Big Sur可能中断了Postgres的安装](https://postgresweekly.com/link/98730/web)
最新版本的macOS可能会导致现有Postgres安装出现问题。如果适合您，那么此技巧可能会有所帮助。


`Dave Page `
# 💡本周提示


对于使用PostgreSQL JDBC驱动程序的Java开发人员，您可以使用reWriteBatchedInsertsconnection参数显着加快批处理操作。


如果为reWriteBatchedInserts=true，则JDBC驱动程序将以限制对数据库的调用次数的方式将批处理插入重写为多行插入。


例如，驱动程序从以下位置更改批处理插入：


```
insert into foo (col1, col2, col3) values (1,2,3);
insert into foo (col1, col2, col3) values (4,5,6);
```


成：


```
insert into foo (col1, col2, col3) values (1,2,3), (4,5,6);
```


正确使用时，reWriteBatchedInserts可以将批处理插入性能提高2-3倍。如果您想要一个更扩展的示例，Vlad Mihalcea也写了更多有关reWriteBatchedInserts去年的内容。

本周的提示由Cockroach Labs赞助，在此演示中了解有关CockroachDB的信息：“分布式SQL：现代的云原生PostgreSQL。”

**🗓即将举办的Postgres活动**

[CHINA 2020和PGConf.Asia 2020](https://postgresconf.org/conferences/AsiaChina2020)
