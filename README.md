# TradingIndicators
A set of simple trading indicators I've built to support my trading. Currently in ThinkOrSwim's thinkscript, but I plan to update them to tradingview soon once I move over to it

#Squeezer
"Squeezer" is a volatility tracking tool that works off the concept of the "Squeeze", when volatility contracts due to market pressure on either side. This is typically denoted by when the Bollinger Bands stay in between the Keltner Channels. When a stock is in a squeeze on a larger time frame (30min/1hr/4hr) it typically bounces between those two prices, until it "fires" to either side, at which point we typically see RAPID price movement.

This indicator works on the 5 minute chart on ThinkOrSwim, and it shows at the top of the chart screen bubbles that show which time frames are on a squeeze (5min/15min/30min/1hr/4hr), and if they are what the upper and lower bound is (based on Keltner Channels). Unfortunately it is not *dynamic* in the sense that if you move to a higher time frame chart, it shows an error due to the fact that ThinkOrSwim runs the data based on the current chart, and HAS to process every timeframe that is selected.
