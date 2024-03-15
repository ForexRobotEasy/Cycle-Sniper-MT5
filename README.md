# Cycle Sniper MT5

Cycle Sniper MT5 is a trading robot developed by the Forex Robot Easy Team. It is designed to identify market cycles and open trades based on the direction of these cycles. The robot uses two cycle indicators, 'CycleIndicator1' and 'CycleIndicator2', to determine whether to open a buy or sell trade.

## Installation

To use Cycle Sniper MT5, you need to include the necessary libraries and input parameters in your MetaTrader 5 (MT5) platform. 

### Libraries
- Trade.mqh
- Indicators.mqh

### Input Parameters
- StopLoss: The stop loss level in pips.
- TakeProfit: The take profit level in pips.
- TradeVolume: The trading volume in lots.

## How it Works

The trading function, `OnTick()`, is executed on every tick of the market. 

1. The cycle indicators, `cycleIndicator1` and `cycleIndicator2`, are calculated using the `iCustom()` function. These indicators represent the current market cycles.

2. The robot checks if the cycle indicators are valid (not equal to zero).

3. If both cycle indicators are positive, a buy trade is opened. The entry price is set as the current Ask price, and the stop loss and take profit levels are calculated based on the input parameters.

4. If both cycle indicators are negative, a sell trade is opened. The entry price is set as the current Bid price, and the stop loss and take profit levels are calculated based on the input parameters.

## Product Description

Cycle Sniper MT5 is a powerful trading robot developed by the Forex Robot Easy Team. It uses advanced cycle indicators to identify market cycles and open trades accordingly. 

Key Features:
- Accurate cycle detection: The robot uses two cycle indicators to accurately identify market cycles.
- Buy and sell trades: Cycle Sniper MT5 opens buy trades when the cycle indicators are positive and sell trades when the cycle indicators are negative.
- Customizable parameters: The robot allows you to set the stop loss, take profit, and trading volume according to your risk tolerance and trading strategy.

Limitations:
- Dependency on cycle indicators: The effectiveness of Cycle Sniper MT5 relies on the accuracy of the cycle indicators used. It is important to monitor and update these indicators as market conditions change.
- No additional risk management: The robot does not include additional risk management features such as trailing stops or breakeven levels. It is recommended to use appropriate risk management techniques alongside this robot.

Please note that ForexRobotEasy is not the official developer of Cycle Sniper MT5. We provide this sample code to demonstrate how the product works. For detailed reviews and trading results of this product, please visit the official developer's website at [Cycle Sniper MT5 Review](https://forexroboteasy.com/forex-robot-review/cycle-sniper-mt5-review-key-features-limitations/). To find the official developer of this product, please use the MQL5 platform.
