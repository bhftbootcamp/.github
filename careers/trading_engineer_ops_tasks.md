<pre>
  ___ _  _ ___ _____                     |
 | _ ) || | __|_   _|                    |  Contact us:  <a href= "mailto: epopova@bhft.com">epopova@bhft.com</a>
 | _ \ __ | _|  | |                      |  Open-source: <a href="https://github.com/bhftbootcamp">https://github.com/bhftbootcamp</a>
 |___/_||_|_|   |_|                      |
 | _ ) ___  ___| |_ __ __ _ _ __  _ __   |  
 | _ \/ _ \/ _ \  _/ _/ _` | '  \| '_ \  |  Level:    <b>Junior</b>
 |___/\___/\___/\__\__\__,_|_|_|_| .__/  |  Position: <b>TradingOps Analyst</b>
                                 |_|     |
</pre>

# Trading Operations Tasks

## #1. Building the spread between the futures and spot markets

Plot the spread between the [close price](https://en.wikipedia.org/wiki/Open-high-low-close_chart) of minute candles of the futures contract [BTCUSDT](https://www.binance.com/en/futures/BTCUSDT) and the corresponding spot market on the [Binance](https://www.binance.com/en) exchange for the year 2023, using [LightweightCharts](https://github.com/bhftbootcamp/LightweightCharts.jl) for visualization and [CryptoAPIs](https://github.com/bhftbootcamp/CryptoAPIs.jl) for data acquisition.

## #2. Calculation of the absolute value of income from funding

Determine the total income from the funding rate for a ‘long’ position of 1000 contracts [AUCTIONUSDT](https://www.binance.com/en/futures/AUCTIONUSDT) on [BinanceUSDMFutures](https://www.binance.com/en/futures/home). Calculate this income in dollars for the period from 00:00 UTC December 27, 2023, to 00:00 UTC December 28, 2023. Build a cumulative yield chart using any of the following visualization tools: LightweightCharts, MatplotLib or Julia Plots.

## #3. Arbitrage instruments search

Create a script that connects to the exchanges via API, requests all necessary data, and returns a list all possible arbitrage instruments grouped by base currency. Use data from [Binance](https://www.binance.com/en), [Bybit](https://www.bybit.com/en/), [Coinbase](https://www.coinbase.com/) and [Gateio](https://www.gate.io). [CryptoAPIs](https://github.com/bhftbootcamp/CryptoAPIs.jl) contains the necessary APIs.

Example output:

```yaml
Binance
  1INCH
    - 1INCH/BTC
    - 1INCH/BUSD
  AAVE
    - AAVE/BNB
    ...
Bybit
  1INCH
    - 1INCH/EUR
    ...
```

## #4. Acquiring OHLC data

Create a script that collects L1 market data from a cryptocurrency exchange (use any) and stores it in [PostgreSQL](https://en.wikipedia.org/wiki/PostgreSQL) with [TimescaleDB](https://www.timescale.com/) plugin. Based on the acquired data formulate 1s-candles [OHLC](https://en.wikipedia.org/wiki/Open-high-low-close_chart)) and visualize them using [LightweightCharts](https://github.com/bhftbootcamp/LightweightCharts.jl). Don't forget to define indexes and hypertables. Be ready to answer questions about your queries based on [EXPLAIN ANALYZE](https://www.postgresql.org/docs/current/sql-explain.html).

## #5. Ethereum transaction fees

Acquire historical [GAS](https://ethereum.org/en/developers/docs/gas/) fees on [Ethereum](https://ethereum.org/en/) blockchain from 00:00 UTC December 27, 2023, to 00:00 UTC December 28, 2023 and plot a graph showing rate of change. Use [LightweightCharts](https://github.com/bhftbootcamp/LightweightCharts.jl) for data visualization.
