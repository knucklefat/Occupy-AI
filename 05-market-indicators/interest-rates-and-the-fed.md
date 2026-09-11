# Interest Rates and the Fed

**In one sentence:** The Federal Reserve sets the price of short-term money and the size of its own balance sheet, and because every asset on earth is valued by discounting future cash flows at some interest rate, understanding what the Fed is doing (and what markets expect it to do next) is the single most important piece of macro context an investor can have.

## What the Fed actually controls

The Fed has a "dual mandate" from Congress: maximum employment and stable prices, which it defines as 2% inflation measured by the PCE price index. Its main tools:

- **The federal funds rate.** The overnight rate at which banks lend reserves to each other. The Federal Open Market Committee (FOMC) sets a *target range* (currently 3.50–3.75%) and steers the actual rate inside it by paying interest on bank reserves (IORB) and offering an overnight reverse-repo facility. Every other short-term rate (Treasury bills, money-market yields, prime rate, SOFR) keys off this.
- **Forward guidance.** Statements, press conferences, and the quarterly "dot plot" that signal where policy is headed. Because markets price the *expected path* of rates, talk is a tool.
- **The balance sheet.** Buying bonds (quantitative easing, QE) pushes down long-term yields and adds reserves to the banking system; letting bonds mature without reinvesting (quantitative tightening, QT) does the reverse. The balance sheet peaked near $9 trillion in 2022 and stood at about $6.73 trillion in late August 2026, with the Fed saying it is now "maintaining ample reserves."

The FOMC meets eight times a year. The 2026 schedule: January 27–28, March 17–18, April 28–29, June 16–17, July 28–29, September 15–16, October 27–28, December 8–9. Decisions come at 2:00 p.m. ET on the second day, followed by the chair's press conference. Minutes are released three weeks later. Four meetings a year (March, June, September, December) include the Summary of Economic Projections and the dot plot.

## The indicators

| Indicator | What it measures | Free source | Frequency | How to read it | Notes |
|---|---|---|---|---|---|
| **Fed funds target range / effective rate** | Policy rate; effective rate is the actual traded average | [Fed press releases](https://www.federalreserve.gov/monetarypolicy/fomccalendars.htm); FRED `DFEDTARU`, `DFF`, `FEDFUNDS` | Daily / after each FOMC | Level vs. inflation gives the *real* policy rate (see below). Direction of the last move and guidance matter more than level. | Dissents in the vote (three members wanted a hike in July 2026) telegraph the committee's lean. |
| **Dot plot** | Each FOMC participant's anonymous projection of the year-end rate for the next 2–3 years and "longer run" | [Fed SEP](https://www.federalreserve.gov/monetarypolicy/fomccalendars.htm) | Quarterly (Mar/Jun/Sep/Dec) | Median dot = committee's central expectation. The longer-run dot is the Fed's estimate of the "neutral" rate. | Dots are projections, not promises; they have been wrong by 100+ basis points a year out. Compare median dots to market pricing to see who's more hawkish. |
| **CME FedWatch** | Market-implied probability of each rate outcome at upcoming meetings, derived from fed funds futures | [CME FedWatch](https://www.cmegroup.com/markets/interest-rates/cme-fedwatch-tool.html) | Live | Shows the odds of hike/hold/cut per meeting. Markets move when data shifts these odds, not when the Fed acts as expected. | Excellent for the next 1–2 meetings; increasingly unreliable beyond six months. |
| **Fed balance sheet (total assets)** | Size of the Fed's holdings of Treasuries, MBS, and loans | [H.4.1 release](https://www.federalreserve.gov/releases/h41/); FRED `WALCL` | Weekly, Thursday 4:30 p.m. ET | Rising = QE/liquidity injection; falling = QT. Also watch bank reserves (`WRESBAL`). | The 2020–21 expansion coincided with a huge asset boom; the 2022–24 shrinkage coincided with a bear market and recovery, so the link to stocks is loose. |
| **Real interest rates** | Nominal rate minus expected inflation; the true cost of money | FRED `DFII10` (10-yr TIPS yield), `DFII5`; or fed funds minus core PCE | Daily | Positive and rising real rates are restrictive for valuations, gold, and long-duration assets (growth stocks, long bonds). Negative real rates favor them. | The 10-year TIPS yield went from −1% in 2021 to +2% in 2023, the sharpest tightening of real rates in 40 years. |
| **2-year Treasury yield** | Market's best guess of the average fed funds rate over the next two years | FRED `DGS2` | Daily | If the 2-year is well above fed funds, markets expect hikes; well below, cuts. | Often a better "Fed forecaster" than the Fed's own dots. |
| **10-year Treasury yield** | The benchmark long-term risk-free rate; drives mortgage rates, equity discount rates | FRED `DGS10` | Daily | Decompose into expected short rates + term premium + inflation compensation (see breakevens). | 4.73% at end of August 2026. |
| **Taylor rule estimate** | A formula for where the policy rate "should" be given inflation and the output/unemployment gap | [Atlanta Fed Taylor Rule Utility](https://www.atlantafed.org/cqer/research/taylor-rule) | Updated with data | If the actual rate is far below the rule, policy is loose; far above, tight. | A guide, not a law. The Fed has never followed it mechanically. |

## The Taylor rule in one paragraph

John Taylor's 1993 formula says the policy rate should equal the neutral real rate (he used 2%) plus current inflation, plus half the amount inflation exceeds target, plus half the output gap. So with inflation at 3.5%, a 2% target, and the economy at potential, the rule prescribes roughly 2 + 3.5 + 0.75 + 0 = 6.25%. Variants swap in different neutral-rate assumptions (the Fed's longer-run dot implies a real neutral rate closer to 1%) and different gap measures, which is why the Atlanta Fed's tool shows several versions at once. The point is not the exact number; it is that the rule gives you a neutral yardstick for calling policy "tight" or "loose" independent of whatever the Fed says about itself.

## How rate changes move stocks and bonds

**Bonds** are mechanical: price moves opposite to yield, scaled by duration. A bond fund with 7-year duration loses roughly 7% of its value when yields rise one percentage point. Short-term bonds and T-bills barely move; 30-year Treasuries swing violently.

**Stocks** are messier, because rates affect them through three channels that can pull in opposite directions:

1. **Discount rate.** Higher rates make future earnings worth less today. This hits long-duration equities (unprofitable growth, tech) hardest, which is why 2022's rate shock crushed the Nasdaq more than the Dow.
2. **Earnings.** If rates rise because the economy is strong, profits are rising too, which can more than offset the discount-rate hit. Stocks often rise during the early part of a hiking cycle.
3. **Relative attractiveness.** When T-bills yield 5%, the bar for owning stocks rises (see the equity risk premium in the valuation file).

The empirical record: the *first* rate cut of a cycle is not reliably bullish. Cuts in 2001 and 2007 were followed by severe bear markets because they came in response to a collapsing economy; cuts in 1995, 1998, and 2019 were "insurance" cuts into a still-growing economy and were followed by strong gains. In other words, *why* the Fed is moving matters more than *which way*. Likewise, hiking cycles into strong growth (1994, 2004–06, 2016–18) saw stocks rise on net despite volatility, while 2022's hikes into slowing growth produced a 25% drawdown.

A rule of thumb from the bond market: stocks handle gradual, well-telegraphed rate rises fine; they struggle with *rapid* rises (more than ~100 basis points in the 10-year within a few months) and with *surprises* that reveal the Fed is behind the curve.

## Where things stand (as of September 11, 2026)

- Target range 3.50–3.75%, unchanged since the July 28–29 meeting, where three members dissented in favor of a quarter-point *increase*.
- Fed Chair Kevin Warsh's Jackson Hole speech in late August signaled that summer's inflation improvement was not enough; FedWatch odds of a September hike moved from the mid-40s to roughly 55–66% depending on the day and the data.
- PCE inflation ran 3.7% headline / 3.3% core through June; CPI 3.4% / 2.5% through July. Oil near $100 from the Iran/Strait of Hormuz disruption is the main headline driver.
- The 2-year yield (4.34%) sits well above the fed funds midpoint (3.625%), which is the market's way of saying it expects rates to go up, not down.
- The balance sheet is stable at ~$6.7 trillion; QT has effectively ended.

The unusual feature of this cycle is a Fed contemplating hikes with unemployment at 4.1% and a positively sloped yield curve. That combination (tightening into a supply-driven inflation shock) has few precedents; 1973–74 and 1979–80 are the closest, and neither was kind to stocks.

## How to use it

1. **Check FedWatch weekly.** Know what is priced for the next two meetings. A hike or cut that is 90% priced is a non-event when it happens; the surprise is what matters.
2. **Track the real policy rate.** Fed funds minus core PCE. Above roughly +1% is restrictive; below zero is stimulative. It is currently only mildly positive (about +0.3 to +0.5%), which is why hawks argue policy isn't really tight.
3. **Use the 2-year as your Fed forecaster.** It aggregates every trader's view and updates instantly.
4. **Match duration to your view.** If you think rates are going higher, keep bond maturities short. If you think the next big move is down, extend.
5. **Don't fight the Fed, but don't front-run it either.** The old adage works because Fed policy determines liquidity; but the 2022 lesson is that the *direction of change* in policy matters more than the level, and the 2001/2007 lesson is that cuts into a recession don't save you.

## Key takeaways

- The FOMC sets a target range for the overnight rate; everything else in fixed income is priced off expectations for its path.
- The dot plot shows what the Fed thinks; the 2-year yield and CME FedWatch show what the market thinks. When they disagree, the market has the better record, but not by much.
- Real rates (nominal minus inflation) determine how tight policy actually is; nominal levels alone mislead.
- Rate cuts are only bullish when the economy isn't falling apart. Ask why the Fed is moving.
- Bond prices move inversely to yields, scaled by duration; know your fund's duration.
- The balance sheet's link to stock prices is real but loose; don't build a strategy on "liquidity" alone.
- As of September 2026 the Fed is at 3.50–3.75% and leaning toward a hike, with PCE inflation well above target and oil near $100.

## Sources

- [Federal Reserve FOMC statement, July 29, 2026](https://www.federalreserve.gov/newsevents/pressreleases/monetary20260729a.htm)
- [FOMC minutes, June 16–17, 2026](https://www.federalreserve.gov/monetarypolicy/fomcminutes20260617.htm)
- [Federal Reserve calendar and FOMC schedule](https://www.federalreserve.gov/monetarypolicy/fomccalendars.htm)
- [CME FedWatch Tool](https://www.cmegroup.com/markets/interest-rates/cme-fedwatch-tool.html)
- [Yahoo Finance: September 2026 rate-hike odds](https://finance.yahoo.com/economy/policy/articles/fomc-september-2026-odds-rate-201618784.html)
- [CNBC: September Fed decision now a coin flip](https://www.cnbc.com/2026/08/28/-september-fed-decision-now-a-coin-flip-as-rate-hike-odds-increase.html)
- [Advisor Perspectives: Treasury Yields Snapshot, Aug 28, 2026](https://www.advisorperspectives.com/dshort/updates/2026/08/28/treasury-yields-snapshot-august-28-2026)
- [MacroRadar: Fed balance sheet](https://www.macroradar.io/fed-balance-sheet)
- [Federal Reserve H.4.1 balance sheet release](https://www.federalreserve.gov/releases/h41/)
- [Atlanta Fed Taylor Rule Utility](https://www.atlantafed.org/cqer/research/taylor-rule)
- [FRED: 10-Year TIPS yield (DFII10)](https://fred.stlouisfed.org/series/DFII10)
- [FRED: Fed total assets (WALCL)](https://fred.stlouisfed.org/series/WALCL)
