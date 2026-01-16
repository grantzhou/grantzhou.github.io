---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-2-8
---
### PostgreSQL每周新闻#492 - 2023年2月8日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/492)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_300,h_160/e_make_transparent/co_white,e_outline:7/rrkstxca0vg7e1eww6yw.jpg)
## [什么性能更好：FILTER 还是 CASE？](https://postgresweekly.com/link/135028/web)
Lukas 指出，SQL 的 FILTER 子句是聚合函数中等效 CASE 表达式的其他选择，但正如我们所知，等效查询可以具有不同的性能配置文件！ 剧透：对于 FILTER 与 CASE 也是如此。


`Lukas Eder `
## [来到 Postgres 16：一种保留连接槽的新方法](https://postgresweekly.com/link/135030/web)
您长期以来一直能够使用 superuser_reserved_connections 为超级用户保留连接槽，但是 Postgres 16 的新补丁提供了一种通过 pg_use_reserved_connections 为非超级用户保留连接槽的方法 角色。


`Pavlo Golub `
## [数据库缓存，没有复杂性](https://postgresweekly.com/link/135027/web)
PolyScale.ai 提供亚毫秒级的读取查询，没有缓存开发的典型成本和复杂性。 使用我们的无服务器边缘网络或内部部署在几分钟内完成部署。


`PolyScale.ai `
## [在 GPT 中嵌入 Postgres 模式的冒险](https://postgresweekly.com/link/135037/web)
尝试说服 OpenAI 的 GPT 根据提示返回有用的 SQL 查询的有趣实验，但仍有大量工作要做。


`William Pride `
## [用于更有效 CRUD 的简单 SQL 技巧](https://postgresweekly.com/link/135038/web)
创建、读取、更新、删除 (CRUD) 范例是许多使用数据库的应用程序的基本元素，您可以利用 SQL 使 CRUD 任务更加原子化，正如 Paul 所说，“做更多数据库的事情。”


`Paul Ramsey `
## [如何获取行及其所有依赖项？](https://postgresweekly.com/link/135039/web)
获取表格的一行很容易，但是如果您还想获取它引用的所有行怎么办？ Hubert 开始尝试构建此类文档的功能——这个过程与最终结果一样有趣。


`Hubert depesz Lubaczewski `
## [Postgres 会使用我的索引吗？ Postgres 的假设索引](https://postgresweekly.com/link/135040/web)
HypoPG 可以创建假设索引（B 树、BRIN 和哈希索引，但不是 GIN 或 GIST）并测试 Postgres 是否会使用它们。 您可以将它与 EXPLAIN 结合使用，为您的查询生成正确的索引。


`Craig Kerstiens `
## [pgModeler 1.0 发布：Postgres 数据库建模器](https://postgresweekly.com/link/135046/web)
一种以可视化方式创建和编辑数据库模型的简单方法。 它被打包为付费产品，但也是开源的，因此您可以构建自己的产品。 官方主页和 GitHub 仓库。

`Raphael Araújo e Silva `
## [免费电子书：如何为您的查询创建最佳 Postgres 索引](https://postgresweekly.com/link/135052/web)


`pganalyze `
## [pg_ivm 1.5：增量视图维护 Postgres 扩展](https://postgresweekly.com/link/135054/web)
当只有一小部分视图发生变化时，IVM 可以比重新计算更有效地更新物化视图。 v1.5 添加（基本）CTE 支持。


`SRA OSS LLC `
## [pg_dumpbinary 2.9：以二进制格式转储数据库](https://postgresweekly.com/link/135058/web)
使用二进制格式进行转储在特定情况下有一些好处。


`lzlabs `
## [pgFormatter 5.5：SQL 语法美化器](https://postgresweekly.com/link/135062/web)
主要是一个错误修复版本。 这里有一个在线演示。


`Gilles Darold `

