---
layout: post
title: PostgreSQL 每周新闻 2026-11-25
---
### PostgreSQL每周新闻#675 - 2026年11月25日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/675)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/mjxv2zfstxmfeqeu2pnj.jpg)

## [Postgres.app 3.0 为 Mac 带来简便的 Postgres 19](https://postgresweekly.com/link/193351/rss)

如果你不使用 macOS，可以继续往下翻，但对于 Mac 用户来说，这是一个在 Mac 上轻松运行 Postgres 的好方法的重要版本。3.0 添加了 Postgres 19 和 PostGIS 3.7，并更新了用户界面（如上图）。你可以获取仅包含 19 版本的构建，或包含 14 到 19 所有版本的构建。

**Jakob Egger 等**

💡 注意，v3.0 已经"解绑"了一些之前安装的扩展，如 [pgRouting](https://postgresweekly.com/link/193352/rss) 和 [wal2json](https://postgresweekly.com/link/193353/rss)。这些现在作为[独立下载](https://postgresweekly.com/link/193354/rss)提供。


## [停止扫描不需要的行](https://postgresweekly.com/link/193350/rss)

随着 Postgres 表的增长，查询速度会变慢，仅靠索引只能做到这么多。TimescaleDB 按时间自动分区数据，允许 Postgres 跳过不相关的块，只查询需要的内容。更快的查询，更少的调优，仍然是你熟悉的 Postgres。

**Tiger Data (TimescaleDB 的创建者)** 赞助商


## [在 Postgres 19 中使用 `pg_stash_advice` 强制执行连接顺序](https://postgresweekly.com/link/193355/rss)

Postgres 19 的计划建议模块为我们提供了迄今为止最接近（官方）查询提示的东西。Laurenz 测试了一个连接顺序，将查询从 405ms 降至约 10ms，在查询 ID 下存储该建议，但也主张谨慎使用这种方法。

**Laurenz Albe (CYBERTEC)**

💡 我说"官方"是因为还有其他方法可以通过像 [pg_hint_plan](https://postgresweekly.com/link/193356/rss) 这样的扩展做*类似*的事情，它使用类似 Oracle 的提示，现在有了 [Postgres 19 版本](https://postgresweekly.com/link/193357/rss)。


**简讯：**

- 如果你使用 Docker 的 `postgres:latest`，请记住[它现在已切换到 Postgres 19](https://postgresweekly.com/link/193358/rss)。如果你的卷包含 v18 数据库，更新的容器会出错，你应该固定 `postgres:18` [直到升级](https://postgresweekly.com/link/193359/rss)。

- 🇨🇦 流行的 [PGConf.dev 又回来了](https://postgresweekly.com/link/193360/rss)，将于 2027 年 5 月 11-14 日在蒙特利尔举行，[征稿已开放](https://postgresweekly.com/link/193361/rss)（截止 1 月 12 日）。

- 🇸🇪 而在大西洋另一边，[Nordic PGDay 2027](https://postgresweekly.com/link/193362/rss) 将于 3 月 16 日在斯德哥尔摩举行。[征稿开放](https://postgresweekly.com/link/193363/rss)至 1 月 8 日。

- Robert Haas 和 Jonathan Katz [重新审视 Postgres 19 推迟发布的原因](https://postgresweekly.com/link/193364/rss)。


## [我们仍在犯的 Postgres 错误](https://postgresweekly.com/link/193365/rss)

来自 NYC 聚会的幻灯片，讨论在规模化时可能出现的错误或误解（有趣地从零开始索引！），涵盖 MVCC 怪癖、开放事务、批量删除和未使用的索引。还有一个[仓库](https://postgresweekly.com/link/193366/rss)，其中包含展示这些问题的 SQL。

**Scott Mead (Databricks)**


## [Postgres 19 恢复后剩下什么](https://postgresweekly.com/link/193367/rss)

Postgres 19 在后期失去了各种预期功能，但*实际*包含了什么？Zsolt 介绍幸存下来的功能。

**Zsolt Parragi (Percona)**


📄 [在 Postgres 19 中压缩表](https://postgresweekly.com/link/193368/rss) – 关于 `REPACK (CONCURRENTLY)` 如何进入 v19 的内幕故事，来自为保留它而奋斗的提交者。**Álvaro Herrera (EDB)**

📄 [如何处理缓慢的 Postgres 关闭](https://postgresweekly.com/link/193369/rss) – 你可能认为*停止* Postgres 比启动它更快，但事实并非如此，Laurenz 探讨了原因。**Laurenz Albe (CYBERTEC)**


## 分类广告：

⚡ 已经在使用 Postgres？[Rebase](https://postgresweekly.com/link/193370/rss) 添加 REST、类型化 SDK、认证、存储、函数和定时任务，还有现成的管理面板。MIT 许可证。


## 🛠 代码和工具

## [PGlite 0.6：编译为 WebAssembly 的 Postgres 19](https://postgresweekly.com/link/193371/rss)

用于浏览器（以及 Node 和 Bun）的 Postgres WASM 构建现在运行 Postgres 19，因此在测试中尝试新功能只需 `npm install` 即可。来自旧版本的持久化数据需要[转储和恢复](https://postgresweekly.com/link/193372/rss)。

**ElectricSQL**

💡 目前还没有博客文章，所以上面的链接指向相当简洁的发行说明，但如果你是 PGlite 新手，[文档](https://postgresweekly.com/link/193426/rss)是一个不错的起点。


## [gopgext：用 Go 编写 Postgres 扩展](https://postgresweekly.com/link/193373/rss)

上周我们介绍了 Rust 的 [pgrx](https://postgresweekly.com/link/193374/rss)，现在轮到 Go 了！有了这个，你可以用注释标记 Go 函数，它会使用 [TinyGo](https://postgresweekly.com/link/193375/rss) 将它们构建成 Postgres 扩展，包含 C 粘合代码和 SQL。但这是非常新和实验性的。

**Jesús Espino**

💡 如果你喜欢 Go，请查看我们的姊妹通讯 [Go Weekly](https://postgresweekly.com/link/193376/rss) :-)


## [PgJDBC 42.7.15：Java/JDBC 驱动程序的众多安全修复](https://postgresweekly.com/link/193377/rss)

官方 JDBC 驱动程序一次性关闭了十四个安全[公告](https://postgresweekly.com/link/193378/rss)（六个评级为高），其中一些 bug 可以追溯到多年前。

**pgjdbc**


- [WAL-G 3.0.10](https://postgresweekly.com/link/193379/rss) – 备份/恢复工具的功能丰富版本，包括新的 `wal-send` 命令，允许备用服务器从备份存储流式传输 WAL。

- [pg_parquet 0.6](https://postgresweekly.com/link/193380/rss) – Crunchy Data 的用于[复制到 Parquet 文件和从 Parquet 文件复制](https://postgresweekly.com/link/193381/rss)的扩展现在支持 Postgres 19。

- 🔎 [pg_textsearch 1.6](https://postgresweekly.com/link/193382/rss) – Tiger Data 的 BM25 排名文本搜索扩展也加入了 Postgres 19 行列，还有一些效率和排名改进。

- [PGSync 8.0](https://postgresweekly.com/link/193383/rss) – Postgres 到 Elasticsearch/OpenSearch 同步工具。

- [Npgsql 11.0](https://postgresweekly.com/link/193384/rss) – 用于 Postgres 的 ADO.NET 数据提供程序。