---
layout: post
title: PostgreSQL 每周新闻 2024-2-7
---
### PostgreSQL每周新闻#541 - 2024年2月7日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/541)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/yladwotimj1d9jqsoadf.jpg)
## [Postgres 就足够了：用 Postgres 做所有事情？](https://postgresweekly.com/link/150940/web)
它只是一个充满链接的 GitHub 要点，但依靠 Stephan Schmidt 的Just Use Postgres for Everything中传达的想法来展示可让您完成所有操作的各种项目，添加后台作业、映射、审计日志记录、矢量搜索等功能， API 服务，更直接地连接到我们最喜欢的数据库。


`Chase Pursley `
## [电子书：调整 Autovacuum 以获得最佳 Postgres 性能](https://postgresweekly.com/link/150939/web)
了解调整调度和性能设置、减少工作时间的 autovacuum 开销、xmin 范围及其阻止真空、为什么要避免反环绕真空以及如何通过调整死元组来减少膨胀阈值。


`pganalyze `
## [在 Postgres 中实现系统版本化表](https://postgresweekly.com/link/150942/web)
尽管有temporal_tables 扩展，但 Postgres 中没有对系统版本化表的官方支持，但是如果您想自己实现这个想法怎么办？三个触发器和一个索引来救援！


`Jean Niklas hyPiRion L'orange `
**本周摘要：**
*   Postgres 中对本机 UUID v7 支持的工作进展顺利，并在本周的Hacker News上引发了相当多的讨论。


*   📺 祝贺 Lukas Fittl 和pganalyze的“5 分钟的 Postgres”达到100 集，这是他们的一系列方便的小型 Postgres 视频（完整的 YouTube 播放列表）。


*   DB-Engines 将 Postgres 称为2023 年年度 DBMS，虽然 Adrien Nayrat 并不担心Postgres本身的未来，但他担心DBA 和 DBA 技能组的未来。


*   🇧🇪 2024 年比利时 PGDay将于 5 月举行，如果您想在那里发言，演讲者征集现已开放。


*   🇨🇭 2024 年瑞士 PGDay也已宣布，将于 6 月在苏黎世附近举行。它也有一个公开的演讲者征集活动。


*   Paul Ramsey 写了一些关于为今年五月在温哥华举行的PGConf.dev 会议构建程序的文章。


## [PlanSplainer：可视化查询计划的新方法？](https://postgresweekly.com/link/150960/web)
explain.depesz.com可能是用于此任务的最著名的基于 Web 的工具，但这是一个有趣的替代方案，它以更直观的方式呈现该计划。


`markmeeus `
## [IntegreSQL：用于管理独立 Postgres 数据库进行测试的 API](https://postgresweekly.com/link/150963/web)
提供 RESTful JSON API，用于管理 Postgres 模板并启动（和管理数据库池）数据库以进行集成测试。


`all about apps GmbH `
## [PGTera：渲染 Tera HTML 模板的扩展](https://postgresweekly.com/link/150964/web)
Tera是一个受 Jinja2 启发的 Rust 模板引擎，如果您需要从数据库返回完整的渲染 HTML 视图，它是另一个选择。


`Frankie Primerano `
## [pgenv：用于 Shell 的 Postgres 二进制管理器](https://postgresweekly.com/link/150966/web)
使构建和运行不同的 Postgres 版本以及在它们之间切换以进行测试等变得更简单。它刚刚获得了用于获取特定实例状态的命令。


`Ferrari, Wheeler, et al. `
## [Ibis 8.0：Python 的数据框架](https://postgresweekly.com/link/150968/web)
为 Python 中的数据整理提供通用接口，重点关注表格数据（使用数据框架）并支持所有主要数据库系统，包括 Postgres 和 SQLite。


`Ibis Developers `
## [Directus 10.9：使用实时 GraphQL 和 REST API 封装 SQL 数据库](https://postgresweekly.com/link/150970/web)
一个基于 Node.js 的系统，可以充当 Postgres、SQLite、MySQL、Oracle 和其他数据库的前端，提供现代化的仪表板、客户端、以及 REST 和 GraphQL API。


`Monospace, Inc. `
## [PgManage 1.0 RC 1](https://postgresweekly.com/link/150972/web)
 - 基于 Web 的 Postgres 管理工具。


## [Goose 3.18](https://postgresweekly.com/link/150973/web)
 - 数据库迁移工具。支持SQL和Go函数。


## [CloudNativePG 1.22.1](https://postgresweekly.com/link/150974/web)
 - Postgres 的 Kubernetes 运算符。


## [data-diff 0.11](https://postgresweekly.com/link/150975/web)
 - 比较数据库内或跨数据库的表


## [pgBouncer 1.22.0](https://postgresweekly.com/link/150976/web)
 - 流行的连接池。


## [PGXN 工具 Docker 镜像改进。](https://postgresweekly.com/link/150977/web)




# 💡本周提示


**🗓即将举办的Postgres活动**
