---
layout: post
title: PostgreSQL 每周新闻 2024-2-28
---
### PostgreSQL每周新闻#544 - 2024年2月28日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/544)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/se2eajmmmhygjxtuvonz.jpg)
## [Azure Database for PostgreSQL 的 azure_ai 扩展](https://postgresweekly.com/link/151824/web)
Microsoft 与 OpenAI 密切关系的好处之一是它可以直接在 Azure 中使用，现在您可以使用 azure_ai 扩展以及 pgvector 从 Azure Database for PostgreSQL 中直接使用 Azure OpenAI 处理该工作的任何基于嵌入的结果。 克莱尔在 ▶️ 这个五分钟的截屏视频中展示了这一切在实践中的样子。


`Claire Giordano (Microsoft) `
## [PGlite：WebAssembly 中的 Postgres](https://postgresweekly.com/link/151826/web)
人们之前已经将 Postgres 带入 WebAssembly 环境中，尽管通常中间有一个 Linux VM 层。 PGlite 将 Postgres 的 WASM 版本打包到 TypeScript 库中，该库可以在浏览器或 Node.js 或 Bun 上运行，并且压缩后仅 3.7MB！ 这是一个令人兴奋的发展 - 我们期待看到它下一步的发展。


`ElectricSQL / Neon `

💡 您可以在 Anton Zhiyanov 设计的这个基于[浏览器的简单游乐场](https://postgresweekly.com/link/151827/web)中体验真实世界的 PGlite 部署。

## [2024 年数据库格局状况](https://postgresweekly.com/link/151823/web)
Redgate 的最新调查结果显示，随着组织继续采用多个数据库平台，PostgreSQL 继续位列最常用数据库的前四名。 了解有关数据库领域最新趋势的更多信息。


`Redgate Software `
## [剩下的就是历史：WAL 的调查](https://postgresweekly.com/link/151828/web)
作为示例恢复场景的一部分，Brian 将逐步查看预写日志历史记录，从而更深入地了解 Postgres 使用的 WAL 文件包含的内容。


`Brian Pace (Crunchy Data) `
## [使用 NULL 时要学习的 11 个教训](https://postgresweekly.com/link/151829/web)
NULL 表示 SQL 中缺失的、未知的或“非”值，它有一些有趣的属性和行为需要注意。


`Francesco Tisiot `

**本周摘要：**

*   Postgres 提供商 ElephantSQL 已宣布终止其 Postgres 服务，并最终于 2025 年初关闭。


*   David Wheeler 将于今年 5 月在加拿大温哥华主持 PGConf 的一部分，举办 Postgres 扩展生态系统峰会。


*   在 pgsql-hackers 列表中，Andrew Atkinson 发布了有关为 Postgres 新手创建改进的 README 体验的信息。


## [pgvector 中的两种类型的索引](https://postgresweekly.com/link/151834/web)
pgvector 是用于处理和查询向量的流行扩展，并且向量需要与规范不同的索引类型。 Semab 比较了所提供的 IVFFLAT 和 HNSW 选项。


`Semab Tariq (Stormatics) `
## [fdw_tuple_cost 的默认值更新为 0.2 – 为什么？](https://postgresweekly.com/link/151836/web)
快速浏览一下 Postgres 最近的变化。


`Umair Shahid (Stormatics) `
## [当少即是多时：数据库连接扩展](https://postgresweekly.com/link/151838/web)
Postgres 服务器可以处理的连接越多越好......对吗？ 不总是。 如果 max_connections 设置为不切实际的数字，即使这些连接没有被使用，也会产生负面影响。 （一篇经典文章，但可能值得重温。）


`Richard Yen `

📰 机密

想要将您的应用程序扩展到数百万用户吗？ 📈 了解如何自信地[自动扩展数据库](https://postgresweekly.com/link/151839/web)，使其始终满足实际需求。

📢 免费分布式 Postgres DB，具有 3 个节点集群，并可从 pgEdge Cloud 跨 3 个区域进行一键配置。 [报名并获得一件很酷的 T 恤](https://postgresweekly.com/link/151840/web)。


## [在 SLES 15 上安装 Postgres 变得更容易（更好）](https://postgresweekly.com/link/151841/web)
适合 SuSE Enterprise Linux 用户。


`David Detter `
## [使用 Kubernetes、Postgres 和 CloudNativePG 最大化微服务数据库](https://postgresweekly.com/link/151842/web)


`GABRIELE BARTOLINI`

🛠 代码和工具

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/zxexum9qj7kpbhiyth6h.jpg)

## [pg-lock-tracer：基于 eBPF 的锁定跟踪器](https://postgresweekly.com/link/151843/web)
在 Linux 上运行时，使用 eBPF 工具来挖掘 Postgres 中与锁定相关的瓶颈。 与 pg_locks 不同，您可以获得锁定活动和计时的连续视图，并且可以生成锁定的动画视图。


`Jan Nidzwetzki `
## [pgagroal 1.6：高性能 Postgres 连接池](https://postgresweekly.com/link/151844/web)
引入了对 CLI/JSON 输出、客户端证书以及 macOS 的支持。


`Red Hat Inc. `
## [pg_dumpbinary v2.15：将 Postgres 数据库转储为二进制格式](https://postgresweekly.com/link/151845/web)
这不会生成 SQL 转储，而是生成二进制转储（可以通过随附的 pg_restorebinary 工具恢复）。 在各种边缘情况下，二进制转储可能更可取，例如当使用（非常）大的 bytea 列或使用可能破坏标准转储的 \0 值的自定义类型时。


`HexaCluster `


## [Zapatos 6.4](https://postgresweekly.com/link/151846/web) – TypeScript 的零抽象类型安全 Postgres：一个非 ORM 数据库。

## [Postgres JDBC 更新](https://postgresweekly.com/link/151847/web) – 发布所有维护版本以解决 CVE-2024-1597。

## [Lantern 0.2](https://postgresweekly.com/link/151849/web) – Postgres 的新 HNSW/usearch 矢量扩展。

## [SQLpage 0.19](https://postgresweekly.com/link/151851/web) – 面向数据分析师的纯 SQL Web 应用程序构建器。

## [pg_graphql 1.5.1](https://postgresweekly.com/link/151852/web) – 为 Postgres 提供 GraphQL 支持。

## [Good Job 3.25](https://postgresweekly.com/link/151853/web) – Postgres 支持的 Rails 作业队列。