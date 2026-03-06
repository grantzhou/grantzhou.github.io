---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: PostgreSQL 每周新闻 2025-10-30
---
### PostgreSQL每周新闻#622 - 2025年10月30日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/622)
![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/fxxr7ew1lsnr4rl5kffr.jpg)
## [pgfeaturediff：比较 Postgres 版本之间的功能](https://postgresweekly.com/link/176351/web)
该网站基于 Postgres 官方功能矩阵，让您可以轻松直接地比较两个您选择的 Postgres 版本之间的功能差异。

`Sebastian Steenssøe`

💡 [PG 版本报告](https://postgresweekly.com/link/176353/web_是一個類似的實用工具，您只需提供伺服器的版本字串，即可查看 CVE、錯誤、EOL 日期以及與 Postgres 17 的比較。


## [Agentic Postgres：在 Postgres 中原生建立 AI 應用程式](https://postgresweekly.com/link/176350/web)
Tiger Data 的全新 Agentic Postgres 将 AI 原生功能引入 Postgres，包括可 fork 的资料库、内建记忆体、混合搜寻和代理 API。只需几秒钟即可建立零拷贝分支，安全地进行实验。在 Tiger 上免费试用，无需信用卡。

`TigerData  `

## [📊 Kafka 速度很快，但我还是会用 Postgres](https://postgresweekly.com/link/176354/web)
受最近一篇关于用 Postgres 代替 Redis 的文章启发，作者决定探究 Postgres 是否足以应对那些你通常会考虑使用 Kafka 的场景。

`Stanislav Kozlovski`

💡 这篇文章引发了 [Hacker News 今年关于 Postgres 最热烈的讨论之一](https://postgresweekly.com/link/176357/web)。


* 🇨🇭 [CERN PGDay 2026](https://postgresweekly.com/link/176358/web) 是一个 Postgres 主题活动，将于明年 2 月 6 日在日内瓦郊外举行。征稿截止日期为 12 月 7 日。

* 🇪🇺 Floor Drees 分享了她[上周参加 PGConf EU 活动的体验](https://postgresweekly.com/link/176359/web)。

* 🎤 Talking Postgres 播客采访了 Postgres 贡献者 Andres Freund，探讨了[在 Postgres 18 中实现非同步 I/O 时遇到的问题（以及成功之处！）](https://postgresweekly.com/link/176360/web)。

* 👥 Postgres 计划[更新了其贡献者页面](https://postgresweekly.com/link/176361/web)，新增了[几位贡献者](https://postgresweekly.com/link/176362/web)，并将四位贡献者晋升为主要贡献者。


## [pg_textsearch：真正的 BM25 排名和混合检索](https://postgresweekly.com/link/176363/web)
Tiger Data 对 ParadeDB 的 BM25 全文搜寻排名印象深刻，因此希望开发一款能够在他们基于 Postgres 的系统上运行的类似工具。目前该工具仅在 Tiger Cloud 上提供预览版，尚不确定未来是否会开源，但我们对此充满期待。

`Green and Arye (Tiger Data)`


📄[使用 Postgres 扩充功能传回多行资料](https://postgresweekly.com/link/176366/web) – 如果您正在开发自己的 Postgres 扩展，本文将对您有所帮助。作者：Shaun Thomas

📄 [Oracle 采用原生布林资料类型 vs. Postgres](https://postgresweekly.com/link/176367/web) – Oracle 终于获得了 Postgres 几十年来一直拥有的功能。作者：Pavan Chary

📄 [Postgres 18 的 UUIDv7：更快更安全的按时间顺序排列的 ID](https://postgresweekly.com/link/176368/web)。作者：Vinicius Negrisolo


## **发布**

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/jspdqcd32umpy3toq4r9.jpg)

## [PostgREST 14.0：适用于任何 Postgres 资料库的 REST API](https://postgresweekly.com/link/176369/web)
一个流行且历史悠久的 Haskell 伺服器，可为您选择的 Postgres 资料库提供 RESTful API。 v14.0 版本说明。

`Steve Chavez and Joe Nelson`

## **📰 分类广告**

日本领先的 C2C 内容创作平台 [note.com](https://postgresweekly.com/link/176371/web) 如何以 JIT 存取控制取代其 GitHub Actions + SSH 代理流程，从而实现更安全的 Aurora Postgres 存取。

🌐 [凭借数十年的 PostgreSQL 经验，我们拥有专业的支援团队，可自信地在任何规模下部署](https://postgresweekly.com/link/176372/web)。


## [pg_easy_replicate 0.4：以最小的停机时间切换资料库](https://postgresweekly.com/link/176373/web)
一个基于 Ruby 的编排器，可简化在两个 Postgres 资料库之间设定逻辑复制的任务，然后让您以最小的停机时间切换到较新的资料库。

`Shayon Mukherjee`


[TimescaleDB 2.23](https://postgresweekly.com/link/176374/web) – 为 Postgres 资料库提供时间序列功能的扩充。现已全面支援 Postgres 18，预设启用 UUIDv7 压缩，并可将超表设定为不记录日志。

[WhoDB 0.66](https://postgresweekly.com/link/176375/web) – 适用于多个资料库的轻量级新一代资料浏览器。

[PgDog 0.1.13](https://postgresweekly.com/link/176376/web) – 为 Postgres 资料库提供自动分片的水平扩展功能。

[ChartDB 1.17](https://postgresweekly.com/link/176377/web) – 开源的基于图表的资料库编辑器。