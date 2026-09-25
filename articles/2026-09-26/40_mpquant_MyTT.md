# mpquant/MyTT

- 来源: GitHub
- 关键词: 同花顺
- 链接: https://github.com/mpquant/MyTT
- 描述: MyTT将通达信,同花顺,文华麦语言等指标公式,最简移植到Python中,核心库单个文件，仅百行代码,十几个核心函数，神奇的实现所有常见技术指标算法（不依赖talib库）的纯python实现和转换通达信MACD,RSI,BOLL,ATR,KDJ,CCI,PSY等公式,全部基于pandas函数计算方法封装，简洁且高性能，能非常方便的应用在股票指标公式,股市期货量化框架分析,自动程序化交易,数字货币量
- 语言: Python
- ⭐ 2868
- 最后推送: 2026-06-13

## README 摘要

MyTT (My麦语言 T通达信 T同花顺)
MyTT是您量化工具箱里的瑞士军刀，精炼而高效，它将通达信,同花顺,文华麦语言等指标公式indicators,最简移植到Python中,核心库单个文件，仅百行代码,实现和转换同花顺通达信所有常见指标MACD,RSI,BOLL,ATR,KDJ,CCI,PSY等,全部基于numpy和pandas的函数封装，简洁且高性能，能非常方便的应用在各自股票股市技术分析，股票自动程序化交易,数字货币BTC等量化等领域.Mini Python library with most stock market indicators.

license(https://img.shields.io/:license-gpl-blue.svg)(https://badges.gpl-license.org/)

 功能特点
 核心库轻量化： 项目库就一个文件 MyTT.py(https://github.com/mpquant/MyTT/blob/main/MyTT.py),不用安装设置，可自由裁剪，随用随走 from MyTT import  即可 

 代码人类化：)  没有什么炫耀的编程花样，初学者也能看懂，自己就能自行增加指标，马上就能用在项目中。

 不需要安装ta-lib库,是纯python代码实现的的核心逻辑，很多人都有安装ta-lib库的痛苦经历

 和通达信，同花顺的指标写法完全兼容，一个新的指标基本不用做修改，直接拿来即可使用

 超高性能，基本不用循环，全是靠numpy,pandas的内置函数实现各种指标

 和Talib库一样是多天参数进，多天指标出（序列进，序列出），便于画图和观察趋势

 MyTT实现的各种指标和通达信，同花顺，雪球等软件的技术指标一致到小数点后2位

 MyTT高级进阶版本，收录了高级复杂用法的函数和实验验证
