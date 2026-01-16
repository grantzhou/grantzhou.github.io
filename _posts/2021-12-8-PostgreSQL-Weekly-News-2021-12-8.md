---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-12-8
---
### PostgreSQL每周新闻#434 - 2021年12月8日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/434)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/zjceqauobhlzgzbmberf.jpg)
## [pg_graphql：Postgres 的 GraphQL 扩展](https://postgresweekly.com/link/117209/web)
Supabase 团队已经开源了一个扩展（他们承认仍在进行中）为 Postgres 添加了 GraphQL 支持，诸如模式生成和查询解析之类的东西完全保留在数据库服务器的范围内，并且不是一些外部服务（尽管Postgraphile在这方面是一个不错的选择）。


`Oliver Rice (Supabase) `
## [理解 GIN 索引：好与坏](https://postgresweekly.com/link/117211/web)
使用花哨的数据类型、JSONB 文档，并且想要索引？跳过 B 树索引，直奔 GIN ;-) Lukas 介绍了 GIN 索引（现在大约 15 年前引入 Postgres）的用途和一些潜在的陷阱。


`Lukas Fittl `
## [开发更快的工作方式。快速构建内部工具](https://postgresweekly.com/link/117212/web)
自定义仪表板、管理面板、CRUD 应用程序——在 Retool 中更快地构建任何内部工具。立即免费开始使用。


`Retool `
## [pgFormatter 5.2：格式化 SQL 代码的工具](https://postgresweekly.com/link/117219/web)
您可以在线测试它，或者您可以从 GitHub获取源代码（它是用 Perl 编写的）并自己运行它。


`MigOps `
## [使用 PostGIS 加快空间索引的技巧](https://postgresweekly.com/link/117221/web)
如果您要存储有关地理区域的信息，则可能存在大量重叠，这可能会使索引效率降低。Paul 解释了空间索引如何对其输入的顺序敏感以及如何缓解问题。


`Paul Ramsey `
## [压缩pgdump转储xz](https://postgresweekly.com/link/117222/web)
“对如何压缩一组 SQL 转储进行了不科学的观察，” Luca 说，他观察到大多数 SQL 转储由于其文本性质而具有高度可压缩性。他使用xz，一种可以实现比标准更高的压缩率的工具gzip来压缩所述转储并取得很大成功。


`Luca Ferrari `
## [🧹在 PostgreSQL 数据库中执行的 5 种数据清理技术](https://postgresweekly.com/link/117223/web)
l,null,"en


`Timescale `
## [一些基本的索引最佳实践](https://postgresweekly.com/link/117224/web)
一些合理的基本建议，主要围绕不要过度索引和明智地选择你的索引战。


`Michael Christofides `
## [使用pg_rewrite了整洁的表分区](https://postgresweekly.com/link/117225/web)
pg_rewrite是Cybertec的扩展，可以把非分区表到分区一个以“几乎没有锁定。”


`Hans-Jürgen Schönig `
## [DBDoc：Database Schema Documenter](https://postgresweekly.com/link/117227/web)
一种工具（用 Clojure 编写），提供了一种向表中添加文档的简单方法。您在一个简单的文本文件中描述表，然后将其作为注释应用于数据库中的实际表，使它们可以在诸如psqlDBeaver、Postico 等工具中查看。


`Micah Elliott `
# 💡本周提示


**🗓即将举办的Postgres活动**
