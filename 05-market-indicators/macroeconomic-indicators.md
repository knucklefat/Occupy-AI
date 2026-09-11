# Macroeconomic Indicators

**In one sentence:** Macroeconomic indicators are the government and private-survey statistics (growth, inflation, jobs, factory activity, spending, housing, confidence) that describe where the economy is and where it might be going; they move markets on release day, but their real value to a long-term investor is in tracking direction and trend, not in reacting to any single number.

## Why these numbers matter to investors

Stock prices are, in the end, a bet on future corporate profits discounted by interest rates. Profits track the economy; interest rates track inflation and the Federal Reserve's response to it. So the handful of statistics below feed both halves of that equation. Each is released on a fixed schedule, is free, and is revised over time (sometimes heavily), which is why traders often care more about the gap between the reported figure and the consensus forecast than about the figure itself.

A useful mental model: some indicators are **leading** (they tend to turn before the economy does: jobless claims, PMI new orders, building permits, consumer expectations), some are **coincident** (they describe the present: payrolls, industrial production, retail sales), and some are **lagging** (they confirm what already happened: unemployment rate, CPI, GDP). Markets themselves are a leading indicator, which is why they often move on data before the data "looks bad."

## The master table

| Indicator | What it measures | Free source | Release cadence | How to read it | Track record / caveats |
|---|---|---|---|---|---|
| **Real GDP** | Total inflation-adjusted output; annualized quarterly growth rate | [BEA](https://www.bea.gov/data/gdp/gross-domestic-product); FRED `GDPC1`, `A191RL1Q225SBEA` | Quarterly; advance estimate ~4 weeks after quarter ends, then two revisions | Trend growth ~1.8–2.0%; two negative quarters is the informal recession shorthand (the official arbiter is the NBER). | Backward-looking and heavily revised; markets rarely move much on it. The Atlanta Fed's [GDPNow](https://www.atlantafed.org/cqer/research/gdpnow) gives a running estimate before release. |
| **CPI (Consumer Price Index)** | Prices paid by urban consumers for a fixed basket; "core" strips food and energy | [BLS CPI](https://www.bls.gov/cpi/); FRED `CPIAUCSL`, `CPILFESL` | Monthly, ~10th–15th, 8:30 a.m. ET | Compare year-over-year to the Fed's 2% goal (which is set on PCE, not CPI); watch core and "supercore" (services ex-shelter) for underlying pressure. | The single most market-moving release of the last five years. Shelter (about a third of the index) lags real-world rents by ~12 months. |
| **PCE price index** | The Fed's preferred inflation gauge; broader basket, weights update as spending shifts | [BEA Personal Income & Outlays](https://www.bea.gov/data/personal-consumption-expenditures-price-index); FRED `PCEPI`, `PCEPILFE` | Monthly, last week of month | Core PCE year-over-year vs. 2% target. Typically runs 0.3–0.5 pts below CPI. | Largely predictable from CPI and PPI, so it moves markets less; matters for Fed rhetoric. |
| **Nonfarm payrolls / unemployment rate** | Jobs added (establishment survey) and jobless rate (household survey) | [BLS Employment Situation](https://www.bls.gov/news.release/empsit.nr0.htm); FRED `PAYEMS`, `UNRATE` | First Friday of the month, 8:30 a.m. ET | Breakeven job growth is roughly 50–100k/month depending on labor-force growth; a rising unemployment rate matters more than the level (see the Sahm rule). | Payroll figures are revised twice, sometimes by 100k+, and get an annual benchmark revision. The unemployment rate is a lagging indicator: it usually rises only after a recession begins. |
| **Initial jobless claims** | New filings for unemployment insurance | [DOL](https://www.dol.gov/ui/data.pdf); FRED `ICSA`, `CCSA` (continuing claims) | Weekly, Thursday 8:30 a.m. ET | Use the 4-week average. Sub-250k is healthy; a sustained rise of ~50k+ from the low has preceded every recession. | The best high-frequency labor indicator; noisy week to week (holidays, weather, strikes). |
| **ISM Manufacturing PMI** | Purchasing managers' survey of factory activity (new orders, production, employment, deliveries, inventories) | [ISM](https://www.ismworld.org/supply-management-news-and-reports/reports/ism-report-on-business/) | First business day of month, 10:00 a.m. ET | 50 = dividing line between expansion and contraction for manufacturing. ISM's August 2026 release states that a PMI above 47.5, sustained over time, generally indicates the overall economy is expanding (the threshold has been restated several times over the years). New Orders and Prices sub-indexes are the most-watched. | Strong leading properties for industrial profits and commodity demand; manufacturing is only ~10% of US GDP, so it can be below 50 for long stretches (all of 2023–24) without a recession. |
| **ISM Services PMI** | Same survey for the service sector (~70%+ of the economy) | [ISM](https://www.ismworld.org/supply-management-news-and-reports/reports/ism-report-on-business/) | Third business day of month, 10:00 a.m. ET | 50 threshold. Business Activity, New Orders, Employment, and Prices Paid sub-indexes. | Shorter history (since 1997) and more volatile than the manufacturing index; the Prices sub-index is a good early inflation warning. |
| **Retail sales** | Dollar value of sales at retailers, food services; "control group" excludes autos, gas, building materials, restaurants | [Census](https://www.census.gov/retail/sales.html); FRED `RSAFS`, `RSXFS` | Monthly, ~mid-month, 8:30 a.m. ET | Consumer spending is ~68% of GDP. Control group feeds directly into GDP estimates. | Nominal (not inflation-adjusted), so high inflation flatters it; heavily revised. |
| **Housing starts and building permits** | New residential construction begun; permits are the leading component | [Census/HUD](https://www.census.gov/construction/nrc/index.html); FRED `HOUST`, `PERMIT` | Monthly, ~17th–19th, 8:30 a.m. ET | Permits lead starts; starts lead broader activity. Housing is small in GDP but highly rate-sensitive, which makes it an early read on monetary policy transmission. | Ed Leamer's famous paper title: "Housing IS the business cycle." Housing downturns preceded 8 of the last 10 recessions. Very weather-sensitive month to month. |
| **Conference Board Consumer Confidence** | Survey of ~3,000 households on current conditions and six-month expectations; weighted toward labor-market perceptions | [Conference Board](https://www.conference-board.org/topics/consumer-confidence) | Last Tuesday of the month, 10:00 a.m. ET | Index (1985=100). The Board flags Expectations below 80 as a level that "often signals a recession ahead." | Correlates with job availability; the "jobs plentiful minus jobs hard to get" spread is a useful sub-indicator. |
| **University of Michigan Consumer Sentiment** | Survey of ~1,000 consumers, weighted toward personal finances and buying conditions; includes inflation expectations | [UMich Surveys of Consumers](https://www.sca.isr.umich.edu/); FRED `UMCSENT`, `MICH` (1-yr expectations) | Preliminary 2nd Friday, final 4th Friday, 10:00 a.m. ET | Index (1966=100). Long-run average ~85. The 1-year and 5-year inflation expectations are what the Fed watches. | Sentiment is a *contrarian* stock indicator: extremely low readings (below ~60) have historically been followed by strong 12-month returns. Since 2022 it has been badly depressed by inflation and has become unusually partisan. |
| **Conference Board Leading Economic Index (LEI)** | Composite of 10 leading series: claims, manufacturing hours, new orders (two series), permits, stock prices, credit index, yield spread, consumer expectations, ISM new orders | [Conference Board](https://www.conference-board.org/topics/us-leading-indicators) | Monthly, ~third week, 10:00 a.m. ET | The Board's recession rule: six-month annualized decline worse than about −4.3% *and* a majority of components falling (the "diffusion" test). | Called every recession since 1960 but produced a persistent false signal in 2022–24 (its six-month growth rate was negative for over four years without a recession). Components are all available separately. |

## Current snapshot (as of September 11, 2026)

- **Jobs:** August payrolls +162,000 (well above the prior 12-month average of ~31,000); unemployment 4.1%; average hourly earnings +3.1% year-over-year.
- **Inflation:** July CPI +3.4% headline, +2.5% core (August CPI due September 11). The Fed's Lisa Cook cited PCE at 3.7% headline and 3.3% core through June. Energy has been the swing factor: WTI crude is back near $100 after the spring's Middle East supply shock.
- **ISM:** Manufacturing 54.6 (eighth straight month of expansion; Prices Paid 71.1). Services 55.4, with Business Activity at 61.7 (best since 2022) but Employment at 47.8 and Prices at 72.6 (highest since August 2022).
- **Confidence:** UMich sentiment 51.7 in August, down 6.3% on the month; 1-year inflation expectations 4.0%, 5-year 3.3%.
- **LEI:** 99.5 in July (+0.2%); six-month growth rate turned positive for the first time in over four years.

Read together: solid activity, stubborn inflation, weak sentiment. That is a "late-cycle" pattern in which the risk is a Fed that has to tighten again (markets were pricing roughly 55–65% odds of a hike at the September 15–16 FOMC) rather than one in which demand is collapsing.

## Release calendar cheat sheet

| Week of month | What lands |
|---|---|
| Week 1 | ISM Manufacturing (day 1), ISM Services (day 3), Jobs report (first Friday), JOLTS |
| Week 2 | CPI (~10th–15th), PPI, UMich preliminary (2nd Friday), NFIB small-business survey |
| Week 3 | Retail sales, industrial production, housing starts/permits, LEI, Philly Fed & Empire manufacturing |
| Week 4 | Durable goods, new/existing home sales, Conference Board confidence (last Tuesday), GDP (quarter-end months), PCE (last week), UMich final |
| Every Thursday | Initial jobless claims, 8:30 a.m. ET |

Bookmark the official calendars: [BLS release schedule](https://www.bls.gov/schedule/news_release/), [BEA release schedule](https://www.bea.gov/news/schedule), [Census economic indicators calendar](https://www.census.gov/economic-indicators/calendar-listview.html), and the [Federal Reserve calendar](https://www.federalreserve.gov/newsevents/calendar.htm).

## How to use it

1. **Watch the trend, not the print.** Use three-month averages for payrolls and claims, and year-over-year rates for prices. A single miss is noise; three consecutive misses in the same direction is information.
2. **Compare to consensus, then to the Fed.** The market reaction depends on the surprise versus economists' forecasts (published on any economic calendar) and on whether the surprise changes the odds of a Fed move.
3. **Prefer leading over lagging.** Claims, PMI new orders, and permits will tell you about a turn months before the unemployment rate or GDP do.
4. **Cross-check hard data against soft data.** Surveys (PMI, confidence) can diverge from actual output for a year or more, as they did in 2022–24. When they disagree, trust the hard data on the *level* of activity and the soft data on the *direction of risk*.
5. **Don't trade the data.** Retail investors who reposition on release day are competing with algorithms that read the number in microseconds. The edge is in the slow, patient read of the cycle.

## Key takeaways

- Every major indicator is free from its source agency or from FRED; you do not need a terminal.
- Inflation (CPI/PCE) and jobs are the two releases that move markets most, because they most directly drive Fed policy.
- Manufacturing PMIs are excellent leading indicators of industrial profits but can stay below 50 for years without a recession because manufacturing is a small slice of the US economy.
- Consumer sentiment is more useful as a contrarian stock-market indicator than as an economic forecast; extreme pessimism has usually been a buying opportunity.
- The LEI's spotless pre-2020 record was tarnished by a multi-year false alarm; no composite is infallible.
- The unemployment rate lags the cycle; jobless claims lead it.
- As of September 2026 the data describe a solid economy with sticky inflation, which shifts the policy risk toward rate hikes rather than cuts.

## Sources

- [BLS Employment Situation, August 2026](https://www.bls.gov/news.release/empsit.nr0.htm)
- [BLS Consumer Price Index, July 2026](https://www.bls.gov/news.release/cpi.nr0.htm)
- [CNBC: August 2026 jobs report](https://www.cnbc.com/2026/09/04/jobs-report-august-2026.html)
- [Kiplinger: August CPI preview](https://www.kiplinger.com/investing/economy/cpi-report-august-2026-what-to-expect)
- [ISM Manufacturing PMI, August 2026 (PR Newswire)](https://www.prnewswire.com/news-releases/manufacturing-pmi-at-54-6-august-2026-ism-manufacturing-pmi-report-302865127.html)
- [ISM Services PMI, August 2026 (PR Newswire)](https://www.prnewswire.com/news-releases/services-pmi-at-55-4-august-2026-ism-services-pmi-report-302868046.html)
- [Conference Board LEI, July 2026](https://www.prnewswire.com/news-releases/the-conference-board-leading-economic-index-lei-for-the-us-edged-up-in-july-302856410.html)
- [Advisor Perspectives: Consumer Sentiment Falls in August 2026](https://www.advisorperspectives.com/dshort/updates/2026/08/28/consumer-sentiment-falls-in-august)
- [Conference Board US Leading Indicators](https://www.conference-board.org/topics/us-leading-indicators)
- [University of Michigan Surveys of Consumers](https://www.sca.isr.umich.edu/)
- [FRED Economic Data, St. Louis Fed](https://fred.stlouisfed.org/)
- [Atlanta Fed GDPNow](https://www.atlantafed.org/cqer/research/gdpnow)
- [Yahoo Finance: FOMC September 2026 hike odds](https://finance.yahoo.com/economy/policy/articles/fomc-september-2026-odds-rate-201618784.html)
