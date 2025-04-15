---
layout: post
title: PostgreSQL 每周新闻 2025-4-3
---
### PostgreSQL每周新闻#595 - 2025年4月3日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/595)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/quqznyttxi5khg6tyhgf.jpg)
## [🕒 深入了解 Postgres 中的时间](https://postgresweekly.com/link/167920/web)
如果你曾经在处理 Postgres 中的时间时，总是祈祷好运，那么这本书正适合你。Radim 提供了丰富的示例和建议，探讨了不同时间数据类型的工作原理，以及如何使用时区、间隔、时间范围等。

`Radim Marek`

## [扩展 Postgres 的路线图](https://postgresweekly.com/link/167921/web)
一位经验丰富的 Postgres 专家提供了扩展 Postgres 部署时需要考虑的一系列步骤，从首先正确获取数据模型，到索引、硬件、调整和分片。


`Kaarel Moppel`
## [使用 Blacksmith 将 Docker 构建速度提升 2 到 40 倍](https://postgresweekly.com/link/167919/web)
只需更改一行代码，Blacksmith 即可将 Docker 层缓存挂载到 GitHub Actions 运行器中，从而实现 Docker 增量构建。Blacksmith 已被


`Blacksmith  `
## [📈 使用 OrioleDB 优化 Postgres](https://postgresweekly.com/link/167922/web)
OrioleDB 是 Postgres 的替代存储引擎，它扩展了表访问方法框架，以优化现代硬件上的性能。但性能提升了多少呢？Brian 进行了一些测试。


`Brian Misachi `

### 本周摘要：

🌐 在《[地缘政治 Postgres](https://postgresweekly.com/link/167923/web)》一书中，Bruce Momjian 反思了 Postgres 的开放性如何使其能够应用于原本可能受到限制的领域和行业。对一人开放意味着对所有人开放，这既有其利弊。

Postgres 顾问 [Frédéric Delacourt](https://postgresweekly.com/link/167924/web) 是最新一期 PostgreSQL 本周人物的受访者。

[Electric Cloud 已进入公测阶段](https://postgresweekly.com/link/167925/web)——这是其开源 Postgres 同步引擎的托管版本，该引擎最近[已发布 1.0 版本](https://postgresweekly.com/link/167926/web)。

### 代码和工具：

## [使用 Postgres 创建直方图](https://postgresweekly.com/link/167927/web)
直方图通过将值分组到不同的箱体中并显示每个箱体的频数来可视化数据分布。Postgres 有一个 width_bucket 函数可以帮助您实现这一点，Elizabeth 在这里展示了一些精彩的查询。


`Elizabeth Christensen`

📄 [等待 Postgres 18：Docker 容器体积缩小 34%](https://postgresweekly.com/link/167929/web) – “Postgres 18 的最小 (CloudNativePG) 镜像大小为 262MB – 比 Postgres 17 的最小 CNPG 镜像（413MB）小 34%。” Jeremy Schneider

📄 [SQL 也面临困境，但 MongoDB 文档却大放异彩](https://postgresweekly.com/link/167930/web) – Franck 在 MongoDB 工作，但也是 Postgres 的忠实粉丝，所以看到他进行详细的比较很有意思。也有一些不错的评论。Franck Pachot

📄 [使用 pgai 将维基百科导入 Postgres](https://postgresweekly.com/link/167931/web) – 如果您想尝试 pgai 的向量嵌入功能，维基百科提供了一个庞大的数据集供您入门。 Hans-Jürgen Schönig

📄 [TimescaleDB 来帮忙：加速统计——TimescaleDB](https://postgresweekly.com/link/167932/web) 快速处理分析时间序列工作负载的能力让这位更熟悉 MySQL 生态系统的工程师 Kamil Ruczyński 赞叹不已。

### 🛠 代码和工具

## [pg_auto_failover 2.2：自动故障转移扩展](https://postgresweekly.com/link/167933/web)
用于监控和管理 Postgres 集群自动故障转移的扩展和服务。现已支持 Postgres 17。


`Microsoft `

## [🤖 Postgres Pro：一个让 AI 代理调整和改进数据库使用情况的 MCP 服务器](https://postgresweekly.com/link/167661/web)
我怀疑它需要重命名（以免与同名公司混淆？），但这是一个有趣的第一步，通过 MCP 服务器在现代 AI 模型和代理与 Postgres 之间架起一座桥梁，让 AI 代理查询您的 Postgres 数据库以调整索引、进行更改、运行 SQL 等。

`Crystal Corp. `

[FerretDB 2.1](https://postgresweekly.com/link/167936/web) – 一款功能类似于 MongoDB 的数据库，但使用 Postgres 进行存储。

[BemiDB 0.48](https://postgresweekly.com/link/167937/web) – 针对分析优化的单二进制 Postgres 只读副本。

[pgroll 0.11](https://postgresweekly.com/link/167938/web) – 零停机、可逆的 Postgres 模式迁移。

[pg-boss 10.2](https://postgresweekly.com/link/167939/web) – 基于 Postgres 的 Node.js 作业队列系统。

[pg_dumpbinary v2.19](https://postgresweekly.com/link/167940/web) – 将数据库转储为二进制格式。

[Martin 0.16](https://postgresweekly.com/link/167941/web) – 基于 Rust 的快速 PostGIS 地图瓦片服务器。

[Prisma 6.6](https://postgresweekly.com/link/167942/web) – 适用于 Node.js 和 TypeScript 的流行 ORM。