# On-Chain Valuation Indicators

**In one sentence:** On-chain valuation indicators compare Bitcoin's market price to what holders actually paid for their coins, and while they have flagged every major cycle top and bottom since 2011, the extremes they reach have been shrinking each cycle, so treat their thresholds as moving targets rather than fixed lines.

## Why these indicators exist

Every Bitcoin transaction is public, and every coin carries a timestamp of when it last moved. That lets analysts reconstruct something stocks cannot offer: the aggregate cost basis of every holder. "Realized capitalization" (realized cap) values each coin at the price when it last moved on-chain rather than at today's price. It is, in effect, the total amount of money the current holder base has put into Bitcoin. Nearly every indicator on this page is a ratio built from realized cap.

A note on data freshness: Glassnode, CryptoQuant and Coin Metrics compute these from the full chain and update daily. Free tiers show most Bitcoin charts with a lag of a day or so, which is fine for weekly decision-making.

## MVRV ratio and MVRV Z-score

**What it measures.** MVRV (Market Value to Realized Value) is market cap divided by realized cap. At 1.0, the average holder is at break-even. At 2.0, the average coin is worth twice what its holder paid. The Z-score version subtracts realized cap from market cap and divides by the standard deviation of market cap, which stretches out the extremes and makes cycle tops and bottoms easier to see.

**Where to get it free.** [lookintobitcoin.com MVRV Z-Score](https://www.lookintobitcoin.com/charts/mvrv-zscore/), [checkonchain.com](https://charts.checkonchain.com/), [bitcoinmagazinepro.com MVRV](https://www.bitcoinmagazinepro.com/charts/mvrv-zscore/), [Glassnode Studio (free tier)](https://studio.glassnode.com/charts/realizedprice-mvrv?a=BTC).

**How to read it.** Roughly: Z-score below 0 has coincided with capitulation bottoms (early 2015, December 2018, March 2020, November 2022, each roughly -0.3 to -0.5). Z-score above 7 has marked the blow-off tops of 2013 (around 9 to 10), 2017 (around 9.5) and April 2021 (around 7.5). Between 3.5 and 7 is a caution zone where bull markets can run for months.

**Track record and the important caveat.** The October 2025 top at $126,198 (Fortune's figure) is the indicator's most humbling result. The Z-score peaked only in the low-to-mid 3s in December 2024 and was lower still at the actual price top, never approaching the historical 7+ red zone. Anyone waiting for a "classic" top signal never got one. The lesson: realized cap is now so large (ETF and treasury buyers accumulated at high prices) that the ratio cannot stretch as far as it once did. Every cycle's peak Z-score has been lower than the previous one. **As of September 2026**, with Bitcoin in the high $70,000s and realized price somewhere in the low-to-mid $50,000s, MVRV is roughly 1.4 to 1.5 and the Z-score is around 1 (one tracker printed 0.42 on August 8 when price was near $64,000). That is a "fair-to-cheap" zone historically, not a capitulation reading.

## Realized price

**What it measures.** Realized cap divided by circulating supply: the average on-chain cost basis of all coins. Glassnode also splits it by holder age. The short-term holder (STH) cost basis covers coins moved within the last 155 days; the long-term holder (LTH) cost basis covers older coins.

**Where to get it free.** [Glassnode realized price and MVRV](https://studio.glassnode.com/charts/70aa2400-53ee-4cb3-477e-b55793aa210a?a=BTC), [MacroMicro realized price](https://en.macromicro.me/charts/143271/bitcoin-realized-price), [Glassnode STH cost basis](https://studio.glassnode.com/charts/btc-sth-realized-price-mvrv?a=BTC).

**How to read it.** Price below realized price means the average holder is underwater; this has only happened in deep bear markets (2015, 2018–19, March 2020, mid-2022 to early 2023) and every one of those was, in hindsight, a generational buying window. The STH cost basis is a much faster line: in bull markets it acts as support (dips bounce off it), and in bear markets it acts as resistance. Glassnode's Week On-Chain for late August 2026 put the STH cost basis near $70,000 to $71,000, with price reclaiming it during the August rally and a band of heavy long-term-holder supply between $83,000 and $86,000 overhead.

**Track record.** Realized price as a bear-market floor is one of the strongest signals in the toolkit. It has never been "wrong" as a value zone, only early: price spent months below it in 2015 and 2022.

## NUPL (Net Unrealized Profit/Loss)

**What it measures.** (Market cap minus realized cap) divided by market cap. It is the share of the network's value that is unrealized profit. Mathematically it is 1 minus 1/MVRV, so it is the same information on a 0-to-1 scale that is easier to bucket.

**Where to get it free.** [lookintobitcoin.com NUPL](https://www.lookintobitcoin.com/charts/relative-unrealized-profit--loss/), [checkonchain.com](https://charts.checkonchain.com/).

**How to read it.** The usual color bands: below 0 "capitulation" (bottoms), 0 to 0.25 "hope/fear", 0.25 to 0.5 "optimism/anxiety", 0.5 to 0.75 "belief/denial", above 0.75 "euphoria/greed". Tops in 2013 and 2017 pushed into euphoria; the 2021 top barely touched 0.75; the 2025 top peaked around 0.6, again below the classic threshold. Bottoms in 2015, 2018, 2020 and 2022 all went negative.

**Track record.** Same strengths and same shrinking-extremes problem as MVRV. Useful as a regime label, not a timing tool.

## SOPR (Spent Output Profit Ratio)

**What it measures.** For coins that moved today, the price at which they were sold divided by the price at which they were acquired. Above 1 means coins are being sold at a profit on average; below 1 means at a loss. Variants: adjusted SOPR (ignores coins held under an hour), STH-SOPR and LTH-SOPR.

**Where to get it free.** [Glassnode SOPR](https://studio.glassnode.com/charts/indicators.Sopr?a=BTC), [CryptoQuant SOPR](https://cryptoquant.com/asset/btc/chart/market-indicator/sopr), [checkonchain.com](https://charts.checkonchain.com/).

**How to read it.** In a bull market, SOPR dipping to 1.0 and bouncing means holders refuse to sell at a loss, which is a healthy pullback. In a bear market SOPR struggles to get above 1.0 (sellers exit at break-even). LTH-SOPR above 4 to 8 has marked euphoric tops, because old coins are being cashed out at multiples of their cost.

**Track record.** Good as a confirmation of trend regime; noisy day to day. Use the 7-day or 30-day average.

## Puell Multiple

**What it measures.** Daily miner revenue in dollars divided by its 365-day average. It captures whether miners are earning far more (or far less) than they are used to, which affects how much they need to sell.

**Where to get it free.** [lookintobitcoin.com Puell Multiple](https://www.lookintobitcoin.com/charts/puell-multiple/), [CryptoQuant](https://cryptoquant.com/asset/btc/chart/network-indicator/puell-multiple), [bitcoinmagazinepro.com](https://www.bitcoinmagazinepro.com/charts/puell-multiple/).

**How to read it.** Below about 0.5 has coincided with major bottoms (2015, 2019, March 2020, 2022). Above roughly 4 marked the 2013 and 2017 tops; the 2021 top reached only the mid-3s and the 2025 top stayed well under that. Halvings mechanically cut the multiple (issuance halves overnight while the 365-day average still reflects the old rate), so readings in the year after a halving run low.

**Track record.** Decent at bottoms, weakening at tops for the same "diminishing extremes" reason. As of September 2026 the multiple sits below 1, consistent with miners earning less than their trailing-year average because price is 38% below the peak.

## Reserve Risk

**What it measures.** Price divided by "HODL bank", a measure of the accumulated opportunity cost long-term holders have borne by not selling. Low reserve risk means holders are confident and price is low relative to that conviction; high reserve risk means holders are being paid richly to keep holding.

**Where to get it free.** [lookintobitcoin.com Reserve Risk](https://www.lookintobitcoin.com/charts/reserve-risk/).

**How to read it.** Green zone (historically below about 0.002 on the original scale) marked 2015, 2018–19, 2020 and 2022 bottoms. Red zone (above 0.02) marked 2013, 2017 and 2021 tops. Glassnode has since revised the formula, so check which version a chart uses before comparing to historical thresholds.

**Track record.** Excellent at bottoms, slow and early at tops.

## HODL Waves and Realized Cap HODL Waves

**What it measures.** The share of supply that last moved within each age bracket (1 day, 1 week, 1 month, ... , 10+ years), shown as stacked bands. The realized-cap version weights each band by dollars rather than coins, which makes young-coin spikes (new money arriving) far more visible.

**Where to get it free.** [Unchained HODL Waves](https://unchained.com/hodlwaves/), [Glassnode HODL Waves](https://studio.glassnode.com/charts/supply.HodlWaves?a=BTC), [Coin Metrics charts](https://charts.coinmetrics.io/).

**How to read it.** Young bands (under 3 months) swelling to 30%+ of realized cap has occurred near every cycle top: new buyers piling in while old holders distribute. Old bands (1 year+) swelling to record highs occurs in bear markets as coins go dormant. A contraction in the 1y+ band while price rises means long-term holders are selling into strength, the classic late-cycle signature.

**Track record.** More a diagnostic than a signal; useful for confirming what phase of the cycle the market is in.

## Long-term holder supply

**What it measures.** Total coins held for more than 155 days. The complement, short-term holder supply, is the speculative float.

**Where to get it free.** [Glassnode LTH supply](https://studio.glassnode.com/charts/supply.LthSum?a=BTC), [checkonchain.com](https://charts.checkonchain.com/), [CryptoQuant](https://cryptoquant.com/).

**How to read it.** LTH supply falls during bull markets (old holders sell into demand) and rises during bear markets and consolidations. The turn from net distribution to net accumulation has historically happened during weak, boring price action and preceded recoveries. CoinDesk reported in July 2026 that Glassnode saw long-term holders return to net accumulation of roughly 50,000 to 100,000 BTC, well below the ~400,000 BTC accumulation waves of late 2024 and spring 2025, and Glassnode explicitly said it was "too early" to call a full accumulation regime because the largest wallets had not yet joined.

**Track record.** One of the most reliable regime indicators, but it says nothing about how long a bottom takes to form.

## How to use it

1. Check the regime first: is price above or below realized price, and above or below the STH cost basis? That answers "bull or bear" more honestly than any moving average.
2. Then check stretch: MVRV Z-score and NUPL. A Z-score under 1 says the market is not overheated; above 3 says be careful; above 5 in the ETF era would be extraordinary.
3. Then check behavior: LTH supply direction and SOPR. Are old coins moving to new hands (late cycle) or going dormant (early cycle)?
4. Treat thresholds as ranges that shrink each cycle. Compare the current reading to the previous cycle's peak, not to 2017's.
5. Never use these to time weeks. Their historical accuracy is measured in months; they were "early" by 3 to 9 months at nearly every turn.

## Key takeaways

- Realized cap (what holders actually paid) is the foundation; MVRV, NUPL, and realized price are all views of the same number.
- Price below realized price has been a generational buying zone every time, but it can persist for months.
- Every cycle's peak MVRV Z-score has been lower than the last; the 2025 top never reached the classic "red zone", so waiting for it would have meant missing the exit.
- SOPR holding above 1 on dips confirms a bull market; failing to clear 1 on rallies confirms a bear.
- Puell Multiple and reserve risk are better at bottoms than tops.
- LTH supply turning from falling to rising is the earliest reliable sign that a bottom is forming, though not that it has finished.
- As of September 2026, the on-chain picture reads "fair value, mid-cycle, neither euphoric nor capitulated": Z-score around 1, price above STH cost basis (~$70–71K) but below the $83–86K wall of long-term-holder supply.

## Sources

- [Look Into Bitcoin: MVRV Z-Score](https://www.lookintobitcoin.com/charts/mvrv-zscore/)
- [Nakamoto Notes: MVRV Z-Score zones](https://nakamotonotes.com/mvrvz-explanation)
- [Glassnode Week On-Chain, Week 35 2026 "Doubt at the Boundaries"](https://research.glassnode.com/the-week-onchain-week-35-2026/)
- [Glassnode Week On-Chain, Week 34 2026 "Squeeze into Supply"](https://research.glassnode.com/the-week-onchain-week-34-2026/)
- [CoinDesk: Bitcoin long-term holders have returned to accumulation (July 2026)](https://www.coindesk.com/markets/2026/07/02/bitcoin-long-term-holders-have-returned-to-accumulation)
- [Fortune: Price of Bitcoin, September 3, 2026](https://fortune.com/article/price-of-bitcoin-09-03-2026/)
- [AhaSignals MVRV Z-Score methodology page](https://ahasignals.com/current-bitcoin-mvrv-z-score/)
- [Look Into Bitcoin: Puell Multiple](https://www.lookintobitcoin.com/charts/puell-multiple/)
- [Look Into Bitcoin: Reserve Risk](https://www.lookintobitcoin.com/charts/reserve-risk/)
- [Glassnode Studio: LTH Supply](https://studio.glassnode.com/charts/supply.LthSum?a=BTC)
- [Checkonchain charts](https://charts.checkonchain.com/)
