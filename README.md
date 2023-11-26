# Waiting Night Expert Advisor

## Overview
Waiting Night is an Expert Advisor designed to execute trades during quiet hours in the forex market. It is developed by Forex Robot Easy Team and can be found at [Forex Robot Easy](http://forexroboteasy.com). This ReadMe file provides an overview of the code and how it works.

## Code Description

### External Libraries
The code makes use of two external libraries: `Trade.mqh` and `PositionInfo.mqh`. These libraries provide functions and classes for trading operations and position information.

### Currency Pairs
The Expert Advisor trades a specific list of currency pairs during quiet hours. The `currencyPairs` array contains the list of currency pairs to be traded. You can modify this array to include or exclude currency pairs as per your requirements.

### User-friendly Settings
The Expert Advisor provides user-friendly settings that can be adjusted according to the trader's preferences. These settings include:
- `riskLevel`: Risk level adjustment feature.
- `takeProfit`: Take profit in pips.
- `stopLoss`: Stop loss in pips.
- `maxSpread`: Maximum allowed spread in points.
- `slippage`: Maximum allowed slippage in points.

### Trading during Quiet Hours
The `TradeDuringQuietHours` function is responsible for executing trades during quiet hours. It iterates over the `currencyPairs` array and checks the spread of each currency pair. If the spread is within the maximum allowed spread, it places two stop orders (Buy and Sell) with the specified take profit and stop loss levels.

### Entry Point
The `OnTick` function acts as the entry point of the Expert Advisor. It checks if the current time is within the defined quiet hours (e.g., 00:00 - 06:00) and calls the `TradeDuringQuietHours` function to execute trades during this period.

## Product Description
Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

Waiting Night is an Expert Advisor designed to take advantage of the quiet hours in the forex market. It trades a selected list of currency pairs during the specified quiet hours (e.g., 00:00 - 06:00). The Expert Advisor places two stop orders (Buy and Sell) with user-defined take profit and stop loss levels. It also allows adjustment of risk level and has settings to control maximum spread and slippage.

For detailed reviews and trading results of this product, please visit [Waiting Night MT5 Review - Your Forex Market Advantage](https://forexroboteasy.com/forex-robot-review/waiting-night-mt5-review-your-forex-market-advantage/).
