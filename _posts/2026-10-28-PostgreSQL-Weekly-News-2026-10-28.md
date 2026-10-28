---
layout: post
title: PostgreSQL 每周新闻 2026-10-28
---
### PostgreSQL每周新闻#671 - 2026年10月28日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/671)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/fjmq5nbgoygs2qyhpggn.jpg)

## ['Region'：数据完整性的一课](https://postgresweekly.com/link/192052/rss)

Lætitia 的一位同事添加了一个自由文本 `region` 列，并计划在应用代码中验证它，但 Lætitia 不会批准。在这里，她为在数据库中保留规则提出了理由，探讨了域、枚举、`CHECK` 约束和查找表，以及如何在大表上添加约束而不阻塞流量。

**Lætitia Avrot**


## [在 1 亿向量上创建索引只需不到两小时](https://postgresweekly.com/link/192051/rss)

大型 pgvector 表上的 HNSW 索引使用大量内存，可能需要数天才能构建。认识一下 pg_vectorsearch：现有向量列的开源替代方案。在 1 亿向量上：25 GB 索引，95% 召回率下 6 毫秒查询。[查看基准测试](https://postgresweekly.com/link/192051/rss)。

**Tiger Data（TimescaleDB 创建者）** 赞助商


## [📖 PostgreSQL 18 查询优化：199 页免费书籍](https://postgresweekly.com/link/192053/rss)

Postgres Pro 的查询调优课程，重新塑造成一本紧凑的英文书籍。它涵盖了规划器如何工作、访问方法、连接策略、统计信息、读取执行计划和调优方法。[这是 PDF 版本](https://postgresweekly.com/link/192054/rss)。

**Pavel Tolmachev (PostgresPro)**


## **本周摘要：**

- Microsoft [开始向 Postgres 开发人员推销 SQL Server](https://postgresweekly.com/link/192055/rss) 作为*"升级"*，吹捧其 32,767 连接限制。SQL Server 专家 [Brent Ozar 并不买账](https://postgresweekly.com/link/192056/rss)，Microsoft 的作者在评论中出现进行反驳。

- 🇺🇸 [PgDay Boston 2027](https://postgresweekly.com/link/192057/rss) 将于 2027 年 4 月 10 日在 Tufts University 举行。[注册已开放](https://postgresweekly.com/link/192058/rss)，[CFP](https://postgresweekly.com/link/192059/rss) 也已开放（截止日期为 1 月 15 日）。

- 🇺🇸 [Postgres Day SF](https://postgresweekly.com/link/192060/rss) 是一个免费聚会（注册需要批准），将于 11 月 4 日在 PlanetScale 的旧金山办公室举行，与 Bruce Momjian 和 Fabrizio Mello 一起庆祝 Postgres 30 周年。

- 📅 [POSETTE 2027](https://postgresweekly.com/link/192061/rss)，Microsoft 的年度虚拟 Postgres 活动，将于 2027 年 3 月 30-31 日回归。目前还没有 CFP。


## [为什么我不信任 `ON DELETE CASCADE`](https://postgresweekly.com/link/192062/rss)

一个大的级联 `DELETE` 加上常规迁移可能会冻结对表的写入。Tom 解释了其背后的锁队列、一些复制陷阱，以及他为什么更喜欢软删除。

**Tom Pang (PlanetScale)**


## [读副本如何几乎摧毁其主数据库](https://postgresweekly.com/link/192063/rss)

Google Cloud 会自动增长磁盘，因此 Photoroom 并不担心空间。然后一次回填使 BI 副本落后太多，以至于主库为它保留了 31.7TB 的 WAL。磁盘增长接近硬限制，缩小它意味着停机。

**Marek Zaremba-Pike (Photoroom)**


## [用一周的回滚窗口将 74GB 从 RDS 迁出](https://postgresweekly.com/link/192064/rss)

Prisma 使用逻辑复制将其控制台数据库从 RDS 迁出，没有写入暂停，然后*反向*运行复制，以便可以回退到 RDS 一周。

**Siket and Datta (Prisma)**


📄 [您的应用不需要 Postgres Superuser](https://postgresweekly.com/link/192065/rss) - Superuser 可以在服务器上运行命令，所以这里是应该授予应用和代理的权限。*Umair Shahid (Stormatics)*

📄 [Postgres 19 延迟了，这是 AI 的错](https://postgresweekly.com/link/192066/rss) *Robert Haas*

📄 [为分析调优 Postgres](https://postgresweekly.com/link/192067/rss) - 来自 PGConf.EU 的幻灯片和记录，关于在不减慢应用数据库的情况下运行报告。*Karen Jex*

🎙️ Karen 还加入了 Claire Giordano 的 *Talking Postgres* 播客，谈论[她从 Oracle DBA 到 Postgres 贡献者的历程](https://postgresweekly.com/link/192068/rss)。


## 分类广告：

⚡ [Rebase](https://postgresweekly.com/link/192069/rss) 将您的 Postgres 转变为 API 和团队可以使用的管理面板。我们自己的 CRM：23 个表，零手写管理屏幕。

⏱️ 一个 5 行查找表将 0.3 毫秒的 Postgres 查询变成了 467 毫秒。[在生产环境发现之前找到您的问题](https://postgresweekly.com/link/192070/rss)。现在处于预览状态。


## 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ey5jp6aqzwln1cm4yc4d.jpg)

## [pgVolvra：对错误 `UPDATE` 和 `DELETE` 的 Flashback 风格 '撤消'](https://postgresweekly.com/link/192071/rss)

基于触发器的行历史记录，让您通过事务 ID 预览和撤销错误的语句或迁移。纯 SQL，不需要 superuser，因此它也适用于托管 Postgres。[GitHub 仓库](https://postgresweekly.com/link/192072/rss)。

**Muhammad Aqeel (pgEdge)**


## [pgrust 0.4 Beta：Postgres 的 Rust 重写版本开放](https://postgresweekly.com/link/192073/rss)

Postgres 的实验性 Rust 重新实现添加了新的 JIT 引擎、事务列存储表和自动内存大小调整（不再需要 `work_mem` 调优？）。

**Michael Malis**

💡 ClickHouse 在 9 月份因每查询代码和缓存问题[将 pgrust 从 ClickBench 中移除](https://postgresweekly.com/link/192074/rss)。随着 v0.4 的源代码公开，它[又回来了](https://postgresweekly.com/link/192075/rss)，并且成为[基准过拟合争论](https://postgresweekly.com/link/192076/rss)的核心。


## [pg_pinecone：Pinecone 为 pgvector 列提供的向量索引](https://postgresweekly.com/link/192077/rss)

一个新的扩展，使用 IVF 和 RaBitQ 量化为现有 pgvector 列建立索引，在搜索期间应用过滤器。其原生引擎在 Postgres 17 和 18 上本地运行，Pinecone 报告在 100 万向量上索引为 136MB，而 HNSW 为 2GB。[GitHub 仓库](https://postgresweekly.com/link/192078/rss)。

**Daddala and Mahanna (Pinecone)**


![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/yerrrdxckhvcxirfirjy.jpg)

- [pg_hdr_histogram 1.0](https://postgresweekly.com/link/192079/rss) *（上图）* - 将值分布（例如延迟）存储为紧凑的 HDR 直方图，然后查询 p99 风格的百分位数，并在时间窗口或服务器之间无损地合并它们。

- [mcdview](https://postgresweekly.com/link/192080/rss) - 将 Postgres 模式转储（或 Prisma、pgModeler 或 Rails 模式）转换为可搜索、可共享的交互式 ER 图。您可以[在线试用](https://postgresweekly.com/link/192081/rss)或[在此查看其输出示例](https://postgresweekly.com/link/192082/rss)。

- [Citus 14.3](https://postgresweekly.com/link/192083/rss) - 分布式 Postgres 扩展为多分片 `ORDER BY` 查询添加了排序合并执行，并为 `OR` 子句添加了每分片修剪。

- [SPQR 3.2](https://postgresweekly.com/link/192084/rss) - Yandex 的 Postgres 分片路由器添加了 `spqrmigrate`，一个模式迁移工具。