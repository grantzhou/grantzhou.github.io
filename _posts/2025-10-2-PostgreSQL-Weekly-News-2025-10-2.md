---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-10-2
---
### PostgreSQL每周新闻#618 - 2025年10月2日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/617)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/y9wrtagqf7bunkiwxang.jpg)
## [深入了解 Postgres 18 的功能](https://postgresweekly.com/link/175084/web)
如果我们仍然保持著上周发布 Postgres 18 时的兴奋之情，请见谅。 Tudor 将以比冗长的发布说明更容易理解的方式，向您介绍各种令人兴奋且实用的新功能。

`Tudor Golubenco (Xata)`

💡 Bytebase 的 Tianzhou 在《[Postgres 18 新功能－开发者视角](https://postgresweekly.com/link/175087/web)》中也发表了类似的综述。本期稍后，我们也将深入探讨 Postgres 18 的具体功能。

## [🚀 将 Postgres 扩展到 2PB 数据量和每日数万亿指标](https://postgresweekly.com/link/175083/web)
TimescaleDB 的创建者 TigerData 正在将 Postgres 推向新的极限：扩展到 2PB 数据量和每日 1.5 万亿指标——无需专有黑盒或隐藏工具。使用 Tiger Postgres，您可以获得大规模扩展，同时保留您熟悉和喜爱的 SQL。

`TigerData    `

## [Postgres 18 中的 psql 新增了管道功能](https://postgresweekly.com/link/175088/web)
从 Postgres 18 开始，psql 配备了在 SQL 脚本中使用管道的命令，Daniel 指出这「可以大幅提升查询吞吐量」。

`Daniel Vérité`


### **本周摘要**

* Postgres 18 刚刚发布，但 Hubert Lubaczewski 期待著 Postgres 19 的到来，并发布了一系列部落格文章，介绍 [GROUP BY ALL](https://postgresweekly.com/link/175089/web) 的引入、[random(min, max) 的日期和时间戳版本](https://postgresweekly.com/link/175090/web)，以及在 EXPLAIN 中[显示 memoize 规划器估算值](https://postgresweekly.com/link/175091/web)。

* EDB 的 Floor Drees 分享了 EDB 公司为[新 Postgres 贡献者引入的幕后花絮](https://postgresweekly.com/link/175092/web)。


## [如何执行 UPDATE ... LIMIT](https://postgresweekly.com/link/175093/web)
抱歉，您不能在 Postgres 中使用带有 LIMIT 的 UPDATE（或 DELETE）（尽管某些 SQL 方言，如 MySQL 的方言，支持它）但您可以（谨慎地）使用其他方法。


`Laurenz Albe`


## [Postgres 18 及后续版本：从 AIO 到 Direct IO？](https://postgresweekly.com/link/175094/web)
Postgres 18 最令人兴奋的功能之一是它支援非同步 IO，但我们能否利用 Direct IO 并完全跳过作业系统缓存，做得更好？


`Laurenz Albe`

## [我如何学习使用 wal_inspect](https://postgresweekly.com/link/175096/web)
pg_walinspect 是一个用于检查预写日志内容的模组。


`Hettie Dombrovskaya`

📄 [在 Postgres 中实作卡尔曼滤波器来平滑 GPS 资料](https://postgresweekly.com/link/175098/web)——这绝对是我以前在 SQL 中从未见过的功能。 Thorsten Rieß

📄 [Postgres 18：RETURNING 子句中的旧行与新行](https://postgresweekly.com/link/175099/web) Brandur Leach

📄 [Postgres 18 中 COPY 命令如何变得更加用户友好](https://postgresweekly.com/link/175100/web) Deepak Mahto

📄 [Postgres 18 中的累积统计](https://postgresweekly.com/link/175101/web) Cédric Villemain


## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/xpbhlpxeazos0yneoxrx.jpg)

## [PG Back Web 0.5：具有 Web 介面的 Postgres 备份系统](https://postgresweekly.com/link/175102/web)
一款基于 Go 语言的应用，旨在为 Postgres 备份、定时备份（包括备份到 S3）、备份监控和 Webhook 带来更友善的使用者介面。它以 Docker 映像的形式提供，现在也支援 Postgres 18。

`Luis Eduardo`

## [介绍 Elephantshark：一款监控 Postgres 网路流量的工具](https://postgresweekly.com/link/175103/web)
一款基于 Ruby 的工具，位于 Postgres 协定交换的双方之间，在解析和记录讯息的同时双向转送讯息。 GitHub 仓库。

`George MacKerron (Neon)`

[pgrx 0.16.1](https://postgresweekly.com/link/175105/web) – 使用 Rust 建立 Postgres 扩充功能的方法（完整功能集请点击此处）– 现已支援 Postgres 18。

[VectorChord 0.5.3](https://postgresweekly.com/link/175107/web) – Postgres 中可扩充、快速且磁碟友善的向量搜寻。

[pgmetrics 1.18](https://postgresweekly.com/link/175108/web) – 从正在运行的 Postgres 伺服器收集并显示统计资料。

[ChartDB 1.16](https://postgresweekly.com/link/175109/web) – 以图表为基础的开源资料库编辑器。