Equity Analysis — Python
Personal finance project portfolio built during my Summer Internship Programme (SIP) 2026.
All analysis is done in Python using Google Colab — data sourced from NSE via Yahoo Finance.

Repository Structure
Equity-Analysis/
│
├── Equity Analysis.ipynb              ← Week 1: Return & Volatility Analysis
├── week2_momentum_screener.ipynb      ← Week 2: Nifty 50 Momentum Screener
├── nifty50_momentum_screener.csv      ← Screener output data (Excel-ready)
└── equity_executive_summary.docx      ← Executive summary report (Week 1)

Projects
Week 1 — Return & Volatility Analysis
Stocks: HDFC Bank · Reliance · Infosys · TCS · ICICI Bank
Benchmark: Nifty 50
Period: 1 Year
What it covers:

1-year price trend and normalised returns vs Nifty 50 benchmark
Daily return distributions and cumulative return comparison
Annualised volatility and 30-day rolling volatility
Correlation heatmap across the 5-stock basket
Summary dashboard — Sharpe ratio, max drawdown, best/worst day, % positive days

Key finding: ICICI Bank had the best risk-adjusted return (Sharpe: 0.87 over 5Y) with the lowest max drawdown (-22.3%). Infosys-TCS showed 0.80 correlation — holding both adds minimal diversification benefit.

Week 2 — Nifty 50 Momentum Screener
Universe: All 50 Nifty stocks across 14 sectors
Period: 1 Year (data as of May 2026)
What it covers:

Returns calculated across 4 timeframes — 1M, 3M, 6M, 1Y
Composite momentum score using weighted ranking (1Y: 30%, 6M: 30%, 3M: 25%, 1M: 15%)
Buy / Neutral / Avoid signals based on composite rank
Top 10 leaders and Bottom 10 laggards with bar charts
Sector momentum heatmap — average returns by sector across all timeframes
Full 50-stock heatmap
CSV export for Excel-based analysis

Key finding: Energy and Metals dominated — HINDALCO ranked #1 (1Y: +66.6%), driven by India's infrastructure capex cycle and commodity recovery. IT sector ranked last — INFY, HCLTECH, and TCS all negative across every timeframe, reflecting the US tech spending slowdown.

Tools & Libraries
ToolPurposePython 3Core languageyfinanceNSE/BSE price data via Yahoo FinancepandasData manipulation and return calculationsnumpyStatistical computationsmatplotlibPrice charts, bar charts, return plotsseabornCorrelation and heatmap visualisationsscipyRegression (CAPM Beta — upcoming)Google ColabCloud execution environment

How to Run

Open Google Colab
Click File → Upload notebook
Select any .ipynb file from this repo
Click Runtime → Run all
All data downloads automatically — no manual input required


Note: Momentum screener downloads data for all 50 stocks and takes approximately 60 seconds to complete Section 2.


Key Concepts Covered
Return Analysis

Daily, cumulative, and annualised returns
Calendar year performance breakdown
% positive trading days

Risk & Volatility

Annualised volatility (σ × √252)
Rolling 30-day volatility
Max drawdown and current drawdown from peak

Risk-Adjusted Performance

Sharpe Ratio = (Return − Risk-Free Rate) / Volatility
Treynor Ratio = (Return − Risk-Free Rate) / Beta
India 10-Year G-Sec (6.8%) used as risk-free rate

Portfolio Theory

Correlation matrix and diversification analysis
Sector rotation via heatmap

Momentum Factor

Multi-timeframe return ranking
Composite weighted scoring
Sector-level momentum clustering


Upcoming

Week 3: CAPM Beta and Sharpe Ratio Analysis (Old Economy vs New-Age Tech)
Week 4: Equity Research Note — fundamental analysis on a single stock
Week 5: DCF Valuation Model in Excel


Author
Kishore
PGDM Finance — Thiagarajar School of Management (TSM), Madurai
SIP 2026

Data sourced from Yahoo Finance via yfinance. All analysis is for learning and portfolio-building purposes only and does not constitute investment advice.
