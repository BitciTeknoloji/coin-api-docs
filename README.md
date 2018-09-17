# Bitci.com coin instant API document.
The documentation for Bitci.com coin instant API document.

## Usage
Append your exchange's URL to the beginning of the methods to use the API. For example, to get ticker info from Bitci.com, use [https://www.bitci.com/Api] (https://www.bitci.com/Api)

## Questions & Problems
Please use the [issues](https://github.com/BitciTeknoloji/coin-api-docs/issues) on this github project to ask questions and report bugs.

## Request Limits

* .../Api/Coin/ requests are limited to 10 requests per 100 miliseconds.
* Other requests are limited to 1 request per 100 miliseconds.
* If you make more than 50 consequent unauthorized requests your IP address will be blocked.

## Coin / Currency Ticker

<code>GET</code> .../Coin/BTC_TRY
* BTC_TRY
**Result:**
``` json

{
	"coinCode": "BTC",
	"coinName": "Bitcoin",
	"currencyCode": "TRY",
	"currencyName": "Türk Lira",
	"price": 39802.35,
	"open": 42000.00,
	"high": 45000.00,
	"low": 2000.00,
	"change": 1.06,
	"volume": 55.72,
	"timestamp": 1508242980
}

```

<code>GET</code> .../Coin/BTC_CHFT
* BTC_CHFT
**Result:**
``` json

{
	"coinCode": "BTC",
	"coinName": "Bitcoin",
	"currencyCode": "CHFT",
	"currencyName": "Crypto Holding",
	"price": 39802.35,
	"open": 42000.00,
	"high": 45000.00,
	"low": 2000.00,
	"change": 1.06,
	"volume": 55.72,
	"timestamp": 1508242980
}

```

* coinCode: Api coin code.
* coinName: Api coin long name.
* currencyCode: Api currency code.
* currencyName: Api currency long name.
* price: Last price.
* open: Price of the opening in the last 24 hours.
* high: Highest price in the last 24 hours.
* low: Lowest price in the last 24 hours.
* change: Change price in the last 24 hours.
* volume: Total volume in the last 24 hours.
* timestamp: Unix UTC timestamp date and time.

## Available Coin / Currency Tickers

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
