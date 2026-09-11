# Market Breadth Indicators

**In one sentence:** Breadth indicators measure how many stocks are participating in a market move rather than how far the index has gone; because the S&P 500 is weighted by size, a handful of giants can carry it higher while most stocks fall, and that kind of narrow, "unhealthy" advance has preceded most major tops, while broad "thrusts" off a low have preceded most major bull runs.

## Why breadth matters

The S&P 500 is capitalization-weighted. In 2024–26 the ten largest companies made up roughly 35–40% of the index, so it is entirely possible for the index to rise on a day when 300 of its 500 members decline. Breadth indicators strip out that distortion by counting stocks instead of dollars. The logic:

- **Healthy advances are broad.** When most stocks, sectors, and sizes rise together, the move reflects a general improvement in earnings or liquidity and tends to persist.
- **Tops are narrow.** As a bull market ages, leadership concentrates; more and more stocks quietly roll over while the index is held up by a few winners. The advance/decline line peaked in April 1998, two years before the S&P 500's 2000 top; it peaked in June 2007, four months before the October 2007 top.
- **Bottoms are climactic, and recoveries are explosive.** Panic lows see nearly every stock falling; the first weeks off the low see nearly every stock rising, producing "breadth thrust" readings that have almost never occurred outside the start of a major advance.

Breadth is a technical indicator, meaning it is derived from price and volume rather than fundamentals. It is best used to *confirm or question* what the index is telling you, not as a standalone forecasting system.

## The indicators

| Indicator | What it measures | Free source | Frequency | How to read it | Track record |
|---|---|---|---|---|---|
| **Advance/Decline (A/D) line** | Cumulative running total of (advancing stocks − declining stocks) each day, usually on the NYSE | StockCharts [`$NYAD`](https://stockcharts.com/h-sc/ui?s=$NYAD) (cumulative), [`$SPXADP`](https://stockcharts.com/h-sc/ui?s=$SPXADP); WSJ Market Data | Daily | Should make new highs alongside the index. A **negative divergence** (index at new high, A/D line failing to confirm) for several months is the classic warning. | Divergences preceded the 1929, 1972, 1987, 2000, and 2007 tops by 4–24 months. False signals: brief divergences in 2011, 2014, and 2023 resolved without a bear market. Interest-rate-sensitive issues (preferreds, closed-end funds) on the NYSE distort it; the S&P 500-only version is cleaner. |
| **% of stocks above 200-day moving average** | Share of index members trading above their long-term trend line | StockCharts [`$SPXA200R`](https://stockcharts.com/h-sc/ui?s=$SPXA200R) (S&P 500), `$NYA200R` (NYSE); [Barchart](https://www.barchart.com/stocks/momentum) | Daily | Above 80%: strong but stretched. 50–80%: healthy bull. Below 40%: weak. Below 20%: washout (typically near major lows). | Readings under 20% marked the 2008–09, 2011, 2020, and 2022 lows. Readings above 85% have usually been followed by consolidation but not necessarily by declines. |
| **% above 50-day MA** | Same for the short-term trend | StockCharts `$SPXA50R` | Daily | More volatile; below 20% = short-term oversold, above 85% = short-term overbought. | Good for 1–3 month tactical timing; noisy for anything longer. |
| **New highs / new lows** | Number of stocks hitting 52-week highs vs. lows | StockCharts [`$NYHL`](https://stockcharts.com/h-sc/ui?s=$NYHL); WSJ Market Data | Daily | Expanding new highs confirm an uptrend. New lows above ~10% of issues in an uptrend signal rot beneath the surface. The **Hindenburg Omen** flags days with *both* many new highs and many new lows (above ~2.2% each) while the index is rising. | The Hindenburg Omen has flagged before every crash since 1987, but also fires dozens of times with nothing happening; on its own it is close to worthless. New-low expansions are more reliable as warnings. |
| **McClellan Oscillator** | 19-day EMA minus 39-day EMA of net advances (advances − declines); a momentum measure of breadth | StockCharts [`$NYMO`](https://stockcharts.com/h-sc/ui?s=$NYMO); [McClellan Financial](https://www.mcoscillator.com/) | Daily | Zero line = neutral. Above +100 = overbought, below −100 = oversold (ratio-adjusted version). Divergences from price and crosses of zero are the main signals. | Extremely oversold readings (below −100) have been followed by rallies in most cases; the *Summation Index* (running total, `$NYSI`) crossing above zero has a good record of confirming new uptrends. |
| **Equal-weight vs. cap-weight** | Ratio of the equal-weight S&P 500 (RSP) to the cap-weight index (SPY); shows whether the average stock is keeping up with the giants | Any charting site: plot `RSP:SPY`; [Invesco RSP page](https://www.invesco.com/us/financial-products/etfs/product-detail?productId=RSP) | Daily | A falling ratio means narrow leadership. Persistent narrowness (2023–24, 1998–2000) is a caution flag; a turn upward often marks broadening participation. | Ratio hit multi-decade lows in 2024 during the "Magnificent Seven" era; RSP outperformed SPY by ~5 points in early 2026 as leadership broadened. Cap-weight has beaten equal-weight over 10 years, so the ratio is a health check, not a trade by itself. |
| **Zweig Breadth Thrust** | 10-day EMA of advances ÷ (advances + declines) moving from below 0.40 to above 0.615 within 10 trading days | Compute from NYSE A/D data; StockCharts `$NYADV` and `$NYDEC`; [McClellan Financial commentary](https://www.mcoscillator.com/learning_center/weekly_chart/watching_for_a_zweig_breadth_thrust_signal/) | Rare (a few times a decade) | A signal means the market went from broad selling to broad buying in two weeks: the signature of a major low. | 19 signals since WWII per Carson Group; stocks were higher 12 months later every time, averaging roughly +23%, median 6-month gain ~13%. Signals: Mar 2009, Oct 2011, Jan 2019, Mar 2023, Nov 2023, Apr 2025. Sample is small and StockCharts and Zweig's original data differ slightly, so purists dispute a few signals. |
| **Sector and index breadth** | Share of S&P sectors, or of Russell 2000 / Nasdaq stocks, above moving averages | StockCharts `$RUTA200R`, `$NDXA200R` | Daily | Broad rallies lift small caps and cyclicals; if only large-cap tech is above its 200-day, the rally is fragile. | Small-cap confirmation strengthens signals; small-cap failure to confirm (2023–24) can persist for a long time. |

## A note on current conditions (as of September 2026)

After the extreme concentration of 2023–24, participation broadened in 2025–26: equal-weight beat cap-weight in the first half of 2026 as investors questioned AI capital-spending returns, and mid-year readings showed roughly three-quarters of large-cap stocks above their 200-day averages. That is a healthier configuration than late 2024 despite higher valuations. The thing to watch into the September 15–16 FOMC and the $100-oil environment is whether new lows expand while the index holds up; that would be the divergence pattern that matters.

## How to use it

1. **Confirm the trend.** In an uptrend, check monthly that the A/D line and % above 200-day are making highs with the index. If they are, ignore the bears. If the index is making highs alone for three months or more, tighten risk.
2. **Buy thrusts.** A Zweig thrust, or the McClellan Summation Index turning up from deeply negative territory with % above 200-day rising from under 20%, is one of the few technical signals with a strong long-term record. Act on it with a multi-month horizon.
3. **Read washouts as opportunity.** Fewer than 20% of stocks above their 200-day average has marked every major low of the last 20 years. It is a "start buying" signal, not a "the bottom is in" signal.
4. **Use the equal-weight ratio as a health gauge.** Narrow markets are fragile but can stay narrow for a year; use narrowness as a reason to diversify away from the leaders, not as a reason to sell everything.
5. **Ignore the Hindenburg Omen headlines.** It fires far too often to be actionable.
6. **Combine with sentiment.** Breadth thrust plus extreme fear is the highest-conviction buy setup in this library; breadth divergence plus extreme greed is the highest-conviction "reduce risk" setup.

## Key takeaways

- Breadth counts stocks; the index counts dollars. When they disagree for months, the stocks usually win.
- A/D line divergences preceded the 2000 and 2007 tops by months to years but also produce false alarms; use them to tighten risk, not to call tops.
- Fewer than 20% of stocks above their 200-day average has marked every major low of the past two decades.
- The Zweig Breadth Thrust has a near-perfect (if small-sample) 12-month record; it fires only a few times a decade and last fired in April 2025.
- The McClellan Oscillator and Summation Index are the standard tools for breadth momentum; oversold extremes below −100 have reliably preceded bounces.
- The equal-weight/cap-weight ratio is the simplest way to see whether the average stock is participating; participation broadened in 2025–26.
- All of these are free on StockCharts, Barchart, and the WSJ market-data pages; you don't need a paid platform.

## Sources

- [StockCharts ChartSchool: Advance-Decline Line](https://chartschool.stockcharts.com/table-of-contents/technical-indicators-and-overlays/technical-indicators/advance-decline-line)
- [StockCharts ChartSchool: McClellan Oscillator](https://chartschool.stockcharts.com/table-of-contents/technical-indicators-and-overlays/technical-indicators/mcclellan-oscillator)
- [StockCharts ChartSchool: Percent Above Moving Average](https://chartschool.stockcharts.com/table-of-contents/technical-indicators-and-overlays/technical-indicators/percent-above-moving-average)
- [McClellan Financial: Watching for a Zweig Breadth Thrust Signal](https://www.mcoscillator.com/learning_center/weekly_chart/watching_for_a_zweig_breadth_thrust_signal/)
- [Carson Group: Houston, We Have a Zweig Breadth Thrust (April 2025)](https://www.carsongroup.com/insights/blog/houston-we-have-a-zweig-breadth-thrust-and-four-more-bullish-developments/)
- [SentimenTrader: Zweig breadth thrust variation](https://sentimentrader.com/blog/a-variation-of-the-zweig-breadth-thrust-indicator-triggered-an-alert)
- [Kiplinger: RSP vs SPY 20-year returns](https://www.kiplinger.com/investing/etfs/rsp-vs-spy-why-these-sp-500-etfs-have-such-different-20-year-returns)
- [Convextrade: SPY vs RSP 2026 comparison](https://convextrade.com/compare/spy-vs-rsp)
- [History of Market: S&P 500 breadth](https://historyofmarket.com/sp500/sp500-breadth/)
- [WSJ Market Data: Advances and declines](https://www.wsj.com/market-data/stocks/marketsdiary)
- [Barchart: Stocks above moving averages](https://www.barchart.com/stocks/momentum)
