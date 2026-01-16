---
layout: post
title: PostgreSQL 每周新闻 2025-4-3
---
### PostgreSQL每周新闻#595 - 2025年4月3日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/595)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/tcpmnscofpjqcvobjdzq.jpg)
## [Postgres 与 SQL Server：B 树索引差异一探](https://postgresweekly.com/link/167644/web)
Postgres 和 Microsoft 的 SQL Server 都使用 B 树索引作为其默认索引机制，但它们的方法有很大不同。即使您不使用 SQL Server，这也是一个幕后的好机会，您将了解 Postgres 的工作方式以及重复数据删除如何显著减少索引大小。Lukas 还比较了 Postgres 和 SQL Server 如何处理其他索引类型。

`Lukas Fittl`

## [MVCC 的内部原理：更新与插入的隐性成本](https://postgresweekly.com/link/167645/web)
Postgres 的多版本并发控制 (MVCC) 功能虽然非常有用，但会增加某些操作的开销，例如更新行（而不是插入行）。Rohan 深入探讨了原因和方式。


`Rohan Reddy Alleti`
## [Aurora 遇到了限制？](https://postgresweekly.com/link/167643/web)
Aurora 遇到了区域 HA、故障转移延迟和手动分片方面的瓶颈。CockroachDB 使用 Postgres，但更进一步 — 具有全局一致性、零停机操作和轻松扩展。观看此点播网络研讨会中的并排技术细分。


`Cockroach Labs `
## [2025 Postgres 扩展迷你峰会二](https://postgresweekly.com/link/167646/web)
几位 Postgres 用户和开发人员最近举行了一场虚拟活动，讨论了在 Postgres 中添加“扩展搜索路径”功能的最新进展，以便 Postgres 安装更容易发现和获取新安装的扩展（活动有一个 50 分钟的视频，但记录也很好）。


`Wheeler, Eisentraut, Drees et al. `

### 本周摘要：

* 🎤 如果您正在寻找一些与 Postgres 相关的访谈，[Postgres.fm](https://postgresweekly.com/link/167648/web) 的内容不断增强，最近的节目包括 [SQL 与 NoSQL 的讨论、关于使用快照的讨论以及与 PgDog（以及之前的 PgCat）创建者的聊天](https://postgresweekly.com/link/167649/web)。

* 🇺🇸 [PGDay Chicago](https://postgresweekly.com/link/167652/web) 将于本月晚些时候举行，门票仍有售 - [时间表](https://postgresweekly.com/link/167653/web)现已公布。

* 🇺🇸 留在伊利诺伊州的 Hettie Dombrovskaya 介绍了 [Prairie Postgres](https://postgresweekly.com/link/167654/web)，这是一项在美国中西部提供 Postgres 相关活动、培训和网络机会的新举措。

### 代码和工具：

## [📊 RTABench：实时分析的基准](https://postgresweekly.com/link/167655/web)
由 Timescale 团队构建的开源基准，与许多传统数据库基准不同，它专注于跨规范化表和增量预聚合物化视图的实际查询。


`Timescale`
## [更轻松地调试 Postgres](https://postgresweekly.com/link/167657/web)
Hans-Jürgen 分享了一种使用表继承以有趣的方式调试事务的技术。


`Hans-Jürgen Schönig`

📄 [使用 Postgres 在 Go 中构建实时通知系统](https://postgresweekly.com/link/167658/web) Ravi (Finly)

📄 [不要将端口 5432 暴露给公共互联网](https://postgresweekly.com/link/167659/web) Christophe Pettus

### 🛠 代码和工具

## [Autobase 2.2.0：Postgres 的自托管 DBaas 平台](https://postgresweekly.com/link/167660/web)
适用于您想要在自己的硬件上使用类似于 RDS 或 Cloud SQL 的东西的情况。它可以自动执行部署和维护，确保高可用性、可扩展性和成本效益。v2.2 在所有集群组件中添加了 TLS 支持、ARM 兼容性以及到 Hetzner 对象存储的自动备份。


`Autobase `

## [Trunk：Postgres 扩展注册表](https://postgresweekly.com/link/167661/web)
一个由 Rust 驱动的开源软件包安装程序和 Postgres 扩展注册表，已提供 200 多个扩展。Trunk 是在 Tembo 聘请 PGXN 的 David Wheeler 致力于改善 Postgres 扩展生态系统之前构建的。PIG 是该领域的另一个选择。


`Tembo `

### 📰 分类广告
有使用 Linux、Kubernetes 和 Postgres 的经验？[加入 pganalyze，为全球顶级公司转变数据库性能](https://postgresweekly.com/link/167663/web)。

🐘 [POSETTE：Postgres 活动](https://postgresweekly.com/link/167664/web) - 6 月 10 日至 12 日。查看此免费虚拟活动的时间表和演讲者！[立即注册](https://postgresweekly.com/link/167665/web)


## [pg_sentence_transformer：在后台工作程序中运行 HuggingFace 句子转换器模型](https://postgresweekly.com/link/167666/web)
一个原型扩展，它启动后台工作程序并计算给定源表的嵌入，并将其存储到新创建的嵌入表中，而无需使用外部 LLM 服务。


`Krzysztof Leśniak `

[postgres-meta 0.88](https://postgresweekly.com/link/167667/web) –用于管理 Postgres 的 RESTful API。
