---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-4-5
---
### PostgreSQL每周新闻#500 - 2023年4月5日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/500)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/yw3wd7naizflpl0tpinh.jpg)
## [PL/Rust 1.0：用 Rust 编写 Postgres 函数](https://postgresweekly.com/link/137764/web)
这特别令人兴奋，因为 PL/Rust 函数不像 PL/pgSQL 或 PL/Python 函数那样被解析，而是被编译成本地机器代码。 这以更动态的形式提供了扩展风格的性能水平。 我怀疑我们很快就会看到很多进展和用例。 更多信息在这里。

`TECHNOLOGY CONCEPTS AND DESIGN, INC. `
## [如何使用下一代 Postgres 获得最多 5 个 9s 的正常运行时间](https://postgresweekly.com/link/137766/web)
近乎零的停机时间对于许多行业来说都是关键任务。 了解如何通过高级冲突管理和数据丢失保护，通过多主复制和数据分发来降低风险并提高生产力和客户满意度。


`EDB `
## [SQL:2023 已经完成，但有什么新内容？](https://postgresweekly.com/link/137767/web)
最新版本的 SQL 标准现在与所谓的“ISO 神”一起发布，并将在适当的时候发布。 没有数据库完全遵循 SQL 标准，但是查看新功能可能很有用，因为随着时间的推移，标准中的功能往往会过滤到 Postgres 中（反之亦然，正如刚刚添加到规范中的 JSON 类型所见）。


`PETER EISENTRAUT `
## [谷歌提供“随处”运行的 AlloyDB 版本](https://postgresweekly.com/link/137768/web)
谷歌一年前首次推出 AlloyDB for PostgreSQL，作为一种托管的 Postgres 兼容服务，在风格上与 Amazon Aurora 有点相似，但来自谷歌。 他们现在可以预览 AlloyDB Omni，这是一个可下载的 AlloyDB 版本，专为在 Google 的云上运行而设计。


`GOOGLE CLOUD BLOG `
## [Citus Con 终极指南：Postgres 活动](https://postgresweekly.com/link/137770/web)
Citus Con 是一项免费的在线 Postgres 活动，由 Postgres 团队于 4 月 18 日至 19 日在 Microsoft Azure 举办。 在这篇文章中，您可以了解更多关于所提供的一切，或者让克莱尔 ▶️ 以视频形式说服您？


`CLAIRE GIORDANO `
## [Hydra：在 Columnar Postgres 上引入更新和删除](https://postgresweekly.com/link/137784/web)
Hydra 是一个 Postgres 驱动的数据仓库/OLAP 系统，被称为“开源 Snowflake 替代品”。 他们现在发布了难题的最新部分：支持在其他不可变和仅附加列存储上进行更新和删除，这篇文章解释了如何做到这一点。 GitHub 回购。


`JONATHAN DANCE (HYDRA) `
## [Postgres 中的行锁](https://postgresweekly.com/link/137777/web)
Laurenz 快速介绍了 Postgres 中四种不同类型的行锁（与表锁相对），为什么你会选择某些类型，以及它们在幕后如何工作。 所有非常容易理解和有用的东西都需要知道。


`LAURENZ ALBE `
## [表示不重叠的时间范围](https://postgresweekly.com/link/137778/web)
由于竞争条件，保证不重叠的时间范围（例如酒店预订）并不容易。 Postgres 的排除约束和范围类型可以提供帮助。

`TOBIAS PETRY `
## [一个特别插图的 Postgres 迁移故事](https://postgresweekly.com/link/137779/web)


`CRUNCHY BRIDGE `
## [归咎于 Postgres 错误](https://postgresweekly.com/link/137780/web)
Postgres 日志中的错误消息可能并不总是数据库本身的错误。 罗伯特研究了可能会出现用户错误或操作系统问题的情况。


`ROBERT HAAS `
## [从你的 Postgres 轻松做 Mongodb兼容](https://postgresweekly.com/link/137781/web)
探索通过 MongoDB 外部数据包装器（现在所有新的 Crunchy Bridge 部署都支持）将 MongoDB 和 Postgres 配对的好处。


`CHRISTOPHER WINSLETT (CRUNCHY DATA) `
## [使用 Postgres 进行集成测试](https://postgresweekly.com/link/137782/web)
了解在测试场景中使用 Postgres 的几种方法，每种方法各有优缺点。


`EGON ELBRE `
## [使用基于角色的访问控制的 Aurora 数据库授权](https://postgresweekly.com/link/137783/web)
了解在测试场景中使用 Postgres 的几种方法，每种方法各有优缺点。


`PINYANI AND LONAPPAN (AWS) `



