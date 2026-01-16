---
layout: post
categories: [PostgreSQL]
tags: [PGWeekly]

title: Pgpool-II 4.0.0和pgpoolAdmin 4.0.0现已正式发布。
---

由Pgpool Global Development Group发布于2018-10-21

## 什么是Pgpool-II？

Pgpool-II是一个工具，它为PostgreSQL添加了很多有用功能，包括：
* 连接池
* 负载均衡
* 自动故障转移等等。

## 主要版本
Pgpool全球开发组（Pgpool Global Development Group）很高兴宣布推出Pgpool-II 4.0.0和pgpoolAdmin 4.0.0。

Pgpool-II 4.0.0具有以下新功能：
* 添加SCRAM和证书身份验证支持。
* 检测PostgreSQL的“假”主服务器。
* 负载平衡的改进：
* 写查询后更多负载平衡精细控制。
* 特定查询的负载平衡控制。
* 允许为负载平衡参数指定负载平衡权重。
* 将最后一个状态更改时间戳添加到SHOW POOL NODES。
* 导入PostgreSQL 11 SQL解析器。
* 记录客户端消息。
等等

[请查看发行说明。](http://www.pgpool.net/docs/latest/en/html/release.html)
您可以[下载源代码和RPM](http://pgpool.net/mediawiki/index.php/Downloads)。

### [PG相关的开源项目](https://www.postgresql.org/about/newsarchive/related/)
