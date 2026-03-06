---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-7-17
---
### PostgreSQL每周新闻#556 - 2024年7月17日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/562)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/xdevwityrinadlvs7ujg.jpg)
## [谁负责 Postgres？](https://postgresweekly.com/link/157631/web)
Postgres 与许多数据库不同，它不直接受推动其发展的仁慈领导者或公司的控制。它有一个核心团队，PostgreSQL 社区协会拥有商标，但谁是“负责人”？Bruce 建议，我们所有人都是。


⚠️ 在本文的电子邮件版本中，我们在商标持有人方面犯了一个错误。下周的版本将发布正确的更正。感谢 Jonathan Katz 强调这一点！


`BRUCE MOMJIAN `

## [Postgres 可以替代 Redis 作为缓存吗？](https://postgresweekly.com/link/157632/web)
Redis 是一种流行的高性能内存数据存储服务器，常用于缓存，但如果我们可以“将 Postgres 用于一切”，那么 Postgres 是否可以代替它完成这项工作？ Raphael 进行了调查。


`RAPHAEL DE LIO `
## [Honeybadger 的全栈可观察性](https://postgresweekly.com/link/157630/web)
Honeybadger 的新日志平台有点像 Splunk、DataDog 或 CloudWatch Logs，但具有优秀的组件和合理的价格。此外，它还易于与 Crunchy Bridge、Journald、AWS 等集成！


`HONEYBADGER  `
## [自动清理调优基础知识](https://postgresweekly.com/link/157634/web)
手动运行 VACUUM 回收删除和更新行而导致的表中浪费的空间/膨胀。然而，自动清理系统会替我们完成这项工作，并且可以根据您的情况进行调整，以获得正确的空间/性能权衡。


`TOMAS VONDRA  `

### 本周摘要：

* 🇬🇧 [PGDay UK 2024 已公布其时间表](https://postgresweekly.com/link/157635/web)——它将于今年 9 月在伦敦举行，现已开放[报名](https://postgresweekly.com/link/157636/web)。

* 🇺🇸 [PASS Summit](https://postgresweekly.com/link/157649/web) 数据库活动也将于今年 11 月重返西雅图。他们在这里公布了 [Postgres 专业阵容](https://postgresweekly.com/link/157650/web)。

* Amazon RDS Data API for Aurora PostgreSQL [现已在另外 10 个 AWS 区域可用](https://postgresweekly.com/link/157637/web)。

* 无服务器 Postgres 平台 Xata 引入了[多版本架构迁移](https://postgresweekly.com/link/157638/web)。

* Ubicloud 的 [Ozgun Erdogan](https://postgresweekly.com/link/157639/web) 是本周 PostgreSQL 人物的受访者。

### 🛠 代码和工具

## [使用 AI 为 Postgres 生成数据结构](https://postgresweekly.com/link/157640/web)
我们可能还需要一段时间才能信任 LLM 和 AI 模型来诊断疾病或运行发电厂，但在帮助您定义模型和模式方面，它们可以快速为您指明正确的方向。


`HANS-JÜRGEN SCHÖNIG `

## [▶ 讨论 Postgres 初创企业生态系统](https://postgresweekly.com/link/157641/web)
Postgres FM 播客的 Nikolay 和 Michael 讨论了围绕 Postgres 迅速变化和增长的商业生态系统，包括 Neon、Tembo 和 Aiven 等公司。（35 分钟）


`POSTGRES․FM`

## [按降序排列的键集分页](https://postgresweekly.com/link/157643/web)
一些解决您在使用 SQL 时可能遇到的有趣的排序和分页问题的解决方法。


`LAURENZ ALBE`
📄 [使用 Postgres 进行系统日志聚合](https://postgresweekly.com/link/157644/web) – 谈论使用 Postgres 做所有事情 - JAKUB KOŁODZIEJCZAK

📄 [使用 pg_easy_replicate 设置逻辑复制和切换](https://postgresweekly.com/link/157645/web) - SHAYON MUKHERJEE

📄 [维护扩展统计数据的成本有多高？](https://postgresweekly.com/link/157646/web) - ANDREI LEPIKHOV

📄 [将 DuckDB 放入 Postgres 来查询 Iceberg](https://postgresweekly.com/link/157647/web) - MING YING (PARADEDB)

📄 [如何在 AWS 上安装 TimescaleDB](https://postgresweekly.com/link/157648/web) - JUAN JOSE (TIMESCALE)

