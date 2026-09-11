# Technical Analysis Fundamentals

**In one sentence:** Technical analysis studies price and volume history to judge supply, demand, and crowd behavior — and while the academic evidence for most indicators as stand-alone money-makers is weak, a handful of concepts (trend, momentum, support/resistance, volume confirmation) are genuinely useful for timing entries and managing risk.

## What technical analysis assumes

Three premises: the price already reflects everything known, prices move in trends more often than chance would predict, and crowd behavior repeats because human psychology does. The first premise is shared with efficient-market theory; the second and third are where technicians and academics argue. Read the "what the evidence says" section before you decide how much weight to give any of this.

## Price and volume: the raw material

- **Price** is plotted as a line (closing prices), bars, or **candlesticks** (open, high, low, close per period; a filled/red body means close below open, hollow/green means close above).
- **Volume** is how many shares traded. Its job is *confirmation*: a price move on heavy volume reflects broad participation; the same move on thin volume is easier to reverse.
- **Timeframe** changes everything. A stock can be in an uptrend on the weekly chart and a downtrend on the hourly. Pick the timeframe that matches your holding period and check one level above it for context.

## Trend

A trend is a sequence of **higher highs and higher lows** (uptrend) or **lower highs and lower lows** (downtrend). Sideways is a range. The oldest rule in the discipline — trade with the trend — is also the one with the most academic support, because it is a restatement of the **momentum effect**: stocks that have gone up over the past 6–12 months tend, on average, to keep going up for a few months more.

**Trendlines** connect successive lows in an uptrend (or highs in a downtrend). A break of a well-tested trendline is a warning, not a verdict.

## Support and resistance

**Support** is a price level where buying has repeatedly appeared; **resistance** is where selling has repeatedly appeared. They form at prior highs/lows, round numbers, and moving averages. Two useful ideas:

- **Role reversal.** Once resistance is broken, it often becomes support (buyers who missed the breakout buy the retest), and vice versa.
- **The more times a level is tested, the weaker it usually gets** — each test absorbs some of the orders sitting there.

Support and resistance are zones, not exact prices. Draw them as bands.

## Moving averages

A **simple moving average (SMA)** is the average close over the last N periods; an **exponential moving average (EMA)** weights recent prices more. They smooth noise and define trend:

- **Price above a rising 200-day SMA** = long-term uptrend. This one filter would have kept an investor out of most of the worst bear-market drawdowns historically, at the cost of some whipsaws.
- **50-day SMA** is the common intermediate-term reference.
- **Golden cross** = 50-day crosses above 200-day (bullish); **death cross** = 50-day crosses below 200-day (bearish). Because both averages lag, these signals arrive late; they confirm trends rather than predict them, and many death crosses occur near lows.

Moving averages work best in trending markets and generate costly false signals in ranges.

## Momentum oscillators

**RSI (Relative Strength Index).** Compares the size of recent gains to recent losses over 14 periods on a 0–100 scale. Traditional reading: above 70 "overbought," below 30 "oversold." In a strong uptrend, RSI can stay above 70 for weeks — overbought is not a sell signal by itself. More reliable uses: **divergence** (price makes a new high but RSI does not, suggesting weakening momentum) and RSI holding above 40–50 during pullbacks in an uptrend.

**MACD (Moving Average Convergence Divergence).** The difference between a 12-period EMA and a 26-period EMA, with a 9-period EMA of that difference as the "signal line," and a histogram of the gap. MACD crossing above the signal line is a bullish momentum signal; below is bearish. Like all moving-average tools, it lags and whipsaws in ranges. Divergences between MACD and price are its more useful application.

**Bollinger Bands.** A 20-period SMA with bands two standard deviations above and below. The bands widen when volatility rises and narrow when it falls. Two uses: a **"squeeze"** (very narrow bands) often precedes a large move in either direction; and touches of the outer band mark statistically stretched prices, though in a trend price can "walk the band" for a long time.

## Volume indicators

- **On-Balance Volume (OBV):** running total that adds volume on up days and subtracts on down days. If price rises but OBV falls, the rally lacks participation.
- **Volume-weighted average price (VWAP):** the average price weighted by volume over a session; institutions use it as an execution benchmark. Price above VWAP = buyers in control that day.
- **Volume on breakouts:** a breakout above resistance on volume 1.5–2× the average is more credible than one on average volume.
- **Accumulation/distribution line** and **Chaikin Money Flow** refine OBV by weighting where the close sits in the day's range.

## What the academic evidence actually says

This is the section most technical analysis guides skip.

**Against:** The efficient-market hypothesis and random-walk literature (Fama, Malkiel) found that simple chart rules could not beat buy-and-hold after costs. Burton Malkiel's *A Random Walk Down Wall Street* remains the standard popular statement of the case.

**For, with caveats:** Brock, Lakonishok, and LeBaron (1992) tested moving-average and trading-range-breakout rules on the Dow Jones Industrial Average from 1897 to 1986 and found buy signals were followed by meaningfully higher returns than sell signals — a result that reopened the academic debate. But Sullivan, Timmermann, and White (1999) re-examined the same rules with a "Reality Check" bootstrap that corrects for **data snooping** (the tendency to find "profitable" rules by testing thousands and reporting the best). The best rule still looked good in the original 1897–1986 sample even after the snooping adjustment, but showed no significant profitability in the ten years out of sample (1987–1996).

**The survey:** Park and Irwin (2007) reviewed 95 modern studies (1988–2004). Fifty-six found positive results, twenty negative, nineteen mixed — but the authors stressed that most studies suffered from data snooping, after-the-fact rule selection, and inadequate treatment of transaction costs and risk, and declined to draw a firm conclusion.

**What survives scrutiny:**
- **Momentum** (buying past 6–12 month winners) is one of the most robust anomalies in finance, documented across countries and asset classes since Jegadeesh and Titman (1993). Trend-following is essentially its practitioner cousin.
- **Trend filters** like the 200-day moving average reduce drawdowns in backtests, though they do not reliably increase returns and cost you in whipsaw years.
- **Short-term reversal** (last month's biggest winners tend to lag next month) is also robust.
- Lo, Mamaysky, and Wang (2000) found that some chart patterns carry statistically detectable information about future return distributions, but that is not the same as being profitable after costs.

**What does not:** Most single indicators (RSI, MACD crossovers, Bollinger touches) used mechanically, and most claims about precise pattern targets. The more specific the rule, the more likely it is a data-snooping artifact.

The honest summary: technical analysis is most defensible as a **risk-management and timing overlay** on decisions made for other reasons, and least defensible as a stand-alone prediction engine.

## How to actually do it

1. Decide your holding period and choose a matching chart timeframe (daily for weeks-to-months, weekly for months-to-years). Look at one timeframe above for context.
2. Identify the trend on the higher timeframe: is price above or below a rising or falling 200-day (or 40-week) average? Are highs and lows rising or falling?
3. Mark the two or three most obvious support and resistance zones from prior swing highs and lows.
4. Add volume and one momentum tool (RSI or MACD). Look for divergences, not overbought/oversold readings.
5. Define the entry (e.g., a pullback to support in an uptrend, or a breakout on above-average volume), the invalidation point (where you are wrong — typically just below support or the breakout level), and the position size such that hitting the invalidation costs no more than a fixed fraction of capital (often 1–2%).
6. Write the plan down before entering. Do not add indicators to justify a trade you already want to make.
7. Review trades monthly: were the signals you used actually predictive for you, after costs?

## Key takeaways

- Trend, support/resistance, and volume confirmation are the core; everything else is derived from them.
- Moving averages define trend and lag by design; golden/death crosses confirm, they do not predict.
- RSI and MACD are most useful for divergence, least useful as mechanical overbought/oversold triggers.
- Bollinger squeezes flag coming volatility, not its direction.
- Volume validates price moves; a breakout on weak volume is suspect.
- Academic evidence: momentum and trend filters are robust; most specific indicator rules are not, and data snooping explains many reported "profits."
- Use technical analysis to time entries and define risk, not as the sole reason to own something.

## Sources

- [StockCharts ChartSchool: Chart Analysis and Technical Indicators](https://chartschool.stockcharts.com/table-of-contents/chart-analysis)
- [Brock, Lakonishok & LeBaron (1992), "Simple Technical Trading Rules and the Stochastic Properties of Stock Returns," Journal of Finance](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1540-6261.1992.tb04681.x)
- [Sullivan, Timmermann & White (1999), "Data-Snooping, Technical Trading Rule Performance, and the Bootstrap," Journal of Finance](https://onlinelibrary.wiley.com/doi/10.1111/0022-1082.00163)
- [Park & Irwin (2007), "What Do We Know About the Profitability of Technical Analysis?" Journal of Economic Surveys](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1467-6419.2007.00519.x)
- [Investopedia: Relative Strength Index (RSI)](https://www.investopedia.com/terms/r/rsi.asp)
- [Investopedia: Moving Average Convergence/Divergence (MACD)](https://www.investopedia.com/terms/m/macd.asp)
- [Investopedia: Bollinger Bands](https://www.investopedia.com/terms/b/bollingerbands.asp)
- [Investopedia: Golden Cross](https://www.investopedia.com/terms/g/goldencross.asp)
