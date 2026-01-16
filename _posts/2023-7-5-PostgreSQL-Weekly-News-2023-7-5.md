---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-7-5
---
### PostgreSQL每周新闻#513 - 2023年7月5日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/513)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_350,h_100/e_make_transparent/co_white,e_outline:7/lhwcvgc1asd4fzaahty4.png)
## [查看连接的 13 种方法](https://postgresweekly.com/link/142004/web)
连接表通常是 SQL 和关系数据库中的基本操作，并且有很多方法来描述和思考它们。Justin 涵盖了 13 种这样的方法，从“N+1 解决方案”或“平面地图”到更神秘的选项，如“通过图形的路径”或“环形产品”。


`Justin Jaffray `
## [Postgres 16 Beta 2发布](https://postgresweekly.com/link/142006/web)
Postgres 16 最终发布的倒计时继续进行，Beta 2 包括对 Beta 1 中发现的各种错误的修复。一如既往，我们提供了详尽的发行说明列表。


`PostgreSQL News `
## [网络研讨会：高级 Autovacuum 调优和即将推出的 pganalyze VACUUM Advisor](https://postgresweekly.com/link/142003/web)
解最重要的 VACUUM 指标、xmin Horizo 等概念、如何防止事务 ID 环绕、估计膨胀等。我们将介绍即将推出的 pganalyze VACUUM 顾问程序并展示其针对每个表的调整建议。


`pganalyze `
## [谷歌跃上 (pg)Vector 列车](https://postgresweekly.com/link/142008/web)
就在上周，Jonathan Katz 告诉我们向量是 Postgres 中的新 JSON，紧接着，Google 为 AlloyDB 和 Google Cloud SQL 添加了 pgvector 支持。我们鼓励您将其与 Google 基于矢量的Vertex AI 匹配引擎 数据库一起使用。


`Ghai and Narasimhan (Google Cloud) `
## [Heroku 推出新的 Postgres 计划](https://postgresweekly.com/link/142011/web)
作为世界上最大的 Postgres 数据库管理者之一，很高兴看到与 Heroku 相关的好消息。他们通过提供高达 6TB 空间、768GB 内存和 16K IOPS 的新计划帮助用户进一步扩展。如果你需要问价格..😅


`Jonathan K. Brown (Heroku) `
## [最近邻索引：什么是pgvector的“ivfflat”索引？](https://postgresweekly.com/link/142021/web)
pgvector 使用反向文件平面 (ivfflat) 算法来加速您存储的向量的近似最近邻搜索。这篇文章以一种非常容易理解的方式解释了这个概念，即使您是向量空间的新手。


`Arye and Sewrathan (Timescale) `
## [Postgres 谜题的乐趣：表面积和 3D 切片](https://postgresweekly.com/link/142022/web)
🧊 Greg 使用 SQL 和 Postgres 完成 2022 年代码来临挑战的旅程继续进行，包括更多令人费解的 SQL、PL/pgSQL，甚至是各种 3D 可视化。现在，如果只有 ChatGPT 可以编写这种级别的代码，我会感到震惊..


`Greg Mullane `
## [再见etcd，你好Postgres：用SQL数据库运行Kubernetes？](https://postgresweekly.com/link/142024/web)
你能用Kubernetes 核心的 Postgres 替换 etc 吗？是的。为什么？当作者说“为什么不”时，很明显您正在享受某人的实验结果！但如果你需要的话，这当然是可能的..


`Martin Heinz `
## [Epsio的PostgreSQL增量物化视图](https://postgresweekly.com/link/142025/web)


`Epsio `
## [pgBackRest中的差异备份与增量备份](https://postgresweekly.com/link/142026/web)
pgBackRest是一种流行的备份和恢复解决方案，可以进行完整备份、增量备份和差异备份。增量备份是包含自上次完整备份或增量备份以来更改的所有内容的备份，但差异备份可以通过仅基于最新的完整备份来提供更高的弹性。


`Stefan Fercot `
## [当 Postgres 数据文件丢失时会发生什么](https://postgresweekly.com/link/142028/web)
如果与表关联的数据文件“丢失”，可能是由于操作系统或硬件问题，您可能会遇到麻烦，但这里有一些注意事项考虑做。


`Abhishek Deb `
# 💡本周提示


**🗓即将举办的Postgres活动**
