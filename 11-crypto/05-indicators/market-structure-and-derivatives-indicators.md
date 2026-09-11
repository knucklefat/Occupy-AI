# Market Structure and Derivatives Indicators

**In one sentence:** Derivatives data (funding, open interest, basis, liquidations, options) tells you how leveraged and how one-sided traders are right now, which makes it the best toolkit for reading the next few days to weeks and nearly useless for anything longer.

## Why derivatives matter so much in crypto

Crypto futures and perpetual swaps trade several times the volume of spot. Perpetual swaps ("perps") are futures with no expiry that stay tethered to spot via a funding payment between longs and shorts. Because leverage is cheap and available 24/7, positioning gets crowded, and crowded positions get flushed. Most sharp moves of 5 to 15% in a day are liquidation cascades, not news. If you understand funding, open interest and liquidation maps, you understand most of crypto's short-term price behavior.

## Funding rates

**What it measures.** The periodic payment (usually every 8 hours) between perp longs and shorts. Positive funding means longs pay shorts, which happens when the perp trades above spot because buyers are aggressive. Negative funding means shorts pay longs. Rates are quoted per 8 hours; multiply by roughly 1,095 to annualize (0.01% per 8h is about 11% per year, the "neutral" baseline on Binance).

**Where to get it free.** [Coinglass funding rates](https://www.coinglass.com/FundingRate), [Coinglass BTC funding history](https://www.coinglass.com/FundingRate/BTC), [Velo data](https://velo.xyz/), exchange pages (Binance, Bybit, Hyperliquid) show live rates.

**How to read it.** Persistently high positive funding (above 0.05% per 8h, roughly 50%+ annualized) means longs are paying dearly to stay in and the market is vulnerable to a long squeeze. Deeply negative funding means shorts are crowded and a short squeeze is likely. The February 28, 2026 episode is a clean example: after the US and Israeli strikes on Iran knocked Bitcoin to about $63,000, CoinDesk reported funding at minus 6% annualized, a three-month low, and the market subsequently squeezed higher. In late August 2026 Glassnode described funding as "near neutral" even as price rallied 26%, meaning the rally was not built on perp leverage, which is a healthier structure than a funding-fueled melt-up.

**Track record.** Extreme funding is a solid contrarian signal on a 1-to-3-week horizon. It says nothing about the cycle. Note that funding in the ETF era is systematically dampened by cash-and-carry funds (they short perps against spot ETF holdings), so the 2021-style 100%+ annualized readings have become rare.

## Open interest (OI)

**What it measures.** The total notional value (or coin count) of outstanding futures and perp contracts. Rising OI means new positions are being opened; falling OI means positions are being closed, either voluntarily or by liquidation.

**Where to get it free.** [Coinglass open interest](https://www.coinglass.com/open-interest/BTC), [Coinglass futures overview](https://www.coinglass.com/currencies/BTC/futures), [CME Group BTC futures data](https://www.cmegroup.com/markets/cryptocurrencies/bitcoin/bitcoin.html), [Glassnode derivatives](https://studio.glassnode.com/charts/derivatives.FuturesOpenInterestSum?a=BTC).

**How to read it.** Always look at OI in coin terms (BTC) as well as dollars, because dollar OI rises mechanically with price. The four combinations: price up + OI up = new longs (trend building, but fragile); price up + OI down = short covering (squeeze, often fades); price down + OI up = new shorts (or hedging); price down + OI down = long liquidations (capitulation). Glassnode noted that during the August 2026 squeeze, OI shrank 11% in coin terms while price rose, the signature of short covering rather than fresh conviction. CME OI is worth tracking separately because it reflects institutional and basis-trade positioning rather than retail leverage.

**Track record.** OI at record highs relative to market cap has preceded most major flushes (May 2021, November 2021, August 2024, October 2025). It does not tell you the direction, only that a large move is likely.

## Basis and annualized premium

**What it measures.** The gap between a dated futures price (for example, the 3-month CME contract) and spot, expressed as an annualized percentage. It is the return available to a "cash-and-carry" trade: buy spot, sell the future, collect the spread with no price risk.

**Where to get it free.** [Coinglass](https://www.coinglass.com/), [Velo](https://velo.xyz/), [Laevitas](https://app.laevitas.ch/) (free tier), CME's own quotes versus Coinbase spot.

**How to read it.** A basis of 5 to 10% annualized is normal in calm bull markets. Above 20% (as in early 2021 and again briefly in late 2024) means speculators are paying huge premiums for leverage; hedge funds arbitrage it away by shorting, which is why it rarely persists. A basis below the Treasury bill yield (about 3.5 to 4% as of September 2026) means the trade is unattractive and basis-trade capital leaves, which shows up as ETF outflows paired with CME short covering. This mechanism explains part of the January to July 2026 ETF outflows: as the premium compressed, arbitrage funds unwound spot ETF longs against CME shorts.

**Track record.** Extreme basis is a reliable "froth" flag. Compressed basis is useful for interpreting ETF flow data correctly (see the flows page).

## Liquidations and liquidation maps

**What it measures.** Forced closures of leveraged positions when margin runs out. Exchanges publish them (with some under-reporting); aggregators sum them. Liquidation "heatmaps" estimate where clusters of leverage would be forced out at given price levels.

**Where to get it free.** [Coinglass liquidations](https://www.coinglass.com/liquidations/BTC), [Coinglass liquidation heatmap](https://www.coinglass.com/pro/futures/LiquidationHeatMap), [Hyperliquid liquidation data via Hyperdash](https://hyperdash.info/).

**How to read it.** A day with $500 million to $1 billion+ in liquidations is a flush; the largest events (October 10, 2025 was the biggest on record at well over $10 billion by most tallies) reset leverage for weeks and often mark local extremes. Glassnode reported that August 19, 2026 saw the largest single-day short flush since 2019, and that shorts were 85% of liquidations during the August squeeze. Heatmaps show where price is "magnetized": large clusters of long liquidations below price are a downside target, large short clusters above are an upside target. The Yahoo Finance summary for early September 2026 cited about $3 billion of long liquidation leverage below price on Binance versus $1.8 billion of short leverage above, a mild downside skew.

**Track record.** Liquidation cascades are coincident by definition. Heatmaps are useful for setting expectations about where a squeeze stops; they are not forecasts.

## Options: implied volatility (DVOL) and skew

**What it measures.** Implied volatility (IV) is the market's expectation of future price swings, backed out of option prices. Deribit's DVOL index is the Bitcoin equivalent of the VIX: a 30-day forward IV, annualized. Skew compares the IV of puts to calls at equal distance from spot; positive put skew means downside protection is expensive (fear), call skew means upside is bid (greed). Max pain is the expiry price at which option buyers lose the most in aggregate.

**Where to get it free.** [Deribit DVOL on TradingView](https://www.tradingview.com/symbols/DVOL/), [Deribit metrics page](https://metrics.deribit.com/), [Laevitas](https://app.laevitas.ch/), [Coinglass options](https://www.coinglass.com/options), [Glassnode DVOL chart](https://studio.glassnode.com/charts/derivatives.DvolOhlc?a=BTC).

**How to read it.** DVOL has spent most of the ETF era between about 40 and 70. Readings below 40 are complacent and usually precede a big move (direction unknown); readings above 80 have appeared only in crashes and manias. The 25-delta skew is the sentiment read: when puts trade 10+ vol points over calls, fear is high and often near a local low; when calls trade over puts by that much, the crowd is chasing. Glassnode noted a $14 billion options open interest for the September 25, 2026 expiry with max pain around $69,000 to $70,000 and a "dealer gamma flip" near $82,300, meaning above that level market makers' hedging would amplify moves rather than dampen them. Those specific levels expire, but the concept (large expiries pin price toward max pain in the final week) repeats every quarter.

**Track record.** IV is a good regime gauge and a decent contrarian signal at extremes. Skew extremes are one of the better short-term sentiment reads because they reflect money spent, not surveys.

## Spot versus perp volume

**What it measures.** The ratio of spot trading volume to perpetual futures volume. Also watch "cumulative volume delta" (CVD) on spot versus perps: is net buying happening on spot exchanges (real demand) or on perps (leverage)?

**Where to get it free.** [The Block: spot vs derivatives volume](https://www.theblock.co/data/crypto-markets/spot), [Kaiko research (free posts)](https://research.kaiko.com/), [Coinglass spot vs futures](https://www.coinglass.com/pro/futures/Cryptofutures).

**How to read it.** Rallies led by spot CVD (Coinbase, Bitstamp, Kraken buying) are more durable than rallies led by perp CVD. When perp volume is more than 5 to 6 times spot, the market is casino-heavy and the next move is likely to be violent.

**Track record.** More a quality-of-move diagnostic than a signal. Useful for deciding whether to trust a breakout.

## Coinbase premium

**What it measures.** The percentage difference between Bitcoin's price on Coinbase (USD, US investors, institutional custody) and Binance (USDT, global). CryptoQuant publishes it as an index.

**Where to get it free.** [CryptoQuant Coinbase Premium Index](https://cryptoquant.com/asset/btc/chart/market-data/coinbase-premium-index), [crypto.news explainer](https://crypto.news/what-is-the-coinbase-premium-index/).

**How to read it.** Positive premium means US buyers (often ETFs' authorized participants, which mostly buy on Coinbase) are paying up: US demand. Persistent negative premium means US selling, common through much of 2022 and again in early 2026. Readings above about 0.1 have appeared near strong institutional buying (October 2025 printed 0.18, the highest since March 2024, per BeInCrypto).

**Track record.** Decent as a confirmation of ETF-era demand; it tracks ETF flows closely, which makes it partly redundant with the Farside data. Sudden flips from negative to positive during a drawdown have been good short-term buy signals.

## Korean premium ("kimchi premium")

**What it measures.** The percentage by which Bitcoin trades on Korean exchanges (Upbit, Bithumb, in KRW) above global prices. Korean capital controls limit arbitrage, so the premium reflects domestic retail demand.

**Where to get it free.** [CryptoQuant Korea Premium Index](https://cryptoquant.com/asset/btc/chart/market-data/korea-premium-index), [Kimchi premium tracker (kimpga.com)](https://kimpga.com/).

**How to read it.** A premium above roughly 5% has coincided with retail manias (it hit 40%+ in January 2018 and around 20% in spring 2021). A discount signals local disinterest, common at bottoms. BeInCrypto noted Bithumb trading 7.47% above Binance during a February 2025 dip, and Bitcoin.com reported a 2% premium in 2026 as the first since the pre-war shock, showing the range: small positive premiums are normal, large ones are frothy. Interesting historical wrinkle: when both the Coinbase and Korean premiums spiked together (March 2024, February 2025), the market weakened for 3 to 6 months before resuming, so simultaneous spikes are not a clean buy.

**Track record.** Excellent at flagging retail euphoria in its historical peaks; a mediocre signal in normal ranges.

## How to use it

1. Daily or weekly, glance at three numbers: BTC funding (annualized), OI in BTC terms, and DVOL. That covers leverage, positioning size and expected turbulence.
2. Fade extremes on a short horizon only: funding above 50% annualized or below zero for days, OI at records, skew at 10+ points either way.
3. Before trusting a breakout, check whether spot CVD or perp CVD led it and whether OI rose (new conviction) or fell (short covering).
4. Use liquidation heatmaps to set expectations about where a move stalls, not to predict which way it goes.
5. Use basis to interpret ETF flows: when basis is compressed, outflows are often arbitrage unwinds rather than investors leaving.
6. Remember the horizon: none of this informs a 12-month view. It exists to help you avoid buying into a crowded long or panic-selling into a crowded short.

## Key takeaways

- Funding and OI describe leverage; extremes in either are the most reliable 1-to-3-week contrarian signals in crypto.
- Read OI in coin terms and in combination with price direction; rising price with falling OI is short covering, which tends to fade.
- Basis above 20% annualized is froth; basis below T-bill yields drains arbitrage capital and shows up as ETF outflows that are not "investors leaving".
- Liquidation cascades are what most sudden crypto crashes actually are; the largest ones reset leverage and often mark local extremes.
- DVOL below 40 is complacency, above 80 is panic or mania; put/call skew is the best cheap sentiment read because it reflects money spent.
- Coinbase premium tracks US institutional demand; the Korean premium flags retail mania when it exceeds mid-single digits.
- As of September 2026: funding near neutral, OI down in coin terms after the August short squeeze, DVOL mid-range, mild downside liquidation skew, big September 25 expiry with max pain near $69–70K. A balanced, not stretched, structure.

## Sources

- [Coinglass BTC futures dashboard](https://www.coinglass.com/currencies/BTC/futures)
- [Coinglass funding rates](https://www.coinglass.com/FundingRate)
- [Coinglass liquidations](https://www.coinglass.com/liquidations/BTC)
- [CoinDesk: Funding plunges to -6% as Bitcoin tries to reclaim $64,000 (February 28, 2026)](https://www.coindesk.com/markets/2026/02/28/bitcoin-sets-up-potential-short-squeeze-as-funding-plunges-to-6)
- [Glassnode Week On-Chain, Week 34 2026 "Squeeze into Supply"](https://research.glassnode.com/the-week-onchain-week-34-2026/)
- [Glassnode Week On-Chain, Week 35 2026 "Doubt at the Boundaries"](https://research.glassnode.com/the-week-onchain-week-35-2026/)
- [Yahoo Finance: Bitcoin price prediction for September 2026](https://finance.yahoo.com/markets/crypto/articles/bitcoin-price-prediction-september-2026-080209568.html)
- [Deribit Insights: DVOL implied volatility index](https://insights.deribit.com/exchange-updates/dvol-deribit-implied-volatility-index/)
- [TradingView: DVOL](https://www.tradingview.com/symbols/DVOL/)
- [CryptoQuant Coinbase Premium Index (API docs)](https://docs.cryptoquant.com/api-reference/btc-market-data/coinbase-premium-index)
- [crypto.news: What is the Coinbase Premium Index (2026)](https://crypto.news/what-is-the-coinbase-premium-index/)
- [BeInCrypto: Coinbase and Korea premiums spike](https://beincrypto.com/coinbase-and-korea-premium-surge/)
- [Bitcoin.com News: Korea premium hits 2% (2026)](https://news.bitcoin.com/bitcoin-premium-in-south-korea-hits-2-for-first-time-since-pre-war-market-shock/)
- [The Block: spot volume data](https://www.theblock.co/data/crypto-markets/spot)
