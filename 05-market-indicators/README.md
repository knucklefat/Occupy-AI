# 05 — Market Indicators

**In one sentence:** This section catalogs the economic, policy, credit, valuation, sentiment, breadth, commodity, and calendar indicators that investors watch, explains what each one actually measures, where to get it for free, how to read it, and, most importantly, how much predictive power it has really shown.

Every indicator here is free. Most live on [FRED](https://fred.stlouisfed.org/) (the St. Louis Fed's database), the rest on government sites, exchange pages, or free data services; the master table below links each one. The section's organizing idea is that indicators fall into families, each answering a different question: *Where is the economy?* (macro), *What is the Fed doing?* (policy), *Is money flowing or drying up?* (credit and liquidity), *What am I paying?* (valuation), *How does everyone feel?* (sentiment), *Is the rally broad or narrow?* (breadth), and *What are commodities saying?* No single indicator is reliable; the yield curve, the Sahm rule, and the LEI all misfired in 2022–24. Read across families, act at the margin, and keep a log. The final file turns all of this into a fifteen-item dashboard with thresholds. Current readings are date-stamped as of September 2026.

## Files in this section

1. [Macroeconomic indicators](macroeconomic-indicators.md) — GDP, CPI/PCE, jobs, claims, ISM PMIs, retail sales, housing, confidence, LEI, and the release calendar
2. [Interest rates and the Fed](interest-rates-and-the-fed.md) — fed funds, FOMC, dot plot, balance sheet, real rates, FedWatch, Taylor rule, how rates move stocks and bonds
3. [Yield curve and recession indicators](yield-curve-and-recession-indicators.md) — 10y–2y and 10y–3m, inversion history, Sahm rule, NY Fed model, LEI, credit spreads
4. [Valuation indicators](valuation-indicators.md) — Shiller CAPE, Buffett indicator, forward P/E, equity risk premium, Fed model, Tobin's Q, and what they predict over 10 years vs. 1 year
5. [Sentiment indicators](sentiment-indicators.md) — VIX, put/call, AAII, CNN Fear & Greed, Investors Intelligence, fund-manager surveys, margin debt, contrarian use
6. [Market breadth indicators](market-breadth-indicators.md) — A/D line, % above 200-day, new highs/lows, McClellan oscillator, equal-weight vs. cap-weight, Zweig breadth thrust
7. [Credit and liquidity indicators](credit-and-liquidity-indicators.md) — high-yield spreads, funding spreads, NFCI, M2, dollar, reverse repo, SLOOS
8. [Commodity and inflation signals](commodity-and-inflation-signals.md) — oil, copper, gold, breakevens, 5y5y forward, commodity indexes, Baltic Dry
9. [Seasonality and calendar effects](seasonality-and-calendar-effects.md) — Sell in May, January effect, presidential cycle, Santa Claus rally, turn-of-month, and why most are weak
10. [How to build a market dashboard](how-to-build-a-market-dashboard.md) — a fifteen-indicator weekly/monthly checklist with FRED IDs, thresholds, and a four-regime framework

## Master table of indicators

| Indicator | Category | Free source | Update frequency | Covered in |
|---|---|---|---|---|
| Real GDP (and Atlanta Fed GDPNow) | Macro: growth | [BEA](https://www.bea.gov/data/gdp/gross-domestic-product); FRED `GDPC1`; [GDPNow](https://www.atlantafed.org/cqer/research/gdpnow) | Quarterly (3 estimates); GDPNow ~weekly | Macro |
| CPI (headline, core) | Macro: inflation | [BLS](https://www.bls.gov/cpi/); FRED `CPIAUCSL`, `CPILFESL` | Monthly, ~10th–15th | Macro |
| PCE price index (headline, core) | Macro: inflation | [BEA](https://www.bea.gov/data/personal-consumption-expenditures-price-index); FRED `PCEPI`, `PCEPILFE` | Monthly, last week | Macro, Dashboard |
| Nonfarm payrolls, unemployment rate, wages | Macro: labor | [BLS](https://www.bls.gov/news.release/empsit.nr0.htm); FRED `PAYEMS`, `UNRATE` | Monthly, first Friday | Macro, Dashboard |
| Initial and continuing jobless claims | Macro: labor (leading) | [DOL](https://www.dol.gov/ui/data.pdf); FRED `ICSA`, `IC4WSA`, `CCSA` | Weekly, Thursday | Macro, Yield curve, Dashboard |
| ISM Manufacturing PMI | Macro: activity | [ISM](https://www.ismworld.org/supply-management-news-and-reports/reports/ism-report-on-business/) | Monthly, 1st business day | Macro, Dashboard |
| ISM Services PMI | Macro: activity | [ISM](https://www.ismworld.org/supply-management-news-and-reports/reports/ism-report-on-business/) | Monthly, 3rd business day | Macro |
| Retail sales (and control group) | Macro: consumption | [Census](https://www.census.gov/retail/sales.html); FRED `RSAFS` | Monthly, mid-month | Macro |
| Housing starts and building permits | Macro: housing (leading) | [Census/HUD](https://www.census.gov/construction/nrc/index.html); FRED `HOUST`, `PERMIT` | Monthly, ~17th–19th | Macro |
| Conference Board Consumer Confidence | Macro: sentiment | [Conference Board](https://www.conference-board.org/topics/consumer-confidence) | Monthly, last Tuesday | Macro |
| University of Michigan Consumer Sentiment and inflation expectations | Macro: sentiment | [UMich](https://www.sca.isr.umich.edu/); FRED `UMCSENT`, `MICH` | Twice monthly (prelim 2nd Fri, final 4th Fri) | Macro, Sentiment |
| Conference Board Leading Economic Index (LEI) | Macro: composite leading | [Conference Board](https://www.conference-board.org/topics/us-leading-indicators) | Monthly, ~3rd week | Macro, Yield curve |
| Fed funds target range / effective rate | Policy | [Fed](https://www.federalreserve.gov/monetarypolicy/fomccalendars.htm); FRED `DFEDTARU`, `DFF` | 8 FOMC meetings/yr; daily effective | Rates, Dashboard |
| FOMC dot plot / Summary of Economic Projections | Policy | [Fed SEP](https://www.federalreserve.gov/monetarypolicy/fomccalendars.htm) | Quarterly (Mar/Jun/Sep/Dec) | Rates |
| CME FedWatch (market-implied rate odds) | Policy | [CME](https://www.cmegroup.com/markets/interest-rates/cme-fedwatch-tool.html) | Live | Rates, Dashboard |
| Fed balance sheet / bank reserves | Policy, liquidity | [H.4.1](https://www.federalreserve.gov/releases/h41/); FRED `WALCL`, `WRESBAL` | Weekly, Thursday | Rates, Credit |
| 2-year and 10-year Treasury yields | Policy, rates | FRED `DGS2`, `DGS10` | Daily | Rates |
| 10-year TIPS real yield | Policy, rates | FRED `DFII10` | Daily | Rates, Commodities, Dashboard |
| Taylor rule estimates | Policy | [Atlanta Fed](https://www.atlantafed.org/cqer/research/taylor-rule) | With data releases | Rates |
| 10y–2y Treasury spread | Recession | FRED `T10Y2Y` | Daily | Yield curve |
| 10y–3m Treasury spread | Recession | FRED `T10Y3M` | Daily | Yield curve, Dashboard |
| NY Fed recession probability (yield-curve model) | Recession | [NY Fed](https://www.newyorkfed.org/research/capital_markets/ycfaq) | Monthly | Yield curve |
| Sahm rule | Recession (real-time) | FRED `SAHMREALTIME`, `SAHMCURRENT` | Monthly, with jobs report | Yield curve, Dashboard |
| Chauvet-Piger smoothed recession probability | Recession (nowcast) | FRED `RECPROUSM156N` | Monthly | Yield curve |
| Shiller CAPE (P/E10) | Valuation | [Shiller data](http://www.econ.yale.edu/~shiller/data.htm); [multpl](https://www.multpl.com/shiller-pe) | Monthly | Valuation, Dashboard |
| Buffett indicator (market cap / GDP) | Valuation | [Current Market Valuation](https://www.currentmarketvaluation.com/models/buffett-indicator.php); [GuruFocus](https://www.gurufocus.com/stock-market-valuations.php) | Quarterly (GDP) | Valuation |
| Forward P/E and earnings revisions | Valuation | [FactSet Earnings Insight](https://insight.factset.com/topic/earnings) | Weekly | Valuation, Dashboard |
| Implied equity risk premium | Valuation | [Damodaran](https://pages.stern.nyu.edu/~adamodar/New_Home_Page/datafile/histimpl.html) | Monthly | Valuation |
| Fed model (earnings yield vs. 10-yr) | Valuation | Compute from FactSet + FRED `DGS10` | Weekly | Valuation |
| Tobin's Q | Valuation | FRED `NCBEILQ027S` / `TNWMVBSNNCB` | Quarterly (Z.1) | Valuation |
| VIX | Sentiment | [Cboe](https://www.cboe.com/tradable-products/vix/); FRED `VIXCLS` | Real-time | Sentiment, Dashboard |
| Put/call ratio | Sentiment | [Cboe](https://www.cboe.com/us/options/market_statistics/daily/); StockCharts `$CPC`, `$CPCE` | Daily | Sentiment |
| AAII Investor Sentiment Survey | Sentiment | [AAII](https://www.aaii.com/sentimentsurvey) | Weekly, Thursday | Sentiment, Dashboard |
| Investors Intelligence Advisors' Sentiment | Sentiment | [Investors Intelligence](https://www.investorsintelligence.com/); [Yardeni](https://www.yardeniquicktakes.com/bull-bear-ratio/) | Weekly, Wednesday | Sentiment |
| CNN Fear & Greed Index | Sentiment (composite) | [CNN](https://www.cnn.com/markets/fear-and-greed) | Daily | Sentiment |
| BofA Global Fund Manager Survey | Sentiment / positioning | Press summaries ([Mace News](https://macenews.com/)) | Monthly, mid-month | Sentiment |
| FINRA margin debt | Sentiment / leverage | [FINRA](https://www.finra.org/investors/learn-to-invest/advanced-investing/margin-statistics) | Monthly, ~3-week lag | Sentiment |
| NAAIM Exposure Index | Sentiment / positioning | [NAAIM](https://www.naaim.org/programs/naaim-exposure-index/) | Weekly | Sentiment |
| NYSE Advance/Decline line | Breadth | StockCharts `$NYAD`; [WSJ](https://www.wsj.com/market-data/stocks/marketsdiary) | Daily | Breadth, Dashboard |
| % of S&P 500 above 200-day / 50-day MA | Breadth | StockCharts `$SPXA200R`, `$SPXA50R` | Daily | Breadth, Dashboard |
| New 52-week highs / lows | Breadth | StockCharts `$NYHL` | Daily | Breadth |
| McClellan Oscillator and Summation Index | Breadth | StockCharts `$NYMO`, `$NYSI`; [McClellan Financial](https://www.mcoscillator.com/) | Daily | Breadth |
| Equal-weight vs. cap-weight S&P (RSP:SPY) | Breadth | Any charting site | Daily | Breadth |
| Zweig Breadth Thrust | Breadth | Compute from `$NYADV`/`$NYDEC` | Rare | Breadth |
| High-yield OAS (ICE BofA) | Credit | FRED `BAMLH0A0HYM2` | Daily | Credit, Yield curve, Dashboard |
| Investment-grade / BBB / CCC spreads | Credit | FRED `BAMLC0A0CM`, `BAMLC0A4CBBB`, `BAMLH0A3HYC` | Daily | Credit |
| Funding spreads (CP–bill, SOFR vs. fed funds; TED discontinued) | Credit / funding | FRED `DCPF3M`, `DTB3`, `SOFR`, `DFF` | Daily | Credit |
| Chicago Fed NFCI / ANFCI | Financial conditions | [Chicago Fed](https://www.chicagofed.org/research/data/nfci/current-data); FRED `NFCI`, `ANFCI` | Weekly, Wednesday | Credit, Dashboard |
| Goldman Sachs / Bloomberg FCI | Financial conditions | Press coverage | Daily | Credit |
| M2 money supply | Liquidity | FRED `M2SL`; [H.6](https://www.federalreserve.gov/releases/h6/) | Monthly | Credit |
| Overnight reverse repo (RRP) | Liquidity | FRED `RRPONTSYD` | Daily | Credit |
| Treasury General Account | Liquidity | FRED `WTREGEN` | Weekly | Credit |
| US dollar index (DXY; Fed broad index) | Liquidity / global | Any quote site; FRED `DTWEXBGS` | Daily | Credit |
| Senior Loan Officer Opinion Survey (SLOOS) | Credit / lending | [Fed](https://www.federalreserve.gov/data/sloos.htm); FRED `DRTSCILM` | Quarterly | Credit |
| Bank loans and leases (H.8) | Credit / lending | FRED `TOTLL` | Weekly | Credit |
| Crude oil (WTI, Brent) | Commodity | FRED `DCOILWTICO`, `DCOILBRENTEU`; [EIA](https://www.eia.gov/petroleum/) | Daily | Commodities |
| Copper (and copper/gold ratio) | Commodity / growth | FRED `PCOPPUSDM`; [Trading Economics](https://tradingeconomics.com/commodity/copper) | Daily | Commodities |
| Gold | Commodity / monetary | [LBMA](https://www.lbma.org.uk/prices-and-data/precious-metal-prices); [World Gold Council](https://www.gold.org/goldhub/data/gold-prices) | Daily | Commodities |
| 10-year and 5-year breakeven inflation | Inflation expectations | FRED `T10YIE`, `T5YIE` | Daily | Commodities |
| 5-year, 5-year forward inflation rate | Inflation expectations | FRED `T5YIFR` | Daily | Commodities |
| Broad commodity indexes (GSCI, BCOM, CRB) | Commodity | [S&P GSCI](https://www.spglobal.com/spdji/en/indices/commodities/sp-gsci/); FRED `PALLFNFINDEXQ` | Daily / monthly | Commodities |
| Baltic Dry Index | Shipping / global demand | [Trading Economics](https://tradingeconomics.com/commodity/baltic) | Daily | Commodities |
| Container freight (Freightos FBX, Drewry WCI) | Shipping / supply chain | [Freightos](https://fbx.freightos.com/) | Weekly | Commodities |
| Retail gasoline prices | Inflation / sentiment | [EIA](https://www.eia.gov/petroleum/gasdiesel/); FRED `GASREGW` | Weekly, Monday | Commodities |
| Seasonal patterns (Sell in May, presidential cycle, Santa Claus rally, turn-of-month, September effect) | Calendar | [Stock Trader's Almanac](https://www.stocktradersalmanac.com/); academic papers linked in file | Annual | Seasonality |

## Key takeaways

- Everything worth watching is free; FRED alone covers roughly two-thirds of this table.
- Indicators come in families; the informative signal is agreement across families, never a single reading.
- Recession indicators (yield curve, Sahm rule, LEI, SLOOS) have excellent but imperfect records, and all misfired together in 2022–24.
- Valuation predicts ten-year returns well and one-year returns not at all.
- Sentiment and breadth work as contrarian and confirming tools at extremes, not in the middle.
- Credit spreads are the best free early warning; when they are calm, imminent bear-market risk is low.
- Calendar effects are mostly too weak to trade; use them to time actions you were taking anyway.
- As of September 2026 the composite picture is late-cycle: solid growth and internals, but stretched inflation, policy, real rates, credit complacency, and valuation.

## Sources

- [FRED, Federal Reserve Bank of St. Louis](https://fred.stlouisfed.org/)
- [Bureau of Labor Statistics](https://www.bls.gov/)
- [Bureau of Economic Analysis](https://www.bea.gov/)
- [Federal Reserve Board](https://www.federalreserve.gov/)
- [Federal Reserve Bank of New York: Yield Curve as a Leading Indicator](https://www.newyorkfed.org/research/capital_markets/ycfaq)
- [Federal Reserve Bank of Chicago: NFCI](https://www.chicagofed.org/research/data/nfci/current-data)
- [Institute for Supply Management](https://www.ismworld.org/)
- [The Conference Board](https://www.conference-board.org/)
- [Robert Shiller's online data](http://www.econ.yale.edu/~shiller/data.htm)
- [Cboe](https://www.cboe.com/)
- [AAII Sentiment Survey](https://www.aaii.com/sentimentsurvey)
- [StockCharts](https://stockcharts.com/)
- [Investopedia: Economic Indicators](https://www.investopedia.com/terms/e/economic_indicator.asp)
