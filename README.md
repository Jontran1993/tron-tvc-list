# Adding new token
The JSON schema for the tokens includes: address, name, decimals, symbol, logoURI, official homepage, MarketCap link, existing Markets.

Follow the steps below to add a new token：
1) Fork this repo.
2) change the JSON file `tokenlist.json`, adding such as: (PLEASE DO NOT REMOVE EXISITING TOKENS)
```
{
      "address": "TTnDjUCEmMRs13t9rBPCiQXKqHDgSMSP7K",
      "symbol": "USDT",
      "name": "TRC20",
      "decimals": 6,
      "logoURI": "https://coingecko.com/coins/images/325/large/Tether.png?1696501661",
      "homepage": "https://coingecko.com",
      "MarketCapLink": "https://coinmarketcap.com/currencies/tether/",
      "existingMarkets": [
          {
              "source": "Binance",
              "pairs": [
                  "USDC/USDT",
                  "USDT/BUSD",
                  "USDT/BNB",
                  "USDT/USDC"
              ]
          },
          {
              "source": "Poloniex",
              "pairs": [
                  "USDT/USDC"
              ]
          },
          {
              "source": "coingecko",
              "pairs": [
                  "USDT/USDC"
              ]
          }
    ]
}
```
* `address`[Required]: your token address.
* `symbol`[Required]: your token symbol.
* `name`[Required]: your token name.
* `logoURI`[Required]: the logo URI of your token.
* `homepage`[Required]: the home page of your token.
* `MarketCapLink`[Optional]: the coinmarketcap or coingecko link for your token.
* `existingMarkets`[Required]: where to trade with your token.
3) Submit PR with the changed JSON file.


