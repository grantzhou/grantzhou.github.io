---
layout: post
title: PostgreSQL 每周新闻 2026-4-8
---
### PostgreSQL每周新闻#643 - 2026年4月8日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/643)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/fwcg92rcerfavcxjv2kt.jpg)

## [AWS 工程师报告 Postgres 性能在 Linux 7.0 上减半](https://postgresweekly.com/link/183419/rss)

在基于 ARM 的实例上运行 Postgres 17，且使用 Linux 7.0 内核（目前处于 RC 阶段）时，一名工程师发现性能下降了 49%，这导致了一个[内核补丁](https://postgresweekly.com/link/183420/rss)以恢复 Linux 的默认抢占模式。然而，最初做出这一改变的内核开发人员表示 Postgres 需要现代化其锁机制——考虑到 Linux 7.0 将在本月晚些时候发布，这是一个很大的要求。

Michael Larabel (Phoronix)

💡 目前尚不确定这是否也会影响 x86-64，但[初步实验表明并没有](https://postgresweekly.com/link/183421/rss)。


## [您不必参加全部 44 场 Postgres 演讲](https://postgresweekly.com/link/183418/rss)

POSETTE: An Event for Postgres 2026 是一个免费的虚拟开发者活动，将在 6 月 16-18 日举行。全部 44 场演讲都将直播，之后也可以观看。现场参加可以与演讲者和其他参会者进行讨论。[查看日程并标记您的日历。](https://postgresweekly.com/link/183418/rss)

Microsoft | AMD  *赞助商*


## [📊 PostgresBench: Postgres 服务的可重现基准测试](https://postgresweekly.com/link/183422/rss)

ClickHouse 想要对其托管的 Postgres 服务进行压力测试并与竞争对手进行比较，因此他们构建了这个基准测试系统。正如基准测试文章中常见的那样，ClickHouse 在结果中名列前茅，但该系统是[开源的](https://postgresweekly.com/link/183423/rss)，因此方法论可以很容易地被重现和审查。

Lionel Palacin (ClickHouse)


## [`pg_column_size()`: 所见非所得](https://postgresweekly.com/link/183424/rss)

TOAST 引入了模糊性，Lætitia 希望修补 Postgres 的文档，以更准确地说明 `pg_column_size` *真正*显示的内容。

Lætitia Avrot


## [📘 Lift the Elephant: 一本关于超越查询扩展的书](https://postgresweekly.com/link/183425/rss)

一本 160 页的 PDF 书籍，提供了 Postgres 中存在哪些性能杠杆、为什么它们重要以及如何系统地进行调优的思维导图。适合希望获得实际操作手册的中级用户。这是一个付费产品，但如果需要也可以免费获取。

Alex Yarotsky

💡 我们与这本书没有经济利益关系；作者给我们发送了一份副本供审阅。

📄 [等待 Postgres 19: 添加 `UPDATE`/`DELETE` .. `FOR PORTION OF`](https://postgresweekly.com/link/183426/rss) – `UPDATE`/`DELETE` 的扩展，可基于范围或多范围列进行"时间更新/删除"。*Hubert Lubaczewski*

📄 [Postgres 和 Oracle 中的 Schema：有什么区别？](https://postgresweekly.com/link/183427/rss) – 表面上相似，细节上却大不相同。*Laurenz Albe*

📄 [您需要调优 Postgres Vacuum 吗？](https://postgresweekly.com/link/183428/rss) – 检查膨胀和调优 Postgres 的 autovacuum 进程的入门指南。*Christensen and Jones (Snowflake)*

📄 [什么是排序规则，为什么我的数据损坏了？](https://postgresweekly.com/link/183429/rss) *Shaun Thomas*


## 分类广告：

[以 API 构建的规模收集实时搜索数据](https://postgresweekly.com/link/183430/rss)，专为分析师、工程师和 AI 团队打造。


## 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/dm11sns3iit7dgr6smi8.jpg)

## [不要让 AI 触碰您的生产数据库：改用 `dryrun`](https://postgresweekly.com/link/183431/rss)

对于许多任务，如果代理可以*查看有关*您的数据库的信息会有所帮助，但它们并不真正需要完整的连接。[dryrun](https://postgresweekly.com/link/183432/rss) 是 Radim 新推出的"离线优先" Postgres MCP 服务器，它允许 AI 代理访问他们需要的帮助您的内容，但使用 JSON 快照而不是连接到您的实时数据库。

Radim Marek


## [pgmicro: 进程内 Postgres 重新实现](https://postgresweekly.com/link/183433/rss)

来自 [Turso](https://postgresweekly.com/link/183434/rss) 创始人，*pgmicro* 使用 `libpg_query` 解析 SQL 并将其直接编译为 SQLite 字节码。作为 npm 包和 CLI 发布，带有线协议服务器选项，可用于现有的 Postgres 客户端。

Glauber Costa (Turso)


## [`rpg`: 用 Rust 编写的现代 Postgres 终端](https://postgresweekly.com/link/183435/rss)

一个用 Rust 编写的 psql 兼容终端，具有内置的 DBA 诊断和 AI 助手。单个二进制文件，无依赖关系，跨平台。

Nik Samokhvalov

- [pg_clickhouse v0.1.10](https://postgresweekly.com/link/183436/rss) – 从 Postgres 查询 [ClickHouse](https://postgresweekly.com/link/183437/rss) 数据库。现在有更多兼容性改进，如 `JSON`/`JSONB`/`TEXT` 操作符的映射以及众多窗口函数，包括 `RANK`、`PERCENT_RANK` 和 `ROW_NUMBER`。

- [pg_trickle v0.16](https://postgresweekly.com/link/183438/rss) – 声明式、自动刷新的物化视图。[pg_ivm](https://postgresweekly.com/link/183439/rss) 是这个领域的另一个好解决方案。

- [pgfmt 2.0](https://postgresweekly.com/link/183440/rss) – 基于 Rust 的 Postgres 风格 SQL 格式化工具，支持多种 SQL 风格指南（但[这是默认的](https://postgresweekly.com/link/183441/rss)）。

- [libpqxx 8.0 / 8.0.1](https://postgresweekly.com/link/183442/rss) – Postgres 的官方 C++ 客户端 API。