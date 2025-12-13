# Simple-Trading-Strategy
This project is a part of the upcoming app which will enable greenhorn of quant finance to have an insight into the backtest of the past data of any stock included in yahoo finance. It will analyze the best trading strategy, only have buying long and selling short included, of the stock in 2025.
This project will include 10 or more simple quant trading startegies included simple moving average, MFI, and mean reversion strategy, which have already been finished.

#Useful Information
In my algorithm, a Position value of 100 represents buying long and a Position value of -100 represents selling short. The first notebook bar is the function that generates the trading strategy. You can change some parameters to balance the return and risks (stock volatility).

## Simple Moving Average
I tested this strategy with stock data of AAPL(APPLE), MSFT(Microsoft) and BX(Blackstone). The test results are available in the repositories with all of the 3 tests have a ROI of over 50% and a Sharpe Ratio of above 2.3 (which is excellent for a invest,ent strategy). This strategy is the most simple one and the parameters are fixed. If adjusted, they can help you to balance the volatitity of the startegy's return and the money return of that strategy.

## Mean Reversion Strategy
Similar to Simple Moving Average Startegy, this strategy's parameters are also fixed but can be changed in the code i provided in the repositories. This strategy perform really well on the stoc of Blackstone, which has an ROI of over 250%, but perform quite poor in Apple's data. 

## MFI Index Strategy
This strategy requires some parameter that you need to adjust in the process. The variable 'Boundary' is used for for balancing money return of the strategy and the volatility of that stock's strategy. With a high value may give you a startegy with high return but high risk and a low value may give you low return and low risk. After performing sensitive analysis, the more precise stock data users use, the higher return you may get, the precisio of data can be adjusted from the variable 'interval', you can check it up in yahoo finance.

## Exponential Moving Average
This trading strategy is a renewed version of simple moving asverage strategy. It gives stock prices that are close to the stock's current position a higher weight, so it may closer to reality. It performs better after parameter adjustment than simple moving average. As it involves parameter adjustment, it may be more complicated to handle than simple moving strategy. 
