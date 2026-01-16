---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-11-2
---
### PostgreSQL每周新闻#479 - 2022年11月2日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/479)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,w_350,h_90/e_make_transparent/co_white,e_outline:7/vpntubykyv5ujmbzw501.png)
## [Postgres 数据仓库中的 B-tree 与 BRIN 索引](https://postgresweekly.com/link/130992/web)
Hans-Jürgen 将其描述为两种流行索引类型之间的“史诗般的战斗”，并进行了一次小型演示，从本质上证明了为什么进行自己的基准测试是有意义的。


`Hans-Jürgen Schönig `
## [在无需停机下，利用 updatable VIEW来安全地重新命名表](https://postgresweekly.com/link/130993/web)
只需使用 ALTER TABLE x RENAME TO y? 在生产环境中，您可能不想这样做，因为它可能会使当前使用数据库的客户端感到困惑，但有一种方法可以干净利落地完成它。


`Brandur Leach `
## [PostgreSQL 和 TimescaleDB 中更好的数据聚合的提示](https://postgresweekly.com/link/130994/web)
熟悉 TimescaleDB 连续聚合，它们如何使您能够快速方便地检索数据聚合，以及充分利用它们的额外提示。


`Timescale `
## [为新手在 Postgres 中加载数据](https://postgresweekly.com/link/130995/web)
快速涵盖从 CSV、JSON、备份文件、通过外部数据包装器、甚至通过查询生成数据的各种路径。 将 jq 与 \copy 一起使用是一种我以前没有考虑过的简洁方法。


`Elizabeth Christensen `
## [Postgres 数据库和模式](https://postgresweekly.com/link/131000/web)
Craig 研究过各种规模的 Postgres 数据库，但它们都有共同的层次。 这是针对初学者的，可以快速解释集群、数据库、模式和实例之间的区别。


`Craig Kerstiens `
## [跨分区数据 UNIQUE 保证做法](https://postgresweekly.com/link/131001/web)
来自瀚高软件的 Cary 解释跨分区数据 UNIQUE 保证的方法


`Cary Huang (Highgo) `
## [基于推送模式的逻辑复制](https://postgresweekly.com/link/131002/web)

`OSKAR DUDYCZ`

## [如何通过三个步骤在 Ubuntu 上升级 PostGIS 相关库 - 例如 GEOS 或 GDAL。](https://postgresweekly.com/link/131003/web)

`FLORIAN NADLER`
## [如何将 Oracle 分层查询迁移到 Amazon Aurora](https://postgresweekly.com/link/131005/web)

`RAGHAV AND CHINTHA (AWS)`
## [pg_stat_kcache：收集有关磁盘访问和 CPU 消耗的统计信息](https://postgresweekly.com/link/131006/web)
位于 pg_stat_statements 之上并创建几个视图，您可以使用这些视图来测量 CPU 时间、页面错误、交换、读取和写入的字节数，以及在数据库和查询级别的更多内容。


`Dalibo and PoWA Team `
## [使 Postgres 更实惠。 10 美元/月起](https://postgresweekly.com/link/131007/web)


`Crunchy Bridge `
## [适用于 Windows 的 PostgreSQL 15 64 位 FDW](https://postgresweekly.com/link/131008/web)
特别是用于 file_textarray_fdw（处理任意分隔的文本）和 odbc_fdw（方便连接到 ODBC 数据源）的 64 位二进制文件。


`Leo Hsu and Regina Obe `
## [pg_dump-aws-lambda：通过 AWS Lambda 将 pg_dump 输出流式传输到 S3](https://postgresweekly.com/link/131009/web)
在 AWS 上还有其他方法可以执行此类操作，但这是一种非常直接且灵活的数据库备份方式。


`James H `
## [PGroonga：将全文搜索功能扩展到所有语言](https://postgresweekly.com/link/131010/web)
将 Groonga 全文搜索引擎引入 Postgres，它可以比 Postgres 默认更适合某些用例，例如日语或中文。



