# Yield Curve and Recession Indicators

**In one sentence:** A handful of indicators (the slope of the Treasury yield curve, the Sahm unemployment rule, the New York Fed's recession-probability model, the Conference Board's LEI, and corporate credit spreads) have historically flagged recessions months in advance; they are worth watching because recessions cause most big bear markets, but each has now produced at least one false alarm, so they are best read as a panel, not as individual oracles.

## The yield curve: what it is and why it predicts

The "yield curve" is a plot of Treasury yields against maturity. Normally it slopes upward: lenders demand more to tie up money for 10 years than for 3 months. When short-term yields rise *above* long-term yields, the curve is "inverted." Two spreads are watched: the **10-year minus 2-year** (the one traders quote) and the **10-year minus 3-month** (the one academics and the New York Fed prefer, because the 3-month bill most directly reflects current Fed policy).

Why would inversion predict recession? Three overlapping explanations:

1. **It reflects the Fed being tight.** The short end is set by the Fed; the long end reflects where markets think rates will settle. Inversion means the market expects the Fed to have to cut, which usually happens because the economy weakens.
2. **It squeezes bank lending.** Banks borrow short and lend long. When that spread vanishes, lending becomes unprofitable and credit contracts.
3. **It is partly self-fulfilling.** Because everyone knows the signal, inversions tighten financial conditions on their own.

Campbell Harvey's 1986 dissertation first documented the 10y–3m relationship; Estrella and Mishkin's work at the New York Fed in the 1990s turned it into the probit model the Fed still publishes.

## The inversion track record

Using the 10-year/3-month spread (monthly averages), inversions and the recessions that followed:

| Inversion began | Recession began (NBER) | Lag | Notes |
|---|---|---|---|
| Dec 1968 | Dec 1969 | ~12 months | |
| Jun 1973 | Nov 1973 | ~5 months | Oil-shock recession |
| Nov 1978 | Jan 1980 | ~14 months | |
| Oct 1980 | Jul 1981 | ~9 months | Double-dip; Volcker tightening |
| Jun 1989 | Jul 1990 | ~13 months | |
| Jul 2000 | Mar 2001 | ~8 months | Dot-com bust |
| Aug 2006 | Dec 2007 | ~16 months | Longest lead before GFC |
| Mar / May 2019 | Feb 2020 | ~9–11 months | Recession triggered by COVID; the signal was arguably lucky |
| Oct 2022 (10y–3m); Jul 2022 (10y–2y) | None as of Sep 2026 | — | Longest and deepest inversion in over 40 years (10y–2y bottomed near −1.08% in July 2023; 10y–3m near −1.9% in mid-2023); un-inverted in late 2024 with no recession following |

One well-known false positive predates the table: a brief 1966 inversion was followed by a slowdown but no NBER recession. The 1998 inversion (Russia/LTCM) was also shallow and brief with no recession.

Score since the late 1960s: 8 recessions, all preceded by inversion; 2 or 3 inversions without a recession (1966, 1998, 2022–24). That is an excellent but no longer perfect record, and two details matter:

- **The lag is long and variable** (5 to 16 months to the recession's start; often longer to the stock-market low). Selling stocks at inversion has historically meant missing substantial gains: the S&P 500 rose roughly 20% between the August 2006 inversion and its October 2007 peak.
- **Recessions tend to begin after the curve *re-steepens*,** as the Fed starts cutting the short end. A steepening driven by falling short rates ("bull steepener") is the late-cycle warning; a steepening driven by rising long rates ("bear steepener," which is what happened in 2024–26) is a different animal.

**Current reading (September 9, 2026, Treasury par yields):** 10y–2y spread about +0.40 percentage points (10-year 4.83%, 2-year 4.43%); 10y–3m about +0.9 point (3-month bill about 3.95%, sitting *above* the 3.50–3.75% policy range because markets are pricing a hike). Not inverted. (The 10-year closed August at 4.73% and jumped to 4.95% on September 10.)

## The other recession indicators

| Indicator | What it measures | Free source | Frequency | How to read it | Track record |
|---|---|---|---|---|---|
| **10y–2y spread** | Long minus medium Treasury yield | FRED [`T10Y2Y`](https://fred.stlouisfed.org/series/T10Y2Y) | Daily | Below zero = inverted. | See table above. |
| **10y–3m spread** | Long minus policy-linked short yield | FRED [`T10Y3M`](https://fred.stlouisfed.org/series/T10Y3M) | Daily | Below zero = inverted. Academic favorite. | Same, with 1966/1998/2022 false alarms. |
| **NY Fed recession probability** | Probit model converting the 10y–3m spread into the probability of recession 12 months ahead | [NY Fed](https://www.newyorkfed.org/research/capital_markets/ycfaq) | Monthly | Historically, readings above ~30% have preceded every recession since 1960; peak readings above 40% are rare. | Peaked near 70% in 2023 with no recession; read 13.9% in the September 2026 update (data through August). |
| **Sahm rule** | Three-month average unemployment rate minus its low over the prior 12 months | FRED [`SAHMREALTIME`](https://fred.stlouisfed.org/series/SAHMREALTIME), [`SAHMCURRENT`](https://fred.stlouisfed.org/series/SAHMCURRENT) | Monthly with jobs report | Crossing +0.50 has coincided with the *start* of every recession since 1970; it's a real-time confirmation tool, not a forecast. | First false positive in July 2024 (0.53; peaked 0.57). Claudia Sahm attributed it to a labor-supply surge rather than layoffs. Reads −0.07 for August 2026. |
| **Conference Board LEI** | Composite of 10 leading series | [Conference Board](https://www.conference-board.org/topics/us-leading-indicators) | Monthly | Recession signal when six-month annualized change falls below about −4.3% and most components decline. | Caught every recession since 1960, then flagged one from mid-2022 through 2024 that never came. Six-month change turned positive in mid-2026. |
| **High-yield credit spread** | Extra yield junk bonds pay over Treasuries | FRED [`BAMLH0A0HYM2`](https://fred.stlouisfed.org/series/BAMLH0A0HYM2) | Daily | Above ~5% = stress; above 8% has coincided with every recession. | Excellent coincident/slightly-leading indicator of profit trouble; 2.71% on September 9, 2026, which is close to record tights. |
| **Chauvet-Piger smoothed probability** | Markov-switching model on four coincident series (payrolls, industrial production, real income, real sales) | FRED [`RECPROUSM156N`](https://fred.stlouisfed.org/series/RECPROUSM156N) | Monthly (2-month lag) | Above 50% = recession likely under way. | Nowcast, not forecast; 0.76% as of the September 2026 update. |
| **Initial jobless claims (4-week avg)** | New unemployment filings | FRED [`ICSA`](https://fred.stlouisfed.org/series/ICSA) | Weekly | Sustained rise of 50k+ from cycle low. | Has led every recession; noisy. |

## Why the 2022–24 signals failed (and what that means)

Almost every recession indicator flashed red in 2022–23: the deepest inversion since 1981, LEI down for 20+ months, NY Fed probability near 70%, M2 shrinking, and then the Sahm rule tripping in mid-2024. No recession came. The best explanations:

- **Post-pandemic distortions.** Excess household savings, locked-in 3% mortgages that insulated consumers from rate hikes, and an immigration-driven labor-supply surge that raised unemployment without layoffs.
- **The manufacturing/services split.** Most leading indicators are manufacturing-heavy; the 2022–24 slowdown was concentrated there while services boomed.
- **Fiscal stimulus** (CHIPS, IRA, deficits above 6% of GDP) offset monetary tightening.
- **Term-premium compression.** Years of QE may have suppressed long yields, making inversion easier to trigger than in past decades.

The lesson is not that these indicators are useless; it is that they measure the *conditions* under which recessions usually occur, not the recession itself. When several are elevated, the odds are higher and a defensive tilt is reasonable; but a portfolio built around "the curve inverted, so sell everything" would have missed a 50%+ rally.

## How to use it

1. **Build a panel.** Track the spread, NY Fed probability, Sahm rule, LEI, HY spreads, and claims on one page (the dashboard file shows how). Count how many are flashing.
2. **Weight confirmation over forecast.** Inversion and LEI are forecasts with long lags; the Sahm rule, claims, and credit spreads confirm in real time. The dangerous window is when forecasters have been red for a year *and* the confirmers start turning.
3. **Watch the re-steepening.** Historically the equity damage came after the curve un-inverted via falling short rates. A curve that steepens because long rates rise (like 2024–26) is a different, inflation-driven regime.
4. **Don't act on one signal.** The historical cost of a false positive (missed gains) has been larger than the historical benefit of a true one for most long-term investors. Use signals to adjust risk at the margin (trim leverage, raise cash modestly, favor quality) rather than to go to zero.
5. **Remember what a recession does to stocks.** Median S&P 500 drawdown around recessions since WWII is about 25–30%, and the market bottoms several months before the recession ends. If you see a recession coming, the plan should include *when to buy back*.

## Key takeaways

- Every US recession since the late 1960s was preceded by a 10y–3m inversion, but three inversions (1966, 1998, 2022–24) were not followed by one.
- Lags run 5–16 months to recession and stocks typically rise during the lag; selling at inversion has been costly.
- The Sahm rule is a real-time confirmation tool (unemployment already rising), not a forecast, and it too misfired in 2024.
- The NY Fed model, LEI, and credit spreads each add information; together they are far more useful than any one alone.
- The 2022–24 false alarm was driven by pandemic-era distortions and fiscal stimulus, which suggests the indicators measure vulnerability rather than destiny.
- As of September 2026 the curve is positively sloped (+0.40 on 10y–2y), the Sahm rule is negative, credit spreads are near record tights, and model recession odds are low; the macro risk is inflation and Fed tightening, not an imminent contraction.
- Use these signals to adjust risk at the margin, and always pair a "sell" plan with a "buy back" plan.

## Sources

- [NY Fed: The Yield Curve as a Leading Indicator](https://www.newyorkfed.org/research/capital_markets/ycfaq)
- [FRED: 10-Year minus 2-Year spread (T10Y2Y)](https://fred.stlouisfed.org/series/T10Y2Y)
- [FRED: 10-Year minus 3-Month spread (T10Y3M)](https://fred.stlouisfed.org/series/T10Y3M)
- [FRED: Real-time Sahm Rule (SAHMREALTIME)](https://fred.stlouisfed.org/series/SAHMREALTIME)
- [thetrading.tools: Sahm Rule current reading](https://www.thetrading.tools/sahm-rule)
- [thetrading.tools: Yield curve current reading](https://www.thetrading.tools/yield-curve)
- [EconomicGreenfield: Recession Probability Models, September 2026](https://www.economicgreenfield.com/2026/09/09/recession-probability-models-september-2026/)
- [Conference Board LEI, July 2026](https://www.prnewswire.com/news-releases/the-conference-board-leading-economic-index-lei-for-the-us-edged-up-in-july-302856410.html)
- [Cleveland Fed: Yield Curve and Predicted GDP Growth](https://www.clevelandfed.org/indicators-and-data/yield-curve-and-predicted-gdp-growth)
- [Advisor Perspectives: Treasury Yields Snapshot, Aug 28, 2026](https://www.advisorperspectives.com/dshort/updates/2026/08/28/treasury-yields-snapshot-august-28-2026)
- [govspending.org: High-Yield OAS](https://govspending.org/series/BAMLH0A0HYM2/)
- [FRED: Smoothed US Recession Probabilities (RECPROUSM156N)](https://fred.stlouisfed.org/series/RECPROUSM156N)
