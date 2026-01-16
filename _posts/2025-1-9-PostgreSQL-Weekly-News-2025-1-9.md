---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-1-9
---
### PostgreSQL每周新闻#583 - 2025年1月9日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/583)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/jeyrzliod836uatrt6rp.jpg)
## [PIG:Postgres的新包管理器](https://postgresweekly.com/link/164055/web)
Postgres Install Genius是一个新的包管理器，旨在使数百个Postgres扩展更容易在基于Linux的主流Postgres安装上启动和运行。它来自Pigsty团队，但不需要使用他们专门的Postgres发行版。请注意，这只是各种类似努力中的一项，不是正式的解决方案。

`Pigsty`

## [如何修复Postgres中查询速度慢的常见原因](https://postgresweekly.com/link/164059/web)
Render云平台的一位数据库工程师展示了一个常见但修复得很简单的性能问题，该问题是由外键上缺少索引引起的。


`Eric Fritz `
## [POSETTE 2025：征求建议书（CFP）现已开放！](https://postgresweekly.com/link/164054/web)
博客：由微软Postgres团队组织的免费虚拟开发者活动Postgres活动将于6月10日至12日举行。CFP开放至2月9日。鼓励新的和有经验的演讲者提交！获取详细信息。


`Microsoft `

### 本周摘要：

* 🎧 Hydra的首席执行官和MotherDuck的一名工程师在Postgres FM播客上讨论了pg_duckdb，以及将duckdb引入Postgres的好处。

* Crunchy Data的Elizabeth Christensen反思了“向量”一词的无数用法，尤其是在数据库领域。

* 🇺🇸 PGDay Chicago将于今年4月25日举行，其CFP开放至1月20日，如果你想发言的话。

* ⚡ Abhishek Chanda着眼于如何衡量Postgres查询的功耗。

## [Postgres 18将获得后端级统计数据](https://postgresweekly.com/link/164065/web)
除非出现任何不可预见的问题，否则PostgreSQL 18（可能在2025年底发布）将获得一些改进的后端统计数据，包括一个新的pg_stat_Get_Backend_io函数，用于查看每个服务器后端的I/O活动。


`Bertrand Drouvot `


* 📄 [Postgres容器的挑战](https://postgresweekly.com/link/164066/web)——“结合优秀的Kubernetes运营商，Postgres集装箱如今已准备好投入生产。” - Jeremy Schneider

* 📄 [使用 Procedure 和异步 Web Query Queue - pg_cron](https://postgresweekly.com/link/164067/web) - Paul Ramsey

* 📄 [等待Postgres 18：添加UUID版本7生成函数](https://postgresweekly.com/link/164068/web) - Hubert depesz Lubaczewski

* 📄 [为什么我们放弃etcd，转而使用Postgres来存储元数据](https://postgresweekly.com/link/164069/web) - RisingWave Labs

* 📄 [为什么我的查询没有从分区修剪中受益？](https://postgresweekly.com/link/164070/web) - Shane Borden

* 📄 [如何判断上运行的Postgres端口](https://postgresweekly.com/link/164071/web) - Semab Tariq


### 代码和工具：

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/wzyrlqjeiover3nktqpo.jpg)



## [PostgreSQL Anonymizer 2.0：Postgres的数据掩码](https://postgresweekly.com/link/164072/web)
这个扩展程序不是简单地匿名转储，而是通过让你直接针对你的模式声明掩码规则，直接对你的数据库进行匿名化。2.0版本是使用Rust和PGRX的完全重写，具有改进的虚假数据生成、基于角色的透明动态掩码、使用pg_dump的匿名导出等功能。

`Dalibo`

## [pgspot 0.9：发现Postgres扩展脚本中的漏洞](https://postgresweekly.com/link/164075/web)
由Timescale工程师创建，用于查找TimescaleDB中的漏洞，这是一个SQL脚本分析工具，用于检查漏洞和最佳实践。v0.9将其升级到Postgres 17解析器并修复了一些错误。

`Sven Klemm (Timescale)`

## [SQLite Foreign Data Wrapper for Postgres v2.5](https://postgresweekly.com/link/164076/web)
需要Linux或POSIX兼容系统，但现在支持Postgres 17以及一些额外的数据类型，如uuid、bit和varbit。

`PGSpider`

## [Sqitch 1.5：数据库变更管理工具](https://postgresweekly.com/link/164077/web)
一个独立于数据库和框架（支持Postgres 8.4+）的系统，用于通过SQL脚本管理数据库和模式变更。以下是它与Postgres的工作原理。

`Sqitch`

[libpqxx 7.10.0](https://postgresweekly.com/link/164079/web) – 面向Postgres的官方C++客户端API的一个值得注意的发行版。

[River 0.15](https://postgresweekly.com/link/164080/web) - 快速可靠的Postgres为Go提供后台作业。

[pgxmock 4.4](https://postgresweekly.com/link/164081/web) – 模拟驱动程序，用于测试Go中的Postgres交互。

[Postgres NIO 1.23.0](https://postgresweekly.com/link/164082/web) - Swift的非阻塞、事件驱动客户端。

[Bytebase 3.2](https://postgresweekly.com/link/164083/web) – 团队数据库开发和CI/CD系统。

[pg_timetable 5.10.0](https://postgresweekly.com/link/164084/web) – 高级调度扩展。

[DoltgreSQL 0.16](https://postgresweekly.com/link/164085/web) – 版本控制的Postgres-a-like。

[Hasql 1.9](https://postgresweekly.com/link/164086/web) – Haskell的高性能Postgres驱动程序。

[pg_partman 5.2.4](https://postgresweekly.com/link/164087/web)