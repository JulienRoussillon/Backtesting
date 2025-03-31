# Backtesting
This file contains a class BackTesting which implements any simple trading strategy and backtests it.

Important attributes of the class are:
  - The buy and sell signals the trading strategy implements (buys and sells are executed at open the next day),
  - The ticker on which the strategy is backtested,
  - The starting and ending dates of both the training and testing sets.

Note that the strategies involve portfolios with only one asset, and the buying/selling signals involve the whole portfolio. 

Work is in progress to extend strategies involving multi-asset portfolios and arbitrary sizings.
