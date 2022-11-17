---
layout: post
title: PostgreSQL 每周新闻 2022-11-16
---
### PostgreSQL每周新闻#481 - 2022年11月16日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/481)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_300,h_160/e_make_transparent/co_white,e_outline:7/rrkstxca0vg7e1eww6yw.jpg)
## [在 Postgres 15 中通过 I/O 并发减少复制滞后](https://postgresweekly.com/link/131671/web)
Postgres 15 具有关键的复制改进，但为实现这一目标所做的工作很深入。这篇文章解释了 IO 并发性如何影响复制滞后，还讲述了 Postgres 的 IO 故事如何随着时间的推移而改进，并戏弄了一个未来，数据将异步传输到 Postgres 的缓冲区中，完全避免内核。“我们只触及了表面，” Thomas 说


`Thomas Munro (Microsoft) `
## [将 Postgres 与 Deno Deploy 结合使用](https://postgresweekly.com/link/131670/web)
在边缘访问 Postgres 数据带来了多区域连接和延迟方面的新挑战。了解如何使用 PolyScale 的即插即用数据库边缘缓存在几分钟内解决这些问题。


`PolyScale.ai `
## [PostgreSQL 15.1、14.6、13.9、12.13、11.18 和 10.23 已发布](https://postgresweekly.com/link/131672/web)
维护发布行的一系列错误修复版本。没有一个特别突出的错误，但在这篇文章中列出。由于各个国家/地区的 DST 更改，我们还会获得时区数据更新。它还标志着最终的 v10 版本。


`PostgreSQL Global Development Group `
## [向 2017 年的 Postgres 10 致敬](https://postgresweekly.com/link/131673/web)
在 Postgres 每次主要发布五年后，潮流开始退去，该版本在最终告别发布后达到“生命终结”（EOL）（版本控制政策文档中有关此的更多信息。）Jonathan沉迷于对 Postgres 的“变革性”版本的怀旧，它引入了逻辑复制、声明性分区和 SCRAM 身份验证。


`Jonathan Katz `
## [解释该参数化语句](https://postgresweekly.com/link/131678/web)
EXPLAIN（ANALYZE，BUFFERS）的输出总是有用的，但对于参数化语句来说可能很难获得。除非你的后兜里有 Laurenz 的一些小贴士……


`Laurenz Albe `
## [什么是“Upsert”，什么时候应该使用它？](https://postgresweekly.com/link/131679/web)
这来自 CockroachDB，但通过INSERT ON CONFLICT. （Postgres 15MERGE提供了另一种方法。）


`Charlie Custer `
## [免费电子书：如何为您的查询创建最佳Postgres索引](https://postgresweekly.com/link/131681/web)


`pganalyze `
## [升级前阅读：选择Postgres版本的最佳实践](https://postgresweekly.com/link/131682/web)
关于何时考虑升级 Postgres 版本的思考以及开始这样做之前要问的问题。（作为 Timescale 文章，确实推荐了 Timescale 自己的托管服务，但在最后。）


`Laurence, Roybal and Godeke (Timescale) `
## [PostgreSQL中的JSON：终极指南](https://postgresweekly.com/link/131683/web)
我在本周整理一些 JSONB 查询时遇到了这个问题，发现它很有用。


`Ben Brumm `
## [大规模Postgres：运行多个PgBouncer](https://postgresweekly.com/link/131684/web)
使用pgBouncer的连接池很棒，但在特别高的负载下，运行多个pgBouncer 有好处。


`Elizabeth Christensen `
## [如何在Amazon RDS或Aurora上从IBM Db2重新创建ROW CHANGE TIMESTAMP](https://postgresweekly.com/link/131686/web)
在 Db2 中，创建的列ROW CHANGE TIMESTAMP始终包含上次修改该行的时间戳。你也可以在 Postgres 中这样做吗？触发救援。


`Amazon Web Services `
## [改进的 Aarch64 (arm64) 支持现在可在 Postgres RPM 存储库中使用](https://postgresweekly.com/link/131688/web)
您已经能够安装 aarch64/ARM64 架构的 Postgres rpm 包已有一段时间了，但是一些重点已经放在了完整的 RHEL 9 支持上，改进了对 RHEL 的支持和修复7 和 8，等等。


`David Detter `
# 💡本周提示


**🗓即将举办的Postgres活动**
