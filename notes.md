Error: Timed out waiting for all watched tickers to receive a depth update

Binance Spot Test Network Error;

Using test network API, getting the error below;

binance-triangle-arbitrage@6.2.0 start
node src/main/Main.js

WARNING! Order execution is enabled!

Checking configuration ...
Checking latency ...
Experiencing 58 ms of latency
Fetching exchange info ...
Found 20/20 currently trading tickers
Found 32 triangular trades
Checking balances ...
Checking market conditions ...
Opening 20 depth websockets for 20 tickers ...
Waiting for all tickers to receive initial depth snapshot ...
Error: Timed out waiting for all watched tickers to receive a depth update
at Object.waitForUpdates (/home/tokio/project/binance-triangle-arbitrage/src/main/MarketCache.js:84:70)
at listOnTimeout (node:internal/timers:568:17)
at processTimers (node:internal/timers:510:7)



Solution:-

change the node-binance-api version in package.json to 0.13.0 or the latest version currently it's 0.13.1

++++++++++++++++++++

Author's bot says:-

Haven't updated this project in quite some time. When everything executes in a timely manner, profit will be realized in the base asset. So if your base asset is ETH, then the system is calculating a trade that would net a positive increase of ETH. As always be careful when trading crypto

++++++++++++++++++++

https://github.com/bmino/binance-triangle-arbitrage/issues/148
https://github.com/bmino/binance-triangle-arbitrage/issues/149

