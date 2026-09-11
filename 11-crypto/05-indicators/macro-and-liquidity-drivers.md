# Macro and Liquidity Drivers

**In one sentence:** Bitcoin has behaved far more like a high-beta liquidity asset than an inflation hedge, rising when money and risk appetite are expanding and falling when they contract, so the macro indicators that matter are the ones that measure liquidity and the price of money rather than inflation itself.

## The core finding first

The popular story is that Bitcoin protects against inflation. The evidence from the one real test, 2021–22, says the opposite: US CPI peaked at 9.1% in June 2022 while Bitcoin fell about 75% from its November 2021 high. What Bitcoin actually tracked was the reversal of liquidity: the Fed ending asset purchases, raising rates from zero to over 4% in a year, and shrinking its balance sheet. Bitcoin then bottomed in November 2022 within weeks of the peak in the dollar index and the trough in global money supply growth, and rallied through 2023 as liquidity conditions eased. The cleanest way to describe Bitcoin is a leveraged bet on global liquidity and risk appetite, with a scarcity narrative that occasionally lets it trade with gold. Most of the indicators below are ways to measure that.

## Global M2 and global liquidity

**What it measures.** Global M2 is the sum of broad money supply (cash, deposits, money-market funds) across the major economies (US, eurozone, China, Japan, UK and others), usually converted to dollars. "Global liquidity" indices (from CrossBorder Capital, or DIY versions using central bank balance sheets minus Treasury General Account minus reverse repo) try to capture the money available to financial markets more precisely.

**Where to get it free.** [Newhedge: Bitcoin vs Global M2](https://newhedge.io/bitcoin/bitcoin-vs-global-m2-growth), [TradingView global M2 scripts (search "Global M2")](https://www.tradingview.com/scripts/?q=global+m2), [FRED: US M2](https://fred.stlouisfed.org/series/M2SL), [FRED: Fed balance sheet (WALCL)](https://fred.stlouisfed.org/series/WALCL), [FRED: Treasury General Account](https://fred.stlouisfed.org/series/WTREGEN), [FRED: overnight reverse repo](https://fred.stlouisfed.org/series/RRPONTSYD).

**How to read it.** The year-over-year growth rate of global M2 is the variable, not the level. Bitcoin's 12-month return has tracked M2 growth with a lag that chart-makers put anywhere between 8 and 16 weeks; the lag is not stable and is partly curve-fitted. CF Benchmarks' review of the data found rolling four-year correlations of 0.4 to 0.6 historically, with Bitcoin's R-squared against M2 as high as 0.71 to 0.90 in 2022 but falling to about 0.59 by February 2026, when their M2 model implied a "fair value" near $136,000 against a price near $74,000, one of the widest gaps in the dataset. Gold's R-squared with M2 stayed around 0.72 to 0.80. Their conclusion was that every large gap in the past decade eventually closed in the direction of the liquidity trend, but not on any schedule.

**As of September 2026.** Global M2 growth was running above 10% year-over-year in early 2026 while Bitcoin's year-over-year return was negative, the "decoupling" widely discussed in crypto media. Explanations offered: the dollar's decline mechanically inflates dollar-denominated global M2 without adding real liquidity; the liquidity went to gold and AI equities instead; and treasury-company deleveraging created a crypto-specific supply overhang. Take the M2 charts as a background tailwind indicator, not a price target generator.

**Track record.** Good at explaining regimes in hindsight, poor at timing. The widely shared "M2 leads Bitcoin by 10 weeks" overlays worked in 2023–24 and failed badly in 2025–26.

## Real interest rates

**What it measures.** The nominal Treasury yield minus expected inflation. The cleanest series is the 10-year TIPS yield (the yield on inflation-protected Treasuries), which is a direct market price for the real cost of money. Rising real yields raise the opportunity cost of holding a non-yielding asset.

**Where to get it free.** [FRED: 10-year TIPS yield (DFII10)](https://fred.stlouisfed.org/series/DFII10), [FRED: 10-year breakeven inflation](https://fred.stlouisfed.org/series/T10YIE), [FRED: 10-year nominal yield](https://fred.stlouisfed.org/series/DGS10).

**How to read it.** Bitcoin's best years (2020–21, 2023–24) came with real yields negative or falling; its worst (2022) came with real yields rising from -1% to +1.5%. Gold has the same sensitivity, which is one reason the two correlate in liquidity-driven regimes. As of early September 2026 the 10-year nominal yield had reached about 4.8%, a cycle high per Glassnode's macro note, and with breakevens in the low 2s, real yields were above 2%, the most restrictive backdrop of the ETF era. That Bitcoin rallied 25% in August against that backdrop is unusual and is why many analysts flagged the rally as short-covering rather than macro-driven.

**Track record.** One of the strongest macro relationships for Bitcoin, better than headline inflation and better than M2 on a 3-to-6-month horizon.

## The dollar index (DXY)

**What it measures.** The value of the US dollar against a basket of major currencies (euro, yen, pound, Canadian dollar, Swedish krona, Swiss franc). A strong dollar tightens global financial conditions because so much world debt is dollar-denominated.

**Where to get it free.** [TradingView DXY](https://www.tradingview.com/symbols/TVC-DXY/), [MarketWatch DXY](https://www.marketwatch.com/investing/index/dxy), [FRED: broad dollar index](https://fred.stlouisfed.org/series/DTWEXBGS).

**How to read it.** Bitcoin has been inversely correlated with DXY in most windows since 2018, with the correlation strongest during trending dollar moves (the 2022 dollar spike to 114 coincided with the crypto bear; the 2023 dollar decline coincided with recovery). As of early September 2026 DXY sat near 99, weaker than late July despite hawkish Fed talk, a modest tailwind. Watch the direction over months, not the level.

**Track record.** Reliable inverse relationship in trending dollar regimes, weak in ranges.

## Risk-on correlation with the Nasdaq

**What it measures.** The rolling correlation of Bitcoin's daily returns with the Nasdaq 100 (or S&P 500), typically over 30, 60 or 90 days. High correlation means Bitcoin is trading as a tech-beta risk asset; low or falling correlation means it is trading on its own drivers or with gold.

**Where to get it free.** [TradingView correlation coefficient indicator (add to any BTC chart with NDX as the reference)](https://www.tradingview.com/support/solutions/43000502249-correlation-coefficient-cc/), [The Block: Bitcoin 30-day correlation to S&P 500 and gold](https://www.theblock.co/data/crypto-markets/prices/btc-pearson-correlation-30d), [Kaiko research (free posts)](https://research.kaiko.com/), [Coin Metrics State of the Network](https://coinmetrics.substack.com/).

**How to read it.** From 2020 through 2024 the 90-day BTC–Nasdaq correlation was mostly between 0.4 and 0.7, peaking near 0.8 in 2022. Correlation tends to spike during sell-offs (everything falls together) and fade during crypto-specific rallies. The notable 2026 development, reported by Protos and others on September 7, is a reversal: 90-day BTC–gold correlation at 0.56 (30-day at 0.72, the highest since tracking began in 2017) versus BTC–Nasdaq 100 at 0.30 (30-day 0.22, near a one-year low). Commentators labeled this the "debasement trade": Bitcoin and gold both rising on concerns about government debt and currency purchasing power while tech equities stalled. Whether it persists is unknown; the 2020 episode of gold correlation (about 0.5 in November 2020) lasted only a few months before Bitcoin re-coupled with tech.

**Track record.** Correlation is descriptive, not predictive, but it tells you which macro chart to watch this quarter. When correlation with Nasdaq is high, Bitcoin is a Fed-and-earnings trade; when correlation with gold is high, it is a real-yields-and-dollar trade.

## Fed policy and the rate path

**What it measures.** The federal funds target range, the market's expected path (from fed funds futures), the pace of balance sheet runoff (quantitative tightening) and forward guidance. The rate path matters more than the current level.

**Where to get it free.** [CME FedWatch tool](https://www.cmegroup.com/markets/interest-rates/cme-fedwatch-tool.html), [Federal Reserve FOMC calendar and statements](https://www.federalreserve.gov/monetarypolicy/fomccalendars.htm), [FRED: effective fed funds rate](https://fred.stlouisfed.org/series/DFF), [Trading Economics US interest rate](https://tradingeconomics.com/united-states/interest-rate).

**How to read it.** Bitcoin's large moves have clustered around changes in the expected path: the December 2021 pivot to hawkishness, the late-2023 "pivot" rally when cuts were priced in, and the 2024 cutting cycle. The direction of surprise matters more than the decision. As of early September 2026 the target range was 3.50% to 3.75%, unchanged since December 2025, but after Chair Warsh's hawkish Jackson Hole speech on August 28 markets began pricing a quarter-point hike at the September 16 meeting as the more likely outcome, with July CPI at 3.4% headline and 2.5% core. A hiking cycle restarting with real yields above 2% would be a genuine headwind; a surprise hold would likely be met with relief.

**Track record.** Fed path shifts explain a large share of Bitcoin's multi-month moves since 2021. Individual meeting days are usually noise.

## Treasury liquidity: TGA, reverse repo and bank reserves

**What it measures.** The plumbing behind the headline rate. When the Treasury's cash account (TGA) rises (tax season, post-debt-ceiling rebuilding), it drains reserves from the banking system; when the Fed's reverse repo facility (RRP) drains, it releases liquidity into markets. "Net liquidity" (Fed balance sheet minus TGA minus RRP) is a popular way to combine them.

**Where to get it free.** [FRED: TGA (WTREGEN)](https://fred.stlouisfed.org/series/WTREGEN), [FRED: RRP (RRPONTSYD)](https://fred.stlouisfed.org/series/RRPONTSYD), [FRED: bank reserves (WRESBAL)](https://fred.stlouisfed.org/series/WRESBAL), [Treasury Fiscal Data: daily Treasury statement](https://fiscaldata.treasury.gov/datasets/daily-treasury-statement/).

**How to read it.** Net liquidity rising has coincided with crypto rallies (the 2023 RRP drawdown offset quantitative tightening and supported the recovery). TGA rebuilds after debt-ceiling deals (mid-2023, mid-2025) have coincided with choppy or weak periods. These are weeks-to-months signals with lots of noise; use them to explain why price is fighting the trend, not to trade.

**Track record.** Modest, but the 2023 episode made this a standard part of macro-crypto analysis for good reason.

## Bitcoin as inflation hedge versus liquidity asset: what the evidence says

The academic and practitioner literature, plus the last two cycles, supports these statements:

- Bitcoin's correlation with realized CPI is close to zero and its reaction to hot inflation prints has been negative (because hot prints imply tighter policy). It does not hedge inflation on horizons of months to a couple of years.
- Bitcoin's correlation with liquidity measures (real yields, M2 growth, net liquidity, dollar direction) is meaningful and the sign is consistent: easier money, higher Bitcoin.
- Bitcoin's beta to equities during risk-off episodes has been 2 to 3 times the Nasdaq's; it has fallen further, not held up, in every equity drawdown since 2018 (March 2020, 2022, August 2024, early 2026).
- The "digital gold" behavior appears intermittently, usually when the driver is currency debasement fear rather than growth fear: late 2020 and, per the correlation data, mid-2026. It has not yet been tested in a full recession.
- Over 10-plus years the case is different: Bitcoin has enormously outpaced inflation, so as a long-duration store of value against currency debasement it has worked, but only for holders who could sit through 75 to 85% drawdowns.

The practical conclusion: if you own Bitcoin as a hedge, treat it as a hedge against monetary expansion and financial repression, not against a CPI print, and size it knowing it will fall with stocks in a crisis.

## How to use it

1. Once a month, update four numbers: 10-year TIPS real yield, DXY direction, global M2 growth (YoY) and the market-implied Fed path. That is 90% of the macro picture for crypto.
2. Check which correlation regime you are in (Nasdaq or gold) using a 90-day correlation chart, and watch the corresponding driver more closely.
3. Use net-liquidity plumbing (TGA, RRP) to explain short-term choppiness, not to forecast.
4. Do not buy Bitcoin because CPI is high. Buy it, if at all, because policy is about to get easier or liquidity is expanding.
5. Expect Bitcoin to fall with risk assets in a shock, regardless of the narrative of the moment. Position size accordingly.
6. Be suspicious of any chart that "proves" M2 leads Bitcoin by exactly N weeks; the lag is fitted, and 2025–26 broke it.

## Key takeaways

- Bitcoin is a liquidity asset first: real yields, dollar direction and the Fed's expected path explain most of its multi-month moves.
- The inflation-hedge story failed its 2021–22 test; Bitcoin fell 75% while inflation peaked, because inflation brought tightening.
- Global M2 overlays are useful background and terrible timing tools; the relationship weakened sharply in 2025–26 (R-squared down to about 0.59).
- Rising real yields (above 2% as of September 2026) are the most restrictive macro backdrop of the ETF era, which makes the August 2026 rally look more like positioning than macro.
- Correlation regimes shift: 2020–24 was a Nasdaq-beta regime; mid-2026 shows the strongest gold correlation on record and the weakest Nasdaq link in a year.
- In equity crashes Bitcoin has always fallen harder than stocks; "digital gold" has not yet been tested by a recession.
- As of September 2026: fed funds 3.50–3.75% with a possible hike on September 16, 10-year at about 4.8%, DXY near 99, headline CPI 3.4%. Mixed-to-restrictive, with the dollar the only clear tailwind.

## Sources

- [CF Benchmarks: The M2–Bitcoin relationship, what the data actually shows](https://www.cfbenchmarks.com/blog/the-m2-bitcoin-relationship-what-the-data-actually-shows)
- [BeInCrypto: What analysts say as Bitcoin decouples from global M2 in 2026](https://beincrypto.com/bitcoin-decouple-from-global-m2-in-2026/)
- [Yahoo Finance: Bitcoin continues to decouple from global M2 in early 2026](https://finance.yahoo.com/news/bitcoin-continues-decouple-global-m2-134022834.html)
- [Newhedge: Bitcoin vs Global M2 growth](https://newhedge.io/bitcoin/bitcoin-vs-global-m2-growth)
- [Hokanews (citing Protos): Bitcoin–gold correlation hits nine-year high, Nasdaq link at one-year low (September 7, 2026)](https://www.hokanews.com/2026/09/bitcoin-gold-correlation-hits-nine-year.html)
- [CoinDesk: Bitcoin–Nasdaq correlation turns positive (February 17, 2026)](https://www.coindesk.com/markets/2026/02/17/crypto-slides-as-tech-stocks-and-gold-retreat-bitcoin-nasdaq-correlation-turns-positive)
- [Cambridge Currencies: Fed decision preview, September 16, 2026](https://cambridgecurrencies.com/next-federal-reserve-interest-rate-decision/)
- [Glassnode Week On-Chain, Week 35 2026 (10-year yield at cycle high)](https://research.glassnode.com/the-week-onchain-week-35-2026/)
- [FRED: 10-year TIPS yield](https://fred.stlouisfed.org/series/DFII10)
- [CME FedWatch](https://www.cmegroup.com/markets/interest-rates/cme-fedwatch-tool.html)
- [Fortune: Price of Bitcoin, September 3, 2026](https://fortune.com/article/price-of-bitcoin-09-03-2026/)
