---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-9-27
---
### PostgreSQL每周新闻#523 - 2023年9月27日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/523)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/no4bngifotliu86h9gig.jpg)
## [选择 Postgres 的队列技术](https://postgresweekly.com/link/145500/web)
如果 Postgres 本身就是一个出色的发布/订阅和任务服务器，那么为什么将其用作服务器会被称为“hacky”？为什么大多数流行的后台任务库都使用 Redis？ Adriano 鼓励我们考虑权衡，并考虑像 Postgres 这样的“无聊技术”何时能够准确地满足您的用例的需求。


🗣 Adriano 的帖子引发了广泛的 Hacker News 讨论，许多人分享了有关可扩展性、LISTEN/NOTIFY 的潜在缺点、队列事务的好处、为什么人们不喜欢 RabbitMQ 等的故事和观点。

`Adriano Caloiaro `
## [Postgres 16 中 JSON 功能的更新](https://postgresweekly.com/link/145504/web)
快速地了解一些新功能，包括 IS JSON_OBJECT、JSON_ARRAY()、JSON_ARRAYAGG()、JSON_OBJECT() 和 JSON_OBJECT()


`Christopher Winslett `
## [PostgreSQL 的开源云替代品。 免费开始，并获得 300 美元积分](https://postgresweekly.com/link/145499/web)
利用完全托管的 Postgres 加快创新速度，现已提供高可用性和分布式功能 — 可以在您需要时随时联系顶级 Postgres 专家。


`EDB BigAnimal `
## [📊 幻灯片：Postgres 16 的主要功能](https://postgresweekly.com/link/145505/web)
尊敬的 Postgres 专家 Bruce Momjian 发布了一个易于浏览的幻灯片，涵盖了 Postgres 16 中最重要的改进和功能。


`Bruce Momjian `
## [Timescale Vector：Timescale 如何增强其托管 Postgres 云的 pgvector](https://postgresweekly.com/link/145506/web)
Timescale 人员因在 TimescaleDB 上为 Postgres 带来时间序列数据功能而闻名，他们已将注意力转向向量。 Timescale Vector 目前仅在 Timescale 平台上可用，它通过受 DiskANN 启发的索引方法增强了 pgvector。

🔗 LLM 框架 LangChain 已经宣布支持 Timescale Vector，并发布了一篇文章，更深入地介绍了用例。


`Timescale Team `
**本周摘要：**
*   🔢 Peter Eisentraut 讲述了他如何将数字分组支持引入 SQL 标准（例如 1_000_000），然后引入 Postgres（在 Postgres 16 中提供）的故事。


*   ⭐️ Oracle，是的，那个 Oracle，正在进入 Postgres 托管游戏。 它被认为是一个自然的进步，因为 Oracle Cloud 已经在 Redis 和 OpenSearch 等开源项目之上提供了服务。


*   如果您需要帮助参加下个月的 PGConf NYC，还有两天时间申请 PostgresUS 多样性奖学金。


*   ElectricSQL 是一个构建在 Postgres 之上的新型反应式实时同步层。 将其放入现有的基于 Postgres 的系统中，并将即时本地优先数据同步到您的应用程序中。


## [🎲 使用 Postgres 的随机函数掷骰子](https://postgresweekly.com/link/145516/web)
生成随机数、选择随机行、处理正态分布（通过 Postgres 16 的 random_normal 函数）的示例，以及 Postgres 的“随机”值到底有多随机（或不随机）。


`Paul Ramsey `
## [逻辑复制的演变](https://postgresweekly.com/link/145517/web)
关于Postgres支持逻辑复制的进展的全面摘要，从9.4年前的Postgres中引入逻辑解码到Postgres 16中的最新添加。


`Amit Kapila `
## [设置每用户服务器变量](https://postgresweekly.com/link/145518/web)
Postgres 可以使用大量参数进行配置，其中许多参数可以在运行时更改，其中一些参数仅适用于超级用户。 Postgres 15 添加了使用 GRANT 来让非超级用户更改超级用户限制的服务器变量的功能。


`Bruce Momjian `
## [\watch 的 Postgres 16 改进](https://postgresweekly.com/link/145519/web)
您现在可以指定在停止之前希望它迭代多少次。


`Luca Ferrari `
## [在 GitHub 操作中获取 Postgres 日志](https://postgresweekly.com/link/145520/web)

`BRANDUR LEACH`

## [使用 Citus 监控 Postgres 的性能](https://postgresweekly.com/link/145521/web)

`HANS-JÜRGEN SCHÖNIG`

## [在 Postgres 中捕获变化的所有方法](https://postgresweekly.com/link/145522/web)

`ANTHONY ACCOMAZZO (SEQUIN)`

## [Postgres 16：令人兴奋和不被注意的地方](https://postgresweekly.com/link/145523/web)

`SAMAY SHARMA (TEMBO)`


**代码和工具：**
## [Instant.dev：一个新的以 Postgres 为中心的 JavaScript ORM](https://postgresweekly.com/link/145524/web)
Instant 是一个新发布的 ORM，它是从 Autocode 平台衍生出来的，旨在提供更多 Ruby on Rails/Active Record 风格的体验，使其在日益增长的市场中与大多数其他参与者区分开来。 丰富的 JavaScript ORM 生态系统。


`instant․dev `
## [我们如何使 PostgreSQL 成为更适合 AI 应用的矢量数据库](https://postgresweekly.com/link/145526/web)



`TIMESCALE`
## [Citus 12.1 发布，支持 Postgres 16](https://postgresweekly.com/link/145527/web)
Microsoft 的分布式 Postgres 扩展又向前迈出了一步，增加了 Postgres 16 支持。 发行说明。


`Citus Data `
## [如何尝试 OrioleDB](https://postgresweekly.com/link/145529/web)
OrioleDB 是 Postgres 的替代存储引擎，目前处于测试阶段。 马克分享了他如何运行它的笔记。


`Mark Callaghan `