---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2026-1-7
---
### PostgreSQL每周新闻#629 - 2026年1月7日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/630)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/hsvy3genjwv9bfv9klsi.jpg)
## [2025 年数据库展望：年度回顾](https://postgresweekly.com/link/178895/web)
备受尊敬的数据库专家 Andy Pavlo 精心撰写了一篇精彩的文章，回顾了过去一年资料库领域的主要趋势和动态。 Postgres 被誉为 2025 年的「主导」资料库，但文章内容远不止于此。

`Andy Pavlo`

## [POSETTE 2026－提案征集即将截止！](https://postgresweekly.com/link/178894/web)
新年新目标！诚挚邀请您在 POSETTE（Postgres 盛会）上分享您的 Postgres 真知灼见。 POSETTE 是由微软 PostgreSQL 团队组织的免费线上开发者盛会，将于 2026 年 6 月 16 日至 18 日举行。提案征集将于 2 月 1 日截止。立即行动！

`Microsoft `


## **本周摘要**

🇨🇭 [CERN PGDay 2026](https://postgresweekly.com/link/178898/web) 将于今年 2 月 6 日在瑞士举行，完整行程已公布。

[Postgres 团队表彰](https://postgresweekly.com/link/178900/web)了 12 位对专案做出杰出贡献的新成员，并宣布 Floor Drees 加入贡献者团队，「以帮助分担工作量」。

## [Postgres 效能：云端和本地部署的延迟](https://postgresweekly.com/link/178901/web)
拥有高效能资料库是一回事，但资料库的位置对延迟有很大的影响 — 如果延迟过高，可能会抵消其他所有效能优势。

`Hans-Jürgen Schönig`

## [Postgres 18 的 RETURNING 增强功能](https://postgresweekly.com/link/178902/web)
Postgres 18 增强了 DML 查询（插入、更新等）中使用的 RETURNING 子句，以支援旧别名和新别名，从而明确存取资料的先前状态和目前状态。

`Ahsan Hadi`

## [pg_csv_loader：一款用于快速简单地载入 CSV 档案的工具](https://postgresweekly.com/link/178903/web)
一款基于 JavaScript 的工具，只需极少的配置即可将 CSV 档案载入到 Postgres 资料库中。来源。

`Hubert depesz Lubaczewski`


📄 [使用 Postgres 18 快速复制资料库 – 利用范本资料库](https://postgresweekly.com/link/178905/web)。 Radim Marek

📄 [几个 Postgres 脚本编写技巧](https://postgresweekly.com/link/178907/web)。 Paul Gross

📄 [2025 年 Postgres MCP 伺服器的现况](https://postgresweekly.com/link/178908/web)。 DBHub


## **📰 分类广告**


🚀 [将 AI 代理部署到生产环境](https://postgresweekly.com/link/178909/web)。 Postgres 工具包，支援 MCP、混合搜寻和全球扩充。 [Beta 版现已开放](https://postgresweekly.com/link/178909/web)。

## **🐘 2025 年 Postgres 每周热门文章：**

[在 2025 年最后一期中](https://postgresweekly.com/link/178910/web)，我们回顾了过去一年中最热门的工具和程式码，但这里我们更全面地审视一下过去十二个月中最受关注的内容。这是一份值得重温的精华清单：

## [1. 改变人生的 Postgres 模式](https://postgresweekly.com/link/178911/web)
作者承诺标题并非哗众取宠（虽然显然效果显著，排名第一！），书中提供了十二条精炼实用、来之不易的技巧和见解，涵盖了从使用 UUID 作为主键、表命名到模式和视图的使用等各个方面。

`Ethan McCue`


## [2. 不要这样做（在 Postgres 中）](https://postgresweekly.com/link/178912/web)
Postgres 官方 wiki 上的一个页面一直都很有意思，它汇总了使用 Postgres 时常见的错误以及不应该做的事情，例如“不要使用 char(n)”和“不要使用 serial”。有些建议可能有争议，但都给了理由。

`Postgres Wiki`


## [3. Kafka 速度很快，我会使用 Postgres](https://postgresweekly.com/link/178913/web)
受另一篇关于使用 Postgres 而不是 Redis 进行缓存的文章的启发，作者开始研究 Postgres 是否足以处理你可能自然而然选择 Kafka 的用例。

`Stanislav Kozlovski`


## [4. 如何修复 Postgres 中查询速度慢的常见原因](https://postgresweekly.com/link/178916/web)
Render 的一位资料库工程师展示了一个常见的、但很容易修复的效能问题，该问题是由外键上缺少索引引起的。

`Eric Fritz`


## [5. 将 Postgres 队列扩展到每秒 10 万个事件的经验教训](https://postgresweekly.com/link/178917/web)
RudderStack 决定使用 Postgres 作为其主要队列系统，而不是 Kafka 之类的系统，他们的团队分享了他们从中获得的经验教训。

`Aris Tzoumas (RudderStack)`

## [6. Postgres 17 与 18 的基准测试](https://postgresweekly.com/link/178918/web)
作者对 Postgres 17 和 18 进行了一系列详细的性能基准测试，测试组合多达 96 种，结果令人欣慰地发现 Postgres 18 提供了不错的性能提升，本地磁碟性能更佳，调整设置仍然值得。

`Ben Dicken (PlanetScale)`

## [7. Citus 能容纳 1 兆行吗？](https://postgresweekly.com/link/178919/web)
“Postgres 可以扩展”，但究竟能扩展到什么程度呢？ Hans-Jürgen 决定一探究竟，他进行了一项小型（或大型？）实验，看看 1 兆行的表是否真的可行。

`Hans-Jürgen Schönig`

## [8. 即使你正在执行索引扫描，也不意味著你不能做得更好](https://postgresweekly.com/link/178920/web)
迈克尔说，如果你在查看查询计划时看到索引扫描，你可能会认为你正在朝著高性能查询的方向前进，但还有更多提升空间。

`Michael Christofides`

## [9. Postgres 18 中的 psql 引入了管线功能](https://postgresweekly.com/link/178921/web)
Postgres 18 及更高版本中的 psql 配备了在 SQL 脚本中使用管线的命令，Daniel 指出这「可以大大提高查询吞吐量」。

`Daniel Vérité`

## [10. PostgreSQL 在硬体怪兽时代](https://postgresweekly.com/link/178922/web)
你可能觉得工作站的 CPU 已经很快了，但想像一下，如果拥有一颗每个插槽 192 个核心的 AMD EPYC 处理器，以及 10 TB 的记忆体呢！现代 CPU 的强大效能（更不用说速度更快的储存空间了）促使我们思考如何以现代方式扩展资料库伺服器。

`Lætitia Avrot`