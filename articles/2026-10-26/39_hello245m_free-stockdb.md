# hello245m/free-stockdb

- 来源: GitHub
- 关键词: a股 量化
- 链接: https://github.com/hello245m/free-stockdb
- 描述: 面向 A 股日K、分钟K与ETF分钟数据的本地量化引擎，集成增量同步、本地缓存、复权、批量查询、回测与指标计算。
- 语言: HTML
- ⭐ 3045
- 最后推送: 2026-10-12

## README 摘要

08-10windows，macos，alpine，manylinux版本已发布。08-04mac，linux版本完成，已通过多轮压力测试，即将发布。

 free-stockdb

 本地量化数据引擎

面向 A 股日K、分钟K与 ETF 分钟、tick级数据的本地量化引擎。free-stockdb 将数据同步、清洗、复权、组织为可直接用于批量查询、批量计算研究的数据底座。

❤️双击更新 - 双击启动 - 直接调用。


下载地址1(http://1783355894)

下载地址2(https://github.com/hello245m/free-stockdb/releases/tag/测试版本0.3.5)



数据本地落盘，研究不再依赖远程接口。

| 本地优先 | 增量同步 | 数据支持(按需) | 本地指标计算 | 五种调用方式 |
|---|---|---|---|---|
| 数据在用户磁盘 | 只处理变化数据 | 日/周/月/1/5/15/30分钟/tick | 39 种指标、5 种指数 | Python / HTTP / Excel / HTML / MCP |

mermaid
flowchart TB
    A"数据更新：同步、清洗、复权、增量" -- B"free-stockdb 本地数据与计算引擎"
    B -- C"Python SDK"
    B -- D"HTTP API"
    B -- E"Excel / WPS"
    B -- F"HTML 网页"
    B -- G"AI MCP"


同步后的查询、计算、回测和接口都使用本机数据，不与远程请求链路耦合。

 为什么需要本地数据引擎

全市场批量回测的瓶颈不是策略代码，而是数据工程。以全市场 7000+ 股票分钟线回测为例，远程 API 方案的真实工作量：

|
