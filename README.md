# Bitci.com coin instant API document.
The documentation for Bitci.com coin instant API document.

## Usage
Append your exchange's URL to the beginning of the methods to use the API. For example, to get ticker info from Bitci.com, use [https://www.bitci.com/ApiTickers/Coin] (https://www.bitci.com/ApiTickers/Coin)

## Questions & Problems
Please use the [issues](https://github.com/BitciTeknoloji/coin-api-docs/issues) on this github project to ask questions and report bugs.

## Request Limits

* .../ApiTickers/Coin/ requests are limited to 10 requests per 100 miliseconds.
* Other requests are limited to 1 request per 100 miliseconds.
* If you make more than 50 consequent unauthorized requests your IP address will be blocked.

## Ticker

<code>GET</code> .../ApiTickers/Coin

**Result:**
``` json
[
	{
	"CoinCode": "BTC",
	"CoinName": "Bitcoin",
	"CurrencyCode": "TRY",
	"Price": 39802.35,
	"Open24H": 42000.00,
	"High24H": 45000.00,
	"Low24H": 2000.00,
	"Change24H": 1.06,
	"Volume24H": 55.72,
	"Timestamp": 1508242980
	}
]
```
