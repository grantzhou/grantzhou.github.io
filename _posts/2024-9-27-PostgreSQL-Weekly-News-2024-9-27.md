---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-9-27
---
### PostgreSQL每周新闻#571 - 2024年9月27日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/571)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/v1727358522/ebxxozg8vnblpecfdm9u.jpg)
## [PostgreSQL 17 发布](https://postgresweekly.com/link/160399/web)
重磅版本来了。这是 Postgres 的最新主要版本，比 v16 更进了一步。一些新功能：

* 彻底改进了清理内存的管理，从而显著降低了内存使用量和运行时间。更多信息请见[此处](https://postgresweekly.com/link/160401/web)。
* [增量备份支持](https://postgresweekly.com/link/160402/web)。
* [更快的 B 树索引扫描](https://postgresweekly.com/link/160403/web)
* [MERGE 增强功能](https://postgresweekly.com/link/160404/web)，包括视图支持。
* [从 UUID 中提取元素](https://postgresweekly.com/link/160405/web)的新功能。
* WAL 改进 — 在某些工作负载上写入吞吐量高达 2 倍。
* [SQL/JSON 支持的改进](https://postgresweekly.com/link/160406/web)，包括 JSON_TABLE。
* COPY 的批量加载改进和性能改进，获得了 ON_ERROR ignore 选项以忽略错误。
* 分区表上的[标识列](https://postgresweekly.com/link/160407/web)。

💡 如果您想要所有新功能的完整列表，[发行说明](https://postgresweekly.com/link/160408/web)提供了非常详尽的要点演练。

## [2024 年 PASS 数据社区峰会主题演讲嘉宾公布](https://postgresweekly.com/link/160398/web)
PASS 峰会刚刚公布了今年活动（2024 年 11 月 4 日至 8 日）的主题演讲嘉宾。主题演讲嘉宾包括 Microsoft、Redgate 和一位社区专家，请在下次涨价前立即购买 3 天门票。


`PASS Data Community Summit `
## [使用 BOLT 获得更快的 Postgres](https://postgresweekly.com/link/160409/web)
BOLT 是来自 LLVM 项目的工具，它通过分析分析器数据来优化编译后的二进制文件。它可以用来加速 Postgres 吗？是的！但这很复杂。


`Tomas Vondra `
## [在 Postgres 上构建图像搜索引擎](https://postgresweekly.com/link/160411/web)
pgvector 再次来袭。该技术很简单：拍摄图像，创建它们的嵌入，然后使用其他提供的图像的嵌入通过向量相似性搜索查找相似图像。


`Adam Hendel (Tembo)  `

### 本周摘要：

* ▶️ Talking Postgres 播客邀请了 [Melanie Plageman](https://postgresweekly.com/link/160412/web) 谈论如何成为 Postgres 提交者。我们还得到消息称，Tom Lane 的一集节目即将推出，所以如果您不想错过，可以在此处[订阅该节目](https://postgresweekly.com/link/160413/web)。

* ▶️ 与此同时，在 [Postgres.fm](https://postgresweekly.com/link/160414/web) 上，他们一直在[与 Postgres 提交者 Peter Geoghegan](https://postgresweekly.com/link/160415/web) 讨论为 Postgres 17 添加跳过扫描支持。

* ⚡ 无服务器 Postgres 平台 Neon 迅速推出，并已提供 [Postgres 17](https://postgresweekly.com/link/160416/web)。

* 💰 [Supabase 在 C 轮融资中筹集了 8000 万美元](https://postgresweekly.com/link/160417/web)。


## [不使用 pgcrypto 生成一些安全的随机字节](https://postgresweekly.com/link/160418/web) 
random() 会生成伪随机数，但 pgcrypto 可以获得更好的随机性。但是，如果您的服务器（可能是本地服务器）不是针对 OpenSSL 构建的，则无法使用。幸运的是，Brandur 找到了一个有趣的替代选项。


`Brandur Leach`
## [Postgres 中的分层数据类型](https://postgresweekly.com/link/160419/web)
Hierarchyid 是 SQL Server 中用于表示层次结构（如树）内位置的特殊类型。您可以使用 Postgres 中的任何整数列来实现这一点，但如果您想要更结构化的内容，ltree 提供了更结构化的选项。


`Florent Jardin`
## [当 Postgres 索引出错时](https://postgresweekly.com/link/160422/web)
TLDR：创建索引时要小心 — 这是我在并发索引悄无声息地失败时学到的一个惨痛教训。”


`Arjun Lall`

* 📺 [47 分钟内完成 18 个月的 pgvector 学习](https://postgresweekly.com/link/160423/web) - Avthar Sewrathan (Timescale)

* 📄 [使用 Pgrx 编写 Postgres 扩展以实现可视化查询计划](https://postgresweekly.com/link/160424/web) - David Gomes

* 📄 [从 Oracle 过渡到 Postgres：理解“Schema”的概念](https://postgresweekly.com/link/160425/web) - Umair Shahid

* 📄 [使用 pgBackRest 从备用服务器进行备份](https://postgresweekly.com/link/160426/web) - Stefan Fercot


### 📰 分类广告
🐘 [PostgreSQL 状态调查的最后一天！](https://postgresweekly.com/link/160427/web)请确保在 9 月 30 日之前分享您的想法和经验。

💰 [Dragonfly（25k GitHub 星）](https://postgresweekly.com/link/160428/web)是现代 Redis 替代品。改用 Dragonfly 的组织可以将基础设施成本降低 80%。

[Blacksmith 只需更改一行代码，即可将 GitHub Actions 的运行速度提高 2 倍](https://postgresweekly.com/link/160429/web)，成本降低一半。受到 Ashby 和 Slope 等 100 多家公司的信赖。


### 🛠 代码和工具

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/zsn9cx7qodr8i2sbikjc.jpg)

## [pgMustard v5：快速审查 Postgres 查询计划](https://postgresweekly.com/link/160430/web)
一款帮助审查 Postgres 查询计划的工具，现在增强了对 Postgres 17 的支持，并针对次优 JIT 编译和过长的触发时间等问题提供了新的提示类型。不过，您只能免费使用五次，因为它最终是一项付费服务​​。


`Michael Christofides`
## [PostGIS 3.5.0 发布](https://postgresweekly.com/link/160431/web)
流行的地理空间数据索引和查询扩展的最新版本在 Postgres 17 最终版发布前几个小时发布，因此仍然推荐 RC1，但它应该不错。此处列出了重大更改。


`PostGIS PSC & OSGeo`

[libpg-query-node：从 Node.js 使用 Postgres 的 SQL 解析器](https://postgresweekly.com/link/160433/web)
通过 libpg_query 从 Node 在低级别使用 Postgres 的 SQL 解析器。如果您需要更高级别的解析器，则 pgsql-parser 会使用此库，它能够解析查询并将其序列化为 AST 或从 AST 序列化。


`Dan Lynch`


[River 0.12](https://postgresweekly.com/link/160435/web) – 适用于 Go 的快速可靠的 Postgres 后台作业。

[Bytebase 2.23](https://postgresweekly.com/link/160436/web) – 适用于团队的数据库 devops 和 CI/CD 系统。

[pgAdmin4 v8.12](https://postgresweekly.com/link/160437/web) – 适用于 Postgres 的流行管理平台/面板。