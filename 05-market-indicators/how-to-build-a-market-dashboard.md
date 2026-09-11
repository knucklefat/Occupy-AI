# How to Build a Market Dashboard

**In one sentence:** A personal market dashboard is a one-page list of roughly fifteen free indicators, checked weekly or monthly on a fixed schedule, that tells you which of four regimes the market is in (healthy expansion, late-cycle/overheating, tightening/stress, or recession/washout) so you can adjust risk at the margin and, more importantly, avoid overreacting to headlines.

## Design principles

1. **Few indicators, clear thresholds.** Fifteen is plenty. Every one should have a "normal," "caution," and "alarm" zone written down in advance, so that reading the dashboard is a matter of counting flags, not interpreting vibes.
2. **Cover all five families.** Macro (growth/inflation), policy (the Fed), credit/liquidity, valuation, and market internals (breadth/sentiment). An alarm in one family is noise; alarms in three are a signal.
3. **Fixed cadence.** Weekly for the fast-moving market indicators (15 minutes on a weekend), monthly for the macro data (30 minutes after the jobs report). Never check on a day when the market is down 3%; that is when your judgment is worst.
4. **Free, official sources.** Everything below is available from FRED, a government agency, or a free data page. FRED lets you build a saved dashboard ([fred.stlouisfed.org](https://fred.stlouisfed.org/), "My Account" → "Dashboards") that updates automatically, and its series IDs are listed here so you can add them in two clicks.
5. **Log it.** Keep a simple spreadsheet with the date and each reading. Six months of your own history is worth more than any commentator's opinion, because you'll see how slowly regimes actually change.

## The fifteen indicators

| # | Indicator | Family | Source (FRED ID or link) | Check | Normal | Caution | Alarm |
|---|---|---|---|---|---|---|---|
| 1 | **Initial jobless claims, 4-wk avg** | Macro | FRED [`IC4WSA`](https://fred.stlouisfed.org/series/IC4WSA) | Weekly | Below 250k, flat | Rising 30k+ from cycle low | Rising 50k+ and above 300k |
| 2 | **Unemployment rate / Sahm rule** | Macro | FRED [`UNRATE`](https://fred.stlouisfed.org/series/UNRATE), [`SAHMREALTIME`](https://fred.stlouisfed.org/series/SAHMREALTIME) | Monthly (1st Fri) | Sahm below 0.3 | 0.3–0.5 | Above 0.5 |
| 3 | **ISM Manufacturing PMI (and New Orders)** | Macro | [ISM](https://www.ismworld.org/supply-management-news-and-reports/reports/ism-report-on-business/) | Monthly (1st bus. day) | Above 50 | 45–50 | Below 45, or New Orders below 45 |
| 4 | **Core PCE inflation, y/y** | Macro | FRED [`PCEPILFE`](https://fred.stlouisfed.org/series/PCEPILFE) (compute y/y) | Monthly (last week) | 2–3% | 3–4% or falling below 1% | Above 4% and rising |
| 5 | **Fed funds rate and FedWatch odds** | Policy | FRED [`DFEDTARU`](https://fred.stlouisfed.org/series/DFEDTARU); [CME FedWatch](https://www.cmegroup.com/markets/interest-rates/cme-fedwatch-tool.html) | Weekly | Fed on hold or cutting into growth | Hiking cycle under way | Hiking into slowing growth, or cutting because of crisis |
| 6 | **10y–3m yield spread** | Policy/recession | FRED [`T10Y3M`](https://fred.stlouisfed.org/series/T10Y3M) | Weekly | Above +0.5 | 0 to +0.5, or re-steepening after inversion | Below zero (start the 6–18-month clock) |
| 7 | **10-year real yield (TIPS)** | Policy | FRED [`DFII10`](https://fred.stlouisfed.org/series/DFII10) | Weekly | 0.5–1.5% | Above 2% or below 0% | Rapid rise (>75 bp in 3 months) |
| 8 | **High-yield credit spread (OAS)** | Credit | FRED [`BAMLH0A0HYM2`](https://fred.stlouisfed.org/series/BAMLH0A0HYM2) | Weekly | 3–5% | Below 3% (complacent) or +100 bp from low | Above 5% or +200 bp from low |
| 9 | **Chicago Fed NFCI** | Liquidity | FRED [`NFCI`](https://fred.stlouisfed.org/series/NFCI) | Weekly (Wed) | Below 0 | 0 to +0.5 | Above +0.5 |
| 10 | **Shiller CAPE** | Valuation | [multpl.com](https://www.multpl.com/shiller-pe) or [Shiller data](http://www.econ.yale.edu/~shiller/data.htm) | Monthly | 15–25 | 25–32 | Above 32 (lowers 10-yr expected return, not a timing signal) |
| 11 | **Forward P/E and earnings revisions** | Valuation | [FactSet Earnings Insight](https://insight.factset.com/topic/earnings) (free weekly PDF) | Monthly | P/E 15–19; estimates rising | P/E above 20; estimates flat | P/E above 22 with estimates being cut |
| 12 | **% of S&P 500 above 200-day MA** | Breadth | StockCharts [`$SPXA200R`](https://stockcharts.com/h-sc/ui?s=$SPXA200R) | Weekly | 50–80% | Above 85% or 30–50% | Below 20% (washout; a buy zone) |
| 13 | **S&P 500 vs. its own 200-day MA; A/D line trend** | Trend/breadth | Any chart; StockCharts [`$NYAD`](https://stockcharts.com/h-sc/ui?s=$NYAD) | Weekly | Index above 200-day, A/D confirming | Index above, A/D diverging 3+ months | Index below 200-day with A/D falling |
| 14 | **VIX** | Sentiment | FRED [`VIXCLS`](https://fred.stlouisfed.org/series/VIXCLS) | Weekly | 13–20 | Below 12 (complacent) or 25–35 | Above 35–40 (fear; a buy zone with #12) |
| 15 | **AAII bull–bear spread** | Sentiment | [AAII](https://www.aaii.com/sentimentsurvey) | Weekly (Thu) | ±20 | Bulls above 50% or bears above 45% | Bears above 50% (buy zone) or bulls above 55% with #10 and #8 in caution |

Optional additions if you want more: WTI crude (`DCOILWTICO`), 10-year breakeven (`T10YIE`), the dollar (`DTWEXBGS`), Conference Board LEI six-month change, and the SLOOS net-tightening series (`DRTSCILM`).

## A worked example: the dashboard as of September 11, 2026

| # | Indicator | Reading | Flag |
|---|---|---|---|
| 1 | Claims | Low 200ks (payrolls +162k in August) | Normal |
| 2 | Unemployment / Sahm | 4.1% / −0.07 | Normal |
| 3 | ISM Manufacturing | 54.6; New Orders 53.7; Prices 71.1 | Normal (inflation sub-index hot) |
| 4 | Core PCE | ~3.3% (June); core CPI 2.5% (July) | Caution |
| 5 | Fed | 3.50–3.75%; ~55–65% odds of a September hike | Caution (hiking into a supply shock) |
| 6 | 10y–3m | ~+1.0 (10y–2y +0.40) | Normal |
| 7 | 10-yr real yield | ~2.3% | Caution (restrictive) |
| 8 | HY spread | 2.71% | Caution (complacent, near record tight) |
| 9 | NFCI | Negative (loose) | Normal |
| 10 | CAPE | ~40.7 | Alarm (valuation, not timing) |
| 11 | Forward P/E | Low-to-mid 20s; estimates still rising on AI capex | Caution |
| 12 | % above 200-day | Roughly 70–75% (mid-year readings) | Normal |
| 13 | Trend / A/D | Index above 200-day; breadth broadened in 2026 | Normal |
| 14 | VIX | ~16.5 | Normal |
| 15 | AAII spread | −1.3 (38% bull / 39% bear) | Normal |

Count: 8 normal, 6 caution, 1 alarm. That is a **late-cycle** profile: growth and market internals are healthy, but inflation, policy, real rates, credit complacency, and valuation are all stretched. The playbook for that regime (below) is "stay invested, stop adding risk, keep dry powder, tighten quality," not "sell."

## The four regimes and what to do in each

| Regime | Dashboard signature | Historical examples | Reasonable response |
|---|---|---|---|
| **Healthy expansion** | Macro normal, Fed neutral/easing into growth, spreads normal, breadth broad, valuation moderate | 1993, 2003–04, 2010–11, 2013, 2016–17, 2023 | Fully invested at your target allocation. Add on dips. Ignore noise. |
| **Late-cycle / overheating** | Macro strong but inflation rising, Fed hiking, real rates up, spreads tight, valuation high, sentiment stretched | 1999, 2006–07, 2018, 2021, mid-2026 | Rebalance to target (this alone trims winners). Favor quality, value, shorter-duration bonds, some international. Build cash for the next regime without going below ~80% of target equity. No leverage. |
| **Tightening / stress** | Curve inverted or re-steepening, HY spreads +150–200 bp from low, NFCI rising, breadth diverging, claims rising | 2000, 2007, 2022 | Move to the lower end of your equity range (this is the only regime where a modest tactical underweight is justified). Extend bond duration once the Fed is done hiking. Write down your buy-back plan now. |
| **Recession / washout** | Sahm triggered, spreads above 6–8%, VIX above 40, fewer than 20% of stocks above 200-day, AAII bears above 50% | Late 2008–Mar 2009, Mar 2020, Oct 2022 | Execute the buy-back plan in tranches. This is when valuation finally matters and every sentiment/breadth gauge says buy. It will feel terrible; that's the point. |

Note the asymmetry: three of the four regimes call for being roughly fully invested. The dashboard's main job is to keep you from selling in regimes one and two, and to make sure you are buying in regime four.

## A plain-language framework for reading it together

1. **Start with credit and jobs.** If claims are low and HY spreads are calm, no bear market is likely imminent, whatever the headlines say. Historically, sustained equity declines of 20%+ have almost always been accompanied by one or both deteriorating.
2. **Then ask what the Fed is doing and why.** Hiking into strength: fine. Hiking into a supply shock with growth slowing: dangerous. Cutting because inflation fell: fine. Cutting because something broke: dangerous.
3. **Use valuation to set expectations, not positions.** High CAPE means lower returns over the next decade and a bigger drawdown *if* a bear market comes. It does not tell you when.
4. **Use breadth and sentiment to time the margins.** Washouts (few stocks above their 200-day, VIX above 40, bears above 50%) are where you add. Divergences and euphoria are where you stop adding and rebalance.
5. **Require confirmation across families.** One alarm = note it. Two families in alarm = adjust modestly. Three or more = the regime has changed; follow the playbook.
6. **Move slowly.** Regimes change over quarters, not days. Any dashboard-driven change should be a shift of a few percentage points in allocation, implemented over weeks, with a written reason.
7. **Never abandon the base case.** The base case for a diversified investor is "stay invested and rebalance." The dashboard earns its keep by *occasionally* justifying a small deviation and by *constantly* talking you out of large ones.

## How to use it

1. Set up a free FRED account and create a dashboard with the series IDs above; bookmark ISM, FactSet, StockCharts, CME FedWatch, and AAII for the rest.
2. Every weekend (15 minutes): update items 1, 5–9, 12–15. Note any flag changes.
3. After the jobs report each month (30 minutes): update items 2–4, 10–11. Count flags by family and name the regime.
4. Write one sentence in a log: "September 2026: late-cycle, 6 caution / 1 alarm, main risk is Fed hiking into oil shock; action: rebalanced to target, no new risk."
5. Review the log quarterly and ask whether the regime has changed. Act only when it has, and only by a few percentage points.
6. Once a year, check whether the thresholds still make sense (for example, credit spreads have structurally tightened over the decades; VIX behavior changed with 0DTE options) and revise them deliberately, not in the middle of a selloff.

## Key takeaways

- Fifteen free indicators across five families, with thresholds set in advance, are enough to name the market regime.
- Credit spreads and jobless claims are the first two things to check; when both are calm, imminent bear-market risk is low.
- Valuation sets long-run expectations; breadth and sentiment time the margins; the Fed and credit define the regime.
- Three of the four regimes call for being roughly fully invested; the dashboard's main value is preventing overreaction.
- Require alarms in three families before making a regime call, and then move only a few percentage points, over weeks.
- Keep a written log; your own six-month record beats any pundit.
- As of September 2026 the profile is late-cycle: healthy activity and internals, but stretched inflation, policy, real rates, credit complacency, and valuation. Stay invested, stop adding risk, rebalance, keep some dry powder.

## Sources

- [FRED Economic Data (dashboards and all series IDs above)](https://fred.stlouisfed.org/)
- [CME FedWatch Tool](https://www.cmegroup.com/markets/interest-rates/cme-fedwatch-tool.html)
- [ISM Report on Business](https://www.ismworld.org/supply-management-news-and-reports/reports/ism-report-on-business/)
- [FactSet Earnings Insight](https://insight.factset.com/topic/earnings)
- [StockCharts: $SPXA200R](https://stockcharts.com/h-sc/ui?s=$SPXA200R)
- [AAII Investor Sentiment Survey](https://www.aaii.com/sentimentsurvey)
- [Chicago Fed NFCI](https://www.chicagofed.org/research/data/nfci/current-data)
- [multpl.com: Shiller PE](https://www.multpl.com/shiller-pe)
- [BLS Employment Situation, August 2026](https://www.bls.gov/news.release/empsit.nr0.htm)
- [Federal Reserve FOMC statement, July 29, 2026](https://www.federalreserve.gov/newsevents/pressreleases/monetary20260729a.htm)
- [govspending.org: High-Yield OAS](https://govspending.org/series/BAMLH0A0HYM2/)
- [MacroRadar: VIX](https://www.macroradar.io/vix)
- [thetrading.tools: Sahm rule](https://www.thetrading.tools/sahm-rule)
