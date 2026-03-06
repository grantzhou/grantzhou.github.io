---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-3-24
---
### PostgreSQL每周新闻#398 - 2021年3月24日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/398)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/lwkvswdsvysynlayygvj.jpg)
## [pg_query 2.0：解析Postgres查询的最简单方法](https://postgresweekly.com/link/105081/web)
pg_query是一个用于解析Postgres SQL查询的独立库-版本2增加了对Postgres 13的支持，并包含了一个deparser，以便可以将处理过的解析树转换回SQL。。那里还有很多可以做的。它是一个C库，但也支持Ruby库以及Python和Node.js绑定。


`Lukas Fittl `
## [🐘PostgreSQL 2021的状态调查现已开始✨](https://postgresweekly.com/link/105085/web)
无论你是接触Postgre的新人或是一个几十年的贡献者，我们很乐意听到你的意见。就像去年的调查一样，我们将公布关键的调查结果，并为Postgres社区的每个人提供匿名的源数据👉 开始调查。


`Timescale `
## [入门EXPLAIN(ANALYZE)](https://postgresweekly.com/link/105086/web)
在查询前面加上EXPLAIN可以让您看到Postgres的execution planner是如何解释查询的，以及它计划如何执行查询的。ANALYZE选项更进一步，实际运行查询来补充一些通用信息。


`Kat Batuigas `
## [在单个Citus节点上分片Postgres：如何、为什么和何时](https://postgresweekly.com/link/105087/web)
Citus是为跨越许多节点水平扩展Postgres而设计的，但是如果你只有一个节点呢？你仍然可以把玩和测试。


`Onder Kalaci `
## [关于Postgres索引的三件容易记住的事](https://postgresweekly.com/link/105088/web)
从2020年开始，但我们当时错过了。


`Kat Batuigas `
## [不要让排序规则版本损坏Postgres索引](https://postgresweekly.com/link/105089/web)
“排序规则和依赖关系是有点像闰秒和时区的无聊话题：你知道，在某些东西出问题之前，你通常不必担心的那些晦涩难懂的事情。”


`Thomas Munro `
## [用Rust编写postgresql漂亮的打印机：第1部分](https://postgresweekly.com/link/105090/web)
这是一系列关于pg-pretty开发的博客文章中的第一篇，pg-pretty是一个基于Rust的漂亮的SQL打印机，正在开发中。


`Dave Rolsky `
## [Fauna：Postgres的所有优点，没有运营瓶颈](https://postgresweekly.com/link/105092/web)
Fauna将Postgres的安全性与模式灵活性、现代能力和无限规模结合起来。了解更多。。。


`Fauna `
## [在FreeBSD上管理多个Postgres实例](https://postgresweekly.com/link/105093/web)
通过使用不同的配置文件和rc.conf.


`Luca Ferrari `
## [如何检查和解决Postgres中的膨胀问题](https://postgresweekly.com/link/105094/web)
一个永恒的话题。


`Asif Rehman `
## [为Postgres设置SSL身份验证](https://postgresweekly.com/link/105095/web)


`Hans-Jürgen Schönig `
## [Ltree层次结构：使用Postgres的Ltree类型将ActiveRecord模型组织到树中](https://postgresweekly.com/link/105096/web)
这个库是为Rubyists提供的，但更普遍的是，从2017年开始，您可以使用LTREE在Postgres中保存一棵树。


`Cédric Fabianski `
# 💡本周提示


**🗓即将举办的Postgres活动**
