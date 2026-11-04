---
layout: post
title: PostgreSQL 每周新闻 2026-11-4
---
### PostgreSQL每周新闻#672 - 2026年11月4日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/672)

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/fuijuqlp9k2pt4psbneg.jpg)

## [Postgres 19的`REPACK`：内置的在线膨胀清理](https://postgresweekly.com/link/192360/rss)

Craig最喜欢的新Postgres功能是他认为DBA们最关心的功能。`REPACK`将`VACUUM FULL`和`CLUSTER`合并为一个命令，并添加了一个`CONCURRENTLY`模式，该模式使表保持可读可写，使用逻辑解码（类似于[`pg_squeeze`](https://postgresweekly.com/link/192361/rss)）。他在这里深入探讨了它的优势以及如何使用它。

Craig Kerstiens (Snowflake)


⭐ **Postgres 19仍计划于11月19日发布**，RC2将于11月12日发布。[Jonathan Katz已发布了草案新闻稿](https://postgresweekly.com/link/192362/rss)供审阅，[草案发布说明](https://postgresweekly.com/link/192363/rss)继续扩充。

## [一个Lakehouse上的亚秒级个性化](https://postgresweekly.com/link/192364/rss)

现场演示：了解EDB Postgres AI如何在Apache Iceberg中的一份数据副本上提供亚秒级的下一步最佳行动。Postgres、WarehousePG和ClickHouse共享一个catalog，引擎之间没有管道。[观看演示](https://postgresweekly.com/link/192364/rss)。

EDB 赞助商


## [高效删除4TB表](https://postgresweekly.com/link/192365/rss)

如何在一个有十个副本的主节点上以尽可能小的影响删除一个4TB的表？Radim将明显的`DROP TABLE`方法与批量删除和复制交换进行了比较，并测量了每种方法的优缺点。

Radim Marek


💡 在类似的主题上，NexHealth撰写了[如何在没有停机时间的情况下将4TB数据从实时Postgres数据库迁移出](https://postgresweekly.com/link/192366/rss)到其自己的Aurora集群中。

**简讯：**

- 想要轻松开始为Postgres做贡献？Paul Jungwirth正在举办一个[补丁审查研讨会](https://postgresweekly.com/link/192367/rss)，小团队将审查一个补丁，Robert Haas等提交者将评论这些审查。你可以在[这里报名](https://postgresweekly.com/link/192368/rss)。

- 🏴󠁧󠁢󠁳󠁣󠁴󠁿 Jimmy Angelakos [回顾了10月的Postgres Edinburgh聚会](https://postgresweekly.com/link/192369/rss)，Elizabeth Christensen介绍了Postgres 18和19的新功能。

- Supabase已开放[OrioleDB的公开测试版](https://postgresweekly.com/link/192370/rss)和[Multigres的私有alpha版](https://postgresweekly.com/link/192371/rss)。OrioleDB的替代Postgres存储引擎不需要`VACUUM`，但它还没有准备好投入生产。

- [CloudNativePG现在是CNCF的"孵化"项目](https://postgresweekly.com/link/192372/rss)。Gabriele Bartolini讲述了该项目从2019年在2ndQuadrant启动到今天约2.47亿次operator下载的故事。


## [烧焦的TOAST：为什么DBA害怕大文本列](https://postgresweekly.com/link/192373/rss)

介绍了Postgres如何存储超大列值，通过基准测试显示为什么保持堆小可以加速扫描和更新（这些操作不涉及这些值），以及为什么获取它们仍然可能很昂贵。

Shaun Thomas (pgEdge)


💡 继续TOAST主题，Franck Pachot思考：[TOAST的压缩和out-of-line阈值是否适合](https://postgresweekly.com/link/192374/rss)典型的JSONB文档大小？


## [`'server closed the connection unexpectedly'`解释和测量](https://postgresweekly.com/link/192375/rss)

Chris在Postgres 13、15、17和18上的六个客户端中重现了连接失败，展示了为什么相同的失败会产生不同的诊断信息，以及为什么在`COMMIT`期间丢失连接可能会导致结果不确定。

Chris van Eijk


📄 [超越单个写入器的逻辑复制](https://postgresweekly.com/link/192376/rss) – 构建多区域复制、测试故障转移和处理模式更改的演练，附带可运行的Docker实验室。*Dimitri Fontaine*

📊 [六个数据库引擎中的向量搜索基准测试](https://postgresweekly.com/link/192377/rss) – Postgres和pgvector与MongoDB、MariaDB、AliSQL和Valkey的对比。*Evgeniy Patlan (Percona)*

📄 [复制槽如何填满你的磁盘](https://postgresweekly.com/link/192378/rss) *Anugya Sinha (Microsoft)*

📄 ["自主Postgres"有多真实？](https://postgresweekly.com/link/192379/rss) *Vibhor Kumar (EDB)*


## 分类广告：

📺 [新的4小时freeCodeCamp课程](https://postgresweekly.com/link/192380/rss)：观看如何使用TimescaleDB连续聚合将1.6秒的Postgres查询降至10毫秒。


## 🛠 代码和工具

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/okrdnkb2yf4sxr0mofwq.jpg)

- [pgModeler 2.0](https://postgresweekly.com/link/192382/rss) *（上图）* – 被称为"项目历史上最大的版本"，该数据库建模工具获得了多场景画布和Postgres 18支持，但将导入、差异和SQL执行移到了付费的"Plus"版本。

- [Melange](https://postgresweekly.com/link/192395/rss) – 将基于[OpenFGA](https://postgresweekly.com/link/192396/rss)模型的Zanzibar风格、基于关系的授权编译成PL/pgSQL函数，因此权限检查只需`SELECT check_permission(...)`，无需单独的服务或存储。

- 🌐 [PostGIS 3.7.0](https://postgresweekly.com/link/192383/rss) – 地理空间扩展（现在针对Postgres 19）添加了coverage edges、Float16栅格和更快的`ST_DWithin`。放弃了对Postgres 12/13的支持，地理编码器和地址标准化器移至单独的仓库。

- 🔒 [PostgreSQL Anonymizer 3.3](https://postgresweekly.com/link/192386/rss) – Dalibo的数据掩码扩展修复了12个漏洞，强烈建议现有用户升级。

- 🔒 [pgAdmin 4 v9.19](https://postgresweekly.com/link/192387/rss) – 修复了15个CVE。服务器模式用户应升级，首先设置两个新的管理员允许列表。

- [Postgres.js 4.0](https://postgresweekly.com/link/192384/rss) – 使用调度器重写的Node.js驱动程序，以阻止慢查询阻塞快查询，SCRAM通道绑定和两个安全修复。

- [TimescaleDB 2.31](https://postgresweekly.com/link/192385/rss) – Tiger Data的时间序列扩展获得了一个新的整数压缩器（*目前默认关闭*，但预计在2.32中默认开启），可以使数据库缩小约10%，典型查询速度提高约50%。

- [pg_duckdb 1.2.0](https://postgresweekly.com/link/192388/rss) – DuckDB-in-Postgres扩展移至[DuckDB 2.0](https://postgresweekly.com/link/192389/rss)并添加了初步的Postgres 19支持。目前*"尚未准备好用于生产"*。

- [pg_lion 0.3](https://postgresweekly.com/link/192390/rss) – 基于位图的倒排索引类型（受[roaring bitmaps](https://postgresweekly.com/link/192391/rss)启发，因此得名！），用于在大表上更快地计数、分面和`GROUP BY`。

- [Reylo 0.7](https://postgresweekly.com/link/192392/rss) – 将普通的`.sql`文件导入TypeScript，类型从数据库推断。来自[Zod](https://postgresweekly.com/link/192393/rss)的创建者。