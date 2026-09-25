# shashankvemuri/Finance

- 来源: GitHub
- 关键词: quantitative finance
- 链接: https://github.com/shashankvemuri/Finance
- 描述: Python toolkit for quantitative finance: stock analysis, technical indicators, strategy backtesting, portfolio optimization, and financial modeling.
- 语言: Python
- ⭐ 4288
- 最后推送: 2026-09-12

## README 摘要

Finance

Finance is a Python toolkit for market data, technical indicators, financial analysis,
stock screening, strategy research, backtesting, portfolios and statistical models.
Calculations use explicit inputs, a small dependency set and tested execution conventions.
Models and trading rules are research tools; runnable examples are the starting point.

 Install

Python 3.12 or newer:

bash
git clone https://github.com/shashankvemuri/Finance.git
cd Finance
python -m venv .venv
source .venv/bin/activate   Windows: .venv\Scripts\activate
python -m pip install -e .


Core dependencies are NumPy and pandas. Add only the features you need:

bash
python -m pip install -e '.data'              Public data, Finviz and financial statements
python -m pip install -e '.portfolio,models'  Optimizati
