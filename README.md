# Golden Hunter MT5

Golden Hunter MT5 is a powerful forex trading tool developed by the Forex Robot Easy Team. This code provides a sample implementation of the Golden Hunter MT5 trading strategy. Please note that ForexRobotEasy is not the official developer of this product. This code is provided as a demonstration and should be used at your own risk.

For detailed reviews and trading results of the Golden Hunter MT5, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/golden-hunter-mt5-review-powerful-forex-trading-tool/).

## Table of Contents
- [Dependencies](#dependencies)
- [Input Parameters](#input-parameters)
- [Indicators](#indicators)
- [Trading Functions](#trading-functions)
- [Main Functions](#main-functions)
- [Custom Classes](#custom-classes)

## Dependencies
This code requires the following libraries:
- Trade.mqh
- Indicator.mqh
- Timeseries.mqh

## Input Parameters
- CurrencyPairs: An array of currency pairs to trade. Default value: ['EURUSD', 'GBPUSD', 'BTCUSD']
- TimeFrame: The time frame to use for trading. Default value: PERIOD_M5

## Indicators
- Indicator1: The first indicator used for trading
- Indicator2: The second indicator used for trading
- Indicator3: The third indicator used for trading

## Trading Functions
- Trade: The trading class used to perform buy and sell operations

## Main Functions
### OnTick
This function is called whenever a new tick is received. It checks if the market activity is high and spreads are low. If the conditions are met, it calculates the values of the indicators and checks if all indicators are giving a buy or sell signal. If a buy signal is generated, it opens a buy trade. If a sell signal is generated, it opens a sell trade.

### IsMarketActive
This function checks if the current time is within daylight hours. It returns true if the current time is between 8:00 and 20:00, and false otherwise.

### IsSpreadLow
This function checks if the spread is low for the selected currency pairs. It retrieves the current spread for each currency pair and checks if it is below certain thresholds. It returns true if all spreads are below the thresholds, and false otherwise.

### OnInit
This function is called when the expert is initialized. It initializes the indicators and trading functions.

### OnDeinit
This function is called when the expert is deinitialized. It performs cleanup and deinitialization operations.

### OnTimer
This function is called on a timer event. It can be used to perform necessary operations at regular intervals.

### OnStart
This function is called when the expert is started. It currently does nothing.

## Custom Classes
### CIndicator
This class is used to calculate the values of the indicators. It has a constructor to initialize the indicator variables and a Calculate function to calculate and return the indicator value.

### CTrade
This class is used to perform trading operations. It has a constructor to initialize the trading variables, a Buy function to open a buy trade, and a Sell function to open a sell trade.

For detailed information on how to use the Golden Hunter MT5 and to find the official developer of this product, please refer to the documentation provided by the official developer or visit the [MQL5 website](https://www.mql5.com/).
