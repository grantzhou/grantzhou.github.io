---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-2-22
---
### PostgreSQL每周新闻#494 - 2023年2月22日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/494)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_600,h_120/e_make_transparent/co_white,e_outline:7/a2rxjszdlb7fvtwyasiz.png)
## [使用 SQL 和 Mermaid 创建实体关系 (ER) 图](https://postgresweekly.com/link/135699/web)
Mermaid是一个强大的图表工具，可以将基本文本格式（这里是ER 图的工作原理）转换为完全呈现的可视化图表。你能从 SQL 中动态生成这样的标记供 Mermaid 渲染吗？是的。


`Pavlo Golub `
## [对架构师、构建和部署 HA Postgres 的专家支持](https://postgresweekly.com/link/135698/web)
无论您是需要构建前咨询，希望我们为您构建 HA 基础设施，还是正在寻找持续的构建后支持，Percona 都可以帮助您实现 HA 目标。


`Percona `
## [65 行 SQL 中的类型约束](https://postgresweekly.com/link/135703/web)
在 Postgres 中创建经过验证的数据类型并不是特别困难，并且可以派上用场来实施您的特定模式。Oliver 演示了如何创建一个类型来表示语义版本号。


`Oliver Rice (Supabase) `
## [Unlogged Tables：更快，但不太可靠，Tables](https://postgresweekly.com/link/135704/web)
如果您的用例可以处理缺点，Postgres 中的 Unlogged tables 可以给您带来很大的性能提升，正如 Greg 在这里探讨的那样。也许将它们视为持久临时表？


`Greg Sabino Mullane `
## [对象所有权和默认权限](https://postgresweekly.com/link/135705/web)
涵盖所有权和默认权限的概念，解释如何通过为特定对象提供适当数量的访问权限，将它们用于有效管理数据库中的权限和安全性。


`Ryan Booz `
## [与 Álvaro Hernandez 一起不断发展的 Postgres 生态系统](https://postgresweekly.com/link/135711/web)
与 Álvaro 的 35 分钟播客，他是 Postgres 服务公司 OnGres 的创始人，以对社区的贡献而闻名。他谈到了在 Kubernetes 上运行 Postgres、工具的复杂性以及作为生态系统核心的 Postgres 有线协议。


`Screaming in the Cloud podcast`
## [▶   Postgres 系统列解释](https://postgresweekly.com/link/135712/web)
一段 25 分钟的视频，深入探讨了 ctid、xmin 和 xmax 列。这些是可以在调查事务行为时使用的系统列。有趣的挖掘！


`Hussein Nasser `
## [PgManage 1.0a：Postgres 的 GUI 管理工具](https://postgresweekly.com/link/135717/web)
看似废弃的 OmniDB 的一个新分支，它是一个用于管理 Postgres 9.6–15 的跨平台命令行工具。GitHub 回购。 （由于未签名，在 macOS 上运行有点痛苦，但它处于 alpha 阶段。）


`CommandPrompt Inc. `
## [TimescaleDB 2.10：时间序列数据库扩展](https://postgresweekly.com/link/135719/web)
现在有了完整的 Postgres 15 支持，重新设计了压缩的工作方式（显着提高了INSERT速率），您现在可以在连续聚合中使用连接。


`Timescale `
## [DevOps 工具初学者指南](https://postgresweekly.com/link/135720/web)


`Akamai Connected Cloud `
## [Postgres 的 SQLite 外部数据包装器](https://postgresweekly.com/link/135721/web)
支持 Postgres 11-15 和最近的 SQLite 版本。需要 Linux 或 POSIX 兼容系统。


`PGSpider `
## [pg-semver：语义版本数据类型](https://postgresweekly.com/link/135722/web)
语义版本 2.0.0 规范指定的版本号格式的实现。


`David E. Wheeler, et al. `
# 💡本周提示


**🗓即将举办的Postgres活动**
