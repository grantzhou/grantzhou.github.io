---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-3-15
---
### PostgreSQL每周新闻#497 - 2023年3月15日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/497)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_600,h_120/e_make_transparent/co_white,e_outline:7/iplxngwgax1ktho5k45h.png)
## [PostgreSQL 14内部书籍](https://postgresweekly.com/link/136747/web)
PostgreSQL 14 Internals 已经开发了相当长的一段时间，基于 Egor Rogov 的一系列精彩技术文章， PostgreSQL 14 Internals是一本现已完全完成的书，可在此处以 PDF 格式获取。不要担心它对您来说过于技术化——它包含了代码驱动的示例和图表，并且很容易缩小到您可能感兴趣的主题，例如锁、索引或 Postgres 如何处理查询。


`Egor Rogov and Liudmila Mantrova `
## [Kubernetes 上 PostgreSQL 的 HA 和 DR 秘诀](https://postgresweekly.com/link/136746/web)
看这个点播网络研讨会，了解 Percona Distribution for PostgreSQL Operator 如何让您在 Kubernetes 上部署和管理高可用性和生产级 PostgreSQL 集群。


`Percona `
## [逻辑解码消息的奇妙之处](https://postgresweekly.com/link/136749/web)
您知道可以将数据直接写入 Postgres 的预写日志 (WAL) 吗？然后可以使用逻辑解码来检索此数据并以各种方式处理和中继它。Gunnar 解释了您可能想要这样做的方式和原因（剧透：它可以用于审计日志记录。）


`Gunnar Morling `
## [系统角色：什么、为什么以及如何？](https://postgresweekly.com/link/136750/web)
从 v9.6 开始，Postgres 引入了多种内置角色，例如pg_read_all_data和pg_monitor. Hubert 详细介绍了它们以及它们允许用户做什么，但警告我们它们的全球性。


`Hubert depesz Lubaczewski `
## [Postgres备份简介](https://postgresweekly.com/link/136755/web)
对 Postgres 用户可用的一些备份选项的概述和比较，包括 pg_dump、pg_basebackup 和 pgBackRest。


`Philip Hurst `
## [研究生与人工智能有什么关系？](https://postgresweekly.com/link/136756/web)
查看使用 Ruby 和 OpenAI 的 API 获取数据的嵌入（在本例中为食谱），将它们馈送（哈！）到 Postgres 并存储和查询结果向量。


`Christopher Winslett `
## [采用PgCat：下一代Postgres代理](https://postgresweekly.com/link/136757/web)
Instacart 探索和采用PgCat（具有负载平衡、副本故障转移和并发功能的 Postgres 连接池/代理）的故事。


`Abdelraouf, Kabani, Tanner (Instacart) `
## [网络研讨会：如何使用Postgres查询计划器调试错误计划并加快查询速度](https://postgresweekly.com/link/136759/web)


`pganalyze `
## [使用Rust、Axum、Postgres和Tokio构建博客](https://postgresweekly.com/link/136760/web)
这只是与 Postgres 无关，但展示了一种在新兴的 Rust 框架中使用它的方法。


`SpaceDimp `
## [pg_tiktoken：用于快速BPE令牌化的Postgres扩展](https://postgresweekly.com/link/136763/web)
简化 Postgres 数据库中的文本标记化。您可以使用它tiktoken_encode来轻松标记化输出并tiktoken_count检查文本长度限制，例如 OpenAI 的语言模型中的限制。


`Stas Kelvich (Neon) `
## [pg_timetable v5.3发布](https://postgresweekly.com/link/136764/web)
pg_timetable 是 Postgres 的高级独立作业调度程序。这是一个以日志记录为重点的版本。您现在可以禁用日志记录（可能在高负载环境中有用）、启用日志轮换等。GitHub 回购。


`Pavlo Golub `
# 💡本周提示


**🗓即将举办的Postgres活动**
