# Flows and Supply Indicators

**In one sentence:** Flow indicators track who is buying and selling Bitcoin in size (ETFs, exchanges, stablecoin issuers, whales, treasury companies, miners), and since 2024 the ETF flow tape has become the single most price-relevant daily number in crypto, with the caveat that flows follow price at least as often as they lead it.

## The ETF era changed what matters

Before January 2024, the marginal Bitcoin buyer was a retail trader on an exchange or a fund on Grayscale's trust. Since US spot ETFs launched, the marginal buyer is often an advisor allocating a client's 1 to 3%, a hedge fund running a basis trade, or a corporate treasury. Those flows are visible daily, in dollars, and they are large relative to new supply (about 450 BTC per day, roughly $35 million at $78,000). That is why a page on "flows" is now as important as the on-chain page.

## Spot ETF net flows

**What it measures.** Daily net creations minus redemptions across the US spot Bitcoin ETFs (IBIT, FBTC, GBTC, BITB, ARKB, HODL and others), in dollars. Ethereum ETFs are tracked separately. Since a creation means the issuer must buy Bitcoin in the market, net inflows are direct spot demand.

**Where to get it free.** [Farside Investors Bitcoin ETF flows](https://farside.co.uk/btc/) (the industry standard table, updated each evening US time), [Farside all data](https://farside.co.uk/bitcoin-etf-flow-all-data/), [Coinglass ETF dashboard](https://www.coinglass.com/etf/bitcoin), [SoSoValue ETF dashboard](https://sosovalue.com/assets/etf/us-btc-spot), [Farside Ethereum ETF flows](https://farside.co.uk/eth/).

**How to read it.** Use the 7-day and 30-day sums, not the daily print, because single days are noisy and Farside's figures for some issuers post a day late. Interpretation guide: more than $1 billion per week of net inflows sustained for several weeks has accompanied every leg up since 2024 (February–March 2024, October–December 2024, April–July 2025). Persistent outflows of $200 million to $500 million per day over weeks have accompanied every leg down. Also read who is flowing: IBIT and FBTC are mostly "sticky" advisor and institutional money; GBTC and some smaller funds see fee-driven rotations; large simultaneous IBIT inflows and CME OI increases suggest basis-trade money, which leaves when the futures premium compresses.

**As of September 2026.** August 2026 saw about $3.52 billion of net inflows, reversing seven straight months (January to July) of roughly $5.3 billion of outflows, according to the Yahoo Finance summary. The week ending September 4 added about $987 million, with IBIT taking roughly $454 million on September 3 alone; cumulative net inflows since launch stood near $55.7 billion, per HedgeCo's Farside-based tally. Glassnode's 7-day average peaked around $290 million per day during the August squeeze.

**Track record.** Flows are strongly correlated with price contemporaneously, and the direction of the 30-day sum has been a decent trend filter. Their lead is weak: big inflow days cluster after a rally begins. The best use is as confirmation (is real spot demand behind this move?) and as an early warning when flows turn negative while price is still high, as they did in late October 2025.

## Exchange inflows and outflows

**What it measures.** Coins moving into or out of tagged exchange wallets. Inflows are potential sell pressure; outflows are coins going to custody. Netflow is the difference. CryptoQuant also publishes "exchange whale ratio" (share of inflows coming from the top 10 transactions).

**Where to get it free.** [CryptoQuant exchange netflow](https://cryptoquant.com/asset/btc/chart/exchange-flows/exchange-netflow-total), [Glassnode exchange net position change](https://studio.glassnode.com/charts/distribution.ExchangeNetPositionChange?a=BTC), [Coinglass exchange balance](https://www.coinglass.com/Balance).

**How to read it.** Focus on spikes, not the baseline. A single-day inflow above about 30,000 to 50,000 BTC that is not explained by an exchange's internal wallet reshuffle has often preceded a sell-off within days. Sustained outflows during a drawdown are a modest positive (holders moving to cold storage). Glassnode noted in late August 2026 that wallets in the 100,000+ BTC "custody" band gained 31,500 BTC from exchange outflows, consistent with ETF custodians absorbing supply. Beware: entity tagging is imperfect and the biggest single inflows are frequently Coinbase or Binance moving their own coins.

**Track record.** Inflow spikes are a useful but low-precision sell warning. Netflow trends are mostly a slow restatement of ETF and custody activity now.

## Stablecoin issuance and redemptions

**What it measures.** Net minting (supply growth) versus burning (redemptions) of USDT, USDC and others, and specifically stablecoin balances held on exchanges ("buying power on exchanges").

**Where to get it free.** [DefiLlama stablecoins](https://defillama.com/stablecoins), [CryptoQuant stablecoin exchange reserve](https://cryptoquant.com/asset/stablecoin/chart/exchange-flows/exchange-reserve), [Tether transparency page](https://tether.to/en/transparency/), [Circle USDC transparency](https://www.circle.com/transparency).

**How to read it.** Large Tether mints (often $1 billion "treasury" prints) are frequently a pre-funding of exchange demand, especially from Asia; they are a soft leading signal. Large USDC redemptions have historically meant US institutional risk-off. As of mid-September 2026 total supply was roughly $305 to $310 billion depending on the tracker (DefiLlama ~$310 billion), flat over 30 days and below the May 2026 record near $321 billion, with USDC growing slightly faster than USDT. The stablecoin-supply-ratio (Bitcoin market cap divided by stablecoin cap) is a crude gauge of dry powder; a low ratio means lots of sidelined dollars relative to Bitcoin's size.

**Track record.** Among the better medium-term leading signals in 2020–21 and 2023–24. Less reliable when supply growth is driven by non-crypto uses (payments, treasury yield), which is an increasing share.

## Whale accumulation and distribution

**What it measures.** Balance changes of address cohorts grouped by size (for example 1,000 to 10,000 BTC "whales", 100 to 1,000 BTC "sharks", under 1 BTC "shrimp"). Glassnode's "Accumulation Trend Score" collapses this into a 0-to-1 heatmap.

**Where to get it free.** [Glassnode Accumulation Trend Score](https://studio.glassnode.com/charts/indicators.AccumulationTrendScore?a=BTC), [checkonchain.com cohort charts](https://charts.checkonchain.com/), [Santiment supply distribution (free tier)](https://app.santiment.net/), [BitInfoCharts rich list](https://bitinfocharts.com/top-100-richest-bitcoin-addresses.html).

**How to read it.** The meaningful pattern is disagreement between cohorts. In August 2026, per Glassnode and the Yahoo Finance summary, wallets holding 1,000 to 10,000 BTC shed about 50,000 BTC since June 30 and the count of whale addresses fell from 1,963 to 1,908 during the 25% rally, while ETF-related custody wallets absorbed coins. That is "whales selling into fund buying", a classic mid-cycle handoff, not the "everyone accumulating" pattern that marks strong bottoms. Glassnode's own July 2026 line was that a full accumulation regime needs the largest holders to join, and they had not.

**Track record.** Accumulation across all cohorts simultaneously has preceded strong recoveries (early 2019, mid-2020, early 2023). Whale-only distribution while small wallets buy has marked late-cycle tops. Cohort data is noisy because of exchange and custodian wallets, so use the smoothed score.

## Treasury-company purchases

**What it measures.** Bitcoin bought by publicly traded companies as a treasury asset, led by Strategy (formerly MicroStrategy), plus miners and a wave of "digital asset treasury" companies created in 2025. Their buying is financed by equity and convertible debt, so it depends on their share price trading at a premium to the value of their Bitcoin ("mNAV" above 1).

**Where to get it free.** [BitcoinTreasuries.net](https://bitcointreasuries.net/), [Bitbo Strategy holdings tracker](https://bitbo.io/treasuries/microstrategy), Strategy's own 8-K filings via [SEC EDGAR](https://www.sec.gov/cgi-bin/browse-edgar?action=getcompany&CIK=0001050446&type=8-K), [Strategy's purchase history](https://www.strategy.com/purchases).

**How to read it.** Treasury demand is pro-cyclical by construction: companies can only raise cheap capital when their stock is at a premium, which happens when Bitcoin is rising. When mNAV falls toward or below 1, buying stops and, in the worst case, reverses. 2026 delivered the case study: Fortune reported that Strategy paused purchases for two months, sold roughly $544 million of Bitcoin across four transactions to meet obligations during the drawdown, then resumed with a $370 million buy at about $80,300 on August 31 once the rally lifted its holdings back above cost. Strategy holds about 4% of all Bitcoin, so its behavior is a supply factor in its own right. Watch: mNAV of the major treasury companies, the pace of at-the-market equity sales, and convertible maturities.

**Track record.** Treasury buying added meaningful demand in 2024–25 and supported the late-2025 top; the 2026 reversal showed the flip side. Treat it as an amplifier of the trend, not an independent signal.

## Miner selling

**What it measures.** Coins flowing from miner-tagged wallets to exchanges, and miner reserves (total coins held by miners). Miners are structural sellers because their costs are in fiat.

**Where to get it free.** [CryptoQuant miner outflow](https://cryptoquant.com/asset/btc/chart/miner-flows/miner-outflow), [Glassnode miner net position change](https://studio.glassnode.com/charts/mining.MinersNetPositionChange?a=BTC), [Hashrate Index](https://hashrateindex.com/).

**How to read it.** Miner selling spikes when hashprice falls below break-even (they must sell reserves) and when price spikes (they sell into strength to fund expansion). Post-halving, miner supply is only about 450 BTC a day, so their flows matter less than they did in 2017 or 2020. Public miners' monthly production reports show whether they are "HODLing" or selling 100%+ of production; a shift to selling more than they mine is a stress signal. With fees at under 1% of revenue in September 2026, miner economics are entirely a function of price, and hashprice near $40/PH/day leaves the fleet's average operator with thin margins.

**Track record.** Miner capitulation is a decent bottom marker; miner selling into rallies is normal and not a top signal on its own.

## Grayscale, custodian and ETF holdings data

**What it measures.** Total Bitcoin held by ETFs and large custodians. Coinbase Custody holds the coins for most US ETFs; its on-chain footprint is visible in Arkham and Glassnode entity tags. GBTC's holdings shrank from about 620,000 BTC in early 2024 to well under 200,000 as investors rotated to cheaper funds.

**Where to get it free.** [Arkham Intelligence entity pages (Coinbase Custody, BlackRock)](https://intel.arkm.com/), [Coinglass ETF holdings](https://www.coinglass.com/etf/bitcoin), [Grayscale GBTC holdings page](https://www.grayscale.com/funds/grayscale-bitcoin-trust-etf), [Dune dashboards for ETF holdings](https://dune.com/browse/dashboards?q=bitcoin+etf).

**How to read it.** Total ETF holdings as a share of supply (about 6 to 7% for US spot ETFs by 2026) is the structural measure of "financialized" Bitcoin. Short-term, ETF holdings changes duplicate the flow data. The value of custodian data is in detecting large movements before they show in official flow tables and in checking whether "exchange outflows" are really just ETF custody transfers.

**Track record.** Structural context rather than a signal.

## How to use it

1. Every evening, or at least weekly, read the Farside table: daily print, 7-day sum, which issuers. Ask whether flows confirm the price move.
2. When flows and price disagree (price up, flows negative for two weeks), trust the flows; that pattern preceded the late-2025 decline.
3. Cross-check ETF inflows with CME open interest and the futures basis. If both rise together, part of the inflow is arbitrage, not allocation.
4. Watch stablecoin supply's 30-day change as the medium-term dry-powder signal.
5. Treat treasury-company buying and miner selling as amplifiers of the trend; watch mNAV and hashprice to anticipate when they flip.
6. Use cohort accumulation to judge whether a bottom is broad-based (all sizes buying) or a handoff (whales selling to funds).

## Key takeaways

- Spot ETF net flows (Farside) are the most price-relevant daily number in crypto; read the 7-day and 30-day sums, not single days.
- Flows confirm more than they predict, but a divergence (price high, flows negative) has been an effective early warning.
- Basis-trade money inflates inflows in good times and outflows in bad; check CME OI and the futures premium before calling flows "investor demand".
- Stablecoin supply growth is the best medium-term dry-powder gauge; it was flat through the August–September 2026 rally.
- Treasury companies are pro-cyclical buyers; Strategy's 2026 pause and partial sales showed they can become sellers.
- Exchange inflow spikes are a short-term sell warning; the multi-year decline in balances is structural and not itself bullish.
- As of September 2026: ETF flows strongly positive since August (~$3.5B in August, ~$1B the first week of September), whales distributing into fund demand, stablecoins flat, Strategy buying again. Demand is institutional and narrow rather than broad.

## Sources

- [Farside Investors: Bitcoin ETF flows](https://farside.co.uk/btc/)
- [Farside Investors: Bitcoin ETF flow all data](https://farside.co.uk/bitcoin-etf-flow-all-data/)
- [HedgeCo: Spot Bitcoin ETFs drew about $987 million for the week ending September 4, 2026](https://hedgeco.net/news/09/2026/spot-bitcoin-etfs-drew-about-987-million-for-the-week-ending-september-4.html)
- [HedgeCo: $236.5 million net outflow on September 1, 2026](https://hedgeco.net/news/09/2026/spot-bitcoin-etfs-posted-a-236-5-million-net-outflow-on-september-1.html)
- [Yahoo Finance: Bitcoin price prediction for September 2026 (August flow and whale data)](https://finance.yahoo.com/markets/crypto/articles/bitcoin-price-prediction-september-2026-080209568.html)
- [Glassnode Week On-Chain, Week 34 2026](https://research.glassnode.com/the-week-onchain-week-34-2026/)
- [CoinDesk: Long-term holders return to accumulation (July 2026)](https://www.coindesk.com/markets/2026/07/02/bitcoin-long-term-holders-have-returned-to-accumulation)
- [Fortune: Strategy makes first Bitcoin buy in two months (August 31, 2026)](https://fortune.com/2026/08/31/bitcoin-michael-saylors-strategy-first-buy-two-months/)
- [BitcoinTreasuries.net: Strategy](https://bitcointreasuries.net/public-companies/strategy)
- [KuCoin News: Exchange reserves at multi-year low (March 2026)](https://www.kucoin.com/news/flash/bitcoin-exchange-reserves-hit-all-time-low-amid-shrinking-supply)
- [Stablecoin Beat tracker](https://stablecoinbeat.com/tracker/)
- [Coinglass ETF dashboard](https://www.coinglass.com/etf/bitcoin)
