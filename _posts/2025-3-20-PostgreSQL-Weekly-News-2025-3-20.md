---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-3-20
---
### PostgreSQL每周新闻#591 - 2025年3月13日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/593)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/vs3ewh0adrzndfkmksby.jpg)
## [您可以让 Postgres 扩展](https://postgresweekly.com/link/167071/web)
新闻快讯：Postgres 可以扩展！在上周使用 Citus 对 1 万亿行表进行实验后，我们知道 Postgres 可以扩展，但是一旦超出某个点，使用多台机器就会成为一种潜在的复杂必需，而 PgDog 水平扩展/分片方法仅提供了一种解决方案。

`Lev Kokotov (PgDog)`

💡 继续讨论水平扩展 Postgres 的主题，Craig Kerstiens 在 [Citus：被误解的 Postgres 扩展](https://postgresweekly.com/link/167074/web)中提供了有关 Citus 提供价值的更多信息。

## [从 RIGHT JOIN 的角度考虑 MERGE](https://postgresweekly.com/link/167096/web)
RIGHT JOIN 在 SQL 中并不常见，因为您可以编写一个更通用的 LEFT JOIN 替代方案。但是，右连接语义在 MERGE 语句中起着重要作用。


`Lukas Eder`
## [当然，您可以自行实施身份验证 - 如果您讨厌空闲时间](https://postgresweekly.com/link/167070/web)
不要牺牲您的控制权。FusionAuth 可下载，可在本地开发和测试。单租户架构比纯多租户 SaaS 模型提供更好的规模和安全性，即使您通过云部署也是如此。免费试用！


`FusionAuth  `
## [排除重复主键行故障](https://postgresweekly.com/link/167075/webv)
如果一个表包含不需要的“重复行”（可能由于各种怪癖导致唯一索引损坏而发生），Greg 可以采用多步骤技术来重新控制一切。


`Greg Sabino Mullane  `

### 本周摘要：

* Robert Haas 已重新开始招募他的一对一 Postgres 贡献者指导计划的[申请](https://postgresweekly.com/link/167078/web)者。

* 🇨🇭 2025 年[瑞士 PGDay ](https://postgresweekly.com/link/167076/web)的报名现已开放。它将于今年 6 月在苏黎世附近举行，[征文](https://postgresweekly.com/link/167077/web)截止日期为 4 月 7 日。

* 🇬🇧 另外，如果您在英国，[PgDay UK 2025 的征文截止日期](https://postgresweekly.com/link/167093/web)也为 5 月 12 日。活动本身将于 9 月 9 日在伦敦举行。

* ParadeDB 的 pg_search 现已在[ ]Neon 平台上可用](https://postgresweekly.com/link/167095/web)，为 Postgres 带来更快的 BM25 驱动的全文搜索。

* 🤖 [Tembo 透露了即将推出的“自主 AI 代理”dba](https://postgresweekly.com/link/167079/web)，用于监控和管理 Postgres 部署。但是，请查看下面的代码和工具以了解这个想法的另一种看法。


## [人工智能能比你创建更好的表吗？](https://postgresweekly.com/link/167080/web)
对于最近依赖LLMs完成一些 SQL 繁重工作的人来说，这是一篇有趣的文章。与以往一样，你需要保持警惕，在将任何产品投入生产之前对其进行检查！


`Dave Stokes`
## [▶ 🎤 为什么 Python 开发人员只使用 Postgres](https://postgresweekly.com/link/167081/web)
Python 软件基金会的 Dawn Wages 与 Claire Giordano 一起讨论为什么 Postgres 在 Python 和 Django 社区特别受欢迎。


`Talking Postgres Podcast `

* 📄 [COPY 和 \COPY](https://postgresweekly.com/link/167082/web) – 同一枚硬币的两面。COPY 由服务器运行，而 \copy 是包装 COPY 的 psql 命令。Dave Stokes

* 📄 [如何使用 regexp_matches 和 regexp_match](https://postgresweekly.com/link/167083/web) Tobias McNulty

### 代码和工具：

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/pmla9yfnbjooejd6j7j3.jpg)

## [Xata Agent：Postgres 中的“AI 专家”](https://postgresweekly.com/link/167084/web)
一个开源代理，可监控您的数据库、查找问题的根本原因并提出修复和改进建议。这个领域还处于早期阶段，但看到对这个想法的不同看法很有趣。

`Xata`
## [pgFormatter 5.6：一种格式化 SQL 代码的工具](https://postgresweekly.com/link/167085/web)
您可以在线测试它，也可以从 GitHub 获取源代码（它是用 Perl 编写的）并亲自运行它。v5.6 中的新功能。

`HexaCluster`
## [pg_ivm 1.10：增量视图维护 (IVM) 扩展](https://postgresweekly.com/link/167088/web)
一种更有效的方法来增量更新物化视图，仅应用更改，而不是像 REFRESH MATERIALIZED VIEW 那样完全重新计算视图。

`HexaCluster`
## [pgzx 0.3：使用 Zig 创建 Postgres 扩展](https://postgresweekly.com/link/167089/web)
如果您熟悉使用 pgrx 使用 Rust 构建 Postgres 扩展的方法，那么在 Zig 的世界中也有类似的想法，Zig 是另一种比 Rust 更像 C 的现代系统语言。

`HexaCluster`

[IvorySQL 4.4](https://postgresweekly.com/link/167092/web) – Postgres 17.4 扩展了 Oracle 兼容功能。