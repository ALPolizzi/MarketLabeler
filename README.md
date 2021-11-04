# MarketLabeler
A tool for determining the most profitable trade opportunities in historical OHLC market data
Creates a binomial heap for each period in the given OHLC data containing key, value pairs for each future period which has an exit opportunity for a trade taken in the heap's period which is sufficiently profitable.
The heap sorts by the Time-Adjusted-Profitability (TAP) and the corresponding value is a vector in the form c(Timestamp, 'b'/'s'), which indicates the type of exit trade (buy/sell) and when the opportunity exists.
