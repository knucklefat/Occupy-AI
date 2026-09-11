# Crypto Indicators

**In one sentence:** This section catalogs the on-chain, market-structure, flow, sentiment, macro and cycle indicators that crypto investors actually watch, explains what each one measures and where to get it free, and is candid about which ones have a real track record and which are folklore.

Crypto is unusual among asset classes in how much of its data is public. Every Bitcoin transaction, every miner's revenue, every ETF creation and every futures position on the major exchanges is visible within hours, mostly for free. That transparency has produced an enormous indicator industry, much of it curve-fitted to a handful of past cycles. The eight guides here separate the durable ideas (realized cost basis, flows, leverage, real yields) from the decorative ones (rainbow charts, pi ratios), give each indicator a plain-language reading rule, and report where each stood as of September 2026. The final guide turns the whole set into a 14-row weekly checklist with normal, caution and alarm zones and a regime framework so the data leads to a posture rather than to more charts.

## Guides in this section

1. [On-chain valuation indicators](on-chain-valuation-indicators.md): MVRV and Z-score, realized price, NUPL, SOPR, Puell Multiple, reserve risk, HODL waves, long-term holder supply.
2. [Network and adoption indicators](network-and-adoption-indicators.md): active addresses, transactions, hash rate and difficulty, hashprice, Lightning, stablecoin supply, Ethereum gas and L2s, DeFi TVL, exchange balances.
3. [Market structure and derivatives indicators](market-structure-and-derivatives-indicators.md): funding, open interest, basis, liquidations, DVOL and skew, spot vs perp volume, Coinbase and Korean premiums.
4. [Flows and supply indicators](flows-and-supply-indicators.md): spot ETF flows, exchange flows, stablecoin issuance, whale cohorts, treasury companies, miner selling, custodian data.
5. [Sentiment indicators](sentiment-indicators.md): Fear & Greed, Google Trends, app-store ranks, social data, funding as sentiment, contrarian checklists.
6. [Macro and liquidity drivers](macro-and-liquidity-drivers.md): global M2, real yields, DXY, Nasdaq and gold correlations, Fed path, Treasury plumbing, and the inflation-hedge evidence.
7. [Bitcoin cycle indicators](bitcoin-cycle-indicators.md): halving timeline, 200-week MA, Pi Cycle, 2-year MA multiplier, rainbow chart, cycle overlays, diminishing returns, and the ETF-era debate.
8. [How to build a crypto dashboard](how-to-build-a-crypto-dashboard.md): the weekly checklist, zones, regime framework, and a worked September 2026 example.

## Master table of indicators

| Indicator | Category | Free source | Update frequency | Covered in |
|---|---|---|---|---|
| MVRV ratio / MVRV Z-score | On-chain valuation | [lookintobitcoin.com](https://www.lookintobitcoin.com/charts/mvrv-zscore/) | Daily | Guide 1 |
| Realized price (all, STH, LTH) | On-chain valuation | [Glassnode Studio](https://studio.glassnode.com/charts/btc-sth-realized-price-mvrv?a=BTC) | Daily | Guide 1 |
| NUPL | On-chain valuation | [lookintobitcoin.com](https://www.lookintobitcoin.com/charts/relative-unrealized-profit--loss/) | Daily | Guide 1 |
| SOPR (and STH/LTH variants) | On-chain valuation | [Glassnode Studio](https://studio.glassnode.com/charts/indicators.Sopr?a=BTC) | Daily | Guide 1 |
| Puell Multiple | On-chain valuation | [lookintobitcoin.com](https://www.lookintobitcoin.com/charts/puell-multiple/) | Daily | Guide 1 |
| Reserve Risk | On-chain valuation | [lookintobitcoin.com](https://www.lookintobitcoin.com/charts/reserve-risk/) | Daily | Guide 1 |
| HODL waves / realized-cap HODL waves | On-chain valuation | [Unchained](https://unchained.com/hodlwaves/) | Daily | Guide 1 |
| Long-term holder supply | On-chain valuation | [Glassnode Studio](https://studio.glassnode.com/charts/supply.LthSum?a=BTC) | Daily | Guide 1 |
| Active addresses / transaction count | Network | [Coin Metrics charts](https://charts.coinmetrics.io/) | Daily | Guide 2 |
| Hash rate and difficulty | Network | [mempool.space](https://mempool.space/mining) | Continuous; difficulty every ~2 weeks | Guide 2 |
| Hashprice / miner revenue | Network | [Hashrate Index](https://data.hashrateindex.com/chart/bitcoin-hashprice-index) | Daily | Guide 2 |
| Lightning Network capacity | Network | [mempool.space](https://mempool.space/graphs/lightning/capacity) | Daily | Guide 2 |
| Stablecoin total supply | Network / Flows | [DefiLlama](https://defillama.com/stablecoins) | Daily | Guides 2, 4 |
| Ethereum gas and L2 activity | Network | [Etherscan](https://etherscan.io/gastracker), [L2BEAT](https://l2beat.com/scaling/summary) | Continuous / daily | Guide 2 |
| DeFi TVL | Network | [DefiLlama](https://defillama.com/) | Continuous | Guide 2 |
| Exchange balances | Network / Flows | [CryptoQuant](https://cryptoquant.com/asset/btc/chart/exchange-flows/exchange-reserve) | Daily | Guides 2, 4 |
| Funding rates | Derivatives | [Coinglass](https://www.coinglass.com/FundingRate) | Every 8 hours | Guides 3, 5 |
| Open interest | Derivatives | [Coinglass](https://www.coinglass.com/open-interest/BTC) | Continuous | Guide 3 |
| Futures basis / annualized premium | Derivatives | [Laevitas](https://app.laevitas.ch/) / [Coinglass](https://www.coinglass.com/) | Continuous | Guide 3 |
| Liquidations and heatmaps | Derivatives | [Coinglass](https://www.coinglass.com/liquidations/BTC) | Continuous | Guide 3 |
| DVOL (implied volatility) and skew | Derivatives | [TradingView DVOL](https://www.tradingview.com/symbols/DVOL/), [Deribit metrics](https://metrics.deribit.com/) | Continuous | Guide 3 |
| Spot vs perp volume / CVD | Derivatives | [The Block data](https://www.theblock.co/data/crypto-markets/spot) | Daily | Guide 3 |
| Coinbase premium | Market structure | [CryptoQuant](https://cryptoquant.com/asset/btc/chart/market-data/coinbase-premium-index) | Continuous | Guide 3 |
| Korean (kimchi) premium | Market structure | [CryptoQuant](https://cryptoquant.com/asset/btc/chart/market-data/korea-premium-index) | Continuous | Guide 3 |
| Spot Bitcoin/Ether ETF net flows | Flows | [Farside](https://farside.co.uk/btc/) | Daily (evening US) | Guide 4 |
| Exchange inflows/outflows | Flows | [CryptoQuant](https://cryptoquant.com/asset/btc/chart/exchange-flows/exchange-netflow-total) | Daily | Guide 4 |
| Stablecoin issuance/redemptions | Flows | [DefiLlama](https://defillama.com/stablecoins) | Daily | Guide 4 |
| Whale / cohort accumulation | Flows | [Glassnode Accumulation Trend Score](https://studio.glassnode.com/charts/indicators.AccumulationTrendScore?a=BTC) | Daily | Guide 4 |
| Treasury-company purchases | Flows | [BitcoinTreasuries.net](https://bitcointreasuries.net/) | As filed | Guide 4 |
| Miner selling / reserves | Flows | [CryptoQuant](https://cryptoquant.com/asset/btc/chart/miner-flows/miner-outflow) | Daily | Guide 4 |
| ETF and custodian holdings | Flows | [Coinglass ETF](https://www.coinglass.com/etf/bitcoin), [Arkham](https://intel.arkm.com/) | Daily | Guide 4 |
| Crypto Fear & Greed index | Sentiment | [alternative.me](https://alternative.me/crypto/fear-and-greed-index/) | Daily | Guide 5 |
| Google Trends ("bitcoin") | Sentiment | [Google Trends](https://trends.google.com/trends/explore?date=today%205-y&q=bitcoin) | Daily (weekly on 5-year view) | Guide 5 |
| App-store rankings | Sentiment | [Apple top free apps](https://apps.apple.com/us/charts/iphone/top-free-apps/36) | Daily | Guide 5 |
| Social volume / sentiment | Sentiment | [LunarCrush](https://lunarcrush.com/), [Santiment](https://app.santiment.net/) | Continuous | Guide 5 |
| Global M2 / net liquidity | Macro | [Newhedge](https://newhedge.io/bitcoin/bitcoin-vs-global-m2-growth), [FRED](https://fred.stlouisfed.org/series/M2SL) | Weekly / monthly | Guide 6 |
| Real yields (10-year TIPS) | Macro | [FRED DFII10](https://fred.stlouisfed.org/series/DFII10) | Daily | Guide 6 |
| Dollar index (DXY) | Macro | [TradingView](https://www.tradingview.com/symbols/TVC-DXY/) | Continuous | Guide 6 |
| BTC correlation with S&P 500 and gold (30-day) | Macro | [The Block data](https://www.theblock.co/data/crypto-markets/prices/btc-pearson-correlation-30d) | Daily | Guide 6 |
| Fed funds path | Macro | [CME FedWatch](https://www.cmegroup.com/markets/interest-rates/cme-fedwatch-tool.html) | Continuous | Guide 6 |
| Treasury plumbing (TGA, RRP, reserves) | Macro | [FRED](https://fred.stlouisfed.org/series/WTREGEN) | Daily / weekly | Guide 6 |
| Halving countdown | Cycle | [mempool.space](https://mempool.space/) | Continuous | Guide 7 |
| 200-week moving average | Cycle | [lookintobitcoin.com](https://www.lookintobitcoin.com/charts/200-week-moving-average-heatmap/) | Weekly | Guide 7 |
| Pi Cycle Top | Cycle | [lookintobitcoin.com](https://www.lookintobitcoin.com/charts/pi-cycle-top-indicator/) | Daily | Guide 7 |
| 2-Year MA Multiplier | Cycle | [lookintobitcoin.com](https://www.lookintobitcoin.com/charts/bitcoin-investor-tool/) | Daily | Guide 7 |
| Rainbow chart | Cycle | [blockchaincenter.net](https://www.blockchaincenter.net/en/bitcoin-rainbow-chart/) | Daily | Guide 7 |
| Cycle comparison overlays | Cycle | [Bitbo](https://charts.bitbo.io/cycle-repeat/) | Daily | Guide 7 |

## How to use it

Read Guide 8 first if you want a working process; read Guides 1 and 4 first if you want to understand the two data families that carry the most weight (cost basis and flows). Guides 3 and 5 explain short-horizon signals that are useful for avoiding bad entries and exits, and Guides 6 and 7 provide the long-horizon context. Every guide ends with a "How to use it" section and a track-record judgment, and every current reading is dated as of September 2026 so it can be checked against the live sources.

## Key takeaways

- Cost-basis metrics (realized price, MVRV, NUPL) and flow data (ETF flows, stablecoin supply) are the two families with the best evidence behind them.
- Derivatives data is the best short-horizon tool and useless for long horizons; sentiment is only useful at extremes.
- Bitcoin trades as a liquidity asset, not an inflation hedge; real yields, the dollar and the Fed path matter more than CPI.
- The four-year cycle has kept its timing and lost its amplitude; upper-band "sell" indicators calibrated to 2017 and 2021 have stopped firing.
- Nearly everything here is free; the scarce resource is the discipline to check it weekly against pre-set zones.
- As of September 2026 the composite picture is a fairly valued, institutionally driven recovery facing a restrictive macro backdrop.

## Sources

- [Glassnode Research: The Week On-Chain](https://research.glassnode.com/)
- [Glassnode Academy](https://academy.glassnode.com/)
- [CryptoQuant](https://cryptoquant.com/)
- [Coin Metrics Network Data Charts](https://charts.coinmetrics.io/)
- [Checkonchain](https://charts.checkonchain.com/)
- [Bitcoin Magazine Pro charts](https://www.bitcoinmagazinepro.com/charts/)
- [Look Into Bitcoin](https://www.lookintobitcoin.com/charts/)
- [alternative.me Fear & Greed](https://alternative.me/crypto/fear-and-greed-index/)
- [Coinglass](https://www.coinglass.com/)
- [DefiLlama](https://defillama.com/)
- [Farside Investors](https://farside.co.uk/btc/)
- [The Block Data](https://www.theblock.co/data)
- [mempool.space](https://mempool.space/)
- [Kaiko Research](https://research.kaiko.com/)
