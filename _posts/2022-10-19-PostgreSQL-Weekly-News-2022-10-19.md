---
layout: post
title: PostgreSQL 每周新闻 2022-10-19
---
### PostgreSQL每周新闻#477 - 2022年10月19日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/477)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,e_trim,w_300,h_160/e_make_transparent/co_white,e_outline:7/rrkstxca0vg7e1eww6yw.jpg)
## [Postgres全文搜索与其他](https://postgresweekly.com/link/130315/web)
只要您了解限制（或解决它们），Postgres 的全文搜索功能可以带您走很长的路。Victor 展示了基础知识，并将 Postgres 提供的功能与一些流行的现代替代方案进行了比较。这篇文章引发了对 Hacker News 的广泛讨论，讨论得更深入一些。


`Victor Vados `
## [看一看 Postgres 15：MERGE带有示例的命令](https://postgresweekly.com/link/130318/web)
Postgres 15 的主要新特性之一是对 SQL 标准MERGE语句的支持。您可能曾经使用过的地方UPSERT .. ON CONFLICT，MERGE现在可以通过根据表之间的差异插入、更新和删除行来完成同步表的繁重工作——Jean-Paul 向我们展示了一个用例。


`Jean-Paul Argudo `
## [在几分钟内扩展 Postgres](https://postgresweekly.com/link/130319/web)
 PolyScale 是一种智能的无服务器数据库边缘缓存。使用 PolyScale，您可以在全球范围内分布数据库计算和存储，从而显着降低数据驱动应用程序的延迟。


`PolyScale.ai `
## [流式数据库“呈现”为 Postgres 的方式和原因](https://postgresweekly.com/link/130320/web)
Materialize是一个分布式 SQL 数据库，它不是Postgres，但像许多新兴的数据库系统一样，可以“说出” Postgres 的有线协议以提供互操作性。这篇文章很有趣，但很少见，看看为什么数据库开发人员越来越多地做出这个决定。


`Andy Hattemer (Materialize) `
## [为Postgres 15的公共模式更改做好准备](https://postgresweekly.com/link/130322/web)
Postgres 15引入了与您需要准备的公共模式相关的特权更改——幸运的是，即使在升级之前，您也可以从Paul的建议中受益。


`Paul Ramsey `
## [更新速度变慢？原因和补救措施](https://postgresweekly.com/link/130327/web)
如果事情变得越来越慢，而且你更新表的次数越多，你就会遇到需要快速解决的问题。Laurenz 展示了这样一个原因。


`Laurenz Albe `
## [Postgres 15的配置更改](https://postgresweekly.com/link/130328/web)
快速浏览Postgres15的postgresql中的一些更改。conf选项（其中有6个新项、3个已更改项和1个已删除项-au revoir、stats temp_directory）。


`Ryan Lambert `
## [为Aurora PostgreSQL构建的性能测试框架](https://postgresweekly.com/link/130329/web)
如何使用 CloudFormation、Apache JMeter 和 Python 为基于 Postgres 的 Aurora 数据库构建性能测试框架。


`Amazon Web Services `
## [使用pg_upgrade通过yum将Postgres 9.6和PostGIS 2.4升级到Postgres15 3.3](https://postgresweekly.com/link/130330/web)
通过这些迁移跟随别人的足迹总是好的。


`Regina Obe `
## [注册解锁22-Buildkite举办的CI/CD会议](https://postgresweekly.com/link/130331/web)
📅  


`Buildkite `
## [使用PGDG RPM包在Red Hat衍生发行版上升级Postgres 14至15](https://postgresweekly.com/link/130332/web)
想想 Fedora、RHEL、CentOS、Rocky、Alma Linux 等。


`Jon Jensen `
## [全局索引：另一种解决方法？](https://postgresweekly.com/link/130333/web)
这还不是 Postgres 的功能，但 David 考虑了一种为分区表创建全局索引的方法。


`David Zhang `
## [pg_enquo：一种针对加密数据进行安全查询的方法](https://postgresweekly.com/link/130336/web)
Enquo（代表“加密查询操作”）是一种公认​​的小众（目前）方法，因为它还需要客户端支持（目前仅在 Rust 和 Ruby 中），但看到实验很有趣在这个重要的领域。


`Matt Palmer `
## [OxideDB：教Postgres如何讲MongoDB的有线协议](https://postgresweekly.com/link/130338/web)
一个看起来像 MongoDB 数据库服务器的翻译层，同时使用 PostgreSQL 的 JSON 功能作为底层数据存储。


`Felipe Coury `
## [PostgresML 2.0：训练模型并根据SQL进行预测](https://postgresweekly.com/link/130339/web)
“您使用简单的SQL命令训练模型，并通过您已经使用的机制在应用程序中获得预测：通过标准Postgres连接进行查询。”v2.0是Rust中的1.0兼容完全重写。


`Lev Kokotov and Montana Low `
# 💡本周提示


**🗓即将举办的Postgres活动**
