# Factor-Based-Quantitative-Equity-Backtester
A robust, vectorized Python backtesting engine designed to evaluate multi-factor equity trading strategies. This model simulates a "Mini Quant Fund" by screening a basket of equities, generating buy/sell signals based on technical and momentum factors, executing monthly rebalancing, and rigorously comparing risk-adjusted returns against a benchmark index (NIFTY 50).

Crucially, this engine incorporates real-world trading frictions, including transaction costs and look-ahead bias prevention, to ensure backtest results are realistic and historically reproducible.

[Image of algorithmic trading backtest cumulative returns chart]

## ✨ Core Capabilities

* **Multi-Factor Signal Generation:** Combines trend-following (200-Day SMA), mean-reversion (14-Day RSI), and cross-sectional momentum (3-Month Rate of Change) to identify high-probability entry criteria.
* **Vectorized Backtesting Engine:** Abandons slow, iterative row-by-row looping in favor of high-performance `pandas` matrix operations to calculate signals and returns instantly across the entire asset universe.
* **Realistic Constraint Modeling:** Accurately calculates portfolio turnover during monthly rebalancing to apply realistic transaction costs (commissions/slippage).
* **Institutional-Grade Metrics:** Automatically evaluates performance using Compound Annual Growth Rate (CAGR), Maximum Drawdown (MDD), and the Sharpe Ratio.

## 🛠️ Tech Stack & Skills Demonstrated

* **Language:** Python 3.x
* **Data Ingestion:** `yfinance` (Historical NSE equity and index data)
* **Quantitative Analysis:** `pandas` (Time-series alignment, rolling windows, resample methods), `numpy` (Statistical vector operations

