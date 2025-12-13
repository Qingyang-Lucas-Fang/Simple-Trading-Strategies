# Simple-Trading-Strategy
This project is a part of the upcoming app which will enable greenhorn of quant finance to have an insight into the backtest of the past data of any stock included in yahoo finance. It will analyze the best trading strategy, only have buying long and selling short included, of the stock in 2025.
## The First Strategy-- Simple Moving Average
def strategy(stock,start,end,sma_s,sma_l):
    df=yf.download(stock,start=start,end=end,interval='1h')['Close']
    df['SMA_s'] = df[stock].rolling(50).mean()
    df['SMA_l'] = df[stock].rolling(200).mean()
    df['position'] = np.where(df['SMA_s'] > (df['SMA_l']), 100, -100)
    df['Return_perc'] = np.log(df[stock] / df[stock].shift(1))/100
    df['Strategy'] = df['Return_perc'] * df['position']
    return_rst=df[['Strategy', 'Return_perc']].sum().apply(np.exp)
    df['Strategy']=df['Strategy']/100
    risk_rst=df[['Strategy','Return_perc']].std()*np.sqrt(252)
    df[['SMA_s','SMA_l','position',stock]].plot()
    display(df)
    display(return_rst)
    display(risk_rst)
strategy('BX','2025-01-01','2025-12-10',20, 100)
