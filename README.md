![threeelinestrike](https://github.com/onyxcollc/TOROSO/blob/maaahcus/Branding/Toroso_Arched_Lg.png?raw=true)

# T/OR(O/SO)
Created By Kristopher Kish, Nico Olumese, Dana Lain, Marcus Briscoe and Anna Peng

---
An Algorithmic Trading Application for Stocks & Cryptocurrencies utilizing a Multi-Indicator Stock Screener and Japanese Candlestick Strategy

>*"With a good perspective on history, we can have a better understanding of the past and present, and thus a clear vision of the future." — Carlos Slim Helu*

>"In finance, a trading strategy is a fixed plan that is designed to achieve a profitable return by going long or short in markets. The main reasons that a properly researched trading strategy helps are its verifiability, quantifiability, consistency, and objectivity.
For every trading strategy one needs to define assets to trade, entry/exit points and money management rules. Bad money management can make a potentially profitable strategy unprofitable."
— From Wikipedia




---
## The Toroso Strategy for Screener
Toroso takes into account four different indicators to observe within the screener:
* Volatility
    >although inherantly more dangerous, volatile stocks also have the most potential for profit, making it an efficient way to trade for day traders* Momentum
* Volume (TVI)
    >an amount of stock traded by measurement of how many times it is bought or sold within a timeframe
* Social Sentiment
    >social media platforms have sway over opinions of the masses which directly affects the pricing of assets
* RSI
    > A relative strength index is a technical analysis tool that measures any recent price changes of an asset and consider it either overbought or oversold ![rsi](https://www.tradingwithrayner.com/wp-content/uploads/2020/02/The-truth-about-RSI-1.jpg)

---
## The Toroso Strategy for Trading Indicator
Toroso analyzes the information provided throught the screener and enactsa trade based on the following criterias:

    
* Exponential Moving Average (EMA)
* Bollinger Bands
* Stochastic Oscillator
* Average Directional Index (ADX)
* On-Balance Volume (OBV)
* Candlesticks
---
## Japanese Candlestick Strategy
By analying patterns within candlestick performance, we are able to statistically predict whether a stock or cryptocurrency pattern will reverse or continue. 

Some patterns with high accuracy rates are:
* Three Line strike 83% Accuracy
![threelinestrike](https://www.investopedia.com/thmb/A8D_ZGFg7sf7OIKt-as-o1rDGe0=/1558x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/The5MostPowerfulCandlestickPatterns1-30019e515b6a4ed485b04ab2cfe26157.png)

* Two Black Gapping 68% Accuracy
![twoblackgapping](https://www.investopedia.com/thmb/lBy3nXP5nJcaMJkFR2VcIZnDUQA=/1558x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/The5MostPowerfulCandlestickPatterns2-e99deebdcb68466a92373cad488ed704.png)

* Three Black Crows 78% accuracy
![threeblackcrows](https://www.investopedia.com/thmb/cdbsU1lbGCpNOmwBCAuc05wTEOc=/1558x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/The5MostPowerfulCandlestickPatterns3-f3b280e0165a4b2fa5e5d3b42b36e337.png)

* Evening Start 72% Accuracy
![eveningstar](https://www.investopedia.com/thmb/kCe6bYYGvZm5ofzF3DBE4KYXS3Q=/1559x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/The5MostPowerfulCandlestickPatterns4-d56110580efa4f858ba9ebdf11adba22.png)

* Abandoned Baby 50% Accuracy
![abandonedbaby](https://www.investopedia.com/thmb/tOwiZc2R-HicIQiJKBh4W6kWCVg=/1558x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/The5MostPowerfulCandlestickPatterns5-67b8dd55470347adbe3a028e6ec6a9d6.png)


---
## Our Screener and Algorithm in Action

Our screener initiates the following steps:
1) We begin with all 500 tickers from the S&P500.
2) Filter out stocks below 1 million volume and with closing prices below $1 or above $100
3) Run RSI, Standard deviation, and On balance volume indicators on remaining stocks
4) Filter  out any stock with RSIs below 45 or with high standard deviations (volatility).
5) Run Twitter (Reddit to come) sentiment score on the remaining stocks.
6) Takes the RSI - (total social sentiment *100) for final picks.



---
## The Toroso Process
1. Build Stock Screener Based on Indicators.
2. Indicators are ranked by Sentiment, Technical Analysis, Bond Market, etc…
3. Screener can pull both stock ticker and crypto.
4. Top 1-5 performing tickers based on indicators get passed into the trading algorithm
5. Code Algo active during market hours. No overnight holdings.
6. Algorithm strategy is using basic Moving Averages, RSI, and Candle Stick Techniques
7. Backtest algo on historical data
8. Build Interface:
    * Tab 1: Stock Screener
    * Tab 2: Crypto Screener
    * Tab 3: Run/Stop Algo
9. Deploy Live Algo

---
## Libraries and API's
Kraken, 

Alpaca, 

CCXT,

Reddit API,

Tweepy API 

TA-Lib 

---
## Sources
[Investopedia - 5 most powerful candlestick patterns](https://www.investopedia.com/articles/active-trading/092315/5-most-powerful-candlestick-patterns.asp)


