---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2022-6-8
---
### PostgreSQL每周新闻#458 - 2022年6月8日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/458)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/oso8z5btoxxse7reapue.jpg)
## [2022 年 PostgreSQL 状态调查现已开](https://postgresweekly.com/link/124439/web)
Timescale 的人们正在对 Postgres 社区进行第三次年度调查，鉴于此类调查的结果往往会引起有趣的阅读（您可以在此处阅读去年的结果）它会如果你能参加，那就整洁。（我刚做了，花了 3-4 分钟。） 


`Timescale `
## [自动 Postgres 索引的平衡方法：pganalyze 索引顾问的新版本](https://postgresweekly.com/link/124441/web)
pganalyze索引顾问是一种工具，可以帮助您确定数据库可以从哪些索引中受益，现在有一个新版本的工具可以使用更少的“噪音”和更有帮助（和排名）的建议。


`Jens Nikolaus `
## [用于全球低延迟 Postgres 的无服务器边缘缓存](https://postgresweekly.com/link/124443/web)
在全球范围内扩展读取以实现低延迟、高查询性能（一致的 <1ms）和大量并发。PolyScale.ai 是 Postgres 的即插即用无服务器边缘缓存。无需编写代码或部署基础架构，即可在几分钟内实现全球扩展。


`PolyScale.ai `
## [使用范围分区降低 Amazon Aurora 上的读取 I/O 成本](https://postgresweekly.com/link/124448/web)
Aurora 的“按使用付费”模型会在您希望依赖 I/O 的程度方面产生一些财务影响。这篇文章展示了使用基于时间的分区策略如何降低使用 33TB 数据和每天摄取 44GB 的数据库的成本。


`Imseih and Biran (AWS) `
## [pganalyze 是如何构建它的索引引擎的](https://postgresweekly.com/link/124449/web)
我们在上面提到了 pganalyze 的索引建议工具，但是如果你对它在幕后的实际工作方式感到好奇，那么这篇文章就是为你准备的。


`Lukas Fittl `
## [如何处理逻辑复制冲突](https://postgresweekly.com/link/124450/web)
富士通的 Takamichi Osumi 解释了 Postgres 的新机制（并且已经在 Postgres 15 beta 中可用）如何更容易解决复制冲突。


`Takamichi Osumi `
## [使用PGO v5.1进行有效的 Postgres 集群配置和管理](https://postgresweekly.com/link/124451/web)
PGO 是 Kubernetes 的 Postgres 操作符，用于处理集群管理、定制等。


`Andrew L'Ecuyer `
## [在 State of Engineering 时间报告中查看工程师真正花费了多少小时编码](https://postgresweekly.com/link/124455/web)
l,null,"en


`Retool `
## [Postgres Docker容器迁移备忘单](https://postgresweekly.com/link/124457/web)
这是非常基本的，但是.. “我刚刚完成将 postgres 数据库迁移到新主机。为了记住下次该怎么做，我正在写下我在这里使用的命令。”


`Garrit Franke `
## [ZomboDB：使用 Elasticsearch 为 Postgres 索引提供支持](https://postgresweekly.com/link/124463/web)
几年前我们在测试版中与此相关联，现在是重新审视的时候了！Zombo 使用 Elasticsearch 作为索引类型，为 Postgres 带来了强大的文本搜索和分析功能。ZomboDB 使用 Elasticsearch 作为索引类型，为 Postgres 带来了强大的文本搜索和分析功能，提供了新的和创造性的方式来查询您的数据。您CREATE INDEX ... USING zombodb在现有表上使用，Zombo 管理其余的集成。


`ZomboDB LLC `
## [PGSQL-HTTP：Postgres的HTTP客户端](https://postgresweekly.com/link/124464/web)
你希望能够从触发器调用 Web 服务吗？这是你的机会。


`Paul Ramsey `
## [pgtt 2.8：管理和使用 Oracle 风格的全局临时表的扩展](https://postgresweekly.com/link/124466/web)
现在添加了对 Postgres 15 的支持。


`Gilles Darold `
# 💡本周提示


**🗓即将举办的Postgres活动**
