# Trading and Momentum Strategies

**In one sentence:** Crypto has the strongest, best-documented momentum effect of any major asset class, and simple trend rules have historically cut bitcoin's drawdowns somewhat without cutting its returns — but the same market that rewards patient trend-following destroys leveraged retail traders at industrial scale, and most of what circulates as "trading strategy" is folklore.

## What the academic evidence says

**Liu and Tsyvinski, "Risks and Returns of Cryptocurrency" (NBER 2018; *Review of Financial Studies* 2021).** Using bitcoin, ether and XRP data from 2011 to 2018, the authors found that crypto returns had essentially no exposure to the factors that explain stock, currency and commodity returns — no loading on the market, size, value, or macro variables. What did predict returns was *crypto-specific*: a strong time-series momentum effect (a coin that rose over the past week tended to keep rising over the following one to several weeks) and investor attention (Google search volume and Twitter mentions forecast returns). Their momentum results were robust to the sub-periods they tested.

**Liu, Tsyvinski and Wu, "Common Risk Factors in Cryptocurrency" (*Journal of Finance* 2022).** Extending to roughly 1,800 coins, they showed that a three-factor model — crypto market, size (small coins earn more, with more risk), and momentum (past three-week winners beat losers) — explains most of the cross-section of coin returns. The momentum factor's long-short premium was large, on the order of several percent per week in the early sample, though it decays with liquidity and is expensive to trade in small coins.

**Other work** (Grobys and Sapkota; Tzouvanas et al.; multiple time-series momentum studies through 2024) mostly confirms: short-horizon (1–4 week) momentum and longer-horizon (6–12 month) trend both show up in bitcoin and large altcoins, along with the same reversal at very short horizons (days) seen in equities. The effect has weakened as institutions arrived but has not disappeared.

Why would momentum persist in a market this heavily arbitraged? The usual explanations apply with extra force: attention-driven retail flows that chase price, slow diffusion of information about adoption, and the absence of a valuation anchor that would tell anyone the price is "wrong."

## What a 200-day moving average rule actually did

The most common practical implementation is trend-following: hold bitcoin when its price is above its 200-day moving average (the average of the last 200 daily closes), hold cash when below. Paul Tudor Jones popularized the rule for all assets. We tested it on daily bitcoin data with 0.1% per trade in fees, checking the signal daily with a 5% band around the average to reduce whipsaws:

| Period | 200-DMA rule CAGR | Max drawdown | Round-trip trades | Buy & hold CAGR | Buy & hold max drawdown |
|---|---|---|---|---|---|
| 2014–Sep 2026 | 49% | -67% | 31 | 44% | -83% |
| 2017–Sep 2026 | 60% | -67% | 25 | 58% | -83% |
| 2020–Sep 2026 | 40% | -55% | 17 | 43% | -77% |
| 2022–Sep 2026 | 29% | -26% | 9 | 11% | -67% |

Three honest observations. First, returns are roughly a wash — the rule neither reliably beats nor badly lags holding, which matches the broader trend-following literature. Second, it *does* reduce drawdowns, but less than people expect: the 2018 crash began from a parabolic top where the moving average was far below price, so the rule was still long through the first 50% of the decline. Third, the rule looks best in the most recent, choppier period (2022 onward), which is exactly the kind of sample-dependence that should make you cautious. Without the 5% band, daily signals produced 87 trades and a lower return; in a taxable account, each of those is a short-term capital gain at ordinary income rates, which would erase most of the drawdown benefit.

A reasonable conclusion: a slow trend filter is a legitimate tool for someone who *would otherwise panic-sell at the bottom*, because it gets you out mechanically and back in mechanically. It is not a return enhancer.

## The four-year halving cycle: thesis and critics

**The thesis.** Bitcoin's block reward halves roughly every four years (November 2012, July 2016, May 2020, April 2024). Each halving has been followed by a bull market peaking 12–18 months later, then a 75–85% bear market, then accumulation into the next halving. On our data the peaks came 372, 526, 547 and 535 days after the last four halvings — the October 2025 peak arrived on schedule, and the 2026 bear market is the cycle's next act. Cycle believers buy in the year before a halving and sell 12–18 months after it.

**The critics.** Bitwise's Matt Hougan argued in December 2025 that the cycle is dead: each halving's supply effect is half the size of the last (the 2024 halving removed about $10B a year of new supply from a $2T asset, a rounding error against ETF flows); the past bear markets coincided with Fed tightening and leverage blow-ups (Mt. Gox, ICOs, FTX) rather than being caused by the halving; and institutional demand is steadier than retail mania. The counter-evidence in 2026 cuts both ways: the peak's timing fit the pattern perfectly, but the drawdown so far (about 53% peak-to-trough versus 77–93% in prior cycles) and the muted 2025 rally (peak year-over-year gain about 240% versus 1,000%+ in earlier cycles) suggest the amplitude is compressing even if the rhythm is not. With only four observations, nobody can distinguish a real cycle from coincidence with statistical confidence. Treat it as a useful narrative for expectations, not a trading signal.

## The basis trade (cash-and-carry)

Futures on bitcoin usually trade above spot ("contango") because leveraged longs pay for exposure. A cash-and-carry trade buys spot bitcoin (or a spot ETF) and sells the same amount of futures on CME, locking in the difference as the contracts converge at expiry. It is market-neutral: you do not care where bitcoin goes.

As of the latest reading before this was written (August 7, 2026; treat as "as of September 2026" for planning), CME's front-month annualized basis was about 7.9%, the next month 6.3%, and December 5.7%, versus a two-year Treasury at 4.2% — a gross spread of 1.5–3.7 percentage points over the risk-free rate. In the 2024–25 bull market the basis reached 15–20% at times; in bear markets it can compress to zero or go negative. After financing, margin, fees and the operational risk of a futures position being margin-called while the spot leg sits elsewhere, the net edge for a retail investor is thin and sometimes negative. Hedge funds run this at scale with cheap financing; individuals mostly cannot compete, though the perpetual-futures version (collecting funding payments on a hedged position) is the mechanism behind Ethena's sUSDe and is accessible through that product with its own risks.

## Why leverage kills retail

Crypto exchanges offer 20x, 50x, even 100x leverage on perpetual futures. At 20x, a 5% move against you wipes the position; bitcoin moves 5% in a day several times a month and altcoins do it weekly. On October 10, 2025, a tariff announcement triggered the largest liquidation event in crypto history: about $19 billion of leveraged positions were force-closed in a day, roughly 1.6 million accounts were liquidated, total open interest fell from $217B to $123B, and Hyperliquid's open interest dropped 57%. The previous record days (May 2021, ~$10B; the FTX collapse, ~$1B) look small beside it.

Structural reasons retail leverage traders lose:
- **Path dependence.** A position that is right in a month can be liquidated on the way there. Leverage converts a correct thesis into a loss.
- **Funding costs.** Perpetual longs pay funding to shorts in bull markets, often 10–30% annualized, sometimes far more — a constant drag that grows with leverage.
- **Liquidation cascades.** Forced selling hits stops, which forces more selling; exchanges' liquidation engines and thin order books amplify moves in exactly the direction that hurts crowded positions.
- **The house edge.** Fees, spreads, and the fact that exchanges' liquidation engines take a cut of liquidated positions mean the aggregate expected value of leveraged retail trading is negative before any skill.

No published dataset of retail perpetual-futures P&L shows a majority of accounts profitable over a year; broker-disclosure data for retail CFD and forex trading (70–80% of accounts lose money) is the closest comparable, and crypto's higher volatility makes it worse.

## What works versus what is folklore

| Reasonably supported | Folklore or unsupported |
|---|---|
| Slow trend filters (200-day, 20–40 week) reduce drawdowns at similar returns | Chart patterns, Fibonacci levels, "cup and handle" — no out-of-sample evidence |
| Cross-sectional momentum among large, liquid coins (1–4 week formation) | Indicators fitted to the last cycle (stock-to-flow, rainbow charts, "pi cycle top") |
| Buying after extreme drawdowns with a multi-year horizon (see the DCA file) | Trading news and tweets faster than the market |
| Basis/funding capture when spreads are wide, if you have cheap execution | Altcoin "seasons" timed by narrative |
| Position sizing that cannot be liquidated (no leverage, or tiny) | Doubling down on a losing leveraged position |
| Attention/flow signals as documented by Liu–Tsyvinski, used slowly | Day-trading with 10x+ leverage |

## How to actually do it

1. **Decide whether you are trading or investing.** If your goal is a long-term allocation, you probably want the DCA and rebalancing rules in the other files, not this one.
2. **If you use a trend rule, pick one slow filter and write it down** — e.g., "long bitcoin when weekly close is above the 40-week average by more than 5%; cash when below by more than 5%." Evaluate weekly, not daily.
3. **Run it in a tax-advantaged account** (a bitcoin ETF in an IRA) so the 2–5 trades a year are not taxable events.
4. **Backtest with fees and realistic slippage before trusting anything**, and then assume the live result will be worse than the backtest.
5. **Never use leverage above 2x, and preferably none.** If you must trade perpetuals, treat the margin as money already lost.
6. **If you try the basis trade, do it fully hedged on a regulated venue** (spot ETF plus CME futures at a broker that supports both), with margin held in reserve for a 30% adverse move.
7. **Keep a trading journal with P&L after fees and taxes.** Most people who do this quit trading within a year, which is the point.

## Key takeaways

- Peer-reviewed research (Liu–Tsyvinski 2021, Liu–Tsyvinski–Wu 2022) documents real time-series and cross-sectional momentum in crypto, plus predictive power from investor attention; crypto returns are unrelated to stock or macro factors.
- A 200-day moving average rule on bitcoin since 2014 delivered about the same return as buy-and-hold (49% vs 44% CAGR) with a smaller but still severe drawdown (-67% vs -83%); its value is behavioral, not financial, and it fails to protect against crashes from parabolic tops.
- The halving cycle's timing has held for four cycles (peaks 372–547 days after each halving), but its amplitude is shrinking and n=4 proves nothing; Bitwise calls it dead, BitMEX Research and NYDIG say compressed, not dead.
- Cash-and-carry earned ~1.5–3.7 points over Treasuries gross in mid-2026; net of costs it is a professional's trade.
- October 10, 2025 liquidated ~$19B and ~1.6 million accounts in one day. Leverage makes correct theses lose.
- Almost every popular chart indicator is fitted to the past; the things with evidence are slow, boring, and rarely traded.
- In taxable accounts, active trading's tax drag alone can turn a winning backtest into a loss.

## Sources

- [Liu & Tsyvinski, "Risks and Returns of Cryptocurrency," NBER Working Paper 24877](https://www.nber.org/papers/w24877)
- [Liu & Tsyvinski, Review of Financial Studies (2021)](https://academic.oup.com/rfs/article-abstract/34/6/2689/5912024)
- [Liu, Tsyvinski & Wu, "Common Risk Factors in Cryptocurrency," Journal of Finance (2022), SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3379131)
- [CEPR VoxEU: Risks and returns of cryptocurrencies](https://cepr.org/voxeu/columns/risks-and-returns-cryptocurrencies)
- [Bitwise CIO memo: Predictions for 2026 — the four-year cycle is dead](https://experts.bitwiseinvestments.com/cio-memos/bitwise-predictions-for-2026-the-four-year-cycle-is-dead)
- [Spark Research: Is bitcoin's four-year cycle dead? (both sides)](https://www.spark.money/research/bitcoin-four-year-cycle-dead)
- [CryptoSlate: Bitcoin futures carry tops Treasury yield in matched CME check (Aug 2026)](https://cryptoslate.com/bitcoin-futures-carry-treasury-yield-etf-flows/)
- [CME Group: Cryptocurrency basis watch and implied rate tool](https://www.cmegroup.com/markets/cryptocurrencies/cryptocurrency-basis-watch-and-implied-rate-tool.html)
- [CoinGecko: What is October 10th? Crypto's mass liquidation event explained](https://www.coingecko.com/learn/october-10-crypto-crash-explained)
- [CoinDesk Research: Inside crypto's $19 billion liquidation event](https://www.coindesk.com/research/market-spotlight-the-19-billion-liquidation-that-shook-crypto)
- [FTI Consulting: Crypto crash October 2025 — leverage meets liquidity](https://www.fticonsulting.com/insights/articles/crypto-crash-october-2025-leverage-met-liquidity)
- [Blockchain.com market-price data (used for the moving-average and halving-timing calculations)](https://www.blockchain.com/explorer/charts/market-price)
