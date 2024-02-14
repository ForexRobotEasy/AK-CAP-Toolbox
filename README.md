# AK CAP Toolbox - Forex Trading Robot ReadMe

This ReadMe file provides an overview of the AK CAP Toolbox Forex Trading Robot code. The code is developed by the Forex Robot Easy Team and can be found on their website: [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/ak-cap-toolbox-review-free-simple-forex-software/).

## Code Description

The AK CAP Toolbox Forex Trading Robot is designed to trade based on the Volume Weighted Average Price (VWAP) indicator. It uses the AK CAP Toolbox library and necessary dependencies to handle trading functions and indicators.

The code consists of the following sections:

### 1. Include necessary libraries and dependencies

The code includes the Trade and Indicators libraries to utilize their functions.

### 2. Define global variables

The code defines three global variables: `lotSize`, `stopLoss`, and `takeProfit`. These variables determine the default lot size, stop loss value, and take profit value for trades.

### 3. Initialize AK CAP Toolbox

The `OnInit()` function is called during the initialization of the EA. It initializes the trading functions and indicators by calling the `TradeInit()` and `IndicatorsInit()` functions. It also prints a welcome message.

### 4. Handle trading signals and execute trades

The `OnTick()` function is called on each tick of the market. It retrieves the VWAP value for the current currency pair using the `GetVWAP()` function. It then gets the current price for the currency pair using the `SymbolInfoDouble()` function.

The code checks if the current price is above or below the VWAP and places a buy or sell trade accordingly. It calculates the stop loss and take profit prices based on the current price and the defined values. The `TradeBuy()` and `TradeSell()` functions are used to execute the trades.

### 5. Calculate VWAP for a given currency pair

The `GetVWAP()` function calculates the VWAP for a given currency pair. It retrieves the historical prices and volumes using the `CopyRates()` and `CopyTickVolume()` functions. It then calculates the VWAP by summing the product of each closing price and its corresponding volume, divided by the total volume.

### 6. Handle deinitialization of AK CAP Toolbox

The `OnDeinit()` function is called during the deinitialization of the EA. It cleans up resources and performs any necessary actions by calling the `TradeDeinit()` and `IndicatorsDeinit()` functions. It also prints a final message.

## Product Description

The AK CAP Toolbox Forex Trading Robot is a free and simple software developed by the Forex Robot Easy Team. It utilizes the Volume Weighted Average Price (VWAP) indicator to make trading decisions.

Key features of the AK CAP Toolbox Forex Trading Robot:

- Uses the AK CAP Toolbox library for efficient trading functions and indicators.
- Allows customization of lot size, stop loss, and take profit values.
- Executes buy trades when the current price is above the VWAP.
- Executes sell trades when the current price is below the VWAP.
- Calculates the VWAP based on historical prices and volumes.

Please note that ForexRobotEasy is not the official developer of this product. This ReadMe file only provides a code sample that demonstrates how the AK CAP Toolbox Forex Trading Robot works. To find the official developer and obtain the complete product, please refer to the MQL5 platform. For detailed reviews and trading results of this product, visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/ak-cap-toolbox-review-free-simple-forex-software/).
