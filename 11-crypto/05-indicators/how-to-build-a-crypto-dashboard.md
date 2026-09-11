# How to Build a Crypto Dashboard

**In one sentence:** A useful crypto dashboard is 12 to 15 free indicators checked once a week, each with a pre-agreed normal, caution and alarm zone, combined into a simple regime label that tells you whether to be adding, holding or reducing, and it works only if you write the zones down before you look at the data.

## Design principles

1. **Cover four questions, not one.** Is the market cheap or expensive (valuation)? Is money coming in or leaving (flows)? Is positioning stretched (derivatives)? Is the macro tide rising or falling (liquidity)? Any one category alone will fool you; the combination rarely does.
2. **Weekly, not daily.** Daily checking turns investors into traders. Every indicator below is fine on a weekly cadence, and most are better smoothed.
3. **Zones before data.** Decide what counts as normal, caution and alarm in advance. Otherwise you will rationalize whatever you see.
4. **Count, don't weight.** Weighted composite scores create false precision. Count how many indicators are in each zone and let the majority set the regime.
5. **Expect disagreement.** The most informative weeks are the ones where valuation says cheap and flows say leaving. Disagreement is a signal to wait, not to pick a side.

## The weekly checklist (14 indicators)

Zones are calibrated to the ETF era (2024 onward) where historical thresholds have compressed. "Alarm-high" means overheated; "alarm-low" means capitulation. Both are actionable, in opposite directions.

| # | Indicator | Free source | Normal | Caution | Alarm |
|---|---|---|---|---|---|
| **Valuation** | | | | | |
| 1 | MVRV Z-score | [lookintobitcoin.com](https://www.lookintobitcoin.com/charts/mvrv-zscore/) | 0.5 to 2.5 | 2.5 to 4, or 0 to 0.5 | Above 4 (high) / below 0 (low) |
| 2 | Price vs realized price and STH cost basis | [Glassnode Studio](https://studio.glassnode.com/charts/btc-sth-realized-price-mvrv?a=BTC) | Above both, STH basis acting as support | Below STH basis, above realized | Below realized price (low; historically a buying zone) |
| 3 | NUPL | [lookintobitcoin.com](https://www.lookintobitcoin.com/charts/relative-unrealized-profit--loss/) | 0.25 to 0.5 | 0.5 to 0.65, or 0 to 0.25 | Above 0.65 (high) / below 0 (low) |
| 4 | Long-term holder supply, 30-day change | [Glassnode Studio](https://studio.glassnode.com/charts/supply.LthSum?a=BTC) | Flat or rising | Falling while price rises (distribution) | Falling fast at stretched valuation (high) |
| **Flows** | | | | | |
| 5 | Spot ETF net flows, 30-day sum | [Farside](https://farside.co.uk/btc/) | -$1B to +$3B | -$1B to -$3B, or sustained > +$4B | Below -$3B with price still high (high-risk divergence) |
| 6 | Stablecoin supply, 30-day change | [DefiLlama](https://defillama.com/stablecoins) | +0.5% to +3% | Flat to slightly negative | Below -2% (low) / above +5% in a month (froth) |
| 7 | Exchange netflow, weekly | [CryptoQuant](https://cryptoquant.com/asset/btc/chart/exchange-flows/exchange-netflow-total) | Small net outflow | Single-day inflow > 30K BTC | Repeated large inflows during a rally (high) |
| **Derivatives** | | | | | |
| 8 | BTC funding rate, 7-day avg, annualized | [Coinglass](https://www.coinglass.com/FundingRate/BTC) | 0 to 15% | 15 to 40%, or 0 to -10% | Above 40% (high) / below -10% (low) |
| 9 | Open interest in BTC terms, vs 90-day range | [Coinglass](https://www.coinglass.com/open-interest/BTC) | Mid-range | At 90-day high | Record high with high funding (high) |
| 10 | DVOL (30-day implied vol) and 25-delta skew | [TradingView DVOL](https://www.tradingview.com/symbols/DVOL/), [Deribit metrics](https://metrics.deribit.com/) | DVOL 45 to 65, skew within ±5 | DVOL under 40 (complacent) or 65 to 80 | DVOL above 80, or skew beyond ±10 |
| **Macro** | | | | | |
| 11 | 10-year TIPS real yield, direction over 3 months | [FRED DFII10](https://fred.stlouisfed.org/series/DFII10) | Falling or below 1.5% | Rising, 1.5 to 2% | Rising above 2% (headwind) |
| 12 | DXY, direction over 3 months | [TradingView DXY](https://www.tradingview.com/symbols/TVC-DXY/) | Falling | Flat | Rising sharply (headwind) |
| 13 | Fed path, next-meeting probability | [CME FedWatch](https://www.cmegroup.com/markets/interest-rates/cme-fedwatch-tool.html) | Cuts priced | Hold | Hikes priced |
| **Sentiment** | | | | | |
| 14 | Fear & Greed index, weekly avg | [alternative.me](https://alternative.me/crypto/fear-and-greed-index/) | 30 to 70 | 20 to 30 or 70 to 80 | Above 80 (high) / below 20 (low) |

Optional 15th: Google Trends for "bitcoin" on the 5-year view ([link](https://trends.google.com/trends/explore?date=today%205-y&q=bitcoin)); normal under 25, caution 25 to 50, alarm above 50. It rarely moves, which is exactly why it is worth a glance.

## Scoring and the regime framework

Each week, tally three numbers: how many indicators sit in "alarm-high", how many in "alarm-low", and how many in "caution". Then apply the regime table. The thresholds are deliberately blunt.

| Regime | Definition | Plain-language meaning | Default posture |
|---|---|---|---|
| **Accumulation** | 3+ alarm-low, 0 alarm-high, price below realized price or 200-week MA | Everyone who was going to sell has sold; assets are cheap and hated | Add on a schedule (weekly or monthly buys); expect further drawdown |
| **Recovery** | 0 to 1 alarm-high, few alarm-low, price above STH cost basis, ETF 30-day flows positive, LTH supply flat/rising | The market has a floor and demand is returning, but conviction is thin | Hold core; add on dips to STH cost basis; no leverage |
| **Expansion** | 0 to 2 alarm-high, valuation in caution, flows strongly positive, funding elevated but not extreme | The trend is up and getting crowded; returns are still positive but risk/reward is shrinking | Hold; stop adding; pre-plan trim levels |
| **Euphoria** | 3+ alarm-high (valuation, sentiment, derivatives all stretched), retail signals firing | Everyone is at the party; the next big move is probably down | Trim to a size you can hold through a 60% fall; no new buys |
| **Distribution/Decline** | Valuation falling from caution to normal, ETF 30-day flows negative while price still elevated, LTH supply falling, funding flipping negative | Smart money is leaving; the trend has turned before most people notice | Reduce; wait for accumulation signals before re-adding |
| **Mixed** | Valuation and flows disagree | Signals conflict; the market is in transition | Do nothing new; re-check next week |

The regimes are not a trading system. They are a way to keep your posture consistent with the evidence and to stop you from adding at the top or panic-selling at the bottom, which is where most of the damage is done.

## Worked example: week of September 7–11, 2026

Readings below use the sources cited across this section; where a value is approximate (marked ~) it was estimated from published figures rather than read directly.

| # | Indicator | Reading, as of September 2026 | Zone |
|---|---|---|---|
| 1 | MVRV Z-score | ~1 (Bitcoin ~$78,000 vs realized price in the low-to-mid $50,000s; a tracker printed 0.42 on August 8 at ~$64,000) | Normal |
| 2 | Price vs cost bases | Above realized price; above STH cost basis (~$70–71K); below the $83–86K long-term-holder supply band | Normal |
| 3 | NUPL | ~0.3 (68% of supply in profit per Glassnode) | Normal |
| 4 | LTH supply | Net accumulation of 50–100K BTC per Glassnode (July), but 1K–10K BTC whales shed ~50K BTC since June 30 | Caution (mixed cohorts) |
| 5 | ETF 30-day flows | About +$4.5B (August +$3.52B, first week of September +$0.99B) | Caution (unusually strong after 7 months of outflows; watch for reversal) |
| 6 | Stablecoin supply | ~$303–305B, flat over 30 days (USDT +0.2%, USDC +3.1%) | Caution (no new on-chain dollars behind the rally) |
| 7 | Exchange netflow | Net outflows; custody wallets absorbing coins; no large inflow spikes reported | Normal |
| 8 | Funding | Near neutral through the August squeeze | Normal |
| 9 | Open interest | Fell 11% in coin terms during the squeeze; Binance carries ~$3B long vs ~$1.8B short liquidation leverage | Normal |
| 10 | DVOL and skew | Mid-range; $14B September 25 expiry with max pain $69–70K, dealer gamma flip ~$82.3K | Normal, with event risk |
| 11 | Real yields | 10-year nominal at 4.8% (cycle high); real yield above 2% and rising | Alarm (headwind) |
| 12 | DXY | ~99, weaker than late July | Normal (mild tailwind) |
| 13 | Fed path | 3.50–3.75% held since December 2025; a hike to 3.75–4.00% priced as more likely for September 16 after hawkish Jackson Hole remarks | Alarm (headwind) |
| 14 | Fear & Greed | 56 on September 11 (69 the day before, 74 a week earlier, 27 a month earlier) | Normal |
| 15 | Google Trends | Subdued, far below 2021 levels | Normal |

**Tally:** 0 alarm-high (crypto-native), 2 alarm (macro headwinds), 3 caution, 10 normal.

**Regime:** Recovery, leaning Mixed. Crypto-native data describe a market that is fairly valued, has reclaimed its short-term cost basis, and is being bought by ETFs and sold by whales, with no leverage excess. The macro data describe the most restrictive rate backdrop of the ETF era, with a possible hike days away. The August rally was a short squeeze into ETF demand, not a liquidity-driven advance, and stablecoin supply did not grow to support it.

**Posture implied by the framework:** hold a core position; do not chase into the $83–86K supply band; treat a pullback toward the STH cost basis (~$70K) as the place to add; treat a daily close above roughly $83–86K with positive 30-day ETF flows and rising stablecoin supply as confirmation of Expansion; treat ETF flows turning negative for two consecutive weeks as the trigger to reduce. Key dated event: the September 16 FOMC decision.

**What would change the regime.** Up: Fed holds, real yields fall, stablecoin supply grows 2%+ in a month, price clears the supply band. Down: Fed hikes, ETF 30-day flows flip negative, price loses the STH cost basis and funding goes negative for a week.

## Building it in practice

- **Simplest version:** a note or spreadsheet with 15 rows, the free link, this week's reading and its zone. Fifteen minutes on a Sunday.
- **Spreadsheet version:** Google Sheets with `IMPORTDATA` pulling the alternative.me API (`https://api.alternative.me/fng/?limit=30`) and FRED CSV links (append `/downloaddata` style or use `IMPORTHTML` on FRED series pages); paste Farside and Coinglass numbers by hand.
- **Dashboard version:** a free TradingView layout with BTC weekly, DVOL, DXY and the 200-week MA; a browser bookmark folder with the 14 links opened as a group each week.
- **What not to build:** a real-time feed. It will make you trade.

## How to use it

1. Same day every week, fill in all 14 (or 15) rows before forming an opinion.
2. Tally alarms and cautions; assign the regime from the table.
3. Compare to last week's regime. A regime change is the only event that should change your posture.
4. Pre-write your action for each regime (e.g., "Accumulation: buy X per week"; "Euphoria: sell Y% of holdings") and follow it.
5. Revisit the zone thresholds once a year, because they compress as the market matures; do not revise them mid-cycle to fit what you want to do.
6. Keep a one-line log of each week's regime; over a cycle it becomes your own track record of what worked.

## Key takeaways

- Fourteen free indicators across valuation, flows, derivatives, macro and sentiment are enough; more adds noise.
- Set normal, caution and alarm zones before looking at data, and count zone hits rather than computing a weighted score.
- Six regimes (Accumulation, Recovery, Expansion, Euphoria, Distribution, Mixed) map to five simple postures; only a regime change should change what you do.
- Disagreement between valuation and flows is a "wait" signal, not a puzzle to solve.
- As of September 2026 the dashboard reads Recovery leaning Mixed: fair valuation, neutral leverage, strong ETF inflows, flat stablecoins, and a restrictive macro backdrop with a Fed decision on September 16.
- The next confirmations to watch are the $83–86K supply band, ETF 30-day flows, stablecoin growth and the direction of real yields.
- Weekly cadence and pre-written actions are the whole edge; the indicators are widely known, the discipline is not.

## Sources

- [Look Into Bitcoin: MVRV Z-Score](https://www.lookintobitcoin.com/charts/mvrv-zscore/)
- [Glassnode Studio: STH realized price and MVRV](https://studio.glassnode.com/charts/btc-sth-realized-price-mvrv?a=BTC)
- [Glassnode Week On-Chain, Week 34 2026](https://research.glassnode.com/the-week-onchain-week-34-2026/)
- [Glassnode Week On-Chain, Week 35 2026](https://research.glassnode.com/the-week-onchain-week-35-2026/)
- [Farside Investors: Bitcoin ETF flows](https://farside.co.uk/btc/)
- [HedgeCo: ETF flows for the week ending September 4, 2026](https://hedgeco.net/news/09/2026/spot-bitcoin-etfs-drew-about-987-million-for-the-week-ending-september-4.html)
- [Yahoo Finance: Bitcoin price prediction for September 2026](https://finance.yahoo.com/markets/crypto/articles/bitcoin-price-prediction-september-2026-080209568.html)
- [Stablecoin Beat tracker](https://stablecoinbeat.com/tracker/)
- [DefiLlama stablecoins](https://defillama.com/stablecoins)
- [Coinglass BTC funding](https://www.coinglass.com/FundingRate/BTC)
- [Coinglass BTC open interest](https://www.coinglass.com/open-interest/BTC)
- [TradingView: DVOL](https://www.tradingview.com/symbols/DVOL/)
- [FRED: 10-year TIPS yield](https://fred.stlouisfed.org/series/DFII10)
- [Cambridge Currencies: Fed decision preview, September 16, 2026](https://cambridgecurrencies.com/next-federal-reserve-interest-rate-decision/)
- [alternative.me Fear & Greed Index](https://alternative.me/crypto/fear-and-greed-index/)
- [CME FedWatch](https://www.cmegroup.com/markets/interest-rates/cme-fedwatch-tool.html)
