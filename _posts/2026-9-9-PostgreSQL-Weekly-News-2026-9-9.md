---
layout: post
title: PostgreSQL 每周新闻 2026-9-9
categories: [PostgreSQL]
tags: [PGWeekly]
---
### PostgreSQL每周新闻#664 - 2026年9月9日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/664)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/eqdy9a7btdaispdwx0yl.jpg)

## [*恐怖的* Postgres 19 补丁竞赛](https://www.postgresql.org/message-id/CA%2BTgmob9NY6m0YNFTQ4nFH2d0iC9SQRruDYxfndGKKzh8OC80w%40mail.gmail.com)
虽然还没到万圣节，但在 `pgsql-hackers` 邮件列表的这个引人入胜的讨论串中，Robert Haas 使用 Claude 来*"评估 v19 中最恐怖的补丁"*。其中一个补丁，[SQL/PGQ 属性图](https://www.cybertec-postgresql.com/en/handling-graphs-with-sql-pgq-in-postgresql/)，已经被[从 v19 中移除](https://github.com/postgres/postgres/commit/2b9e1aff4d3d933ae8ee377fef22c2af9c7797e8)，但仍有五个保留下来...

`Robert Haas et al.`

💡 在 `pgsql-hackers` 的另一个讨论串中，还有关于 SQL/PGQ 移除的[更多背景信息](https://www.postgresql.org/message-id/CAAKRu_bEtjWYWhYxSo0o_t3DaZYRQd5PkC0abA0g9Mp4%2BovH0w%40mail.gmail.com)。

## [即将推出：ParadeDB Cloud](https://paradedb.com/cloud)
我们正在构建一个完全托管的 ParadeDB：一个 Postgres 用于应用程序数据、全文搜索、向量检索和聚合。[我们的早期访问候补名单现已开放](https://paradedb.com/cloud)。

`ParadeDB` **赞助商**

### POSTGRES 19：第四个 Beta 版本和一些艰难的选择

原本预计本月晚些时候发布的 Postgres 19，现在其发布日期已[正式待定](https://wiki.postgresql.org/wiki/PostgreSQL_19_Open_Items#Important_Dates)，预计第四个 beta 版本将在 9 月 24 日发布。但[上面的"恐怖补丁"讨论串](https://www.postgresql.org/message-id/CA%2BTgmob9NY6m0YNFTQ4nFH2d0iC9SQRruDYxfndGKKzh8OC80w%40mail.gmail.com)显示，最终将包含哪些内容仍是一个悬而未决的问题：

- [Tom Lane 对 SQL/PGQ *"非常担心"*](https://www.postgresql.org/message-id/646368.1787697184%40sss.pgh.pa.us)，在它被移除的两周前，仍有需要目录更改的修复正在讨论中：*"我敢打赌，如果我们在 v19 中发布它，会有无法修复直到 v20 的发布后错误发现。"*

- [David Rowley 建议](https://www.postgresql.org/message-id/CAApHDvqBudqUpjckbbePwyQnfmCrEOj50pPOXnCR5H5AetAY3Q%40mail.gmail.com)今年*"把回滚的门槛设得低一些"*，考虑到可用开发时间的减少。[Bruce Momjian 指出](https://www.postgresql.org/message-id/ao7-qUPXkwete2Bv%40momjian.us)大量的安全/CVE 修复在这里产生了影响。

- [Joshua Drake 建议将发布推迟到 2027 年春季](https://www.postgresql.org/message-id/CAJvJg-TDxNL%2BHWm27N4h2_O8wZ%3D7YapGcdcbpPyYbpWgUuwS%3Dg%40mail.gmail.com)，而不是移除功能：*"我宁愿要一个晚的 19 版本，也不愿看到这些伟大的功能和辛勤的工作被削减。"*

## [当你无能为力时如何优化](https://hdombrovskaya.wordpress.com/2026/08/25/how-to-optimize-when-you-cant-do-anything/)
Hettie 在一个 750GB、160 亿行的表上有一个生产查询突然运行缓慢。创建正确的索引不是一个选项（需要一天多的时间），但仔细查看底层数据后，她找到了一个巧妙的解决方案。

`Henrietta Dombrovskaya`

### 简讯：

- 🇺🇸 [PostgreSQL@SCaLE 提案征集开放](https://gorthx.wordpress.com/2026/09/08/the-scale-24x-cfp-is-open-get-your-postgres-talks-in/)至 11 月 1 日。Postgres 分会场将在帕萨迪纳的 [SCaLE 24x](https://www.socallinuxexpo.org/scale/24x) 上于 4 月 1-2 日举行。

- 🇮🇳 [PGConf India 2027](https://www.postgresql.org/about/news/pgconf-india-2027-dates-announced-and-cfp-open-3370/) 将于明年 3 月 2-5 日在班加罗尔回归。[提案征集](https://pgconf.in/cfp)开放至 10 月 15 日。

- [Postgres 的 RPM 仓库现在支持 Amazon Linux 2023](https://people.planetpostgresql.org/devrim/index.php?/archives/128-PostgreSQL-RPM-repo-comes-to-Amazon-Linux-2023!.html)。

## [16 个锁应该够任何人用了](https://thebuild.com/blog/sixteen-locks-ought-to-be-enough-for-anybody/)
你知道吗，在规划查询时，Postgres 会对表上的每个索引都加一个（弱）锁，无论是否使用它们？这通常是没问题的，但*直到 Postgres 18*，一旦查询涉及超过 16 个表和索引的组合，这可能会造成问题。

`Christophe Pettus`

📄 [在 Postgres 中插入状态转换](https://thoughtbot.com/blog/inserting-state-transitions-in-postgres) – 一个仅追加的状态表为你提供完整的历史记录，但两个并发的转换可能都会插入。这是如何防止冲突的方法。*Thiago Araújo Silva (thoughtbot)*

📄 [战壕中的故事：我的 Postgres 之路](https://www.pgedge.com/blog/from-the-trenches-my-path-through-postgres) – 一位曾经的 MySQL 倡导者的二十年 Postgres 战争故事。*Shaun Thomas*

📄 [在升级 Amazon RDS for PostgreSQL 和 Amazon Aurora 期间解决循环角色依赖](https://aws.amazon.com/blogs/database/resolve-circular-role-dependencies-during-upgrades-of-amazon-rds-for-postgresql-and-amazon-aurora/) *Ravi Teja Adabala (Amazon)*

📄 [Postgres 计算和 NULL 的歧义性](https://www.crunchydata.com/blog/postgres-calculations-and-the-ambiguity-of-null) *Christopher Winslett (Crunchy Data)*

### 📰 分类广告

🧊 为没人读的数据支付 SSD 价格？[ColdFront 以开源方式自动将旧 Postgres 行分层到 S3](https://github.com/pgEdge/coldfront)。

🎟️ 加入我们于 10 月 2 日的 [Supabase Select](https://supabase.link/JKX1Ifb)。获取关于 Supabase 即将推出功能的第一手信息。[使用优惠码 SUPAWEEKLY 申请参加享受 75 折](https://supabase.link/JKX1Ifb)。

### 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/varezths9zhsyun4zhhh.jpg)

## [Kafgres：嵌入 Postgres 内部的 Kafka 兼容代理](https://rynr.dev/blog/kafgres/)
一个由 [pgrx](https://github.com/pgcentralfoundation/pgrx) 驱动的扩展，从 Postgres 后台工作进程提供 Kafka 有线协议服务，使标准 Kafka 客户端能够针对存储在数据库中的主题进行生产、消费和重新平衡消费者组。

`Raynor Elgie`

## [chdb：从 S3、GCS 和 Azure 快速导入的扩展](https://clickhouse.com/blog/introducing-chdb-postgres)
ClickHouse 的 chDB 引擎被包装成用于批量导入和导出的扩展。`COPY`（或 `CREATE TABLE`）可以从 S3、GCS、Azure 或通过 HTTP 拉取 Parquet、Avro、ORC、Arrow 等格式。尽管还处于早期阶段，但很有前景。

`David Wheeler (ClickHouse)`

- [pg_hardstorage 1.4](https://www.pghardstorage.org/) – 在[第 654 期](https://postgresweekly.com/issues/654)中介绍过，Cybertec 的流优先单一 Go 二进制文件备份/恢复工具继续成熟，1.4 版本是一个修复密集的版本，特别是针对其 pgBackRest、Barman 和 WAL-G 兼容性垫片。

- [Ivory 2.0](https://github.com/veegres/ivory/releases/tag/v2.0.0) – 最初用于在 Patroni 下运行的高可用 Postgres 集群的 Web UI，现在拥有插件架构，也支持 MongoDB 和 Redis 等系统。

- [Barman 3.20](https://github.com/EnterpriseDB/barman/releases/tag/release/3.20.0) – EDB 的备份/恢复管理器添加了到 Google Cloud Storage 的流式多部分上传、Zstd 云备份和更快的压缩恢复。

- [pg_cron 1.6.8](https://github.com/citusdata/pg_cron/releases/tag/v1.6.8) – 添加了 Postgres 19 和原生 Windows 构建支持。

- 🌐 [PostGIS 3.7.0 RC2](https://postgis.net/2026/09/PostGIS-3.7.0rc2/)