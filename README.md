# News Catcher Pro MT5

Developer's Site: [forexroboteasy.com](https://forexroboteasy.com)

Development by: Forex Robot Easy Team

---

This code is an expert advisor (EA) for MetaTrader 5 (MT5) that implements a mean-reversion trading strategy based on intraday seasonal volatility patterns. It includes a news filter to skip trading during unfavorable market conditions.

## Input Parameters

- `lotSize` (default: 0.1): The lot size for trading.
- `stopLoss` (default: 50): The stop loss in pips.
- `takeProfit` (default: 100): The take profit in pips.

## Global Variables

- `newsFilterEnabled`: A boolean flag to enable/disable the news filter.

## Initialization

The expert initialization function (`OnInit()`) initializes the news filter if it is enabled. If the news filter fails to initialize, an error message is printed and the initialization fails.

## Deinitialization

The expert deinitialization function (`OnDeinit()`) cleans up resources and deinitializes the news filter if it is enabled.

## Trading Logic

The expert tick function (`OnTick()`) is called on every tick of the market. It first checks if it's a favorable market condition to trade by calling the news filter check function (`NewsFilterCheck()`) if the news filter is enabled. If the news filter check fails, trading is skipped.

Next, the mean-reversion strategy based on intraday seasonal volatility patterns is implemented. The code for this strategy should be added in the designated section.

After implementing the strategy, trades can be opened based on the strategy by adding the trade opening code in the designated section. Similarly, trades can be closed based on the strategy by adding the trade closing code in the designated section.

## News Filter

The news filter is a separate feature that can be enabled or disabled using the `newsFilterEnabled` flag. It is initialized using the news filter initialization function (`NewsFilterInit()`) and deinitialized using the news filter deinitialization function (`NewsFilterDeinit()`). The news filter check function is implemented in the `NewsFilterCheck()` function.

## Product Description

[News Catcher Pro MT5](https://forexroboteasy.com/forex-robot-review/review-news-catcher-pro-mt5-a-professional-forex-traders-perspective/) is a professional expert advisor developed by the Forex Robot Easy Team. It is designed to implement a mean-reversion trading strategy based on intraday seasonal volatility patterns in the MetaTrader 5 platform.

The EA allows traders to set their desired lot size, stop loss, and take profit parameters. Additionally, it includes a news filter that can be enabled or disabled to skip trading during unfavorable market conditions.

Please note that ForexRobotEasy is not the official developer of this product. The code provided here is a sample that can work as described in the product. To find the official developer of this product, please refer to MQL5.
