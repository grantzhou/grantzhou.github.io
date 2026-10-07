---
layout: post
title: PostgreSQL 每周新闻 2026-10-7
---
### PostgreSQL每周新闻#668 - 2026年10月7日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/668)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/aiq8svld7sdixoiwkkso.jpg)

## [Postgres 中的查询计划重写](https://postgresweekly.com/link/191189/rss)

深入介绍 Postgres 18 规划器的查询转换，包括常量折叠、内联、子查询扁平化和连接消除。了解它*不会*重写的情况也很有用，其中一些可能会让有经验的用户感到困惑（不过 Postgres 19 在可以排除 `NULL` 的情况下添加了 `NOT IN` 重写）。

`Phil Eaton`


## [使用 Red Hat Ansible 大规模管理 EDB Postgres](https://postgresweekly.com/link/191188/rss)

在大型 Postgres 集群中手动管理用户、权限、模式、扩展和 pg_hba？了解 edb.epas_postgresql（一个经过 Red Hat 认证的 Ansible Collection）如何在大规模环境中强制保持一致性。Red Hat 和 EDB 直播，10 月 15 日。

`EDB` **赞助商**


## [Postgres 19 中的查询计划提示](https://postgresweekly.com/link/191190/rss)

这可能是*"一个你可能永远不需要的新 Postgres 功能"*，但 `pg_plan_advice` 和 `pg_stash_advice` 在你*确实*需要以正确的方式引导规划器时值得关注。`EXPLAIN (PLAN_ADVICE)` 还可以让你看到正在发生的事情。

`Elizabeth Garrett Christensen`


**本周摘要：**

- ⭐ [Postgres 19 RC1 计划于 10 月 15 日发布，GA 版本计划于 10 月 29 日发布](https://postgresweekly.com/link/191191/rss)。

- ⏰ **如果你的 `char(n)` 列上有 B-tree 索引，`REINDEX` 即将到来。** 一个[新提交的、反向移植的修复](https://postgresweekly.com/link/191193/rss)停止了对 `bpchar` 索引的去重。预计将在 11 月的次要版本中发布。

- [Aurora PostgreSQL 现在内嵌了 DuckDB](https://postgresweekly.com/link/191194/rss)，可以将 S3 中的 Iceberg 和 Parquet 作为外部表查询，这是在 DuckDB 团队加入 AWS 一个月后。Franck Pachot 通过比较与 `pg_duckdb` 的计划[确认底层是 DuckDB](https://postgresweekly.com/link/191195/rss)。

- [Supabase 正在收购 Turso](https://postgresweekly.com/link/191196/rss)，这家公司背后是 SQLite 的 Rust 重写。Supabase 表示将继续围绕 Postgres 构建，Turso 的技术将为 AI 代理提供按需数据库。

- [PlanetScale 现在为 Postgres 提供专用只读副本](https://postgresweekly.com/link/191197/rss)。

- [Heroku Postgres Advanced 现已全面可用](https://postgresweekly.com/link/191198/rss)。


## ['PlanetScale 发布了文本搜索，我们有很多话要说'](https://postgresweekly.com/link/191199/rss)

PlanetScale 最近推出了 [TIN](https://postgresweekly.com/link/191200/rss)，一个全文搜索扩展，基准测试显示它在查询方面比开源的 [ParadeDB](https://postgresweekly.com/link/191201/rss) 快得多。所以 ParadeDB 开始工作，并表示他们已经*"缩小了差距"*。

`Ming Ying (ParadeDB)`


## [通过基本不移动数据来升级 56TB 数据库](https://postgresweekly.com/link/191202/rss)

面对 Aurora 强制重启截止日期导致的停机，Trigger 的工程师只将 2% 的数据迁移到 PlanetScale，其余数据留在原地。这是一个坦诚的事后分析，涉及 pgcopydb 补丁和第一次切换的失败。

`Daniel Sutton (Trigger)`


## [将 Apache Cloudberry 作为 Postgres 扩展运行](https://postgresweekly.com/link/191203/rss)

一个将 [Apache Cloudberry](https://postgresweekly.com/link/191204/rss)（Greenplum 的开源后代，基于 Postgres 的并行数据仓库）作为一组*扩展*在轻度修补的 Postgres 19 上运行的实验。它揭示了 Postgres 扩展机制的一些有趣限制。

`Igor Suhorukov`


📄 [什么是直接 I/O，为什么 ClickHouse Managed Postgres 在备份中使用它？](https://postgresweekly.com/link/191205/rss)  
*Kaushik Iska (ClickHouse)*

📄 [在 CDC 场景中使用心跳表解决复制延迟](https://postgresweekly.com/link/191206/rss)  
*Luo and Ooi (Amazon)*


## 📰 分类广告：

不离开 Postgres 的列式存储：[TimescaleDB](https://postgresweekly.com/link/191207/rss) 可将大表压缩高达 95% 并加快扫描速度。[获得 $1000 积分](https://postgresweekly.com/link/191207/rss)。

触发器和函数的可视化编辑器。无需扩展的 PL/pgSQL 调试器。免费试用 [dbForge Studio for PostgreSQL 2026.2](https://postgresweekly.com/link/191208/rss)。

⏱️ Postgres 快速运行了准备好的语句恰好五次。第六次慢了 746%。[捕捉查询中的翻转](https://postgresweekly.com/link/191209/rss)。现已进入预览。


## 🛠 代码和工具

## [🤖 Microsoft 为 Postgres 推出 MCP 服务器](https://postgresweekly.com/link/191210/rss)

他们远不是第一个，但看到 Microsoft 以 Rust 驱动（但通过 `npm` 安装）的 MCP 服务器进入这一领域很有趣，它允许 AI 编码代理与 Postgres 一起工作，无论你是否在 Azure 上。

`Aditi Gupta (Microsoft)`

💡 Microsoft 还有[一个 'Postgres 技能' 仓库](https://postgresweekly.com/link/191211/rss)（你可以[在这里阅读](https://postgresweekly.com/link/191212/rss)），涵盖了一般的 Postgres 使用和 Azure 平台特定内容。


## [📊 pgwatch 6.0：Prometheus 源、重建的仪表板和更强大的收集器](https://postgresweekly.com/link/191213/rss)

流行的 Postgres 指标收集器和 Grafana 可视化工具（[演示](https://postgresweekly.com/link/191214/rss)）添加了 Prometheus 导出器作为源，在 Grafana 13 上重建了仪表板，并更好地应对停止响应的数据库。

`CYBERTEC PostgreSQL`


## [pgx-bm25 1.0：纯 C BM25 索引扩展](https://postgresweekly.com/link/191215/rss)

一个新的 PostgreSQL 许可的 BM25 排名全文搜索扩展，其索引存在于索引关系的页面中，因此 WAL 日志记录、复制和 `VACUUM` 都像往常一样工作，无需管理单独的引擎或运行时。

`PGX Inc.`


- ⚠️ [pgBackRest 2.59.3](https://postgresweekly.com/link/191216/rss) - 修复了一个罕见的弱加密子密钥错误，仅升级无法修复，因此如果你的仓库已加密，请查看通知。

- [pg_textsearch 1.5](https://postgresweekly.com/link/191217/rss) - Tiger Data 的 BM25 排名文本搜索扩展。通过 `tsquery` 添加布尔和短语过滤，以及 Postgres 19 支持。

- ⚠️ [pgvector 0.8.7](https://postgresweekly.com/link/191218/rss) - 无处不在的向量搜索扩展修复了一个错误，即创建 IVFFlat 索引可能导致任意代码执行。

- [Debezium 3.7](https://postgresweekly.com/link/191219/rss) - 流行的变更数据捕获平台。现在可以从只读副本进行增量快照，并更好地支持 Postgres 的几何列类型。

- [pg_ivm 1.16](https://postgresweekly.com/link/191220/rss) - 增量视图维护扩展添加了 Postgres 19 支持。