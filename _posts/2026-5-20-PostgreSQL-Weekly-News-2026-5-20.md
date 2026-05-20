---
layout: post
title: PostgreSQL 每周新闻 2026-5-20
---
### PostgreSQL每周新闻#649 - 2026年5月20日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/649)

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/gwgjpo4wrgclv830r3c1.jpg)

## [Postgres 18.4、17.10、16.14、15.18 和 14.23 发布](https://postgresweekly.com/link/185376/rss)

所有受支持的版本都进行了更新，修复了11个安全漏洞和超过60个错误。这些漏洞包括严重的内存损坏和信任边界错误，不仅存在于服务器中，还存在于连接到恶意服务器的客户端中。

`PostgreSQL Global Development Group`


💡 Christophe Pettus 在[《十一个CVE走进一个版本》](https://postgresweekly.com/link/185377/rss)中进行了更深入的探讨。


## [Greptile 会发现那个 Postgres 错误吗？](https://postgresweekly.com/link/185375/rss)

粘贴引入该错误的 GitHub PR，无需注册。Greptile 像审查新 PR 一样审查旧 PR，并显示它会留下的评论。

`Greptile` **赞助商**


**本周摘要：**

- 🎉 David Steele 在最近的[资金困境](https://postgresweekly.com/link/185379/rss)之后，分享了关于 [pgBackRest 项目的官方更新](https://postgresweekly.com/link/185378/rss)：*pgBackRest 将继续*，这要归功于几个重要的新赞助商的支持。

- 🇺🇸 [Postgres Summit US](https://postgresweekly.com/link/185380/rss) 的早鸟票现已开售——会议将于今年 9 月 30 日至 10 月 2 日在纽约举行。

- [Heroku Postgres Advanced](https://postgresweekly.com/link/185381/rss)，Heroku Postgres 平台的下一代版本，现在处于"有限 GA"阶段，用户需要申请访问权限。


## [Postgres 19 Beta 中你会真正*感受到*的四个特性](https://postgresweekly.com/link/185382/rss)

最终版本要到 9 月才会发布，但 beta 版即将推出。Christophe 没有关注重点特性，而是聚焦于改变*"数据库在生产环境中感觉"*的东西，比如 JIT 默认关闭和并行 autovacuum 索引工作进程。

`Christophe Pettus`


## [ORDER BY 丛林：为什么 ORDER BY 别名的行为很奇怪](https://postgresweekly.com/link/185383/rss)

`ORDER BY a` 和 `ORDER BY -a` 看起来几乎相同，但却使用了两个不同的解析器：SQL-92 名称路径和 SQL-99 表达式路径。Radim 追踪了通过别名、`GROUP BY`、窗口函数、引号标识符、`COLLATE` 和 `UNION` 的边界，直到找到负责的函数。

`Radim Marek`


📄 [在 Postgres 中构建自动、上下文化的临床试验审计日志，无需触发器](https://postgresweekly.com/link/185384/rss) – 特别使用 TypeScript 和 Drizzle。`Nathan Leung (Harbor)`

📄 [我们如何节省在索引上浪费的 40GB 空间](https://postgresweekly.com/link/185385/rss) – *"简而言之：不要随意向数据库表添加索引。"* `Ravi Ojha`


**🛠 代码和工具**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/eorbfdjkzu8ed0ytslyu.jpg)


## [plpgsql_wrap 1.0：一种混淆 PL/pgSQL 代码的方法](https://postgresweekly.com/link/185386/rss)

HexaCluster 开源了其扩展，用于分发和运行加密的 PL/pgSQL 过程，这些过程可以在不让最终用户读取的情况下进行转储和重新加载。灵感来自 [Oracle 的 'wrap' 方法](https://postgresweekly.com/link/185387/rss)。

`Gilles Darold (HexaCluster)`


## [🤖 Supabase 现在是官方 ChatGPT 应用](https://postgresweekly.com/link/185388/rss)

Supabase 现在可以与 ChatGPT 应用集成，因此你可以直接从中管理你的数据库、项目和分支。

`Greg Richardson (Supabase)`


## [pgsqlite：SQLite 数据库的 Postgres 协议适配器](https://postgresweekly.com/link/185389/rss)

一个协议适配器，使 SQLite 数据库假装成 Postgres，因此通常的 psql/pgAdmin/驱动程序堆栈可以直接使用它。

`Eran Sandler`


**分类广告：**

🧠 Postgres 警报附带诊断和建议的 SQL 修复，而不仅仅是阈值。[开源](https://postgresweekly.com/link/185390/rss)。

🐘 自托管 Postgres？[试试 ParadeDB](https://postgresweekly.com/link/185391/rss)，一个 Postgres 扩展，支持 Elasticsearch 质量的全文、向量和混合搜索。无需 ETL 管道，无需 Elastic 集群。

[使用 Aiven 的开发层级开始构建 Apache Kafka](https://postgresweekly.com/link/185392/rss)。在企业堆栈上构建，每月 35 美元。在不到 2 分钟内提供带有 100 个分区、Schema Registry 和 REST Proxy 的托管 Kafka。


![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/xdmua8qlejdtwmbie5lu.jpg)

- 📈 [pg_statviz 1.0](https://postgresweekly.com/link/185393/rss) – 用于分析和可视化 Postgres 内部统计信息的扩展和实用工具。现在具有新的 AI 驱动的分析选项。

- [Postgres Language Server 0.25](https://postgresweekly.com/link/185394/rss) – Supabase 为 Postgres 实现的语言服务器协议（LSP）。

- [SQLsmith 1.5](https://postgresweekly.com/link/185395/rss) – 随机 SQL 查询生成器，用于生成和执行各种语句以进行测试。