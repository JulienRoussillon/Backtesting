# Backtesting
This file contains a class BackTesting which implements any simple trading strategy and backtests it.

Important attributes of the class are:
  - The buy and sell signals the trading strategy implements (buys and sells are executed at open the next day),
  - The ticker on which the strategy is backtested,
  - The starting and ending dates of both the training and testing sets.

Note that the strategies involve portfolios with only one asset, and the buying/selling signals involve the whole portfolio. 

Work is in progress to extend strategies involving multi-asset portfolios and arbitrary sizings.

We then backtest the following simple mean reversion strategy: we invest the whole portfolio whenever IBS < 0.15 and 10-day Kauffman efficiency ratio > 0.28. Once in position, we sell the next day at open.

Between 1995 and 2015, we obtain a Sharpe ratio of 1.05, CAGR of 6.21% and maximum drawdown of 7%. The very low drawdown makes it a safe strategy. The drawback is that the strategy underperforms when the market is in a strong trend.
