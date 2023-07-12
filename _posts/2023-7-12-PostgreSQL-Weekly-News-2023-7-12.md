---
layout: post
title: PostgreSQL 每周新闻 2023-7-12
---
### PostgreSQL每周新闻#514 - 2023年7月12日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/514)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_600,h_160/e_make_transparent/co_white,e_outline:12/rrcbnnamutiazyfczv81.png)
## [Microsoft 对类似 PostgreSQL 的分布式数据库进行基准测试](https://postgresweekly.com/link/142340/web)
Microsoft 委托GigaOM对 PostgreSQL 的 Azure Cosmos DB（在幕后使用 Citus）与来自 Cockroach 和 Yugabyte 的其他 Postgres 衍生替代品进行基准测试。结果正在推广的事实告诉您哪个产品已经获胜.. 😅 在 Marco Slot 的一篇文章中，他更详细地解释了为什么Cosmos DB 如此之快，并邀请您自己运行基准测试。


`Alex Woodie (Datanami) `
## [子查询和性能](https://postgresweekly.com/link/142343/web)
SELECT用括号将 a 括起来，并使用它为另一个查询提供值，这样您就得到了一个子查询。Laurenz 介绍了一些示例，目的是帮助我们编写性能良好的子查询。


`Laurenz Albe `
## [即插即用 Postgres 缓存](https://postgresweekly.com/link/142339/web)
通过无服务器缓存加速数据库。使用 PolyScale 的智能数据库边缘缓存提高吞吐量并降低查询延迟。无需配置或编写代码即可在几分钟内实施。


`PolyScale․ai `
## [让我们讨论一次意外的Postgres宕机](https://postgresweekly.com/link/142345/web)
这肯定是您在发生之前需要考虑的事情之一！Shaun 回顾了一家公司 Aurora 迁移的故事，该迁移存在问题，但总体进展顺利。


`Shaun Thomas `
## [更改实时数据库中列的数据类型](https://postgresweekly.com/link/142347/web)
ALTER COLUMN ..— 停止！更改列的数据类型所需的独占锁可能会导致生产数据库很快遇到一些麻烦。如果我们能够更渐进地进行改变呢？


`Mateusz Henicz `
## [以最短的停机时间将 Postgres 从 Google Cloud Platform 迁移到 Amazon RDS ](https://postgresweekly.com/link/142354/web)
您永远不知道什么时候可能需要切换平台，而 AWS 总是特别热衷于提供一种简单的途径。


`Aychin Gasimov (AWS) `
## [保护您的 PostgreSQL 数据库](https://postgresweekly.com/link/142355/web)


`Teleport | goteleport․com `
## [Kanel：从Postgres生成TypeScript类型](https://postgresweekly.com/link/142358/web)
它通过检查实时数据库来工作，并输出代码，您可以将其添加到TypeScript项目中，并与Knex（下面）–GitHub repo之类的东西一起使用。


`Kristian Dupont `
## [Kanel：从 Postgres 生成 TypeScript 类型](https://postgresweekly.com/link/142361/web)
它通过检查实时数据库并输出代码来工作，您可以添加到 TypeScript 项目并与Knex（如下）之类的东西一起使用 - GitHub 存储库。

`knex `
## [ZomboDB：使用 Elasticsearch 为 Postgres 索引提供支持](https://postgresweekly.com/link/142362/web)
通过使用 Elasticsearch 作为索引类型，将额外、强大的文本搜索和分析功能引入 Postgres


`ZomboDB LLC `
## [GoodJob：用于 Ruby on Rails 的多线程、基于 Postgres 的 ActiveJob 后端](https://postgresweekly.com/link/142363/web)
完全支持异步、队列、延迟、优先级、超时和重试，配置接近于零。


`Ben Sheldon `
# 💡本周提示


**🗓即将举办的Postgres活动**
