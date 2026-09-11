# Commodity and Inflation Signals

**In one sentence:** Commodity prices (oil, copper, gold), market-implied inflation expectations (TIPS breakevens and the 5y5y forward), broad commodity indexes, and shipping rates are real-time votes on global growth and inflation that arrive months before the official statistics, which makes them useful cross-checks on the macro data even though each is noisy and driven by its own supply story.

## What commodities tell you that CPI can't

The Consumer Price Index arrives two weeks after the month ends and is dominated by slow-moving components like rent. Commodity prices trade every second and respond immediately to demand, supply, and expectations. That gives them two uses: as early signals of inflation pressure (oil feeds into gasoline and transport within weeks; metals into manufacturing costs within months) and as signals of global growth (copper, shipping rates, and broad commodity indexes rise when the world's factories are busy).

The catch is that every commodity has a supply side that has nothing to do with the economy: OPEC decisions, wars, strikes at Chilean mines, droughts, ship-building cycles. A copper rally may mean "China is booming" or "a mine flooded." So read commodities in groups and cross-check them against the market-implied inflation measures, which are pure demand-and-expectations gauges with no supply story.

## The indicators

| Indicator | What it measures | Free source | Frequency | How to read it | Track record / notes |
|---|---|---|---|---|---|
| **Crude oil (WTI, Brent)** | Price of the marginal barrel; WTI is the US benchmark, Brent the global one | FRED [`DCOILWTICO`](https://fred.stlouisfed.org/series/DCOILWTICO), [`DCOILBRENTEU`](https://fred.stlouisfed.org/series/DCOILBRENTEU); [EIA](https://www.eia.gov/petroleum/) | Daily | Rule of thumb: each sustained $10 rise adds ~0.2–0.3 points to headline CPI over the following months and trims ~0.1–0.2 points from GDP growth. A doubling of oil within a year has preceded most US recessions (1973, 1979, 1990, 2008); James Hamilton's work is the reference. | Oil spikes are demand-killers; oil collapses (2014–16, 2020) hurt energy stocks and credit but help consumers. **WTI ~$97–100 on September 10–11, 2026**, up ~20% in a month, after the spring's Iran/Strait of Hormuz disruption pushed it above $110 and a summer retreat to the $70s. |
| **Copper ("Dr. Copper")** | Industrial metal used in construction, wiring, and electronics; said to have "a PhD in economics" | FRED [`PCOPPUSDM`](https://fred.stlouisfed.org/series/PCOPPUSDM) (monthly, IMF); daily via [Trading Economics](https://tradingeconomics.com/commodity/copper) or any quote site (COMEX HG) | Daily | Rising copper = global industrial demand strong (China is ~50% of consumption). The **copper/gold ratio** is a cleaner growth signal: it strips out the dollar and tends to track the 10-year Treasury yield. | Copper's diagnosis is right more often than wrong but has fooled people: it was strong in 2007 and 2021 near market tops, and it rallied on supply fears (mine disruptions, tariffs, electrification demand) in 2024–26 independent of the cycle. About $6.47/lb on September 11, 2026, near record highs. |
| **Gold** | Monetary metal; responds to real interest rates, the dollar, central-bank buying, and fear | FRED [`GOLDAMGBD228NLBM`](https://fred.stlouisfed.org/series/GOLDAMGBD228NLBM) (daily London fix, discontinued 2024; use [LBMA](https://www.lbma.org.uk/prices-and-data/precious-metal-prices) or any quote site); [World Gold Council](https://www.gold.org/goldhub/data/gold-prices) | Daily | Classic driver: gold rises when *real* yields fall (negative real rates in 2011 and 2020 = gold peaks). Since 2022 that link weakened: gold rose alongside 2%+ real yields, driven by central-bank purchases (China, Poland, Turkey, India) after Russian reserves were frozen, and by sovereign-debt worries. | Gold is not an inflation hedge over 1–5 years (it fell 1980–2000 through plenty of inflation); it is a hedge against monetary disorder and negative real rates. About **$4,490/oz on September 3, 2026**, up ~26% year-over-year and at record highs. |
| **10-year breakeven inflation rate** | Yield on the nominal 10-year Treasury minus the yield on the 10-year TIPS; the inflation rate at which the two would return the same | FRED [`T10YIE`](https://fred.stlouisfed.org/series/T10YIE) | Daily | The market's average expected CPI inflation over 10 years, plus a small risk premium. The Fed's 2% PCE target equals roughly 2.3–2.5% CPI. Above 2.75% = markets doubt the Fed; below 1.5% = deflation scare (2008, 2020). | Breakevens correctly signaled the 2021 inflation surge months before the Fed conceded it. 2.40% on September 11, 2026: anchored despite 3%+ current inflation and $100 oil. |
| **5-year breakeven** | Same for five years; more sensitive to oil | FRED [`T5YIE`](https://fred.stlouisfed.org/series/T5YIE) | Daily | Moves with energy; the 5-year minus 10-year gap tells you whether the market sees inflation as transitory (5yr > 10yr) or persistent. | 2.46% on September 11, 2026, slightly above the 10-year: the market sees the oil shock fading. |
| **5-year, 5-year forward inflation rate** | Expected average inflation over the five-year period beginning five years from now; strips out the near-term noise | FRED [`T5YIFR`](https://fred.stlouisfed.org/series/T5YIFR) | Daily | This is the Fed's favorite "are expectations anchored?" gauge. Stable 2.0–2.5% = anchored. A sustained move above 2.75% would be a genuine credibility problem. | Stayed anchored throughout the 2021–23 inflation, which is one reason the Fed felt able to be patient. 2.34% on September 11, 2026. |
| **Real yields (10-year TIPS)** | Inflation-adjusted risk-free rate | FRED [`DFII10`](https://fred.stlouisfed.org/series/DFII10) | Daily | Covered in the interest-rates file; the driver of gold and growth-stock valuations. | 10-year nominal 4.73% (end of August 2026) minus 2.40% breakeven = real yield about 2.3%, historically restrictive. |
| **Broad commodity indexes** | Baskets of futures: S&P GSCI (energy-heavy, ~60% oil and gas), Bloomberg Commodity Index (BCOM, capped at 33% per sector), Refinitiv/CoreCommodity CRB | [S&P GSCI](https://www.spglobal.com/spdji/en/indices/commodities/sp-gsci/), [BCOM](https://www.bloomberg.com/professional/product/indices/bloomberg-commodity-index-family/); ETFs GSG and DJP as proxies; FRED [`PALLFNFINDEXQ`](https://fred.stlouisfed.org/series/PALLFNFINDEXQ) (IMF all-commodity index, monthly) | Daily | Year-over-year change leads headline CPI by 3–6 months. A broad rally across energy, metals, and agriculture is a stronger growth/inflation signal than any single commodity. | Commodity super-cycles (1970s, 2002–08, 2020–22) coincided with inflation problems; long commodity bear markets (1980–2000, 2011–20) with disinflation. Also a useful equity-market diversifier only in inflationary regimes. |
| **Baltic Dry Index (BDI)** | Daily cost of chartering bulk ships (capesize, panamax, supramax) for iron ore, coal, grain | [Trading Economics](https://tradingeconomics.com/commodity/baltic); [Investing.com](https://www.investing.com/indices/baltic-dry-historical-data) (no FRED series) | Daily | Higher = more demand to move raw materials = stronger global industrial activity. The index cannot be speculated on directly, which makes it a "pure" demand signal, but ship supply is inelastic, so small demand changes cause huge swings. | Famous for peaking at 11,793 in May 2008 and collapsing 94% by December; low of 290 in 2016. Since then vessel oversupply has muted it. 3,521 on September 10, 2026, on the firm side of its post-2010 range. |
| **Container freight rates (Freightos, Drewry WCI)** | Cost of shipping a 40-foot container on major routes | [Freightos Baltic Index](https://fbx.freightos.com/); [Drewry WCI](https://www.drewry.co.uk/supply-chain-advisors/supply-chain-expertise/world-container-index-assessed-by-drewry) | Weekly | Consumer-goods supply-chain gauge; spiked 5–10x in 2021 and again with Red Sea disruptions in 2024. | Better than BDI for tracking finished-goods inflation pressure. |
| **Gasoline prices** | What consumers actually see | [EIA weekly retail gasoline](https://www.eia.gov/petroleum/gasdiesel/); FRED [`GASREGW`](https://fred.stlouisfed.org/series/GASREGW); [AAA](https://gasprices.aaa.com/) | Weekly (Monday) | Each $1/gallon sustained rise costs US households roughly $100–120 billion a year; strongly linked to consumer-sentiment readings and presidential approval. | The single fastest transmission channel from commodities to sentiment. |

## Reading the current picture (as of September 11, 2026)

The commodity complex is sending a split message. **Oil at ~$100** is a supply shock (Hormuz), not a demand boom, and it is doing what oil shocks do: pushing headline CPI up (3.4%), crushing consumer sentiment (UMich 51.7), and forcing a Fed that had been on hold to consider hiking. **Copper near records** and a **firm Baltic Dry Index** say global industrial demand is fine, consistent with ISM manufacturing at 54.6. **Gold at $4,500** says investors want insurance against policy error and sovereign-debt trouble. And the **breakevens at 2.3–2.5%** say the bond market still trusts the Fed to bring inflation back down.

The historical pattern to keep in mind: an oil shock into an economy running near full employment with an already-elevated inflation rate is the 1973 and 1979 script. Both times the Fed was forced to tighten into the shock, and both produced recessions and bear markets within 12–18 months. The anchored 5y5y is the main difference this time; if it starts to drift above 2.75%, that difference is gone.

## How to use it

1. **Watch year-over-year changes, not levels.** A commodity index up 30% year-over-year means headline CPI will rise over the next 3–6 months regardless of what the Fed says; down 20% means the reverse.
2. **Use breakevens to separate signal from noise.** If oil spikes and 10-year breakevens barely move, the market sees it as transitory and you probably should too. If breakevens and the 5y5y rise together with oil, the regime is changing.
3. **Check the copper/gold ratio against the 10-year yield.** When the ratio falls while yields rise (or vice versa), one of them is wrong; historically the ratio has led.
4. **Treat gold as portfolio insurance, sized small.** A 5–10% allocation has historically improved risk-adjusted returns; treating it as a trade on inflation prints has not.
5. **Don't extrapolate supply shocks.** Prices driven by wars and cartels reverse when the disruption ends (oil fell from $110 to $70 between April and June 2026 on cease-fire news). Demand-driven moves persist longer.
6. **Remember commodities are a diversifier only in inflationary regimes.** In deflationary busts (2008, 2020) they fall with stocks.

## Key takeaways

- Commodity prices are real-time votes on growth and inflation that arrive months before CPI, but each has a supply story that can mislead.
- Oil shocks have preceded most US recessions; WTI near $100 in September 2026 is the biggest macro risk on the board.
- Copper and shipping rates say global industrial demand is currently solid, consistent with the PMI data.
- Gold at record highs (~$4,500) reflects central-bank buying and policy-risk hedging more than current inflation; it is not a reliable short-term inflation hedge.
- TIPS breakevens (2.40% 10-year) and the 5y5y forward (2.34%) are the cleanest reads on inflation expectations, and they remain anchored; watch for a sustained move above 2.75%.
- Broad commodity indexes lead headline CPI by 3–6 months; the Baltic Dry Index is a pure but noisy demand gauge.
- All of these are free on FRED, EIA, LBMA, and Trading Economics.

## Sources

- [FRED: 10-Year Breakeven Inflation Rate (T10YIE)](https://fred.stlouisfed.org/series/T10YIE)
- [FRED: 5-Year, 5-Year Forward Inflation Expectation Rate (T5YIFR)](https://fred.stlouisfed.org/series/T5YIFR)
- [CondorEdge: Breakeven inflation dashboard](https://condoredge.com/econ/breakeven-inflation)
- [Convextrade: WTI crude oil price today](https://convextrade.com/today/oil-price)
- [Wikipedia: 2026–2028 world oil market chronology](https://en.wikipedia.org/wiki/2026%E2%80%932028_world_oil_market_chronology)
- [Fortune: Current price of gold, September 3, 2026](https://fortune.com/article/current-price-of-gold-09-03-2026/)
- [MetalCharts: Copper price](https://metalcharts.org/copper-price)
- [Trading Economics: Baltic Dry Index](https://tradingeconomics.com/commodity/baltic)
- [Trading Economics: Copper](https://tradingeconomics.com/commodity/copper)
- [S&P Global: Copper and gold market outlook 2026](https://www.spglobal.com/market-intelligence/en/news-insights/research/2026/04/copper-gold-market-outlook-2026-prices-supply-mining-costs)
- [EIA: Petroleum and other liquids](https://www.eia.gov/petroleum/)
- [World Gold Council: Gold prices](https://www.gold.org/goldhub/data/gold-prices)
- [Kiplinger: August CPI preview (oil at $100)](https://www.kiplinger.com/investing/economy/cpi-report-august-2026-what-to-expect)
