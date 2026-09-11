# Momentum and Trend Following

**In one sentence:** Assets that have been rising tend to keep rising for a while and assets that have been falling tend to keep falling, so a rules-based system that buys recent winners and steps aside from recent losers has historically earned market-like returns with much shallower crashes — at the cost of frequent small losses, lagging in sharp recoveries, and requiring iron discipline to follow.

## Two flavors of momentum

**Cross-sectional (relative) momentum** ranks assets against each other and holds the leaders. "Of these 500 stocks, buy the 50 that rose most over the past 12 months." It says nothing about whether the market as a whole is going up. This is the academic "momentum factor" (Jegadeesh and Titman, 1993) and the basis of ETFs like MTUM. See [factor-investing.md](factor-investing.md).

**Time-series (absolute) momentum**, or trend following, compares an asset to its own past. "Is the S&P 500 above where it was 12 months ago?" or "Is it above its 200-day moving average?" If yes, hold it; if no, hold cash or bonds. This is the basis of managed-futures funds and of most retail "tactical" rules. Its purpose is not to pick winners but to avoid the worst drawdowns.

The two can be combined, and the best-known combination is Gary Antonacci's dual momentum.

## Why it might work

Prices should, in theory, adjust instantly to news. In practice they under-react at first (investors anchor on old prices, information diffuses slowly, institutions build positions gradually) and then over-react (herding, performance chasing). The result is trends that last months, then reverse violently. Risk-based explanations also exist — trend followers get paid for providing liquidity during panics — but the behavioral story is the mainstream one.

## The evidence

- **A century of data.** AQR's "A Century of Evidence on Trend-Following Investing" (Hurst, Ooi, Pedersen, 2017) built a simple time-series momentum strategy across 67 markets (equity indices, bonds, commodities, currencies) from 1880 to the present. It was profitable in every decade, with a Sharpe ratio (return per unit of risk) comparable to or better than equities, and it made money in eight of the ten worst equity drawdowns of the period, including 1929–1932, 1973–1974, 2000–2002, and 2008. This "crisis alpha" is the main reason institutions own it.
- **Moving-average timing.** Meb Faber's 2007 paper "A Quantitative Approach to Tactical Asset Allocation" tested a single rule — hold an asset if it is above its 10-month simple moving average at month-end, otherwise hold cash — across U.S. stocks, foreign stocks, bonds, commodities, and REITs from 1973 onward. Applied to an equal-weight portfolio of those five, the rule delivered roughly equity-like returns with bond-like volatility and drawdowns, cutting the worst decline from about −46% to under −10% (paper figures through 2008; the strategy's edge has narrowed since).
- **Managed futures in 2022.** The year that stocks and bonds fell together, the SG CTA Index (professional trend-following funds) gained roughly 20% (about +20.2% as widely reported), the best calendar year in the index's history going back to 2000 and well ahead of its 2008 gain of about 13% — exactly when the 60/40 portfolio most needed help.
- **Cross-sectional momentum**: 6%–9% annual long-short premium across a century, and present in every major equity market and asset class studied.

## The rules people actually use

| Rule | Mechanics | Signal frequency | Typical result vs. buy-and-hold |
|---|---|---|---|
| **200-day moving average** | Hold the index when price closes above its 200-day (≈10-month) average; move to T-bills when below | Check daily or monthly; monthly reduces whipsaws | Similar long-run return, roughly half the max drawdown, more small losses |
| **12-month absolute momentum** | Hold if the trailing 12-month return exceeds T-bills; else bonds | Monthly | Similar to above; smoother signal |
| **Dual momentum / GEM** (Antonacci) | Monthly: if U.S. stocks' 12-month return > T-bills, hold whichever of U.S. or international stocks has the higher 12-month return; otherwise hold aggregate bonds | Monthly | Backtest 1974–2013: ~17% CAGR vs ~12% for stocks, max drawdown ~−18% vs ~−51% |
| **Faber GTAA** | 10-month SMA applied separately to five asset classes, 20% each | Monthly | Equity-like returns, bond-like drawdowns (1973–2008) |
| **Managed futures / CTA** | Long-short trend signals on 50–150 futures markets, volatility-scaled | Daily | Uncorrelated with stocks; big gains in 2008, 2014, 2022; long flat stretches 2009–2013, 2015–2019 |

Retail access to managed futures: DBMF (iMGP DBi Managed Futures Strategy, ~0.85%), KMLM (KFA Mount Lucas, ~0.90%), CTA (Simplify Managed Futures), and AQR's Managed Futures mutual fund. These typically sit at 5%–15% of a portfolio as a diversifier.

## The drawbacks, which are real

1. **Whipsaws.** In choppy markets the signal flips back and forth, and each flip is a small loss. 2011, 2015–2016, and 2018 were painful years for simple trend rules. The strategy's typical pattern is many small losses punctuated by a large avoided loss.
2. **Lagging recoveries.** Trend rules exit after a decline has started and re-enter after a recovery has started, so they miss the sharpest part of V-shaped rebounds. In March–April 2020 the S&P 500 fell 34% and recovered in five months; most 200-day rules sold near the bottom and re-bought 20% higher.
3. **Post-publication decay.** GEM is the clearest case. Its published backtest (1974–2013) was excellent. An out-of-sample review covering 2014–2026 found GEM returned about 8.4% annualized versus 13.6% for the S&P 500, with a maximum drawdown (−20%) no better than a static 60/40. It still avoided the worst of 2022, but the U.S.-only bull market, two whipsaw-heavy corrections, and a 12-month lookback that kept it in international stocks at the wrong moments cost it dearly. Antonacci's own updated backtest extends the strong results back to 1950, which is genuine evidence, but the live period is the one investors actually experienced.
4. **Taxes.** Every exit in a taxable account is a taxable event; a rule that trades a few times a year converts long-term gains into short-term. Run trend rules in IRAs.
5. **Parameter sensitivity.** 200-day vs. 10-month vs. 12-month vs. 150-day all "work" in backtests, but picking the best one after the fact is data-mining. Corey Hoffstein's research (Newfound) shows that averaging several lookbacks or rebalance dates is more robust than any single choice.
6. **Behavioral difficulty.** Buying back in after a rule says so, at a higher price than you sold, feels terrible. Most people who try trend following abandon it in the first whipsaw. The rule only works if followed every time.

## Momentum crashes (cross-sectional)

Cross-sectional momentum has its own failure mode: after a sharp bear market, the "losers" (which the strategy is short or avoiding) rebound hardest. In 2009 the academic long-short momentum factor lost roughly 80% in a few months as beaten-down financials tripled. Long-only momentum ETFs are far less exposed but still lag badly in reversals (MTUM trailed the S&P 500 significantly in 2020's rebound and again in 2022–2023 as leadership rotated). Momentum should be one tilt among several, not a whole portfolio.

## How to actually do it

For a retail investor who wants trend following as a *risk-management overlay* rather than a full trading system:

1. **Choose the scope.** Apply the rule to one broad index (S&P 500 or total U.S. market via VTI/SPY), not to individual stocks. Individual stocks are too noisy for simple rules.
2. **Choose the rule and write it down.** Recommended: at the last trading day of each month, compare the index close to its 10-month simple moving average (equivalent to the 200-day). Above = hold the index fund; below = hold a short-term Treasury fund (SGOV, BIL, or VGSH). Checking monthly rather than daily cuts whipsaws roughly in half.
3. **Apply it to a portion.** Run the rule on, say, 30%–50% of your equity allocation; leave the rest buy-and-hold. This caps both the tax cost and the regret in either direction.
4. **Use a tax-advantaged account** for the tactical sleeve.
5. **Add a dual-momentum layer only if you want international exposure to rotate**: when in stocks, hold U.S. (VTI) or international (VXUS), whichever has the higher trailing 12-month return. Expect this to lag in U.S.-led bull markets.
6. **Consider managed futures instead** if you want the diversification without running signals yourself: 5%–10% in DBMF, KMLM, or CTA, rebalanced annually. Accept multi-year flat stretches.
7. **Backtest expectations, not returns.** Use Portfolio Visualizer's "Timing Models" tool to see how your rule would have done. Focus on the number of trades per year and worst whipsaw, not the CAGR — the CAGR is the number most likely to be overfit.
8. **Commit for a full cycle** — a bull market, a bear, and a recovery, likely 7–10 years — before judging. Keep a log of every signal and whether you followed it.

## Key takeaways

- Time-series momentum (trend following) reduces crashes; cross-sectional momentum (relative strength) picks winners. They are different tools.
- The 200-day / 10-month moving average rule has cut maximum drawdowns roughly in half over a century of data while keeping long-run returns close to buy-and-hold.
- Trend following's payoff is "crisis alpha": it made money in 2008 and 2022 when almost nothing else did.
- The costs are whipsaws, lagging V-shaped recoveries, and taxes; dual momentum (GEM) trailed the S&P 500 by 5 points a year in 2014–2026 despite a superb backtest.
- Check signals monthly, not daily; average multiple lookbacks; apply to broad indices, not single stocks.
- Run tactical rules in an IRA and on only part of the portfolio.
- The strategy is simple to describe and hard to follow; the discipline is the edge.

## Sources

- [A Century of Evidence on Trend-Following Investing — Hurst, Ooi, Pedersen (AQR, 2017)](https://www.aqr.com/Insights/Research/Journal-Article/A-Century-of-Evidence-on-Trend-Following-Investing)
- [A Quantitative Approach to Tactical Asset Allocation — Meb Faber (SSRN, 2007/2013)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=962461)
- [Extended Backtest of Global Equities Momentum — Gary Antonacci](https://www.optimalmomentum.com/extended-backtest-of-global-equities-momentum/)
- [Dual Momentum out of sample: does GEM still beat buy-and-hold? — Quant for Free (2026)](https://quant4free.com/analysis/dual-momentum/)
- [Fragility Case Study: Dual Momentum GEM — Corey Hoffstein, Newfound Research](https://blog.thinknewfound.com/2019/01/fragility-case-study-dual-momentum-gem/)
- [Time Series Momentum: A Good Time for a Refresh — Alpha Architect](https://alphaarchitect.com/time-series-momentum-aka-trend-following-the-historical-evidence/)
- [Demystifying Managed Futures — AQR (PDF)](https://www.aqr.com/-/media/AQR/Documents/Insights/Journal-Article/Demystifying-Managed-Futures.pdf)
- [Returns to Buying Winners and Selling Losers — Jegadeesh & Titman (1993)](https://onlinelibrary.wiley.com/doi/10.1111/j.1540-6261.1993.tb04702.x)
- [Investopedia: Trend Trading](https://www.investopedia.com/terms/t/trendtrading.asp)
