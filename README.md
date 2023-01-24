<h2>EventBased_Backtester</h2>
 
The event-based backtester uses the Oanda API to download and test financial instruments with custom indicators. This project intends to test initial trading hypotheses without relying on third-party libraries.
By using the EventBased_Backtester we can easily iterate over the parameters of MA, RSI, MACD, ATR and other popular indicators and locate potential regions of higher probability of returns. 

<em>The brighter areas on the heatmaps below depict the higher (historical) returns of different MA crossovers in the USDJPY pair. The darker areas represent the lower returns.</em>  

![png](https://github.com/gamaiun/EventBased_Backtester/blob/main/example.png)

Explanation: **Vectorized vs event based backtesting**.

*Vectorized backtesting* in Python is a method of testing a trading strategy using historical data where the calculations are done using arrays and matrix operations, rather than looping through each data point. This method is computationally efficient and allows for fast execution of backtesting.

*Event-based backtesting*, on the other hand, is a method of testing a trading strategy that simulates the exact sequence of events that occurred in the market, such as trades, orders, and market data updates. This method is more realistic, as it takes into account the timing of market events and how they impact the strategy.

**Three major advantages of event-based backtesting are**:

Realism: Event-based backtesting captures the exact sequence of market events and how they impact the strategy, making it more realistic than vectorized backtesting.

Flexibility: Event-based backtesting can handle complex strategies that involve multiple assets, orders, and market conditions, making it more flexible than vectorized backtesting.

Transparency: Event-based backtesting makes it easy to understand the behavior of the strategy, as it allows for easy inspection of the exact trades and market events that occurred during the backtest.

It's worth noting that event-based backtesting is generally considered more realistic and accurate than vectorized backtesting, but it comes with a tradeoff of computational efficiency, complexity, and scalability. Depending on the use case, one approach may be more beneficial than the other. 

**Two major disadvantages of event-based backtesting compared to vectorized backtesting are:**

Computational efficiency: Event-based backtesting can be computationally intensive as it simulates the exact sequence of market events, which may require a large amount of memory and processing power. This can make it slower than vectorized backtesting, especially for large datasets.

Complexity: Event-based backtesting can be more complex to implement, as it requires a detailed understanding of the market events and how they impact the strategy. This can make it more difficult for traders and researchers to develop and test their strategies.
