My First Quant Project
--
This project is a beginner-level exploration of algorithmic trading. I implemented a simple SMA crossover strategy on SPY to learn basic backtesting, indicator construction, and performance evaluation in Python. 

SMA Crossover Strategy
--

Dataset: SPY
--
Backtest Period: 2015-2025

Frequency: Daily close prices

Libraries: pandas, numpy, matplotlib, yfinance


Overview:
--
This strategy uses a simple trend-following approach:

-Buy when the short-term SMA crosses above the long-term SMA

-Exit when the short-term SMA falls back below

This allows participation in upward trends while cutting exposure during downtrends.


Results:
--
-Sharpe Ratio: 0.1665

-Strategy Total Return: 0.2933

-Buy & Hold Total Return: 1.3784

Returns are based on cumulative daily strategy returns relative to the SPY benchmark.


Parameters:
--
-SMA Fast Window: 20

-SMA Slow Window: 50

-Transaction Fee: 0.001 per trade


Notes:
--
-Strategy performs better in strongly trending markets

-Underperforms in sideways/range-bound conditions

-Frequent signals reduce net performance due to transaction costs
