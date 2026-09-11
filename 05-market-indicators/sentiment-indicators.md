# Sentiment Indicators

**In one sentence:** Sentiment indicators measure how fearful or greedy investors are, through what they say (surveys), what they pay for protection (VIX, put/call ratio), and what they do with their money (margin debt, fund-manager cash); they work as *contrarian* signals mainly at extremes, because when everyone is already bullish there is nobody left to buy.

## Why sentiment matters (and why it's contrarian)

Prices are set by the marginal buyer and seller. If a survey shows 60% of investors bullish, most of them have already bought; the pool of future demand is small and the pool of potential sellers is large. The reverse holds at panic lows: when everyone who could sell has sold, even mildly good news pushes prices up. That is why Warren Buffett's line about being "fearful when others are greedy" is not just folk wisdom; it is a statement about supply and demand.

Two cautions before the table. First, sentiment measures are only reliably useful at *extremes*; in the middle 80% of readings they are noise. Second, extremes of *fear* have a much better record as buy signals than extremes of *greed* have as sell signals, because bull markets can stay overbought for months while panics resolve in weeks. (See the behavioral-finance section of this library for why humans are built this way.)

## The indicators

| Indicator | What it measures | Free source | Frequency | Extreme readings | Track record |
|---|---|---|---|---|---|
| **VIX (Cboe Volatility Index)** | Expected annualized volatility of the S&P 500 over the next 30 days, derived from option prices; the "fear gauge" | [Cboe](https://www.cboe.com/tradable-products/vix/); FRED [`VIXCLS`](https://fred.stlouisfed.org/series/VIXCLS) | Real-time | Below 12: complacent. 15–20: normal (long-run average ~19). 20–30: nervous. Above 30: fear. Above 40: panic. Record closes: 80.86 (Nov 2008), 82.69 (Mar 16, 2020); 52.33 (Apr 2025 tariff shock); intraday 65 (Aug 5, 2024). | VIX spikes above 40 have marked or closely preceded every major low since 1990; 12-month forward S&P returns after such spikes have been strongly positive. Low VIX is *not* a good sell signal; it can stay under 15 for years (2004–06, 2017). |
| **Put/call ratio** | Volume of put options ÷ call options traded; puts are bets on or insurance against declines | [Cboe daily statistics](https://www.cboe.com/us/options/market_statistics/daily/); StockCharts `$CPC` (total), `$CPCE` (equity-only) | Daily | Equity-only ratio: below ~0.5 = heavy call buying (greed); above ~1.0 = heavy put buying (fear). Use a 10-day average. | Useful short-term contrarian signal (days to weeks). Distorted since 2022 by huge zero-day (0DTE) option volumes and by index-hedging flows. |
| **AAII Investor Sentiment Survey** | Weekly poll of American Association of Individual Investors members: bullish, neutral, or bearish on stocks for the next six months | [AAII](https://www.aaii.com/sentimentsurvey) | Weekly (Thursday) | Historical averages: 37.5% bull / 31.0% neutral / 31.5% bear. Bulls above 50% or bears below 20% = greedy; bears above 50% or bulls below 25% = fearful. Bull-bear spread beyond ±30 is extreme. | Bearish extremes (bears >50%: Mar 2009, Aug 2010, Sep 2022, Apr 2025) have been followed by above-average 6- and 12-month returns almost every time. Bullish extremes are weaker signals. Small, self-selected sample (a few hundred respondents). |
| **Investors Intelligence Advisors' Sentiment** | Weekly tally of ~100 independent newsletter writers classified bullish, bearish, or expecting a correction; running since 1963 | [Investors Intelligence](https://www.investorsintelligence.com/) (headline free; detail paid); [Yardeni bull/bear ratio](https://www.yardeniquicktakes.com/bull-bear-ratio/) | Weekly (Wednesday) | Bulls above 55–60% = danger zone; bulls below 40% or bears above 35–40% = opportunity. Bull/bear ratio above 3.0 = extreme optimism, below 1.0 = extreme pessimism. | Long history; the bull/bear ratio hit 4+ before the 1987 crash and in early 2018 and 2021. Better as a "raise caution" flag than a precise timing tool. |
| **CNN Fear & Greed Index** | Composite of seven inputs: S&P momentum vs. 125-day average, 52-week highs vs. lows, McClellan volume summation, 5-day put/call, junk-bond spread, VIX vs. 50-day average, stock-vs-bond 20-day returns | [CNN](https://www.cnn.com/markets/fear-and-greed) | Daily | 0–25 extreme fear; 75–100 extreme greed. | Convenient summary; readings under 20 coincided with the 2018, 2020, 2022, and 2025 lows. It is derived from other indicators on this page, so it adds no new information. |
| **BofA Global Fund Manager Survey** | Monthly survey of ~200+ institutional managers on positioning, cash levels, and "most crowded trade" | Free summaries in the press ([Mace News](https://macenews.com/), Axios, Reuters); full report to BofA clients | Monthly (mid-month) | BofA's own rules: average cash below 4.0% = sell signal; above 5.0% = buy signal. Equity allocation above +50% net overweight is extreme. | The cash rule triggered "sell" in early 2018, 2021, and mid-2026 and "buy" in 2020 and late 2022 with reasonable, if imperfect, results. |
| **Margin debt** | Money borrowed from brokers to buy stocks; FINRA aggregates monthly | [FINRA margin statistics](https://www.finra.org/investors/learn-to-invest/advanced-investing/margin-statistics); [Advisor Perspectives](https://www.advisorperspectives.com/dshort/updates) charts | Monthly (~3-week lag) | Watch the year-over-year change more than the level: growth above ~40–50% has coincided with tops (2000, 2007, 2021). | Peaks preceded the March 2000, October 2007, and December 2021 tops by 0–3 months; but there are too few episodes to call it reliable, and the indicator lags. Record $1.4–1.5 trillion in mid-2026, up ~39% year-over-year. |
| **NAAIM Exposure Index** | Average equity exposure reported by active managers | [NAAIM](https://www.naaim.org/programs/naaim-exposure-index/) | Weekly | Below 30 = fearful; above 90–100 = fully invested/greedy. | Useful at extremes; small sample. |
| **Consumer sentiment (UMich)** | Household mood, covered in the macro file | FRED `UMCSENT` | Monthly | Below 60 is rare and historically bullish for stocks over 12 months. | Readings under 60 (1980, 2008, 2011, 2022) were followed by strong forward returns. |

## Current readings (as of September 11, 2026)

- **VIX:** ~16.5 (September 9), in the calm-to-normal band despite $100 oil and a possible Fed hike.
- **AAII:** 38.0% bullish, 22.7% neutral, 39.3% bearish (week ending September 9); spread −1.3, near neutral, with an unusually low neutral share (investors are polarized, not undecided).
- **Margin debt:** ~$1.4 trillion (July), down 5.7% on the month but up ~39% year-over-year; nominal record set in May–June.
- **Fund managers:** BofA's survey generated a contrarian "sell" signal in mid-2026 on low cash and heavy equity overweights, per press summaries.
- **Valuation context:** Sentiment is neutral-ish while valuation is extreme, which is a less dangerous combination than "extreme greed plus extreme valuation" (early 2000, late 2021) but hardly a green light.

## Reading them together

Sentiment gauges fall into three families, and you want agreement across families before acting:

1. **What people say** (AAII, Investors Intelligence, UMich, FMS positioning): cheap, frequent, but respondents' words and money often diverge.
2. **What people pay for protection** (VIX, put/call, junk spreads): harder to fake, but distorted by option-market structure.
3. **What people have already done** (margin debt, fund-manager cash, NAAIM exposure, fund flows): the most reliable, but lagging.

A genuine panic low shows all three: bears above 50%, VIX above 35–40, and forced deleveraging (margin debt falling sharply). March 2009, March 2020, October 2022, and April 2025 all fit. A genuine euphoric top is harder to spot because it can persist; the best combined tells have been Investors Intelligence bulls above 60%, FMS cash below 4%, margin debt growth above 40% year-over-year, and VIX below 13 *all at once*, which happened in January 2018 and late 2021.

## How to use it

1. **Only act at extremes.** Define them in advance (for example: AAII bears above 50%, VIX above 35, CNN under 20 for fear; Investors Intelligence bulls above 60%, FMS cash under 4% for greed). Ignore everything in between.
2. **Fear extremes are for buying, gradually.** When several fear gauges hit extremes, add to equities in tranches over a few weeks; do not try to catch the exact bottom.
3. **Greed extremes are for trimming, not shorting.** Reduce leverage, rebalance to targets, and stop adding; overbought markets can stay overbought for a long time.
4. **Check the structure of the reading.** A low VIX with rising credit spreads or falling breadth is more dangerous than a low VIX with everything else healthy.
5. **Don't fight fundamentals with sentiment.** Sentiment tells you how far a move may have run, not whether the underlying story (earnings, Fed) is right.

## Key takeaways

- Sentiment is a contrarian indicator that works at extremes and is noise in the middle.
- Extreme fear (VIX above 40, AAII bears above 50%) has a strong record as a 6–12-month buy signal; extreme greed is a weaker, slower sell signal.
- The VIX is a *level* of expected volatility, not a direction; a VIX of 20 implies roughly a ±5.8% one-month, ±20% one-year expected range.
- Put/call ratios are distorted by zero-day options; use multi-day averages and the equity-only series.
- Margin debt peaks have coincided with major tops but there are too few cases to lean on; watch the growth rate.
- BofA's fund-manager cash rule (below 4% sell, above 5% buy) is a simple, decent institutional-positioning gauge available free through press coverage.
- As of September 2026, retail and option-market sentiment are neutral while institutional positioning is stretched and margin debt is at a record: mixed, with the "money already spent" family the most worrying.

## Sources

- [Cboe VIX](https://www.cboe.com/tradable-products/vix/)
- [MacroRadar: VIX current level and history](https://www.macroradar.io/vix)
- [FRED: VIXCLS](https://fred.stlouisfed.org/series/VIXCLS)
- [Cboe daily options market statistics](https://www.cboe.com/us/options/market_statistics/daily/)
- [AAII Investor Sentiment Survey](https://www.aaii.com/sentimentsurvey)
- [AAII past results](https://www.aaii.com/sentimentsurvey/sent_results)
- [Investors Intelligence](https://www.investorsintelligence.com/)
- [Yardeni: Bull/Bear Ratio](https://www.yardeniquicktakes.com/bull-bear-ratio/)
- [CNN Fear & Greed Index](https://www.cnn.com/markets/fear-and-greed)
- [Advisor Perspectives: Margin debt, June 2026](https://www.advisorperspectives.com/dshort/updates/2026/06/24/margin-debt-finra)
- [FINRA margin statistics](https://www.finra.org/investors/learn-to-invest/advanced-investing/margin-statistics)
- [Mace News: BofA Fund Manager Survey coverage](https://macenews.com/bofa-global-research-fund-manager-survey-fund-managers-reduce-cash-holdings-move-into-stocks-and-bonds-in-july/)
- [Axios: Fund managers all in on stocks (May 2026)](https://www.axios.com/2026/05/20/fund-managers-stocks-bofa)
- [NAAIM Exposure Index](https://www.naaim.org/programs/naaim-exposure-index/)
