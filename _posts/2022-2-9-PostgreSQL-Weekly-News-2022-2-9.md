---
layout: post
title: PostgreSQL 每周新闻 2022-2-9
---
### PostgreSQL每周新闻#441 - 2022年2月9日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/441)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/chynsd5ggmdlspllqaas.jpg)
## [PostgreSQL Wire 兼容性的世界](https://postgresweekly.com/link/119478/web)
你会注意到现在有多少数据库系统和数据库工具可以“使用 Postgres”，即使它们在底层完全不同（例如 Aurora、Cloud Spanner）——并且与 Postgres 的兼容有线协议是其中的关键。本文快速了解这意味着什么。


`Phil Eaton `
## [放慢速度，让它们运行得更快](https://postgresweekly.com/link/119479/web)
▶几天前在 FOSDEM 2022 上发表的关于 Postgres 如何处理高并发情况以及连接池如何缓解许多争用问题的演讲。


`Jimmy Angelakos `
## [使用 PostgreSQL 检索最新数据的 5 种方法](https://postgresweekly.com/link/119480/web)
🎓获取用于检索数据库中每个项目的最新值的五种常用方法。最后简要讨论索引如何发挥作用，并且似乎并不总是像您期望的那样帮助查询。


`Timescale `
## [清理更新量大的表](https://postgresweekly.com/link/119481/web)
由于 Postgres 允许您为每个表设置不同的 VACUUM 参数，因此当涉及到比平均更新更多的表时，您可以了解具体情况。


`Alexei Kozlov `
## [如何在 Amazon Linux 2 上安装 Postgres 14 Plus 'contrib'](https://postgresweekly.com/link/119482/web)
我还不需要这样做，但显然安装 Postgres 14 及其contrib包非常棘手，需要进行演练。


`the gabriellephant `
## [五种方法来选择最近的记录（许多项目）](https://postgresweekly.com/link/119484/web)
看看五种不同的方法，用于快速有效地检索 Postgres 数据库中每个项目的最新数据。（鉴于这是来自 Timescale，您可能不会对其中一种解决方案仅适用于 TimescaleDB 感到惊讶 :-)）


`Ryan Booz (Timescale) `
## [将 Pinterest 的 iOS 构建迁移到 Autoscaled EC2 Mac](https://postgresweekly.com/link/119485/web)
l,null,"en


`Buildkite `
## ['超越 Postgres？继续使用 Postgres..'](https://postgresweekly.com/link/119486/web)
这篇文章向我们介绍了Hydra，本质上是智能中间件，它可以将查询路由到相关的后端数据库（包括 OLAP 系统），同时仍然在任何地方使用与 Postgres 兼容的 SQL。


`Joseph Sciarrino `
## [PgCat：用 Rust 重写的 PgBouncer，带有分片和更多功能](https://postgresweekly.com/link/119488/web)
创建者说“我认为将 Pgbouncer 提升到一个新的水平会很酷”，因此淘汰了 Rust 并构建了一个带有分片、负载平衡的 PgBouncer 克隆，和故障转移支持。不过，它处于 alpha 阶段，不建议用于生产。


`Lev Kokotov `
## [pg_timetable 4.4 发布：Postgres的高级作业调度](https://postgresweekly.com/link/119489/web)
最新的4.4.0 版本为外部工具添加了一个 REST API 来执行监控、健康检查和其他维护。


`CYBERTEC PostgreSQL International GmbH `
# 💡本周提示


**🗓即将举办的Postgres活动**
