---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-1-24
---
### PostgreSQL每周新闻#539 - 2024年1月24日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/539)
![img](https://res.cloudinary.com/cpress/image/upload/w_1920,e_sharpen:60,q_auto/e9xvgoqdrvbiofjz2n8v.jpg)
## [一个 PID 锁定全部：查找锁定源](https://postgresweekly.com/link/150356/web)
一个进程可以锁定您的数据库，从而阻止其他进程和查询执行其工作。 如何找到哪个进程？ 杰西深入并分享了一些有用的问题。


`Jesse Soyland `
## [▶ Jonathan Katz 谈论 pgvector](https://postgresweekly.com/link/150357/web)
Postgres 核心团队成员 Jonathan Katz 与主持人 Michael Christofides 一起在 Postgres.fm 播客上谈论日益流行的 pgvector 扩展、其用例、索引方法以及 TOAST 如何参与其中。


`Postgres FM `
## [电子书：调整 Autovacuum 以获得最佳 Postgres 性能](https://postgresweekly.com/link/150355/web)
了解调整调度和性能设置、减少工作时间的 autovacuum 开销、xmin 范围及其阻止真空、为什么要避免反环绕真空以及如何通过调整死元组来减少膨胀。


`pganalyze `

**本周摘要：**

*   Tembo 聘请了 PGXN 创建者 David Wheeler 来负责 Postgres 扩展的发现和分发。


*   PostgreSQL 项目现在是 CVE 编号机构 (CNA)，这意味着它可以直接为其范围内的漏洞颁发 CVE ID。


*   🎧 Marco Slot 和 Jelte Fennema 在 Path to Citus Con 播客（.. Path to POSETTE？😁）上谈论 Postgres 背景下的性能基准测试，包括使用的最佳工具和技术。


*   📊 Pavlo Golub 引入了一个新的 Grafana 仪表板，用于监控 pg_timetable 作业。


*   Hans-Jürgen Schönig 反思了他的 PGConf EU 2023 主题演讲，以及在信任如何存储数据时开源的重要性。


## [POSETTE：2024 年 Citus Con 更名](https://postgresweekly.com/link/150367/web)
微软已经举办虚拟 Citus Con 活动两年了，但到 2024 年，它更名为 POSETTE（代表不太悦耳的“Postgres 开源生态系统对话培训和教育”）。 时间为 6 月 11 日至 12 日，如果您想发言，CFP 将开放。


`Microsoft `
## [🍕 如何使用 SUBSTRING](https://postgresweekly.com/link/150369/web)
在本例中，字符串切片和切块......还有一点披萨。


`Francesco Tisiot `
## [为什么 Postgres RDS 不适合我们](https://postgresweekly.com/link/150370/web)


`MAX KREMER`

**📰 机密:**

[赶上 PostgreSQL 101 系列](https://postgresweekly.com/link/150372/web) - 可供点播观看，该系列涵盖了 PostgreSQL 新用户的一系列关键主题。


**代码和工具**


## [Apache AGE 1.5rc：Postgres 的图形扩展](https://postgresweekly.com/link/150374/web)
AGE 为 Postgres 提供图形数据库功能（通过 openCypher），并受到 AgensGraph 的启发。 v1.5 现在处于候选版本阶段，添加了 Postgres 16 支持，同时进行了一些小的增强。


`Apache Foundation `
## [Postgres 的“功能相当齐全”的 Ansible 角色](https://postgresweekly.com/link/150380/web)
Ansible 2.4+ 角色，可安装和配置 Postgres 12 及以上扩展以及扩展，还可以设置数据库和用户。 Postgres 16 支持本周登陆。


`ANXS `
## [pgmoneta：Postgres 的备份/恢复解决方案](https://postgresweekly.com/link/150382/web)
pgmoneta 以前是 Red Hat 项目，但现在独立，是一个完整的数据库备份和恢复工具包，支持加密、压缩、保留策略、Prometheus 等。


`The pgmoneta Community `
## [supa_audit：Postgres 通用表审计](https://postgresweekly.com/link/150386/web)
一种通用解决方案，通过将历史记录存储在单独的审计表中来跟踪表数据随时间的变化。


`Supabase `
## [oracle_fdw：Oracle 数据库的外部数据包装器](https://postgresweekly.com/link/150388/web)
提供对 Oracle 数据库的高效访问，包括 WHERE 条件和所需列的下推以及全面的 EXPLAIN 支持。


`Laurenz Albe `
## [Reshape 0.7：零停机架构迁移工具](https://postgresweekly.com/link/150390/web)
在迁移过程中，Reshape 可确保新旧架构同时可用，从而允许您逐步推出应用程序。


`Fabian Lindfors `
## [PLV8 3.2.2](https://postgresweekly.com/link/150392/web)
将 JavaScript 用于 Postgres 过程。


## [ScalikeJDBC 4.2](https://postgresweekly.com/link/150394/web)
Scala 的数据库客户端库。

