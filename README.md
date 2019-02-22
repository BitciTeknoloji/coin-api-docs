# Bitci.com coin instant API document.
The documentation for Bitci.com coin instant API document.

## Usage
Append your exchange's URL to the beginning of the methods to use the API. For example, to get ticker info from Bitci.com, use [https://api.bitci.com/api] (https://api.bitci.com/api)

## Questions & Problems
Please use the [issues](https://github.com/BitciTeknoloji/coin-api-docs/issues) on this github project to ask questions and report bugs.

## Request Limits

* .../api/coin/ requests are limited to 3 requests per 1 seconds.
* .../api/ requests are limited to 3 requests per 1 seconds.

## Coin / Currency and Coin Ticker

<code>GET</code> .../coin/BTC_TRY
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

<code>GET</code> .../coin/BTC_CHFT
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
<code>GET</code> .../coin/LTC_BTC
* LTC_BTC
**Result:**
``` json

{
	"coinCode": "LTC",
	"coinName": "Litecoin",
	"currencyCode": "BTC",
	"currencyName": "Bitcoin",
	"price": 0.01255198,
	"open": 0.01235271,
	"high": 0.01268362,
	"low": 0.01223700,
	"change": 1.61,
	"volume": 96.50000000,
	"timestamp": 1508242980
}

```

* coinCode: Api coin code.
* coinName: Api coin long name.
* currencyCode: Api currency code or coin code.
* currencyName: Api currency long name or coin long name.
* price: Last price.
* open: Price of the opening in the last 24 hours.
* high: Highest price in the last 24 hours.
* low: Lowest price in the last 24 hours.
* change: Change price in the last 24 hours.
* volume: Total volume in the last 24 hours.
* timestamp: Unix UTC timestamp date and time.

## Coin / Currency and Coin All Ticker

<code>GET</code> .../ReturnTicker
* ReturnTicker
**Result:**
``` json

[
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
	},
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
	},
	{
		"coinCode": "LTC",
		"coinName": "Litecoin",
		"currencyCode": "BTC",
		"currencyName": "Bitcoin",
		"price": 0.01255198,
		"open": 0.01235271,
		"high": 0.01268362,
		"low": 0.01223700,
		"change": 1.61,
		"volume": 96.50000000,
		"timestamp": 1508242980
	}
	... and more...
]

```

* coinCode: Api coin code.
* coinName: Api coin long name.
* currencyCode: Api currency code or coin code.
* currencyName: Api currency long name or coin long name.
* price: Last price.
* open: Price of the opening in the last 24 hours.
* high: Highest price in the last 24 hours.
* low: Lowest price in the last 24 hours.
* change: Change price in the last 24 hours.
* volume: Total volume in the last 24 hours.
* timestamp: Unix UTC timestamp date and time.

## Available Coin / Currency and Coin Tickers

Bitcoin
*	BTC_TRY
*	BTC_CHFT

Litecoin
*	LTC_TRY
*	LTC_CHFT
*	LTC_BTC

Ethereum
*	ETH_TRY
*	ETH_CHFT
*	ETH_BTC

Ripple
*	XRP_TRY
*	XRP_CHFT
*	XRP_BTC

Bitcoin Cash
*	BCH_TRY
*	BCH_CHFT
*	BCH_BTC

Bitcoin Gold
*	BTG_TRY
*	BTG_CHFT
*	BTG_BTC

Pirl
*	PIRL_TRY
*	PIRL_CHFT
*	PIRL_BTC

Digital Cash
*	DASH_TRY
*	DASH_CHFT
*	DASH_BTC

Z Cash
*	ZEC_TRY
*	ZEC_CHFT
*	ZEC_BTC

Stellar
*	XLM_TRY
*	XLM_CHFT
*	XLM_BTC

Doge Coin
*	DOGE_TRY
*	DOGE_CHFT
*	DOGE_BTC

DigiByte
*	DGB_TRY
*	DGB_CHFT
*	DGB_BTC

Bitcoin Hyper
*	BHY_TRY
*	BHY_CHFT
*	BHY_BTC
