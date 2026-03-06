---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-6-14
---
### PostgreSQL每周新闻#510 - 2023年6月14日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/510)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_350,h_100/e_make_transparent/co_white,e_outline:7/lhwcvgc1asd4fzaahty4.png)
## [让我们让Postgres多线程化？](https://postgresweekly.com/link/140992/web)
🗣受 PGCon 上一些对话的启发，Postgres 贡献者 Heikki Linnakangas 对将 Postgres 从多进程世界转变为使用多线程的单进程世界的想法感到兴奋。不要兴奋；如果发生的话，这将是一项艰巨的任务。反应不一：Tom Lane预测灾难，尽管 Robert Haas 表示支持，但认为基于流程的模型可能需要在未来很长一段时间内保留为一种选择。


`Heikki Linnakangas `
## [任何规模的 Postgres 性能](https://postgresweekly.com/link/140991/web)
通过智能调优顾问和持续的数据库分析提供一致的数据库性能和可用性。控制您的 Postgres 工作负载和查询计划，并授权所有开发团队修复缓慢的查询。立即尝试 pganalyze！


`pganalyze `
## [将Google Sheets数据远程加载到Postgres中](https://postgresweekly.com/link/140995/web)
从 Google 表格中以 CSV 格式获取数据非常简单，但是如何将该 CSV 文件导入 Postgres 数据库呢？有几个选项可以COPY直接通过 HTTP（带有扩展）、FDW 或什至启动一些 PL/Python 来完成这项工作。


`Paul Ramsey `
## [使用 HypoPG 在 Amazon RDS 中构建假设索引](https://postgresweekly.com/link/141017/web)
HypoPG是 Postgres 的一个有趣扩展，它让您假装某些索引存在，但它们不存在，以便查看 Postgres 是否会使用它们。本教程针对 RDS，但这个想法可以在任何地方使用


`Peter Celentano `
## [将 SQL Server 数据库迁移到 Aurora PostgreSQL 的 Babelfish](https://postgresweekly.com/link/141000/web)
PostgreSQL 的 Babelfish包括对 T-SQL 和 SQL Server 线协议的支持，因此可以使用 AWS 的“批量复制程序”实用程序将 SQL Server 数据库迁移到 Babelfish。


`Fernandes, Valentim, and Carvalho Queiroz (AWS) `
## [使用pgBadger自动填写已准备的对账单占位符](https://postgresweekly.com/link/141005/web)
pgBadger是一个Postgres日志分析器，具有特定功能，可以以绑定参数直接插入查询的格式从日志文件中转储所有查询。


`Kaarel Moppel `
## [云上PostgreSQL的开源替代方案。注册以获得早期访问](https://postgresweekly.com/link/141007/web)


`EDB BigAnimal `
## [Suabase Vector：一个面向Postgres和Python的开源向量工具包](https://postgresweekly.com/link/141008/web)
最近每个人都想存储嵌入矢量以用于 ML 驱动的搜索，而 pgvector 使使用 Postgres 变得容易。Supabase 更进一步，通过他们的云平台和 Python 库将其全部包装起来。还有使用它构建图像搜索功能的教程（ ▶️视频版本）。。


`Supabase `
## [credcheck v2.0：凭据检查扩展](https://postgresweekly.com/link/141011/web)
credcheck 可以强制执行有关使用安全凭证进行用户创建、密码更改和用户重命名的规则。v2.0 添加了 Postgres 16 兼容性，以及在用户被禁止之前限制身份验证失败尝试次数的功能。


`Gilles Darold `
# 💡本周提示


**🗓即将举办的Postgres活动**
