---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-9-21
---
### PostgreSQL每周新闻#472 - 2022年9月21日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/472)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/yunuozfyybzlxswa1zc6.jpg)
## [pg_activity 3.0：类似于HTOP的活动监控工具](https://postgresweekly.com/link/128997/web)
就像您可能使用 top 或 htop 来监控进程和 CPU 使用情况一样，pg_activity它为您提供了 Postgres 幕后的类似外观，包括正在运行的查询、最新的性能统计信息等。


`Dalibo `
## [将 Postgres 从 Heroku 迁移到 Crunchy Bridge](https://postgresweekly.com/link/128998/web)
不断发展的业务的开发人员正在寻求迁移 Postgres。他们想要一个至少和 Heroku 一样好的新供应商，拥有新的功能和开发工具。他们测试了 Amazon RDS 和其他几个。了解他们为何选择 Crunchy Bridge 用于他们的云 Postgres。阅读案例研究。


`Crunchy Data `
## [🦀 PostgresML 在 2.0 版本中迁移到 Rust](https://postgresweekly.com/link/128999/web)
使用 Rust 构建 Postgres 扩展的想法正在慢慢加快步伐。将 ML 模型训练和查询添加到 Postgres 的PostgresML扩展的创建者尝试了 Rust，并且对性能改进感到非常震惊，他们全力以赴。 


`Montana Low `
## [序列与Invoice号码](https://postgresweekly.com/link/129001/web)
Postgres序列为 ID 号码的生成提供了一个方便的抽象，那么它们肯定也适用于发票号码吗？没那么快，Hans-Jürgen 说（请注意，他指定的发票号码合法性标准因司法管辖区而异）。


`Hans-Jürgen Schönig `
## [将 Timescale Gem 与 Ruby 结合使用](https://postgresweekly.com/link/129003/web)
TimescaleDB是将 Postgres 转变为成熟的时间序列数据库的扩展，这个全面的演练演示了它在 Ruby 中的使用。


`Jônatas Davi Paganini `
## [▶明天的网络研讨会：优化 Postgres I/O 性能和成本](https://postgresweekly.com/link/129005/web)
l,null,"en


`pganalyze `
## [Postgres 数据流概述](https://postgresweekly.com/link/129006/web)
对基于 Postgres 的系统中的数据可能实际去往和来自何处的高级视图，包括缓存、连接池和缓冲区。一张图表总结了主要思想。


`David Christensen `
## [PSPG 5.5.7：为Postgres表设计的UNIX PAGER](https://postgresweekly.com/link/129010/web)
如果您使用psql，您可能less会将其用作Pager，但它不直接支持表格数据。这样做。多年来我们已经将它链接了几次，但它已经走过了漫长的道路，值得重新关注，特别是因为它现在支持来自众多数据库 CLI 工具的分页输出。另外，它让我想起了 Borland 时代的 DOS IDE，而我就是为此而努力的。


`Pavel Stehule `
## [pgenv 1.3.2：Postgres 虚拟环境管理器](https://postgresweekly.com/link/129011/web)
pgenv 是一个基于 shell 脚本的“管理器”，用于在同一系统上同时处理多个版本的 Postgres。GitHub 存储库。


`Luca Ferrari `
## [dblab：Postgres、MySQL 和 SQLite3 的交互式客户端](https://postgresweekly.com/link/129013/web)
一个跨平台（是的，包括 Windows）TUI 风格的应用程序，用于处理各种数据库系统。当然看起来与标准 CLI 客户端有很大不同！


`Daniel Omar Vergara Pérez `
# 💡本周提示


**🗓即将举办的Postgres活动**
