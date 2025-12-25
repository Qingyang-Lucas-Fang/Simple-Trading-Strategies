# Overview
This project is a part of the upcoming app which will enable greenhorn of quant finance to have an insight into the backtest of the past data of any stock included in yahoo finance. It will analyze the best trading strategy, only have buying long and selling short included, of the stock in 2025. This project is about QUANTITATIVE ALGORITHM TRADING.
This project will include 10 or more simple quant trading startegies included simple moving average, MFI, exponential moving average and mean reversion strategy, which have already been finished.

# Acknowledgement
This content is dedicated to the devotion of 2 parties: The first is Simple Quantitative Trading Strategies (SQTS), operated and led by Qingyang (Lucas) Fang:

<img width="1280" height="640" alt="logo2" src="https://github.com/user-attachments/assets/a9294a34-4dd4-44c7-a571-fd0fc6789163" />

The second is General Math Review (GMR), a local math journal who provoded vital mathematical ans stat support to this content:

<img width="1200" height="415" alt="截屏2025-09-10 上午8 31 50" src="https://github.com/user-attachments/assets/6161747e-ed12-4feb-8483-ba3260542a6c" />



## Useful Information
In my algorithm, a Position value of 100 represents buying long and a Position value of -100 represents selling short. The first notebook bar is the function that generates the trading strategy. You can change some parameters to balance the return and risks (stock volatility).

# Strategies
## Simple Moving Average
I tested this strategy with stock data of AAPL(APPLE), MSFT(Microsoft) and BX(Blackstone). The test results are available in the repositories with all of the 3 tests have a ROI of over 50% and a Sharpe Ratio of above 2.3 (which is excellent for a invest,ent strategy). This strategy is the most simple one and the parameters are fixed. If adjusted, they can help you to balance the volatitity of the startegy's return and the money return of that strategy.
<img width="1321" height="691" alt="Simple Moving Average" src="https://github.com/user-attachments/assets/28796e1d-e1e4-4885-9f34-3e3b83625af4" />


## Mean Reversion Strategy
Similar to Simple Moving Average Startegy, this strategy's parameters are also fixed but can be changed in the code i provided in the repositories. This strategy perform really well on the stoc of Blackstone, which has an ROI of over 250%, but perform quite poor in Apple's data. 
<img width="1299" height="772" alt="Mean Reversion" src="https://github.com/user-attachments/assets/676d6c9e-09d7-4ba4-89ee-77925c128025" />

## MFI Index Strategy
This strategy requires some parameter that you need to adjust in the process. The variable 'Boundary' is used for for balancing money return of the strategy and the volatility of that stock's strategy. With a high value may give you a startegy with high return but high risk and a low value may give you low return and low risk. After performing sensitive analysis, the more precise stock data users use, the higher return you may get, the precisio of data can be adjusted from the variable 'interval', you can check it up in yahoo finance.
<img width="1331" height="697" alt="MFI Strategy" src="https://github.com/user-attachments/assets/984ee6fd-cc12-4a83-b6f1-1edb80606df3" />

## Exponential Moving Average
This trading strategy is a renewed version of simple moving asverage strategy. It gives stock prices that are close to the stock's current position a higher weight, so it may closer to reality. It performs better after parameter adjustment than simple moving average. As it involves parameter adjustment, it may be more complicated to handle than simple moving strategy. <img width="1333" height="693" alt="Exponential Moving Average" src="https://github.com/user-attachments/assets/1889968d-0ae8-42f2-8720-d14b17be08bb" />


# Future Developments
## More Precise Alpha
The alpha I used is largely self-invented, so alpha that are more alert to market situation may improve my stratgies more than anything. The fact is that my strategy may enter a long position or a short position later than the the exact time. This will result in loss of return and higher risk.

# In The End
Plz Leave a star at this repo if you like this, and fell free to leave a comment for possible improvements for this repo, I really appreciate that! If you want to cooperate, just reach out at <LucasFang2@outlook.com>
