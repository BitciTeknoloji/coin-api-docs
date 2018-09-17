# Bitci.com coin instant API document.
The documentation for Bitci.com coin instant API document.

## Usage
Append your exchange's URL to the beginning of the methods to use the API. For example, to get ticker info from Bitci.com, use [https://www.bitci.com/Api/Coin] (https://www.bitci.com/Api/Coin)

## Questions & Problems
Please use the [issues](https://github.com/BitciTeknoloji/coin-api-docs/issues) on this github project to ask questions and report bugs.

## Request Limits

* .../Api/Coin/ requests are limited to 10 requests per 100 miliseconds.
* Other requests are limited to 1 request per 100 miliseconds.
* If you make more than 50 consequent unauthorized requests your IP address will be blocked.

## Ticker

<code>GET</code> .../Api/Coin/BTC_TRY
<code>GET</code> .../Api/Coin/BTC_CHFT

**Result: BTC_TRY **
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
**Result: BTC_CHFT **
``` json
[
	{
	"CoinCode": "BTC",
	"CoinName": "Bitcoin",
	"CurrencyCode": "CHFT",
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

* CoinCode: Api coin code.
* CoinName: Api coin long name.
* CurrencyCode: Api currency code.
* Price: Last price.
* Open24H: Price of the opening in the last 24 hours.
* High24H: Highest price in the last 24 hours.
* Low24H: Lowest price in the last 24 hours.
* Change24H: Change price in the last 24 hours.
* Volume24H: Total volume in the last 24 hours.
* Timestamp: Unix UTC timestamp date and time.

## Available Coin Tickers

Bitcoin
*	BTC/TRY
*	BTC/CHFT

Litecoin
*	LTC/TRY
*	LTC/CHFT

Ethereum
*	ETH/TRY
*	ETH/CHFT

Bitcoin Cash
*	BCH/TRY
*	BCH/CHFT

Bitcoin Gold
*	BTG/TRY
*	BTG/CHFT

Digital Cash
*	DASH/TRY
*	DASH/CHFT

Doge Coin
*	DOGE/TRY
*	DOGE/CHFT

DigiByte
*	DGB/TRY
*	DGB/CHFT
