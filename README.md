README.md

# Sun USDCHF - Trading Robot for USDCHF M1 Market

This trading robot is designed to trade on the USDCHF M1 market using an aggressive scalping strategy. It aims to generate profits by executing buy and sell orders with specified take profit (TP) and stop loss (SL) parameters.

## Developer

Forex Robot Easy Team

## Developer's Site

[forexroboteasy.com](https://forexroboteasy.com)

### Input Parameters

- `takeProfit`: Take Profit parameter for each cycle (default: 10)
- `stopLoss`: Stop Loss parameter for each cycle (default: 5)
- `leverage`: Leverage for the trading account (default: 500)

### Variables

- `accountBalance`: Account balance
- `cycleCount`: Number of cycles
- `copiesSold`: Number of copies sold
- `purchasePrice`: Purchase price
- `earlyAdoption`: Flag for early adoption

### Purchase Price Calculation

The purchase price is calculated based on the number of copies sold. If the number of copies sold is divisible by 5, the purchase price is calculated as 100 times the floor value of copies sold divided by 5. If not divisible by 5, the purchase price is calculated as 100 times the ceiling value of copies sold divided by 5 plus 1.

### Account Balance Check

The code checks if the account balance meets the minimum deposit requirement of $100. If the balance is sufficient, the number of cycles is calculated based on the account balance and purchase price.

### Scalping Strategy Execution

The code executes the scalping strategy for each cycle. It calls the `executeScalpingStrategy` function with the specified take profit and stop loss parameters. If the strategy is successful, it prints a success message indicating the cycle number. Otherwise, it prints a failure message.

### Scalping Strategy Execution Function

The `executeScalpingStrategy` function performs market analysis and makes informed decisions based on historical data. It calls the `analyzeMarket` function to determine whether to buy or sell. If the decision is to buy, it calls the `executeBuyOrder` function with the specified TP and SL parameters. If the decision is to sell, it calls the `executeSellOrder` function.

### Market Analysis Function

The `analyzeMarket` function performs market analysis using historical data and implements logic to leverage strong recurrences from the past. It returns a boolean value indicating the analysis result.

### Buy Order Execution Function

The `executeBuyOrder` function executes the buy order with the specified TP and SL parameters. It implements the code to execute the buy order and returns a boolean value indicating the success of the order execution.

### Sell Order Execution Function

The `executeSellOrder` function executes the sell order with the specified TP and SL parameters. It implements the code to execute the sell order and returns a boolean value indicating the success of the order execution.

---

## Product Description

Sun USDCHF is an advanced trading robot developed by the Forex Robot Easy Team. This robot is specifically designed to trade on the USDCHF M1 market using an aggressive scalping strategy.

With configurable parameters for take profit and stop loss, Sun USDCHF aims to generate consistent profits by executing buy and sell orders based on market analysis and historical data. The robot leverages strong recurrences from the past to make informed trading decisions.

The purchase price of Sun USDCHF is determined based on the number of copies sold. With every 5 copies sold, the price increases by $100. Early adopters have the opportunity to purchase the robot at a discounted price.

To use Sun USDCHF, a trading account with a minimum balance of $100 is required. The number of trading cycles is calculated based on the account balance and the leverage set for the account.

Please note that Forex Robot Easy is not the official developer of this product. We are showcasing a sample code that demonstrates how Sun USDCHF can work as described. For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/sun-usdchf-review-aggressive-scalping-with-independent-cycles/). To find the official developer of this product, please refer to MQL5.
