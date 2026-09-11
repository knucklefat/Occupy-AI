# Credit and Liquidity Indicators

**In one sentence:** Credit and liquidity indicators measure how easy it is to borrow and how much money is sloshing around the system; because bear markets and recessions are usually credit events (lenders pull back, spreads widen, funding dries up), these gauges often detect trouble before the stock market and long before the economic data do.

## Why credit leads equities

Equity holders get paid last. When a company's prospects dim, its bondholders (who have a fixed claim and no upside) notice first and demand more yield. Bond and money-market participants are also mostly institutions with credit analysts on staff, whereas the equity market includes a great deal of momentum and retail money. So "watch credit" is one of the oldest pieces of advice among professional investors: when high-yield spreads widen while stocks keep rising, the stocks are usually wrong.

Liquidity is the broader concept: how much money is available to buy assets. It comes from the Fed (balance sheet, rates), the banking system (lending), the Treasury (its cash balance and bill issuance), and abroad (the dollar). "Financial conditions indexes" try to squash all of this into one number.

## The indicators

| Indicator | What it measures | Free source | Frequency | How to read it | Track record / notes |
|---|---|---|---|---|---|
| **High-yield (junk) bond spread** | Extra yield on below-investment-grade corporate bonds over Treasuries, option-adjusted (OAS) | FRED [`BAMLH0A0HYM2`](https://fred.stlouisfed.org/series/BAMLH0A0HYM2) (ICE BofA US High Yield) | Daily | Long-run average ~5.4% (since 1997). Below 3%: complacent/tight. 3–5%: normal. 5–8%: stress. Above 8%: crisis (2001–02, 2008, 2020). Records: 19.9% Dec 2008; 10.9% Mar 2020. | Spreads widened ahead of the 2007–08 and 2000–01 equity declines and blew out during each. A widening of 150+ basis points from the low while stocks are still rising is the classic warning. **2.71% on September 9, 2026**, near the tightest levels ever recorded. |
| **Investment-grade spread** | Same for BBB-and-above corporates | FRED [`BAMLC0A0CM`](https://fred.stlouisfed.org/series/BAMLC0A0CM); BBB-only `BAMLC0A4CBBB` | Daily | Average ~1.3%; above 2% = stress; above 3% = crisis. | Moves with HY but less; the BBB tier (half the IG market) is where downgrade risk lives. |
| **CCC spread / distress ratio** | Spread on the riskiest tier; share of HY bonds trading above 1,000 bp | FRED [`BAMLH0A3HYC`](https://fred.stlouisfed.org/series/BAMLH0A3HYC) | Daily | CCC spreads above 10% signal rising defaults. | Leads the default rate by ~6–12 months. |
| **TED spread (historical) / SOFR–OIS / FRA–OIS** | Bank funding stress: the gap between what banks pay to borrow from each other and the risk-free rate | TED (`TEDRATE`) was discontinued on FRED in January 2022 and LIBOR ended in mid-2023. Modern equivalents: 3-month commercial paper minus T-bill (FRED `DCPF3M` − `DTB3`); SOFR vs. fed funds (`SOFR`, `DFF`); FRA–OIS is on Bloomberg/press only | Daily | TED above 1% was a crisis (4.6% in Oct 2008). Today: CP–bill spread above 0.5%, or SOFR spiking above the top of the Fed's range at month/quarter ends, signals funding strain. | The September 2019 repo spike (SOFR briefly above 5% while fed funds was ~2.2%) was the modern example: it forced the Fed to restart bill purchases. |
| **Chicago Fed National Financial Conditions Index (NFCI)** | Weighted average of 105 indicators of risk, credit, and leverage across money, debt, equity, and banking markets | [Chicago Fed](https://www.chicagofed.org/research/data/nfci/current-data); FRED [`NFCI`](https://fred.stlouisfed.org/series/NFCI), [`ANFCI`](https://fred.stlouisfed.org/series/ANFCI) (adjusted for the business cycle) | Weekly (Wednesday, 8:30 a.m. ET) | Zero = average conditions since 1971. Positive = tighter than average; negative = looser. Readings above +1 coincided with 2008 and 2020. | The most comprehensive free measure. Conditions have been "loose" (negative) for most of 2023–26 despite high policy rates, because equities and spreads were strong, which is part of why Fed hikes bit less than expected. |
| **Goldman Sachs / Bloomberg Financial Conditions Indexes** | Proprietary composites of rates, spreads, equity prices, and the dollar | Reported in financial press and Goldman research summaries; Bloomberg's `BFCIUS` requires a terminal | Daily | Higher = tighter. Fed officials cite the Goldman index frequently. | Similar signal to NFCI; the value is that Fed speeches reference it. |
| **M2 money supply** | Currency, checking, savings, and money-market deposits | FRED [`M2SL`](https://fred.stlouisfed.org/series/M2SL); [Fed H.6 release](https://www.federalreserve.gov/releases/h6/) | Monthly (~4th week) | Watch year-over-year growth. Long-run ~6%. Growth above 10% (2020–21: 27% peak) is inflationary with a 12–24-month lag; contraction (2022–23, the first since the 1930s) is deflationary. | The 2020–21 surge correctly foreshadowed the 2021–23 inflation, and the 2022–23 contraction the disinflation; but M2's link to inflation was weak from 1990 to 2019. Now ~$23.2 trillion (June 2026), growing roughly 4–5% year-over-year. |
| **Fed balance sheet / bank reserves** | See the interest-rates file | FRED `WALCL`, `WRESBAL` | Weekly | Reserves below ~10% of GDP are considered "scarce"; the 2019 repo crisis hit at ~7–8%. | Reserves at roughly $3+ trillion and the Fed's stated "ample reserves" policy suggest no imminent scarcity. |
| **Overnight reverse repo (RRP) balance** | Cash money-market funds park at the Fed overnight; a measure of excess liquidity | FRED [`RRPONTSYD`](https://fred.stlouisfed.org/series/RRPONTSYD) | Daily | High balances (peak $2.55 trillion, Dec 2022) = excess cash with nowhere to go. Falling balances mean that cash is being absorbed, often by Treasury bill issuance. Once near zero, further QT drains bank reserves directly. | RRP drained from $2.5T to near zero over 2023–25, cushioning QT. With RRP near zero, the liquidity buffer is gone, which is one reason the Fed slowed and then ended QT. |
| **Treasury General Account (TGA)** | The Treasury's checking account at the Fed | FRED [`WTREGEN`](https://fred.stlouisfed.org/series/WTREGEN) | Weekly | Rising TGA (tax season, post-debt-ceiling rebuilds) drains liquidity from markets; falling TGA adds it. | Net liquidity = Fed assets − TGA − RRP is a popular trader's gauge; its correlation with stocks was strong in 2022–23 and weak in other periods. |
| **US dollar index** | Dollar vs. a basket of major currencies (DXY: euro-heavy; Fed's broad index is trade-weighted) | DXY via [ICE](https://www.ice.com/products/194/US-Dollar-Index-Futures) or any quote site; FRED [`DTWEXBGS`](https://fred.stlouisfed.org/series/DTWEXBGS) (broad, Fed) | Daily | A rising dollar tightens global conditions (emerging-market debt is dollar-denominated), hurts US exporters' earnings, and pressures commodities. A falling dollar does the reverse. | Dollar spikes accompanied 2008, 2020, and 2022 stress. DXY ~99 on September 11, 2026, up ~1.7% over 12 months, well below the 2022 peak near 114. |
| **Senior Loan Officer Opinion Survey (SLOOS)** | Fed survey of ~80 banks on whether they are tightening or easing lending standards and seeing more or less demand | [Federal Reserve SLOOS](https://www.federalreserve.gov/data/sloos.htm); FRED [`DRTSCILM`](https://fred.stlouisfed.org/series/DRTSCILM) (net % tightening C&I standards, large/mid firms) | Quarterly (early Feb, May, Aug, Nov) | Net tightening above ~+20% has preceded or accompanied every recession since 1990; above +50% in 2001, 2008, 2020. | 2023 saw net tightening near 50% with no recession (another 2022–24 false alarm). The July 2026 survey showed C&I standards basically unchanged, CRE easing, and credit-card standards tightening modestly. |
| **Bank lending growth** | Total loans and leases at commercial banks | FRED [`TOTLL`](https://fred.stlouisfed.org/series/TOTLL); [Fed H.8 release](https://www.federalreserve.gov/releases/h8/) | Weekly | Year-over-year growth turning negative is a recession-level event. | Slowed to near zero in 2023–24; recovering since. |

## Reading the current picture (as of September 11, 2026)

Credit says "all clear," which is itself the thing to worry about. High-yield spreads at 2.7% price in almost no default risk; IG spreads are similarly tight; NFCI is negative (loose); banks are not tightening; the dollar is stable; M2 is growing at a normal pace; reserves are ample. This is exactly the configuration you see in the late stages of an expansion (2006, 2019, 2021): conditions are loose because nothing has gone wrong yet, and valuations of every risky asset are high for the same reason.

The vulnerabilities: (1) With RRP drained and QT over, there is no liquidity buffer if the Fed has to tighten again in response to $100 oil; (2) Spreads at record tights have nowhere to go but wider, and the historical asymmetry is severe (spreads rarely fall below 2.5% and have risen to 8%+ five times since 1997); (3) Private credit, which now rivals the high-yield bond market in size, is not captured in these public series, so stress there can build unseen.

## How to use it

1. **Put HY OAS on your weekly dashboard.** It is the single best free early-warning indicator. Set a mental alert at +100 bp from the cycle low and a louder one at 5%.
2. **Confirm equity rallies with credit.** If stocks make new highs and HY spreads make new lows, the rally is confirmed. If spreads widen while stocks rise for more than a few weeks, believe the bonds.
3. **Use NFCI for the big picture.** Positive NFCI = the system is tightening, which historically leads earnings and employment down within a few quarters.
4. **Watch funding markets at quarter-ends.** SOFR trading above the Fed's target range or CP–bill spreads jumping means plumbing stress, which the Fed will usually fix but which can produce sharp, brief selloffs.
5. **Read SLOOS for the lending cycle.** Net tightening above 20% is your cue to expect slower growth and weaker small-cap and cyclical earnings.
6. **Use the dollar as a cross-check.** A rising dollar with widening spreads is the risk-off signature; a falling dollar with tightening spreads is risk-on.

## Key takeaways

- Credit markets usually see trouble before equity markets; high-yield spreads are the best free early warning.
- HY OAS at ~2.7% (September 2026) is near record tights: little risk is priced, which limits reward and maximizes surprise potential.
- The TED spread is dead; use CP–bill spreads, SOFR vs. fed funds, and the NFCI instead.
- The Chicago Fed NFCI is the most comprehensive free financial-conditions gauge; zero is average, positive is tight.
- M2's inflation signal worked in 2020–23 after decades of not working; treat it as a slow, blunt instrument.
- With reverse repo drained and QT ended, the system's liquidity cushion is gone; the next tightening will bite harder.
- SLOOS net tightening above 20% has accompanied every recession since 1990 but also misfired in 2023; as of July 2026 banks are not tightening.

## Sources

- [FRED: ICE BofA US High Yield OAS (BAMLH0A0HYM2)](https://fred.stlouisfed.org/series/BAMLH0A0HYM2)
- [govspending.org: High-Yield Credit Spread](https://govspending.org/series/BAMLH0A0HYM2/)
- [Chicago Fed: National Financial Conditions Index](https://www.chicagofed.org/research/data/nfci/current-data)
- [Chicago Fed: About the NFCI](https://www.chicagofed.org/research/data/nfci/about)
- [Federal Reserve: July 2026 Senior Loan Officer Opinion Survey](https://www.federalreserve.gov/data/sloos/sloos-202607.htm)
- [KPMG: Fed survey says lending standards are steady](https://kpmg.com/us/en/articles/2026/q2-2026-fed-sloos.html)
- [Trading Economics: US Dollar Index](https://tradingeconomics.com/united-states/currency)
- [Trading Economics: US Money Supply M2](https://tradingeconomics.com/united-states/money-supply-m2)
- [FRED: M2 (M2SL)](https://fred.stlouisfed.org/series/M2SL)
- [FRED: Overnight Reverse Repurchase Agreements (RRPONTSYD)](https://fred.stlouisfed.org/series/RRPONTSYD)
- [FRED: Nominal Broad US Dollar Index (DTWEXBGS)](https://fred.stlouisfed.org/series/DTWEXBGS)
- [Federal Reserve H.8: Assets and Liabilities of Commercial Banks](https://www.federalreserve.gov/releases/h8/)
- [MacroRadar: Fed balance sheet](https://www.macroradar.io/fed-balance-sheet)
