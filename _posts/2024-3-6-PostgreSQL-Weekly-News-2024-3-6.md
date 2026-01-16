---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2024-3-6
---
### PostgreSQL每周新闻#545 - 2024年3月6日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/545)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/tjhmevzmzmmo1ay0epcc.jpg)
## [使用Postgres扩展构建Q＆A机器人](https://postgresweekly.com/link/152172/web)
在过去的一两年里， pgvector和嵌入模型使得创建高级自然语言搜索系统变得更加容易。在这里，Tembo 展示了他们的堆栈和扩展如何使其成为一个更加简单、直接的过程。 pg_vectorize是一个特别的亮点，因为它是一个扩展，可以使用常见的 LLM 自动执行将文本转换为嵌入的许多过程。


`Adam Hendel (Tembo) `
## [比较Postgres托管服务：AWS，Azure，GCP和Supabase](https://postgresweekly.com/link/152175/web)
一个相当简单、直接的比较，目的不是详尽无遗，而是为托管服务市场上的开发人员提供指导。


`Sai Srirampur (PeerDB) `
## [pganalyze Index Advisor 3.0：工作负载感知索引建议](https://postgresweekly.com/link/152171/web)
上周推出，新顾问可以查找每个表丢失的索引，检测会阻止热更新的索引，让您深入查看所有考虑的索引等等。由PGCon 2023 上引入的约束规划模型提供支持。


`pganalyze `
**本周摘要：**
*   🤖 Francesco Tisiot 启动了一份与 AI 相关的 Postgres 项目和资源的精选列表，并邀请您提交自己的补充内容。


*   📅今年 5 月在加拿大温哥华举行的PGConf.dev 2024 的日程表已发布。


*   📑 如果您想了解一点历史并需要周末阅读，《Postgres 的设计》是1986 年发表的一篇简洁的论文，介绍了 Postgres 的早期阶段及其设计的设想。


*   Microsoft 的 Claire Giordano 谈论Microsoft 的POSETTE Postgres 活动、其新名称是如何选择的以及该活动代表什么。


*   🗣 很高兴看到PostgreSQL 本周人物回归，接受了AWS 的 Divya Sharma 采访，谈论了她的工作、Postgres 的烦恼以及她在 Postgres 16 中最喜欢的东西。


## [数据库灾难以及如何查找它们](https://postgresweekly.com/link/152182/web)
▶您是工程团队的一员，您收到 ping 通知，因为出现了问题……接下来会发生什么？


`Christophe Pettus `
## [1000 多个 Postgres 扩展集中在一个地方](https://postgresweekly.com/link/152183/web)
如果您正在寻找 Postgres 扩展， PGXN是一个很好的起点，但我也喜欢这种基于 GitHub Gist 的更灵活的方法。


`Joel Jakobsson `
## [与 PeerDB 的 Sai Srirampur 讨论 Postgres 快速复制](https://postgresweekly.com/link/152185/web)
▶


`Scott Hanselman podcast`
## [在 Azure 上通过 pg_trgm调整 Postgres LIKE/ILIKE查询的提示](https://postgresweekly.com/link/152186/web)
使用 LIKE 或 ILIKE 进行模式搜索时提高查询性能的提示。


`Sarat Balijepalli `
## [了解完全标准的多主分布式 PostgreSQL 架构的技术优势](https://postgresweekly.com/link/152187/web)
📢需要低延迟和高可用性？。


## [pg_activity 3.5：htop类似活动监控工具](https://postgresweekly.com/link/152189/web)
就像您可能使用 top 或 htop 来监控进程和 CPU 使用情况一样，它pg_activity为您提供了类似的 Postgres 幕后视图，包括正在运行的查询的视图、最新的性能统计数据等。


`Dalibo `
## [Pigsty：一个“包含电池”的 Postgres 发行版](https://postgresweekly.com/link/152190/web)
这个项目的名称总是让我微笑：PIGSTY 实际上是一个缩写词，代表Postgres In Great STYle！它是一个 Postgres发行版，在可用性、部署和可观察性等方面包含大量开箱即用的组件和工具。最新版本将所有内容都推向了 Postgres 16.2 标准，并引入了新的 ParadeDB 和 DuckDB FDW 扩展。


`Ruohang Feng `
## [pg_jsonschema 0.3：JSON 模式验证扩展](https://postgresweekly.com/link/152191/web)
Postgres 对 JSON / JSONB 列的支持是首屈一指的，但是如果您想验证 JSON 数据的结构怎么办？ JSON 架构提供了一种定义基于 JSON 的格式的方法，此扩展允许您使用此类架构验证 JSON 文档。 v0.3 完成了扩展对 Postgres 16 的支持。


`Supabase `
## [pg_ivm 1.8：增量视图维护扩展](https://postgresweekly.com/link/152192/web)
IVM 可以增量更新物化视图，这比完全重新计算更有效REFRESH MATERIALIZED VIEW。


`SRA OSS LLC `
## [Risingwave 1.7](https://postgresweekly.com/link/152193/web)
 - 与Postgres兼容的流数据库。


## [pgvector 0.6.1](https://postgresweekly.com/link/152173/web)
 - Postgres 的矢量相似性搜索。
 

# 💡本周提示


**🗓即将举办的Postgres活动**
