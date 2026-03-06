---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2023-4-19
---
### PostgreSQL每周新闻#502 - 2023年4月19日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/502)
![img](https://res.cloudinary.com/cpress/image/upload/c_fill,g_auto,w_430,h_100/e_make_transparent/co_white,e_outline:7/xyflkz7n00elwtgja9ne.png)
## [dbdev:一个Postgres包管理器](https://postgresweekly.com/link/138502/web)
Supabase 的人们已经将database.dev置于预览状态，该网站包含许多Postgres 的可信语言扩展，建立在AWS 去年开始的一个想法之上。将其视为或dbdev的一种 Postgres 等价物。现在还处于早期阶段，但总体思路是使将扩展安装到 Postgres 环境（包括在云中）变得更容易。


`Supabase `
## [Postgres和SQL:2023:支持什么？](https://postgresweekly.com/link/138505/web)
Peter 最近发布了 SQL:2023 的进展，但现在他快速浏览了 Postgres 实际支持的部分。


`Peter Eisentraut `
## [你一直想要的Postgres提供商](https://postgresweekly.com/link/138501/web)
“Crunchy 是一种多么不同的支持体验。每张支持票都很有价值。我们被鼓励提出问题。我们能够与一个关心数据的合作伙伴一起做更多的工作我们的确是。”


`Crunchy Bridge `
## [分区可以太多吗](https://postgresweekly.com/link/138525/web)
Kaarel 运行了一些基准测试（总共耗时 56 小时）以查看具有 0 到 4096(!) 个分区的性能影响。最终，不是很多： “Postgres 似乎可以很好地处理“正常”数量的分区 - 计划时间似乎按百分比稳步增加，但实际数字并不值得注意。”


`Kaarel Moppel `
## [Postgres 16 数组采样和洗牌函数](https://postgresweekly.com/link/138513/web)
还有更多点点滴滴进入 Postgres 16（预计今年晚些时候发布最终版本），其形式array_sample和array_shuffle功能是从数组中获取随机元素或随机化整个数组。


`Hubert depesz Lubaczewski `
## [Postgres 16 中数字常量中的下划线](https://postgresweekly.com/link/138514/web)
这是相对较小的生活质量改进，但 Postgres 16 将允许您以这种方式编写长数字：1_500_000_000甚至是不太明显的结构，如 3.14159_26535_89793


`Pavlo Golub `
## [PostgREST 11.0：从 Postgres 数据库提供 RESTful API](https://postgresweekly.com/link/138517/web)
这个流行的基于 Haskell 的系统的v11添加了许多细节


`Nelson and Chavez `
# 💡本周提示


**🗓即将举办的Postgres活动**
