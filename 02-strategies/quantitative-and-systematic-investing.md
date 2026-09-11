# Quantitative and Systematic Investing

**In one sentence:** Replace judgment with tested rules — define exactly what you buy, when, and how much, verify the rule on historical data without fooling yourself, then execute it mechanically — because the evidence says a disciplined mediocre rule beats a brilliant discretionary process that is not followed.

## What "quant" actually means

A quantitative investor turns an investment idea into an algorithm: inputs (prices, fundamentals, news, satellite images, credit-card data), a model that converts inputs into forecasts, and a portfolio rule that converts forecasts into positions and sizes. The human designs and monitors the system; the system makes the trades. "Systematic" is the broader word — it covers everything from a two-line moving-average rule to a machine-learning model on tick data.

The opposite is discretionary investing, where a person weighs the evidence and decides. The quant case against discretion is not that people are stupid but that they are inconsistent: the same analyst, given the same facts on two different days, reaches different conclusions. Rules do not have moods. Decades of research (Paul Meehl in psychology, Daniel Kahneman in economics) show simple statistical models matching or beating expert judgment across fields, mostly because models never get tired, scared, or greedy.

## The famous shops and how they differ

| Firm | Founded | Approach | What it teaches |
|---|---|---|---|
| **Renaissance Technologies** (Jim Simons) | 1982 | Medallion Fund: short-horizon statistical arbitrage across thousands of instruments; signals so faint individually that only massive diversification and leverage make them profitable. Staffed by mathematicians, physicists, and signal-processing engineers, not finance people. Medallion reportedly compounded at ~66% gross (~39% net) from 1988–2018 but is closed to outsiders and capped at ~$10 billion because the edge does not scale. | The best edges are small, numerous, fast, and capacity-constrained. Nothing about Medallion is replicable at home. |
| **AQR** (Cliff Asness) | 1998 | Academic factors — value, momentum, carry, defensive/quality, trend — applied across stocks, bonds, currencies, and commodities at long horizons. Publishes its research. Manages ~$100B+ in mutual funds and institutional accounts. | Slow, well-documented premiums with capacity for large money. The closest thing to "quant for everyone." |
| **Two Sigma** | 2001 | Machine learning and alternative data (web traffic, shipping, sentiment) at medium horizons; heavy technology infrastructure. | Data breadth and engineering as the edge. |
| **D.E. Shaw** | 1988 | Multi-strategy statistical arbitrage; pioneered computational finance on Wall Street. | Same lesson as Renaissance: many uncorrelated small bets. |
| **Dimensional Fund Advisors** | 1981 | Fama-French factors implemented in low-cost, patient-trading funds. | Systematic can mean "index-plus," not high frequency. |

The lesson for a retail investor: the strategies at the top of this table require hundreds of PhDs, millisecond execution, and proprietary data. The strategies at the bottom require an ETF ticker. Retail quants should live near the bottom.

## Backtesting: where most quant ideas die (or should)

A backtest simulates a rule on past data. It is the essential tool and the most abused one. The main ways to fool yourself:

**Overfitting (data mining).** With enough parameters, a rule can be tuned to fit the past perfectly and predict the future not at all. If you test 100 variants of a moving-average rule and pick the best one, its backtest is meaningless — you would expect one of 100 random rules to look great. Signs: many parameters, performance that collapses if a parameter changes slightly, an edge that appears only in one period or one market. Defenses: keep rules simple (fewer than five parameters), require the rule to work across markets and decades, hold out a test period you never touch until the end, and apply Campbell Harvey's rule that a strategy discovered through a search should need a much higher statistical bar (a t-statistic above 3, not 2).

**Survivorship bias.** Testing on today's S&P 500 members ignores the companies that went bankrupt or were delisted along the way. A value screen run on survivors looks brilliant because the cheap stocks that died are missing. Use point-in-time databases that include dead companies (Norgate, CRSP, Sharadar; Portfolio Visualizer's ETF data is survivorship-adjusted for fund-level tests).

**Look-ahead bias.** Using information that was not available at the time. Common versions: using annual earnings on January 1 when they were not reported until March; using restated financials; using index membership that was announced later; using a moving average computed on today's close to trade at today's close. Every input must be lagged to when it was actually knowable.

**Transaction costs and slippage.** A strategy with 300% annual turnover that earns 3% over the market in a frictionless backtest loses money once you charge realistic spreads, commissions, and market impact. Assume at least 0.1%–0.2% per round trip for liquid large caps, 0.5%–1% for small caps, and more for anything illiquid. Then assume you are wrong and double it.

**Regime dependence.** A rule fit on 1982–2021 (a forty-year bond bull market) may not survive rising rates. Check performance in sub-periods: does it work in the 1970s, 2000s, and 2020s separately?

**Post-publication decay.** McLean and Pontiff (2016) found that published anomalies' returns fall by roughly a third after publication and more than half once traded. Assume any edge you read about is smaller than reported.

A sound backtest, then, uses clean point-in-time data, lags all inputs, charges realistic costs, holds out a test period, has few parameters, and shows consistent (not spectacular) results across sub-periods and related markets. If your rule survives all that, you have something worth a small allocation.

## Simple systematic rules a retail investor can run

These are examples with real evidence behind them, low turnover, and no proprietary data. Each is described in more detail elsewhere in this section.

| Rule | Mechanics | Evidence | Effort |
|---|---|---|---|
| **Index + annual rebalance** | Fixed stock/bond weights; rebalance once a year | The baseline every other rule must beat | 1 hour/year |
| **10-month moving average** | Monthly: hold index if above 10-month SMA, else T-bills | Faber 2007; AQR century study | 5 minutes/month |
| **Dual momentum (GEM)** | Monthly: U.S. vs. international vs. bonds by 12-month return | Antonacci; strong to 2013, weak since | 5 minutes/month |
| **Magic Formula** | Annually: buy 20–30 stocks ranked best on combined earnings yield + return on capital; hold one year | Greenblatt; ~13% vs ~8% for the market in a 2016–2025 European out-of-sample test | 2 hours/year |
| **Factor ETF tilt** | Hold AVUV/VTV/QUAL alongside a total-market core; rebalance annually | Fama-French; AQR | 1 hour/year |
| **Dividend-growth screen** | Annually: 10+ years of increases, payout < 60%, yield + growth > 12% | Quality proxy; see dividend file | 2 hours/year |
| **Piotroski F-Score value** | Buy low P/B stocks scoring 8–9 on nine accounting-health checks | Piotroski 2000; ~7% above market in original study | 3 hours/year |
| **Equal-weight rebalancing** | Hold the S&P 500 equal-weighted (RSP) instead of cap-weighted | Structural small/value tilt; outperformed cap-weight 2000–2020, lagged 2021–2025 | 0 |

What all of these have in common: monthly or annual frequency, published rationale, and a track record longer than one market cycle. What none of them has: intraday trading, leverage, or a claim to 30% a year.

## Tools

- **Portfolio Visualizer** (free tier): backtests of asset allocations, timing models, factor regressions. The standard retail tool.
- **Portfolio Charts**: long-horizon analysis of lazy portfolios with visual tools for drawdown and withdrawal rates.
- **Screeners**: Finviz, TradingView, Stock Rover, GuruFocus, and broker screeners for fundamental rules.
- **Python** with `pandas`, `yfinance`, `backtrader`, or `zipline-reloaded` for anyone who wants to build their own. The Kenneth French Data Library provides free factor returns back to 1926.
- **Composer, QuantConnect, Alpaca**: platforms for automating rule execution. Useful, but automation of a bad rule just loses money faster.

## The behavioral trap of systematic investing

Systematic investing removes discretion from *trading* but not from *strategy selection*. The most common failure is not a bad rule but rule-switching: a strategy underperforms for two years, the investor abandons it for whatever worked recently, and repeats. This is discretionary investing with extra steps. The fix is to decide, in writing and before starting, what would constitute genuine failure (e.g., "trailing a static benchmark by more than X over ten years, or a drawdown worse than the backtest's worst by more than Y") and to change nothing until that bar is crossed.

## How to actually do it

1. **Start with the baseline.** A three-fund index portfolio rebalanced annually is a systematic strategy. Anything else must beat it after costs and taxes.
2. **Pick one published rule** from the table above whose logic you can explain in a sentence and whose evidence you have read. Do not invent your own rule until you have run someone else's for a few years.
3. **Backtest it yourself** in Portfolio Visualizer or Python — not to confirm the CAGR but to learn how it behaves: worst drawdown, longest stretch of underperformance, number of trades per year.
4. **Stress it**: shift the start date by a year, change the parameter by 20%, apply it to a different market. If the results change dramatically, the rule is fragile.
5. **Charge realistic costs** and run it in a tax-advantaged account if it trades more than once a year.
6. **Size it as a sleeve**: 10%–30% of the portfolio for anything beyond factor tilts. The point is diversification of *process*, not concentration.
7. **Write the operating manual**: the exact rule, the data source, the day of the month you check, the tickers you use, and the abandonment criterion.
8. **Execute mechanically and log every decision**, including the ones where you overrode the rule (you will; note why, and see if the overrides helped — they usually did not).
9. **Review annually** against the manual, not against the market's mood.

## Key takeaways

- Quantitative investing is rules first, execution second, emotion never; the edge is consistency, not genius.
- Renaissance-style high-frequency edges are real but unreachable; AQR/Dimensional-style factor and trend premiums are reachable through ETFs.
- Backtests lie through overfitting, survivorship bias, look-ahead bias, ignored costs, and regime dependence — defend against each explicitly.
- Published anomalies lose a third to a half of their return after publication; discount everything you read.
- Simple rules with few parameters, monthly or annual frequency, and multi-decade evidence are the retail sweet spot.
- Strategy-switching after underperformance is the most common way systematic investors fail; define the abandonment criterion in advance.
- A rebalanced index portfolio is the systematic strategy to beat, and most alternatives do not.

## Sources

- [The Man Who Solved the Market — Gregory Zuckerman (Renaissance Technologies history), summary at Wikipedia](https://en.wikipedia.org/wiki/Renaissance_Technologies)
- [AQR Insights — research library](https://www.aqr.com/Insights/Research)
- […and the Cross-Section of Expected Returns — Harvey, Liu, Zhu (2016) on the factor zoo and the t > 3 threshold](https://academic.oup.com/rfs/article/29/1/5/1843824)
- [Does Academic Research Destroy Stock Return Predictability? — McLean & Pontiff (2016)](https://onlinelibrary.wiley.com/doi/abs/10.1111/jofi.12365)
- [Backtesting — Investopedia](https://www.investopedia.com/terms/b/backtesting.asp)
- [Survivorship Bias — Investopedia](https://www.investopedia.com/terms/s/survivorshipbias.asp)
- [Look-Ahead Bias — Investopedia](https://www.investopedia.com/terms/l/lookaheadbias.asp)
- [Magic Formula back test (2026 update) — Quant Investing](https://www.quant-investing.com/blog/magic-formula-investment-strategy-back-test)
- [Value Investing: The Use of Historical Financial Statement Information — Piotroski (2000)](https://www.jstor.org/stable/2672906)
- [Kenneth R. French Data Library](https://mba.tuck.dartmouth.edu/pages/faculty/ken.french/data_library.html)
- [Portfolio Visualizer](https://www.portfoliovisualizer.com/)
