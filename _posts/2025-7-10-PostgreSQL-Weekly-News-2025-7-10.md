---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-7-10
---
### PostgreSQL每周新闻#607 - 2025年7月10日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/607)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/gqtuz5pep7m41a7lnblp.jpg)
## [SIGTERM 不作为：Postgres 之谜](https://postgresweekly.com/link/171587/web)
ClickHouse 的一个团队在read replica中遇到了一个 bug，该 bug 导致复制设置命令无限期挂起并忽略取消请求，从而导致管道停滞和磁盘占用率上升。不过，最终问题得到了解决，原因已确定，并且已向 Postgres 的维护版本发布了补丁，现在我们可以安全地再次中断read replica上的复制了。

`Kevin Biju Kizhake Kanichery (ClickHouse)`

## [使用 Atlas 驯服复杂的 PostgreSQL 模式](https://postgresweekly.com/link/171586/web)
受 Terraform 的启发，Atlas 为模式迁移提供了一种声明式方法，使团队能够将其模式定义为代码并自动执行规划、验证和部署。


`atlasgo.io `

## [将 Jira 数据库平台迁移到 AWS Aurora](https://postgresweekly.com/link/171272/web)
Atlassian 的 Jira 使用 Postgres，每个用户都有自己的数据库。数百万用户意味着数百万个数据库，将分布在 3,000 台 Postgres 服务器上的 400 万个数据库迁移到 AWS Aurora 绝非易事。

`Pat Rubis (Atlassian) `

### **本周摘要**

* [Fly.io](https://postgresweekly.com/link/171589/web) 应用托管平台已[推出 Postgres 托管服务](https://postgresweekly.com/link/171590/web)。

* [Josef Machytka](https://postgresweekly.com/link/171591/web) 是本周 PostgreSQL 人物的采访对象。

* 🇬🇧 [PGDay UK 2025 ](https://postgresweekly.com/link/171592/web)的日程安排已公布。该活动将于 9 月 9 日在伦敦举行。

## [那么我们为什么不选择最佳查询计划呢？](https://postgresweekly.com/link/171593/web)
探讨潜在的过时的默认值（random_page_cost）如何经常导致次优的索引扫描选择，以及我们可以采取哪些措施来缓解它。

`Tomas Vondra)`


## [掌握复制槽：防止 WAL 膨胀和其他生产问题](https://postgresweekly.com/link/171594/web)
Gunnar 警告说，复制槽有时可能会导致数据库保留大量的预写日志 (WAL) 段。他分享了防止这种情况发生的最佳实践，并介绍了一些关于心跳、复制槽故障转移、监控等方面的良好实践。


`Gunnar Morling`

## [pgsqlite：用于 SQLite 数据库的 Postgres 协议适配器](https://postgresweekly.com/link/171595/web)
一种让 Postgres 客户端能够像连接 Postgres 数据库一样连接并查询 SQLite 数据库的方法。目前处于“实验阶段”。


`Eran Sandler`

* 📄 [Postgres 即将推出：磁盘数据库加密](https://postgresweekly.com/link/171596/web) Lindsay Clark（The Register）

* 📄 [大数据的唯一索引处理](https://postgresweekly.com/link/171597/web) Volodymyr Potiichuk

* 📺 [将 Postgres 同步到客户端](https://postgresweekly.com/link/171598/web) James Arthur

### **🏆 2025 年的热门链接（迄今为止）**

由于这是 Postgres 世界中特别安静的一周，而且我们大约已经度过了一年的一半，因此我们想快速总结一下今年迄今为止最受欢迎的 Postgres Weekly 项目，以防您当时错过它们：


## [1. 改变生活的 Postgres 模式](https://postgresweekly.com/link/171599/web)
作者承诺标题不仅仅是点击诱饵，还提供了十二个不同的简短、来之不易的技巧和见解，涵盖了从使用 UUID 作为主键和表命名到使用模式和视图等领域。

`Ethan McCue`


## [2. 微软在 VS Code 中为 Postgres 推出全新“IDE”](https://postgresweekly.com/link/171600/web)
微软刚刚于两个月前发布了 VS Code 编辑器 Postgres 扩展的公开预览版，该扩展允许你管理数据库对象、使用 IntelliSense 构建查询以及与 Copilot 集成。▶️ Matt McFarland 在 POSETTE 2025 演讲中精彩地展示了它。

`Microsoft`


## [3. 不要这样做（在 Postgres 中）](https://postgresweekly.com/link/171602/web)
我们每隔一两年就会在 Postgres 官方 wiki 上链接到这个有趣的页面，它一直很受欢迎！该页面汇总了使用 Postgres 时“常见错误”以及不该做的事情的各种建议。希望随着时间的推移，能看到更多内容的添加。

`Postgres Wiki`


## [4. Postgres 18 Beta 发布：7 个需要了解的功能](https://postgresweekly.com/link/171603/web)
我们仍在等待 Postgres 18 的最终版本，该版本将在未来几个月内发布，但第一个测试版已于 5 月初发布，Heikki 分享了一些他期待的事情。

`Heikki Linnakangas (Neon)`


## [5. 如何修复 Postgres 中查询速度慢的常见原因](https://postgresweekly.com/link/171605/web)
严格来说，这是 2024 年的条目，但我们早在 1 月份就首次链接到它了！Render 云平台的一位数据库工程师展示了一个常见但很容易修复的性能问题，该问题是由外键缺少索引引起的。

`Eric Fritz`


## [6. Citus 数据库能达到 1 万亿行？](https://postgresweekly.com/link/171606/web)
“Postgres 的扩展性很强”，但究竟能达到什么程度呢？Hans-Jürgen 决定一探究竟，他做了一个小实验（或者说大实验），看看 1 万亿行的表是否可行。

`Hans-Jürgen Schönig`


## [7. Postgres 查询计划可视化工具汇总](https://postgresweekly.com/link/171607/web)
EXPLAIN 命令及其众多选项可让您深入了解 Postgres 的查询执行计划，并且是找出某些查询运行缓慢原因的好方法。虽然原始输出可能难以阅读，但有几种工具可以帮助您分解这些内容。

`Michael Christofidese`

## [8. OpenAI 如何将 Postgres 扩展至更高水平](https://postgresweekly.com/link/171610/web)
OpenAI 工程师 Bohan Zhang 在 PGConf.dev 上的演讲记录，讲述了 OpenAI 如何通过非分片方法（仅使用一个写入器和多个读取器）实现扩展，尽管 Postgres 是“OpenAI 最关键系统的骨干”。如果这对他们来说足够好……

`PixelsTech / Lao Feng`

