---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2021-9-1
---
### PostgreSQL每周新闻#420 - 2021年9月1日
![_config.yml]({{ site.baseurl }}/images/PostgresWeekly.png)
备注：[英文原文地址](https://postgresweekly.com/issues/420)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/jnxtjwrgsljajf5mvegc.jpg)
## [用Postgres解决背包问题](https://postgresweekly.com/link/113075/web)
“背包问题”是一个数学难题，它将一组物品组合在一起，以在指定的限制内获得最大值（有点像将物品装入袋子）。Postgres能帮助组合优化吗？有办法。


`Francesco Tisiot `
## [Postgres中被认为有害的子事务](https://postgresweekly.com/link/113077/web)
这个标题有点容易点击，但尽管如此，本文还是详细介绍了在使用嵌套事务（许多orm和框架可能会为您使用）时可能遇到的一些不利因素，以及改进它们的方法。


`Nikolay Samokhvalov `
## [只需30秒，在Postgres上获得即时实时GraphQL和REST API](https://postgresweekly.com/link/113078/web)
将Hasura经过授权连接到新的或现有的PG数据库，以立即获得REST和GraphQLAPI。支持所有类型的Postgres作品，包括Citus、Timescale、Yugabyte、postgis和vanilla PG。开源，深受开发者喜爱，下载次数超过3亿次。


`Hasura `
## [亚马逊Aurora现在支持Postgres 13](https://postgresweekly.com/link/113079/web)
亚马逊面向性能的“它看起来像Postgres，闻起来像Postgres，但不完全是Postgres”数据库现在与Postgres 13兼容。


`Amazon Web Services `
## [MongoDB的首席技术官Mark Porter，Postgres和MongoDB](https://postgresweekly.com/link/113080/web)
▶两集播客（每集一小时）深入挖掘MongoDB的CTO，他在数据库领域有着广泛的历史，包括在AWS RDS和Aurora项目上的领导努力。


`Joshua D. Drake podcast`
## [如何使用generate_Series（）创建大量样本时间序列数据](https://postgresweekly.com/link/113081/web)
generate_series（）函数提供了一种方便的方法来创建大量数据，例如用于测试、处理SQL查询或基准测试。


`Ryan Booz (Timescale) `
## [缺失一个索引的影响](https://postgresweekly.com/link/113082/web)
我想这是我们第一次链接到以诗的形式写的项目（！）汉斯·尤尔根（Hans-Jürgen）用他的文学之手转向描述一种情况，即失去一个索引会阻碍性能。


`Hans-Jürgen Schönig `
## [Crunchy Bridge：完全管理的多云Postgres](https://postgresweekly.com/link/113083/web)


`Crunchy Bridge `
## [UUID还是缓存序列？](https://postgresweekly.com/link/113084/web)
UUID可能不按顺序排列，但它们生成速度快，在大规模系统中工作良好。Franck考虑了这个属性，但也考虑了调整序列缓存大小如何使序列也具有可伸缩性。


`Franck Pachot `
## [如何在Shell中获得咨询锁？](https://postgresweekly.com/link/113085/web)
当然，Postgres的咨询锁有一个奇怪的用途。


`Hubert depesz Lubaczewski `
## [仅插入表和Postgres 13之前的自动Vacuum问题](https://postgresweekly.com/link/113087/web)
如果您在早于Postgres 13的数据库中有只插入表，那么本文将探讨如何从运行定期vacuum中获益。


`David Christensen `
# 💡本周提示


**🗓即将举办的Postgres活动**
