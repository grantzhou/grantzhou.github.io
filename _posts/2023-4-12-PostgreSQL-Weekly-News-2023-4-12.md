---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-4-12
---
### PostgreSQL每周新闻#501 - 2023年4月12日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/501)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_308,h_100/e_make_transparent/co_white,e_outline:7/vrltbo1rhou91lmjw2rl.png)
## [Postgres JSONB 函数和运算符备忘单](https://postgresweekly.com/link/138103/web)
📄 自称是 Postgres 中各种 JSONB 函数的备忘单，其中包含每个函数的快速示例以及相关运算符。📈 PDF 链接。


`Aiven `
## [Supavisor：来自 Supabase 的 Postgres 连接池](https://postgresweekly.com/link/138105/web)
来自 Supabase Realtime 背后的人们的新 Postgres 连接池。它使用 Elixir（一种 Erlang VM/BEAM 语言）构建，专为多租户设计。它可以作为集群或作为单个节点运行。最初的基准数字很有希望。


`Supabase `
## [三个必读的极端高可用性成功案例](https://postgresweekly.com/link/138102/web)
五个 9 的正常运行时间对于任务关键型数据库至关重要。以下是电信公司、支付平台和项目管理组织如何削减成本、实现滚动维护升级并确保数据丢失保护。


`EDB `
## [SQL Maxis：为什么我们用 Postgres 队列替换 RabbitMQ](https://postgresweekly.com/link/138106/web)
数据仓库同步工具的提供商从他们的系统中删除了 RabbitMQ，并用 Postgres 支持的队列替换了它。继续阅读以了解原因，但最终他们发现 Postgres 解决方案可以提高可靠性和弹性，并且更适合他们的用例。



`Charles Chretien (Prequel) `
## [FerretDB 1.0：一种开源的 MongoDB 替代方案](https://postgresweekly.com/link/138107/web)
FerretDB 内置于 Go 中，将 MongoDB 的有线协议查询转换为由后端的 Postgres 处理的 SQL，因此您可以重现 MongoDB 的体验，而无需进行有争议的许可更改。幕后 Postgres 的另一个例子！


`Peter Farkas `
## [Postgres 16 中的并行聚合](https://postgresweekly.com/link/138120/web)
并行聚合通过分布它们来加速处理大型数据集上的聚合函数。并非所有聚合函数都支持并行化，但现在 Postgres 16 中的函数支持string_agg()并行化array_agg()


`Pavlo Golub `
## [在 Postgres 16+ 中即时更新成本限制](https://postgresweekly.com/link/138121/web)
这将通过允许更快地吸收成本限制更改来解决 VACUUM 运行速度太慢的常见问题。目前，修改限制只会影响未来的 autovacuum 操作，但在未来它将“几乎在你重新加载配置时”影响所有工作人员。


`Robert Haas `
## [以正确的方式设置 Postgres 故障转移和故障回复](https://postgresweekly.com/link/138122/web)
 “这篇博客旨在帮助初学者理解并使用故障转移和故障回复在 PostgreSQL 中设置服务器复制。” 而且，重要的是，最新的方式。


`Tristen Raab `
## [观看：如何使用 Postgres Query Planner 调试错误计划并加快查询速度](https://postgresweekly.com/link/138125/web)


`pganalyze `
## [Citus Con 之路：在公共场合工作](https://postgresweekly.com/link/138134/web)
▶作为下周Citus Con预热的一部分，多产的 Pythonista Simon Willison 和 Citus Data 的 Marco Slot 与 Claire Giordano 和 Pino de Candia 就他们在各种开源方面的工作进行了长达一个小时的对话项目。


`Simon Willison podcast`
## [Pgpool-II 用例和优势](https://postgresweekly.com/link/138123/web)
Pgpool -II是一种流行的连接池和负载均衡器。


`Kai Wagner (Percona) `
## [PL/Rust 刚刚发布：一种简单的尝试方法](https://postgresweekly.com/link/138126/web)


`Yurii Rashkovskii `
## [credcheck v1.0：凭证检查的扩展](https://postgresweekly.com/link/138127/web)
通过定义一组允许特定凭证的规则，在用户创建、密码更改和用户重命名期间启用凭证检查，可以拒绝其他凭证，并在需要时强制密码过期。GitHub 回购。


`MigOps `
# 💡本周提示


**🗓即将举办的Postgres活动**
