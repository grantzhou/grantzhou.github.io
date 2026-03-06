---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-10-11
---
### PostgreSQL每周新闻#525 - 2023年10月11日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/525)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/uf1ztbgy2eeltwyhynu0.jpg)
## [Postgres：下一代？](https://postgresweekly.com/link/146216/web)
Postgres 上的专栏很少涉及核心贡献者的人口统计数据，但 James 指出，有证据表明 Postgres 上的大部分工作是由中位年龄较高的一小群人完成的。这根本不是一件坏事，但建议应该努力鼓励新人参与维护该项目。


`James Governor `
## [pg_bm25：Postgres 内的“弹性”质量全文搜索](https://postgresweekly.com/link/146219/web)
🔎如果您遇到了 Postgres 内置全文搜索选项的一些限制，pg_bm25 是一个新的、基于 Rust 的扩展，它引入了 BM25 索引类型据称“索引速度快 50 秒tsvector，排名结果快 20 倍。” 它可以添加到典型的 Postgres 设置中，但也是ParadeDB的一部分，ParadeDB 是来自同一创建者的基于 Postgres 的 ElasticSearch 替代方案


`ParadeDB `
## [网络研讨会：使用约束编程自动选择索引](https://postgresweekly.com/link/146215/web)
介绍一种新方法，用于根据开发人员或 DBA 选择的目标自动确定为给定 Postgres 查询工作负载创建哪组索引。报名参加太平洋时间 2023 年 11 月 15 日上午 09:30 的网络研讨会。


`pganalyze `
## [Postgres 中事务的新章节](https://postgresweekly.com/link/146221/web)
一个有点误导但事实上真实的标题，因为这实际上是Postgres 官方文档中关注事务处理内部结构的新章节。Bruce Momjian指出，虽然这些文档是新的，但这些原则也适用于较旧的 Postgres 版本。


`PostgreSQL Documentation `
## [验证用户输入的新函数](https://postgresweekly.com/link/146223/web)
Postgres 16 引入了pg_input_is_valid测试给定字符串是否是转换为指定数据类型的有效输入的函数，以及pg_input_error_info执行相同操作但共享有关失败的更多详细信息的函数。


`Luca Ferrari `
## [如何在 AWS 上使用 pg_cirrus 设置 Postgres 集群](https://postgresweekly.com/link/146224/web)
pg_cirrus是一个用于在 Linux 系统上设置 3 节点高可用 Postgres 集群的工具。


`Salman Ahmed `
## [pg_jsonschema 0.2：JSON 模式验证扩展](https://postgresweekly.com/link/146228/web)
Postgres 对 JSON / JSONB 列的支持是首屈一指的，但是如果您想验证JSON 数据的结构怎么办？JSON Schema提供了一种定义基于 JSON 的格式的方法，此扩展允许您根据它们验证文档。


`Supabase `
## [Payload 2.0：无头 Node.js CMS，现在支持 Postgres](https://postgresweekly.com/link/146229/web)
如果您需要一个基于 Node 的无头 CMS，包括可定制的基于 React 的管理系统、GraphQL 或 REST API、灵活的身份验证和文件上传系统等，那么 Payload 有很多值得喜欢的地方v2.0的头条特征是引入了Postgres支持（之前它只使用MongoDB）。


`James Mikrut `
## [Schemalint 1.0.4](https://postgresweekly.com/link/146230/web)
 -  Postgres 模式的 linter。


## [tbls 1.70.0](https://postgresweekly.com/link/146231/web)
 -  以 Markdown 格式自动记录数据库。


## [PgTyped 2.3](https://postgresweekly.com/link/146232/web)
 -  TypeScript 中的原始 SQL，但具有类型安全性。



# 💡本周提示


**🗓即将举办的Postgres活动**
