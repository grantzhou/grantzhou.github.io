---
layout: post
title: PostgreSQL 每周新闻 2022-7-13
---
### PostgreSQL每周新闻#463 - 2022年7月13日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/463)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/s9qtubbavnoqyklkrzoh.jpg)
## [Postgres 15 如何改进UNIQUE以及NULL](https://postgresweekly.com/link/126098/web)
作者查看了最新的 Postgres 15 beta 版，并深入UNIQUE对具有值的列的约束NULL其中可以使 Postgres 将空值视为不同的值或不视为不同的值。开发此功能的 Peter Eisentraut 突然出现在 Hacker News上指出： “这里的背景是 SQL 标准对于实现应该表现的两种方式中的哪一种是模棱两可的。因此，在即将发布的 SQL:202x 中，通过定义行为实现并添加此NULLS [NOT] DISTINCT选项来选择其他行为来解决此问题。”


`Ryan Lambert `
## [在几分钟内在全球范围内扩展您的 Postgres 实例](https://postgresweekly.com/link/126100/web)
PolyScale.ai 是一种即插即用的数据库边缘缓存，可让您的数据库查询在任何地方都保持快速。运行低延迟、多区域应用程序或无服务器功能，无需传统数据库扩展的成本和复杂性。


`PolyScale.ai `
## [Postgres 中的列顺序很重要](https://postgresweekly.com/link/126101/web)
您可能认为数据库表中的列顺序只是该表历史的一个微不足道的结果，在技术层面上并不重要。但它可以，Hans-Jürgen 说，尽管他的例子确实依赖于一个特别极端的例子（！）


`Hans-Jürgen Schönig `
## [2022 年 PostgreSQL 现状调查的初步结果](https://postgresweekly.com/link/126103/web)
处理数据以从大型社区调查中找到见解需要一段时间，因此 Timescale 首先从人口统计数据看浅层（值得注意的是，大多数受访者不是来自北美）和一些开放式问题的答案。


`Ryan Booz `
## [关于 GitLab 的 Postgres 模式设计的一些注意事项](https://postgresweekly.com/link/126108/web)
自从我们看到一篇真实世界的数据库设计文章在巡回演出以来，已经有很长一段时间了，所以很高兴看到 Shekhar 在 Gitlab（似乎设计得很好）的数据库中闲逛了一下。


`Shekhar Gulati `
## [Data to Go：Postgres 逻辑复制](https://postgresweekly.com/link/126109/web)
需要定期将您的数据复制到新位置以进行进一步处理、合并或更多操作？Postgres 10+ 的逻辑复制适合你。这是一个快速解释器，也将其与流复制进行了比较。 


`Elizabeth Christensen `
## [使用OpenCensus和 Google Cloud Tracing 跟踪 Gorm 查询](https://postgresweekly.com/link/126110/web)
GORM是Go 的强大 ORM，Incident 的团队使用它来处理他们的 Postgres 数据库。以下是他们跟踪正在发生的事情以密切关注性能的方式。


`Alex Russell-Saw `
## [免费电子书：了解数据库](https://postgresweekly.com/link/126112/web)
l,null,"en


`Linode `
# 💡本周提示


**🗓即将举办的Postgres活动**
