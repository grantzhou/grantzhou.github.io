---
layout: post
title: PostgreSQL 每周新闻 2026-11-11
---
### PostgreSQL每周新闻#673 - 2026年11月11日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/673)

🕒 如果一切顺利，**Postgres 19 的最终版本将在下周（11月19日，周四）发布**，因此我们可能会将下一期推迟一两天，以便更好地报道它。如果下周的通讯比平时晚一点到达，这就是原因。:-)  
__  
*您的编辑，Peter Cooper*

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/ud1tdm04gaspuqkijouh.jpg)

## [UUIDv4 vs UUIDv7：随机主键的代价](https://postgresweekly.com/link/192694/rss)

如果索引能够适配内存，差异很小，但当超出缓存时差异迅速扩大！在内存受限的基准测试中，UUIDv4 插入速度仅为有序键的三分之二，*并且*生成了更多的 WAL。Nikolay 解释了原因，并分享了切换到 `uuidv7()` 时的一些注意事项。

**Nikolay Samokhvalov (PostgresAI)**


## [您的保留任务不应该是四小时的 DELETE 操作](https://postgresweekly.com/link/192693/rss)

使用 DELETE 清除旧行会导致表膨胀、WAL 负载过重，并让 VACUUM 落后。TimescaleDB 按时间分区，因此保留操作可以在毫秒内删除整个块。相同的 Postgres，相同的 SQL。[在 Tiger Cloud 上开始使用 1000 美元的积分](https://postgresweekly.com/link/192693/rss)。

**Tiger Data (TimescaleDB 的创建者) 赞助商**


## [Postgres 真的在获胜吗？](https://postgresweekly.com/link/192695/rss)

Postgres 是 [DB-Engines 排名](https://postgresweekly.com/link/192696/rss)前四名数据库中唯一获得增长的数据库，可能很快就会超过 SQL Server，但它衡量的是"受欢迎程度"，而不是生产使用情况。在[第二部分](https://postgresweekly.com/link/192697/rss)中，Dave 进一步研究了开发者调查、收购以及 AI 工具默认选择的内容。简而言之，Postgres 的前景继续看好。

**Dave Stokes**


### 本周摘要：

- ⏰ **Postgres 的季度次要版本计划明天发布**，同时还有 Postgres 19 RC2。[草案公告](https://postgresweekly.com/link/192698/rss)列出了 140 多个修复和一些更新后的重新索引步骤。请注意，14.25 将是 Postgres 14 的最终版本。

- [Xata 正在加入 ClickHouse](https://postgresweekly.com/link/192699/rss)，其托管 Postgres 服务在同一天[正式发布](https://postgresweekly.com/link/192700/rss)。与此同时，[EDB 收购了 Altinity](https://postgresweekly.com/link/192701/rss)，一个主要的 ClickHouse 贡献者。

- Google 推出了 [AlloyDB Express](https://postgresweekly.com/link/192702/rss)，这是其 Postgres 兼容数据库的可扩展到零的层级，可在几秒钟内启动，旨在用于原型设计和编码代理。它处于预览阶段，提供免费层级。

- 🗓️ 明天（11月12日，格林尼治标准时间下午5点），有一个[免费的在线 *Postgres Meetup for All* 聚会](https://postgresweekly.com/link/192703/rss)，Adyen 的 Huseyin Demir 将分享使用逻辑复制将庞大的 Postgres 集群升级到 v18 时的成功和失败经验。

- 🇧🇪 [FOSDEM 2027 的 Postgres devroom](https://postgresweekly.com/link/192704/rss) 将于 1 月 30 日在布鲁塞尔举行。CFP 开放至 11 月 28 日。


## [为什么 `VACUUM` 不会缩小您的 Postgres 索引](https://postgresweekly.com/link/192705/rss)

使用 `pageinspect` 逐页查看为什么 `VACUUM` 会清理 B-tree 索引页但无法缩小索引，以及为什么顺序键不会重新填充空隙。还有一个[交互式可视化工具](https://postgresweekly.com/link/192706/rss)供您在小型树上尝试。

**Radim Marek**


## [索引扫描只是故事的一半：磁盘上的顺序如何影响性能](https://postgresweekly.com/link/192707/rss)

探讨为什么相同的索引扫描在涉及并行数据加载的迁移后会变得慢得多。Richard 分享了一个 `ctid` 查询来帮助检测问题。

**Richard Yen**


## [Postgres 在等待什么（以及为什么仪表板无法告诉你）](https://postgresweekly.com/link/192708/rss)

等待事件仪表板通过采样工作，因此它们可能正确地反映了整体时间消耗，但却错误地解释了某个请求为何缓慢。

**Dmitry Fomin (PostgresAI)**


📄 [每个 Git Worktree 一个数据库，几乎不占用磁盘空间](https://postgresweekly.com/link/192709/rss) – 在 APFS 或 Btrfs 等写时复制文件系统上使用 Postgres 18 的 `file_copy_method = clone`。*Dennis Paagman*

📄 [我们的"默认" `postgresql.conf`，逐步讲解](https://postgresweekly.com/link/192710/rss) – Data Egret 在设置或接管集群时通常从连接设置开始的基线。*Ilya Kosmodemiansky (Data Egret)*

📊 [关于 Postgres 18 的十三个小测量](https://postgresweekly.com/link/192711/rss) – 例如，未索引的外键会将 13ms 的级联删除变成 3.6 秒。*Hollis Varden*

📊 [`json` vs `jsonb`：大小和速度，实测](https://postgresweekly.com/link/192712/rss) *Chris van Eijk*


### 🛠 代码和工具

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/gsdwwaye2plumcpa5nd4.jpg)

- [PG Observability Map](https://postgresweekly.com/link/192713/rss) – Postgres 架构的交互式地图 *(见上图)*，您可以将鼠标悬停在组件上以查看哪些统计视图和函数涵盖它。灵感来自 Alexey Lesovsky 的 [pgstats.dev](https://postgresweekly.com/link/192714/rss) 图表（似乎已关闭）。

- [Supavisor 2.10](https://postgresweekly.com/link/192715/rss) – Supabase 的多租户 Postgres 连接池新增了一个设置，用于在事务模式下记录或拒绝会话级别的 `SET`、`LISTEN`、咨询锁和临时表。

- [PgQueuer 2.0](https://postgresweekly.com/link/192716/rss) – 基于 Postgres 的 Python 作业队列，构建在 `LISTEN/NOTIFY` 和 `FOR UPDATE SKIP LOCKED` 之上。([文档](https://postgresweekly.com/link/192717/rss)。)

- 🔒 [pgx 5.12](https://postgresweekly.com/link/192718/rss) – 流行的 Go Postgres 驱动程序修复了某些简单协议批处理中的 SQL 注入和影响某些连接设置的服务器身份验证绕过问题。

- [pgstream 1.6](https://postgresweekly.com/link/192719/rss) – Xata 的复制和 CDC 工具修复了重启可能跳过已提交事务的错误。


### 分类广告：

🔍 [针对慢速 Postgres 查询的只读代理](https://postgresweekly.com/link/192720/rss)。无需手动分类、更大实例或额外副本即可实现更快的查询。[免费且开源](https://postgresweekly.com/link/192720/rss)。

[WarpBuild](https://postgresweekly.com/link/192721/rss) 基础设施以一半的成本运行 GitHub Actions，速度快两倍。使用代码 `START50` [获得 50 美元的免费积分](https://postgresweekly.com/link/192721/rss)。

⚡ [Rebase](https://postgresweekly.com/link/192722/rss) 是 Postgres 的开源后端：REST、身份验证、实时和存储，访问规则由 Postgres RLS 强制执行。


### 最后：谁在大象里面？

![img](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/v7qrulepbkg56zf6otkl.jpg)

## [不要梦想它，成为它！](https://postgresweekly.com/link/192723/rss)

Slonik，Postgres 的吉祥物，出现在许多 Postgres 活动中，但是谁在服装里面？在上个月的 PGConf.EU 上，是 Laurenz Albe，他报告说很*热*，你看不到自己的脚，但每个人都想拍照。他对不认识任何人的首次参会者的建议是……志愿服务！

**Laurenz Albe (CYBERTEC)**