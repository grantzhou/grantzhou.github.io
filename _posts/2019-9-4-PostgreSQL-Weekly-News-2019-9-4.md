---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2019-9-4
---
### PostgreSQL每周新闻#321 - 2019年9月4日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/321)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60/nfgxq8b2htpbgfqcp0ue.jpg)
## [pspg：为postgres表设计的unix分页器](https://postgresweekly.com/link/69363/web)
如果您使用psql，您可能会用less它作为分页器，但它不直接支持表格数据。将要介绍的这个是支持的！最新的主分支版本还支持按列排序。

`Pavel Stehule `

## [如何使用pl/pgsql计算日期范围内的工作小时数](https://postgresweekly.com/link/69365/web)
在一系列日期中有多少工作时间？一个使用pl/pgsql实现的，方便、完美的、容易理解的例子。

`Luca Ferrari `

## [因为你的数据是你的业务](https://postgresweekly.com/link/69366/web)
PGX提供完整的PostgreSQL支持，从紧急服务到日常运营支持，再到战略规划。我们来这里是为了你的数据操作。

`PostgreSQL Experts, Inc. `

## [PostgreSQL 12如何提高性能](https://postgresweekly.com/link/69367/web)
“只需升级就有性能提升”。Postgres12增强了CTE查询，默认情况下对查询进行了JIT编译，索引也得到了改进。

`Jonathan S. Katz `

## [为什么需要用pl pgsql检查你写的pl/pgsql存储过程](https://postgresweekly.com/link/69368/web)
pl/pgsql允许您直接在postgres和sql查询中编写和执行一些非常高级的逻辑，plpgsql检查可以帮助您解决性能和sql注入问题。

`Pavel Stěhule `

## [在google云平台（gcp）上运行postgresql](https://postgresweekly.com/link/69369/web)
看看谷歌平台为postgres用户提供的功能。

`Viorel Tabara `

## [如何设置在amazon rds上测试postgres12beta3](https://postgresweekly.com/link/69370/web)
aws提供postgres的beta版本，用于在其美国东部2地区的“预览环境”中进行测试。

`Jignesh Shah `

## [集装箱时代的it监控：ebpf可观测性的挖掘](https://postgresweekly.com/link/69371/web)
`InfluxData `
## [Postgres连接字符串和PSQL](https://postgresweekly.com/link/69372/web)
你知道有三种不同的方法可以建立到同一个数据库的连接吗？一种键/值方法，流行的“url”方法，在psql中使用命令行选项。

`Dimitri Fontaine `

## [使用pgBackRest设置远程备份和恢复](https://postgresweekly.com/link/69373/web)
`Granthana Biswas `
## [向postgres中添加二进制I/O类型](https://postgresweekly.com/link/69374/web)
`Johann 'Myrkraverk' Oskarsson `
## [Postgres的周期和系统版本控制](https://postgresweekly.com/link/69375/web)
preriod是一个sql:2016特性，有点像postgres的范围类型，这个扩展在postgres中实现了一些基本支持。

`Vik Fearing `

# 💡本周提示
**使用distinct on的基本示例**

上周，我们的技巧是关于select distinct，这是一种不使用group by从列中轻松选择唯一值的方法。本周，我们又向前迈了一步！

当select distinct从列中选择唯一值时，select distinct on选择可以明显匹配各种条件的第一行。这很难单独用文字来解释，所以让我们试试最简单的例子。

让我们创建一个表来存储不同位置的温度。在真实的案例中，您可能也会有一个与时间相关的列，但为了简洁起见，我们在这里使用int：

```
CREATE TABLE temperatures
  (location TEXT,
   temp INT);
   
INSERT INTO temperatures
  (location, temp)
  VALUES
  ('Springfield', 71),
  ('Springfield', 74),
  ('Springfield', 64),
  ('Springfield', 56),
  ('Miami', 84),
  ('Miami', 77),
  ('Miami', 91);
```
现在，假设我们只想得到每个位置记录的最高温度。使用distinct on来完成这个任务：
```
SELECT DISTINCT ON(location) * 
  FROM temperatures
  ORDER BY location, temp DESC;
  
    location |  temp
--------------------
       Miami | 91 
 Springfield | 74
```
如果我们没有使用DISTINCT，我们会得到所有的位置和温度随温度的降序排列。然而，Distinct on（location）将结果分解为每个位置的第一个匹配结果，为每个位置计算出最高温度。

**🗓即将举办的Postgres活动**

- [PostgreSQL Conference Asia 2019](https://postgresweekly.com/link/69378/web)（9月8日至11日，印度尼西亚巴厘岛）
- [PostgresOpen 2019](https://postgresweekly.com/link/69379/web)（9月11日至13日，佛罗里达州奥兰多）-两天的时间里，到处都是关于PostgreSQL和相关技术的教程和演示。
- [PostgresConf Silicon Valley 2019](https://postgresweekly.com/link/69380/web)（9月18日至20日，圣何塞）-时间表（包括培训）现已公布。
- [PostgresConf South Africa 2019](https://postgresweekly.com/link/69381/web)（10月8日至9日，约翰内斯堡）-这是数据库管理和使用postgres的开发人员相互了解的机会。
- [PostgreSQL Conference Europe 2019](https://postgresweekly.com/link/69382/web)（10月15日至18日，意大利米兰）
