---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 June 12, 2024
---
### PostgreSQL每周新闻#558 - 2024年6月12日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/558)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/meagz6djfwwanjeofumi.jpg)  

  
[如何充分利用 Postgres 的内存设置](https://postgresweekly.com/link/156246/web "tembo.io") — Samay
Samay Sharma说得比我好： “我的同事为 Postgres 写了我见过的最全面的内存优化指南之一！它讨论了不同的组件、它们的用途、如何优化它们以及如何将它们组合在一起。”_

Shaun Thomas (Tembo)  
  
[![](https://copm.s3.amazonaws.com/2701c80b.png)](https://postgresweekly.com/link/156245/web)

[立即注册：使用 EXPLAIN 优化慢速查询以修复错误的查询计划](https://postgresweekly.com/link/156245/web "us02web.zoom.us") — The
本次网络研讨会的重点是教授使用 EXPLAIN ANALYZE 优化慢速查询的基本技能，教您在调试查询时会遇到的反模式，并为您提供有关如何解决常见问题的实用建议。

pganalyze sponsor  
  

[如何提升 Postgres 的矢量性能`pgvectorscale`](https://postgresweekly.com/link/156248/web
"www.timescale.com") — 这要归功于 Timescale 推出的一款名为pgvectorscale的新开源 Postgres 扩展，它通过 StreamingDiskANN 索引和统计二进制量化进行了增强。即使与专用矢量存储系统相比，其效果也非常显著。 pgvector

Sewrathan, Pruitt, and Arye (Timescale)  
  
  
🤖 对于 Timescale 来说，这真是相当不平凡的一周，因为他们宣布了 [
`pgai`](https://postgresweekly.com/link/156250/web), 一项更通用的扩展，用于将 AI 驱动的工作流程引入 Postgres。
  
  
**QUICK BITS:**

  * 📅 [微软的 POSETTE Postgres 活动](https://postgresweekly.com/link/156251/web) 正在举行。它是免费的，而且完全在线，因此您仍然可以加入并查看今天和明天的会议。

  * 🌍 核心贡献者 Robert Haas [反思了 Postgres 在社区、多样性和参与度方面的一些剩余问题](https://postgresweekly.com/link/156252/web) 并希望更多来自世界各地的人参与到 Postgres 的组织中。

  * 🇬🇷 [PGConf.EU 2024](https://postgresweekly.com/link/156253/web) 将于今年 10 月在希腊举行。如果您想发言，可以向其征文活动[提交演讲](https://postgresweekly.com/link/156254/web)。提交截止日期为 7 月 1 日。

  * 流行的现代托管平台 Render 即将为其[Postgres 服务提供灵活的扩展计划](https://postgresweekly.com/link/156255/web)。 时间点恢复也将出现在所有付费数据库中

  * 🐘 为了向 Postgres 的吉祥物 Slonik 致敬，EDB 与 Sheldrick Wildlife Trust 合作 [收养了 150 头孤儿大象](https://postgresweekly.com/link/156256/web)。

  
  
[如果使用默认区域设置，速度会降低多少？](https://postgresweekly.com/link/156257/web "www.depesz.com") — A
使用不同排序规则提供程序和排序规则的几种设置的基准测试。令人惊讶的是，它可以产生如此大的差异。

Hubert depesz Lubaczewski  
  
  
[使用 Postgres 对结构化数据进行 RAG](https://postgresweekly.com/link/156258/web
"techcommunity.microsoft.com") — Pamela 展示了一种基于 Python、React 和 Postgres 的方法，该方法使用从 Postgres 表中检索的数据来创建混合搜索系统。

Pamela Fox  
  
  
[对 Amazon RDS for PostgreSQL 部署选项进行基准测试](https://postgresweekly.com/link/156259/web "aws.amazon.com") — A
RDS for PostgreSQL 单可用区数据库实例、多可用区数据库实例和 Amazon RDS 多可用区数据库群集部署之间的性能比较。

Andrea Caldarone (AWS)  
  
  
🔈 [赞助社区](https://postgresweekly.com/link/156260/web) – 与微软的 Claire Giordano 的播客访谈，重点介绍人们可以为 Postgres 社区做出贡献的方式。 Postgres FM

📄 [使用SEMAB TARIQ的性能影响ORDER BYLIMIT](https://postgresweekly.com/link/156261/web) Semab Tariq

📄 [调整 Postgres 以减少 SSD 磨损 ](https://postgresweekly.com/link/156262/web) Yellow Rubber Duck  
  
  
📰 分类广告 
  
🆙 通过无缝管理面板处理 Postgres 数据库等的所有数据。尝试[Rocketadmin](https://postgresweekly.com/link/156263/web)的无编码后台解决方案 。


* * *

🤖 超级pgvector粉丝？[AI 工程师世界博览会](https://postgresweekly.com/link/156264/web) 将于 6 月 25 日至 27 日在旧金山举行，届时将有大量 ML、AI 和矢量存储专家出席。您可以 [在此处享受 30% 的门票折扣](https://postgresweekly.com/link/156265/web)
，或者在[主页底部](https://postgresweekly.com/link/156264/web)注册免费远程门票/直播。

* * *

🙋 有关人工智能工程师世界博览会的更多信息，Postgres Weekly 的编辑 Peter Cooper 将会出席，所以如果你参加的话，去打个招呼吧！ 
  
  
🛠 代码和工具 
  
[![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/yucuphklse6eu4fgmsdy.jpg)](https://postgresweekly.com/link/156266/web)  
  
[PG Ferret：Postgres 的一体化跟踪工具包](https://postgresweekly.com/link/156266/web "github.com") — A new
一个前景光明的新项目。它由 eBPF 提供支持（因此仅适用于 Linux），可让您观察 Postgres 内部运行的查询的踪迹，将 Postgres 活动与应用程序中的活动关联起来，当然还能提升 Postgres 的跟踪能力。

Chris Bellew  
  
  
[pgtt 4.0：管理和使用 Oracle 风格的全局临时表](https://postgresweekly.com/link/156267/web "hexacluster.ai") — For
适用于您想要重现 Oracle 行为的情况。这篇文章解释了您可能需要这样做的原因以及一些替代方法，还解释了为什么 pgtt 是最佳选择。

Gilles Darold  
  
  
  * [PostgREST 12.2](https://postgresweekly.com/link/156268/web) – 适用于任何 Postgres 数据库的 REST API。

  * [DBMate 2.17](https://postgresweekly.com/link/156269/web) – 轻量级、与框架无关的数据库迁移工具。

  * [wal2mongo 1.0.7](https://postgresweekly.com/link/156270/web) –  将数据库更改复制到 MongoDB。

  * [pgxmock 4.1](https://postgresweekly.com/link/156271/web) – 模拟驱动程序以测试 Go 中的数据库交互
