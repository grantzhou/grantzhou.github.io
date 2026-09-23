---
layout: post
title: PostgreSQL 每周新闻 2026-9-23
---
### PostgreSQL每周新闻#666 - 2026年9月23日
![_config.yml]({{ site.baseurl }}/assets/img/PostgresWeekly.png)

备注：[英文原文地址](https://postgresweekly.com/issues/666)

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/orpeyafvjtdmeurbgwki.jpg)

## [展望 Postgres 19：尾声](https://postgresweekly.com/link/190698/rss)

Postgres 19 的 beta 测试阶段充满波折，多个重要特性被撤回且发布日期未定。Shaun 通过 `pgsql-hackers` 邮件列表深入分析原因，并指出 AI 辅助审查发现漏洞的速度超过了提交者处理的能力。关于**好消息**，Elizabeth Garrett Christensen [列出了仍将发布的内容](https://postgresweekly.com/link/190699/rss)，如并行 autovacuum 和 `ON CONFLICT DO SELECT`。

**Shaun Thomas (pgEdge)**

💡 **Beta 4 预计明天（9月24日）发布。** [这份**草稿**发布公告](https://postgresweekly.com/link/190700/rss)列出了撤回的内容，发布候选版本应在10月初发布。

## [分析不应该意味着需要第二个数据库](https://postgresweekly.com/link/190701/rss)

随着数据增长，仪表板查询变慢，通常的解决方案是添加一个仓库和一个管道：同步作业、延迟、过时副本。TimescaleDB 扩展了你已经运行的 Postgres，因此分析在实时数据上保持快速。[获取 $1000 信用额度开始使用](https://postgresweekly.com/link/190701/rss)

**Tiger Data (TimescaleDB 的创建者) 赞助商**

---

## 本周摘要：

- 🔎 PlanetScale [推出了 TIN](https://postgresweekly.com/link/190702/rss)，一个用于 Postgres 的快速 BM25 全文搜索索引。它是闭源的，仅限 PlanetScale 使用，不过他们提供了 [Lead](https://postgresweekly.com/link/190703/rss)，一个开源的**"慢但正确的替代品"**，用于在本地测试 TIN 查询。

- 🎧 在 *Talking Postgres* 节目中，Claire Giordano [与 Peter Eisentraut 交谈](https://postgresweekly.com/link/190704/rss)，谈论他为 Postgres 贡献的 25 年，这始于 `psql` 的 tab 补全功能。

- 🇨🇦 [PGConf.dev 2027](https://postgresweekly.com/link/190705/rss) 将于5月11-14日在蒙特利尔举行。注册已开放。它一直很受欢迎，你可以在[这里观看今年的演讲](https://postgresweekly.com/link/190706/rss)。

- [Google 在 AlloyDB 和 Cloud SQL 中预览了原生 BM25 搜索](https://postgresweekly.com/link/190707/rss)，基于 [`pg_textsearch`](https://postgresweekly.com/link/190708/rss) 扩展构建。

---

## ⚙️ 运维与性能

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/f967fqujsh9acwnl9qvn.jpg)

## [pgBackRest 压缩：更小的备份值得多少 CPU？](https://postgresweekly.com/link/190709/rss)

对 pgBackRest 的压缩算法和级别进行基准测试，找出额外 CPU 在缩小备份方面停止发挥作用的点。剧透：**"低级别的 Zstandard 是最佳选择"**。

**Agustín Gallego (Percona)**

## [Postgres 逻辑复制的十年](https://postgresweekly.com/link/190710/rss)

回顾从 Postgres 10 到 19 的每个版本为逻辑复制添加的内容，通过仅使用核心特性构建多服务器写入设置来展示。

**Dimitri Fontaine**

## [当删除旧行的成本超过工作本身](https://postgresweekly.com/link/190711/rss)

为拥有大表的人提供一些经验教训，批量删除的成本可能超过写入。DBOS 的工程师分享了一些修复方法，比如用批量删除替换级联删除并运行手动 vacuum。

**Kraft and Li (DBOS)**

📄 [Postgres 在哪里存储行锁](https://postgresweekly.com/link/190712/rss) – 每个行锁最终都会作为对堆页的写入，如 `pageinspect` 所示。*Radim Marek*

---

## 🛠 代码和工具

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/w0fiwim4hc6clvxcy8ra.jpg)

## [pgcli 4.7：更友好的 `psql` 现在也可用于脚本](https://postgresweekly.com/link/190713/rss)

一个流行的交互式工作 `psql` 替代品，具有上下文感知的自动补全、语法高亮和命名查询。v4.7 通过 psql 风格的 `-c`、`-f` 和 `-t` 标志，以及 `-y` 跳过破坏性命令提示，使其对脚本编写更有用。

**the dbcli project**

## [pgwrh 1.0 Alpha：使用分片副本的读取扩展](https://postgresweekly.com/link/190714/rss)

一个实验性扩展，将分区表分片到读取副本中，每个副本仅保存部分数据，并从对等节点获取其余数据。不适用于生产环境！

**Michał Kłeczek**

## [pgColumnar 1.0 Alpha 4：列式表访问方法](https://postgresweekly.com/link/190715/rss)

Postgres 表的列式存储选项。这个 alpha 版本可以沿 [Hilbert 曲线](https://postgresweekly.com/link/190716/rss)布局表，因此范围过滤器读取的行组比 Z-order 少多达 2 倍。

**Joshua D. Drake (Command Prompt)**

- [TimescaleDB 2.30](https://postgresweekly.com/link/190717/rss) – Tiger Data 的时间序列扩展使 `ORDER BY ... LIMIT` 查询即使在拥有大量 chunk 的 hypertable 上也很快。

- [PostgreSQL Anonymizer 3.2](https://postgresweekly.com/link/190718/rss) – Dalibo 的数据脱敏扩展增加了更快的假名化函数，并修复了 3 个严重漏洞。

- [pgAdmin 4 v9.18](https://postgresweekly.com/link/190719/rss) – 流行的 Postgres 管理工具。

---

## 📰 分类广告

🚀 将您的 Postgres 生产力提高三倍。[pgEdge AI DBA Workbench](https://postgresweekly.com/link/190720/rss)：用于任何 Postgres v14+ 的 AI 监控和诊断。[开源](https://postgresweekly.com/link/190720/rss)。

🎟️ 10月2日加入我们的 [Supabase Select](https://postgresweekly.com/link/190721/rss)。向行业最佳构建者学习，结识构建开发工具的人。[申请参加享受 25% 折扣：SUPAWEEKLY](https://postgresweekly.com/link/190721/rss)。

---

## 最后...

![](https://res.cloudinary.com/cpress/image/upload/w_1280,e_sharpen:60,q_auto/yp3rlgkd8o5yxbhj9l2b.jpg)

## [🤖 教 4B 模型编写快 81% 的查询计划](https://postgresweekly.com/link/190722/rss)

作为在 Recurse Center 的休假项目，一位开发者使用强化学习训练一个小型模型为连接密集的基准查询编写 `pg_hint_plan` 提示（在其最佳运行中，它击败了 Postgres 自己的计划！）。一篇引人入胜的文章。

**Rohan Bansal**