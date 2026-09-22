# sngyai/Sequoia-X

- 来源: GitHub
- 关键词: akshare
- 链接: https://github.com/sngyai/Sequoia-X
- 描述: A股自动选股系统 — 多种技术形态自动扫描，收盘后自动运行并推送飞书
- 语言: Python
- ⭐ 7512
- 最后推送: 2026-07-10

## README 摘要

Sequoia-X: 王者回归 | The King Returns

 A 股量化选股系统 V2 | A-Share Quantitative Stock Selection System V2

---

 简介 | Introduction

Sequoia-X V2 是面向 A 股市场的量化选股系统，基于现代 Python 工程化标准从零重构。
系统以 OOP 架构、向量化计算和增量数据更新为核心设计原则，每日收盘后自动选股并推送至飞书群。

数据层使用 baostock(http://baostock.com)（免费、无需注册、无限流）拉取历史及增量日 K 数据（后复权），
存储于本地 SQLite，彻底规避东方财富反爬问题。

---

 两种运行模式

bash
python main.py                日常模式：8进程增量补数据 + 跑策略 + 飞书推送（2~3分钟）
python main.py --backfill      回填模式：全市场历史K线一次性灌入（约12分钟）


---

 内置策略 | Strategies

| 策略 | 说明 |
|---|---|
| TurtleTrade | 海龟突破：20日新高 + 成交额过亿 + 阳线防诱多，按涨幅排序 |
| MaVolume | 均线+放量突破 |
| HighTightFlag | 高而窄的旗形整理突破 |
| LimitUpShakeout | 涨停洗盘回踩确认 |
| UptrendLimitDown | 上升趋势中的跌停反包 |
| RpsBreakout | 欧奈尔 RPS 相对强度突破 |

---

 快速开始 | Quick Start

 环境要求

- Python = 3.10

 1. 安装依赖

bash
 推荐使用 uv（快速包管理器）
u
