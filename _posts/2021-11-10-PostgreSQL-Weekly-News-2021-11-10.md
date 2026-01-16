---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-11-10
---
### PostgreSQL每周新闻#430 - 2021年11月10日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/430)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/riadqaypp0rjgulr9lwi.jpg)
## [许多鲜为人知的 Postgres 功能](https://postgresweekly.com/link/116031/web)
Haki 的文章对我们来说通常是猫薄荷，因为它们涵盖了很多领域，因此它与您可能不熟悉的 Postgres 功能的实际示例的综述相吻合。至少值得一读目录！


`Haki Benita `
## [看看新LZ4 TOAST压缩在Postgres的14](https://postgresweekly.com/link/116032/web)
LZ4是一个非常快速的压缩算法（和一个比较现代的一个太），它是用于购买以Postgres的TOAST压缩的选项（如在列上使用了非常大的值，如文本字段）与旧的 PGLZ 选项。LZ4不压缩挺不亚于PGLZ但性能提升是巨大的。


`Haiying Tang `
## [打造您的梦想。再也不用担心您的数据库](https://postgresweekly.com/link/116034/web)
弹性扩展并不意味着要牺牲一致性或熟悉度。使用世界上最先进的 SQL 数据库 CockroachDB Serverless 获得轻松的扩展、自动化操作和有保证的事务一致性。


`CockroachDB Serverless `
## [反对使用IF NOT EXISTS/ 的三种情况IF EXISTS](https://postgresweekly.com/link/116035/web)
许多 DDL 语句接受IF (NOT) EXISTS修饰符，让语句只在特定条件下运行，但过度使用“可能会导致负面后果”，尼古拉认为。


`Nikolay Samokhvalov `
## [Postgres 14enable_memoize为嵌套循环连接带来改进的性能](https://postgresweekly.com/link/116036/web)
快速浏览 Postgres 14 增强功能，您可以通过打开enable_memoize和关闭设置轻松使用它。它启用/禁用查询规划器使用记忆来缓存嵌套循环连接内参数化扫描的结果。这对日常使用有帮助吗？卢卡斯的发现是肯定的。


`Lukas Eder `
## [使用本地 Postgres 的消息队列？](https://postgresweekly.com/link/116039/web)
作者思考了如何仅使用 Postgres 提供的开箱即用的功能来实现排队系统。


`David Christensen `
## [开发人员+PostgreSQL+Percona = 更好的结合](https://postgresweekly.com/link/116040/web)
l,null,"en


`Percona `
## [使用 SQL 查找每天应计收入](https://postgresweekly.com/link/116041/web)
一些有用的查询和示例，用于在一个月的过程中每天累计收入。


`Jonathan S. Katz `
## [pspg 5.5.0：Postgres 数据分页器](https://postgresweekly.com/link/116042/web)
一些 UI 调整，以及对 BSD 文件流模式的支持。


`Pavel Stěhule `
## [Slonik v25：一个复杂的节点 Postgres 客户端库](https://postgresweekly.com/link/116043/web)
一个“经过实战测试”的框架，它抽象了重复的代码模式，防止不安全行为，并提供丰富的调试体验。


`Gajus Kuizinas `
# 💡本周提示


**🗓即将举办的Postgres活动**
