# Bitcoin Cycle Indicators

**In one sentence:** Bitcoin's four-year halving cycle has, so far, kept its timing (peaks 12 to 18 months after each halving) while losing its amplitude (each peak a smaller multiple, each trough a shallower drawdown), so the cycle tools below remain useful for "where are we" and increasingly useless for "how high" or "how low".

## The cycle, stated plainly

Every 210,000 blocks (roughly four years) the block subsidy paid to miners halves. Halvings so far: November 28, 2012 (50 to 25 BTC), July 9, 2016 (25 to 12.5), May 11, 2020 (12.5 to 6.25), and April 19–20, 2024 (6.25 to 3.125). The next halving occurs at block 1,050,000; with the chain at block 965,664 on September 6, 2026 and blocks arriving slightly faster than 10 minutes, that projects to roughly April 2028. Live countdowns: [mempool.space](https://mempool.space/), [NiceHash countdown](https://www.nicehash.com/countdown/btc-halving-2028-05-01-00-00), [bitbo halving page](https://bitbo.io/halving/).

The observed pattern across four completed cycles:

| Cycle | Halving | Peak (approx.) | Months halving to peak | Bottom (approx.) | Peak-to-trough |
|---|---|---|---|---|---|
| 1 | Nov 2012 | Nov–Dec 2013, ~$1,150 | ~12 | Jan 2015, ~$170 | ~-85% |
| 2 | Jul 2016 | Dec 17, 2017, ~$19,700 | ~17 | Dec 2018, ~$3,200 | ~-84% |
| 3 | May 2020 | Nov 10, 2021, ~$69,000 | ~18 | Nov 2022, ~$15,500 | ~-77% |
| 4 | Apr 2024 | Oct 6, 2025, ~$126,000 intraday (~$124,800 daily avg) | ~17.5 | Jul 1, 2026, ~$58,500 daily avg (not confirmed as final) | ~-53% so far |

Two things stand out. The timing has been remarkably consistent: the last three peaks all landed 17 to 18 months after the halving. And the magnitudes have shrunk relentlessly: halving-to-peak gains went from roughly 95x (2012–13) to about 30x (2016–17) to about 8x (2020–21) to about 2x (2024–25). Whether the 2026 drawdown stays near 50% (unprecedentedly shallow) or eventually reaches the historical 75%+ is the open question of this cycle.

## Why the halving might matter, and why it might not

The mechanical argument: new supply falls by half overnight, so with constant demand the price must rise. The counter-argument: the halving is known years in advance and should be priced in; daily new supply (about 450 BTC after 2024) is now trivial next to ETF flows that can exceed 10,000 BTC a day; and the four-year rhythm coincided with global liquidity cycles (2013, 2017, 2021 were all easy-money peaks), which may be the real driver. Both camps agree on one empirical fact: the pattern has repeated four times, and a sample of four is not proof of anything.

## 200-week moving average

**What it measures.** The average closing price over the last 200 weeks (almost four years, one full cycle). Because it spans an entire cycle, it acts as a long-term cost-basis proxy and has been the most-watched "floor" line in Bitcoin.

**Where to get it free.** [Look Into Bitcoin 200-week MA heatmap](https://www.lookintobitcoin.com/charts/200-week-moving-average-heatmap/), [Bitbo 200WMA chart](https://charts.bitbo.io/ma-200w/), [blockchain.com heatmap](https://www.blockchain.com/explorer/charts/200w-moving-avg-heatmap), or add a 200-period SMA to a weekly chart on TradingView.

**How to read it.** Through 2015, 2018–19 and March 2020, weekly closes at or slightly below the 200-week MA marked the bottoms. In 2022 the line broke: price spent roughly six months below it and bottomed about 35% under it. It has never been a resistance level in a bull market. The "heatmap" version colors the line by its own rate of change; a low rate of change (blue/purple) has coincided with bottoms.

**As of September 2026.** By a rough calculation from weekly closes (late 2022 near $16,000 up to 2025 near $100,000 and back), the 200-week MA sits at roughly $65,000 (about $62,000–63,000 at the late-June/early-July lows, per Blockchain.com daily data), which matches the $62,000 to $65,000 "support floor" Glassnode described for the summer 2026 lows. Some sites quote a lower figure; check the live chart. Price near $78,000 is above it; the weekly closes of late June 2026 dipped below it and the early-August low retested it.

**Track record.** Excellent as a bottoming zone for three cycles, broken in 2022. Treat it as "cheap zone" rather than a hard floor.

## Pi Cycle Top indicator

**What it measures.** A mechanical signal that fires when the 111-day moving average crosses above two times the 350-day moving average. It was found by curve-fitting (the ratio 350/111 is close to pi, hence the name) and has no economic rationale.

**Where to get it free.** [Look Into Bitcoin Pi Cycle Top](https://www.lookintobitcoin.com/charts/pi-cycle-top-indicator/), [Newhedge Pi Cycle](https://newhedge.io/bitcoin/pi-cycle-top-indicator), [blockchain.com Pi Cycle](https://www.blockchain.com/explorer/charts/pi-cycle-top-indicator).

**How to read it.** The cross fired within days of the April 2013, December 2013, December 2017 and April 2021 tops, an extraordinary record. It then missed the November 2021 all-time high entirely (no cross), fired in March 2024 near $73,000 ahead of only a 20% correction rather than a cycle top, and, as far as the public charts show, did not fire at the October 2025 peak. As of July 2026 the two averages were far apart with no crossover in sight.

**Track record.** Four hits, then one miss, one false positive and one non-fire at a real top. Its credibility rests on data before 2021. It remains worth watching purely because so many traders watch it, which can make it briefly self-fulfilling.

## 2-Year MA Multiplier

**What it measures.** Two lines: the 2-year (about 730-day) moving average and that same average multiplied by five. Price below the 2-year MA has marked accumulation zones; price above 5x has marked sell zones.

**Where to get it free.** [Look Into Bitcoin 2-Year MA Multiplier](https://www.lookintobitcoin.com/charts/bitcoin-investor-tool/), [Bitbo](https://charts.bitbo.io/2-year-ma-multiplier/).

**How to read it.** Price dipped below the 2-year MA in early 2015, late 2018–early 2019, March 2020 and mid-2022 through early 2023, each a good long-term entry. Price touched or exceeded the 5x line in 2013 and 2017; it came close but did not reach it in 2021 and was nowhere near it in 2025. Like every band indicator, the upper band has become unreachable as the asset matured. By a rough calculation the 2-year MA in September 2026 sits in the high $80,000s (it averages the 2025 run near $100,000), which puts price near $78,000 below it, historically an accumulation reading. Verify on the live chart.

**Track record.** The lower band has worked every cycle; the upper band has not been hit since 2017 and may never be again.

## Rainbow chart (with heavy caveats)

**What it measures.** A logarithmic regression line fitted to Bitcoin's entire price history, with colored bands above and below labeled from "basically a fire sale" to "maximum bubble territory".

**Where to get it free.** [blockchaincenter.net Rainbow Chart](https://www.blockchaincenter.net/en/bitcoin-rainbow-chart/), [Bitbo rainbow](https://charts.bitbo.io/rainbow/).

**How to read it, and why to be careful.** The chart is a curve fit with no economic content. It has been re-fitted at least twice (the original 2014 version, a 2017 re-draw and a 2022 "v2") after price broke below the lowest band, which means its historical "accuracy" is partly the result of the bands being redrawn to include the history. Its creators say explicitly that it is not investment advice and was "meant to be fun". Use it only as a reminder of how far price is from a long-run trend, and never as a target. The same criticism applies with more force to the Stock-to-Flow model, which projected a 2021–24 average price of $288,000 and missed by an order of magnitude; it is a cautionary tale about log-fitted models generally.

**Track record.** Not a signal. A sociological indicator: when the rainbow chart is trending on social media, retail is engaged.

## Cycle comparison charts

**What it measures.** Overlays of price indexed to each halving date (or each cycle low), so the current cycle can be compared to previous ones day by day.

**Where to get it free.** [Bitbo cycle repeat chart](https://charts.bitbo.io/cycle-repeat/), [Look Into Bitcoin cycle chart](https://www.lookintobitcoin.com/charts/bitcoin-price-prediction/), Glassnode's cycle-comparison workbench (free tier).

**How to read it.** They are useful for one purpose: seeing whether the current cycle is early, on schedule or late relative to the pattern. Through 2024–25 the cycle-4 line tracked cycles 2 and 3 closely in timing (peak at about 17.5 months post-halving) while sitting far below them in percentage gain. Post-peak, the 2026 path has been shallower than any prior cycle. Never extrapolate the overlay forward; these charts encourage exactly the kind of pattern-matching that failed people who expected a 2025 "super-cycle" to $200,000+.

**Track record.** Descriptive only.

## The diminishing returns debate

The data are unambiguous: each cycle's peak gain has been a fraction of the previous. Three explanations, all partly true:

1. **Law of large numbers.** A $1.5 trillion asset cannot 30x without becoming larger than gold; percentage returns must fall as market cap grows.
2. **Institutionalization.** ETFs, treasury companies and basis traders dampen both directions: they buy dips and sell rips systematically, and arbitrage capital shorts euphoria. Glassnode's shrinking MVRV Z-score peaks (about 10 in 2013, 7.5 in 2021, low single digits in 2025) are the on-chain fingerprint of this.
3. **Liquidity dominance.** If Bitcoin is mostly a liquidity asset (see the macro page), the amplitude of its cycle is set by the amplitude of the global liquidity cycle, not by the halving, and the 2024–25 liquidity backdrop was modest compared with 2020–21.

The investment implication: model future cycles with lower multiples and shallower drawdowns than history, and be aware that lower amplitude also means the "buy the 80% drawdown" playbook may never trigger again. The 2026 low of roughly -52% may be the new shape of a bear market, or the first leg of a deeper one; nobody knows, and any indicator claiming otherwise is extrapolating.

## Did the ETF era break the cycle?

Arguments that it did: the 2025 peak was the weakest post-halving gain ever; altcoin "seasons" that used to follow Bitcoin's peaks were short (Wintermute noted altcoin rallies averaged about 20 days in 2025 versus about 60 historically) and narrow; the drawdown has been half the historical size; retail euphoria signals (Google Trends, app-store rankings) never fired; Bitwise's Matt Hougan and others argued publicly that the four-year cycle was over and 2026 would set new records (as of September 2026 it has not).

Arguments that it did not: the peak arrived 17.5 months after the halving, exactly on the historical schedule; the market still went through a distribution phase (long-term holders selling into ETF demand), a blow-off in leverage (the record October 10, 2025 liquidation), a 50%+ drawdown and a miner squeeze, all textbook; and on-chain valuation metrics still cycled from stretched to fair, just with smaller amplitude.

The balanced read: the cycle's clock still works, its amplitude has been compressed, and the halving itself is a weaker cause than the liquidity cycle it has happened to coincide with. Plan for a cycle in timing, not in magnitude, and expect the next halving (about April 2028) to be a narrative event more than a supply event.

## How to use it

1. Know where you are on the clock: months since the last halving and months until the next. As of September 2026 you are about 29 months after the 2024 halving and about 19 months before the 2028 one, which in every prior cycle was the accumulation phase.
2. Use the 200-week MA and 2-year MA as "cheap zone" markers, not floors; 2022 proved price can spend months below them.
3. Ignore upper bands (5x multiplier, rainbow "bubble", Pi Cycle) as targets; they have not been reached since 2017–21 and probably will not be.
4. Use cycle-comparison overlays to check timing only.
5. Combine cycle position with on-chain valuation (MVRV Z-score, realized price) and flows before acting; the cycle alone tells you the season, not the weather.
6. Model the next cycle with a lower peak multiple and a shallower trough than history, and size positions for the possibility that "shallower" is wrong.

## Key takeaways

- Four completed cycles show consistent timing (peaks 12 to 18 months after halvings, the last three all at 17 to 18) and collapsing amplitude (95x, 30x, 8x, 2x halving-to-peak).
- The next halving is expected around April 2028; September 2026 is about 29 months post-halving, historically the accumulation phase.
- The 200-week MA (roughly $65,000 in September 2026) and 2-year MA have marked every cycle's cheap zone, but 2022 showed price can break well below them.
- Pi Cycle Top nailed four tops through April 2021, then missed the November 2021 and October 2025 peaks and gave a false positive in March 2024.
- The rainbow chart and Stock-to-Flow are curve fits that have been redrawn or have failed; use them for entertainment, not decisions.
- Diminishing returns are real and structural (size, institutionalization, liquidity dependence); plan for smaller peaks and possibly shallower troughs.
- The ETF era compressed the cycle's amplitude but, so far, did not break its clock; the 2026 drawdown (about 52% at the lows) is the shallowest bear market on record if it holds.

## Sources

- [Ryder: Bitcoin Pi Cycle Top, the chart everyone watches in 2026](https://ryder.id/blogs/post/bitcoin-pi-cycle-top-the-chart-everyone-watches-in-2026)
- [Look Into Bitcoin: Pi Cycle Top Indicator](https://www.lookintobitcoin.com/charts/pi-cycle-top-indicator/)
- [Look Into Bitcoin: 200 Week Moving Average Heatmap](https://www.lookintobitcoin.com/charts/200-week-moving-average-heatmap/)
- [Look Into Bitcoin: 2-Year MA Multiplier](https://www.lookintobitcoin.com/charts/bitcoin-investor-tool/)
- [Bitcoin Magazine: Forecasting the cycle peak with the 200-week moving average](https://bitcoinmagazine.com/markets/bitcoin-price-200-week-moving-average)
- [Mudrex: When will Bitcoin bottom? (updated August 2026)](https://mudrex.com/learn/when-will-bitcoin-bottom-prediction/)
- [Cointelegraph / Wintermute: Why Bitcoin's four-year cycle faltered](https://cointelegraph.com/news/crypto-2026-comeback-hinges-three-outcomes-wintermute)
- [Yahoo Finance: Bitwise chief says Bitcoin will break the four-year cycle](https://finance.yahoo.com/news/bitwise-chief-bitcoin-hit-fresh-160657168.html)
- [BeInCrypto: Bitcoin halving cycle 2028, is the four-year pattern dead?](https://beincrypto.com/learn/bitcoin-halving-cycle-2028/)
- [Fortune: Price of Bitcoin, September 3, 2026 (all-time high figure)](https://fortune.com/article/price-of-bitcoin-09-03-2026/)
- [CoinDesk: Bitcoin falls to $63,000 (February 28, 2026)](https://www.coindesk.com/markets/2026/02/28/bitcoin-sets-up-potential-short-squeeze-as-funding-plunges-to-6)
- [Cryptolexicon: September 6, 2026 difficulty retarget at block 965,664](https://cryptolexicon.org/en/blog/bitcoin-difficulty-rise-hashprice-jump-september-2026/)
- [blockchaincenter.net Rainbow Chart](https://www.blockchaincenter.net/en/bitcoin-rainbow-chart/)
