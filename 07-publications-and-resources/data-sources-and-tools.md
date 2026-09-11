# Data Sources and Tools

**In one sentence:** Almost everything a serious individual investor needs — prices, fundamentals, filings, macro data, backtesting, portfolio tracking, and even raw API access — is free or nearly free, and this page lists the best option for each job with its cost and its catch.

Two warnings before the tables. First, prices change; the figures below were checked in September 2026 and are rounded, so confirm on the pricing page before you pay. Second, more data does not make you a better investor. Most people on this site would be well served by FRED, EDGAR, one fundamentals site, one backtester, and their broker's tools. The rest is for specific jobs.

## Official and primary sources (free)

| Tool | Cost | Best for | Notes |
|---|---|---|---|
| [FRED (St. Louis Fed)](https://fred.stlouisfed.org/) | Free | Every US macro series: rates, inflation, employment, money supply, yield curves, plus many international series | 800,000+ series, chartable and downloadable, with an API and Excel add-in. If someone quotes a macro statistic, FRED is where you check it. |
| [EDGAR full-text search (SEC)](https://www.sec.gov/edgar/search/) | Free | Searching the text of every SEC filing since 2001 — 10-Ks, 10-Qs, proxies, 13Fs, S-1s | Search for a phrase ("going concern," a customer's name, an executive) across all filings. The company-search page at [sec.gov/edgar](https://www.sec.gov/edgar/searchedgar/companysearch) gets you one company's filing history. |
| [Shiller data (Yale)](http://www.econ.yale.edu/~shiller/data.htm) | Free | Monthly US stock prices, dividends, earnings, CAPE, and rates since 1871 | The spreadsheet behind *Irrational Exuberance*. Download it once and you can compute historical valuations yourself. |
| [Kenneth French Data Library](https://mba.tuck.dartmouth.edu/pages/faculty/ken.french/data_library.html) | Free | Fama-French factor returns (market, size, value, profitability, investment, momentum) for the US and international markets, monthly since 1926 | The source data for most factor research. Anyone testing a "value" or "small-cap" claim should start here. |
| [Damodaran data (NYU Stern)](https://pages.stern.nyu.edu/~adamodar/New_Home_Page/data.html) | Free | Industry-level betas, margins, multiples, cost of capital, and equity risk premiums, updated every January | Damodaran's own spreadsheets, used in his valuation course. The equity risk premium page is the standard reference. |
| [TreasuryDirect](https://www.treasurydirect.gov/) | Free | Buying Treasury bills, notes, bonds, TIPS, and I bonds directly; historical auction results | Clunky interface, no fees. The daily yield curve data is also published here. |
| [Investor.gov (SEC)](https://www.investor.gov/) | Free | Compound interest and RMD calculators; checking an advisor's registration; plain-English explanations of products | See the regulators file for detail. |

## Quotes, screening, and charts

| Tool | Cost | Best for | Notes |
|---|---|---|---|
| [Yahoo Finance](https://finance.yahoo.com/) | Free; Premium about $35/month | Quotes, news, basic financials, options chains, historical prices to download | Still the default free quote site. Historical price downloads are handy; the fundamentals are shallow. |
| [Google Finance](https://www.google.com/finance/) | Free | Quick quotes and simple portfolio tracking inside Google Sheets via `GOOGLEFINANCE()` | The Sheets function is the real product: free live and historical prices in any spreadsheet. |
| [Finviz](https://finviz.com/) | Free; Elite about $40/month | Stock screener with dozens of filters, heat maps, insider trades, and quick charts | The fastest free screener on the web. Elite adds real-time data, backtesting, and more filters; most people never need it. |
| [TradingView](https://www.tradingview.com/) | Free; paid from about $15/month | Charts for anything (stocks, ETFs, futures, crypto, macro), with community scripts and a screener | Best charting tool available to individuals. The free tier has ads and limits on indicators and saved layouts. |
| [StockAnalysis.com](https://stockanalysis.com/) | Free; Pro about $10/month | Clean financial statements (10+ years), ratios, ETF holdings, IPO calendars, and a screener | The best free fundamentals site: fast, no clutter, and exportable. Pro extends history to 30+ years and adds more export. |
| [Macrotrends](https://www.macrotrends.net/) | Free (ad-supported) | Long-term charts of a company's revenue, margins, P/E, or any macro series back decades | Ugly and ad-heavy, but it is the quickest way to see 20 years of a company's metric on one chart. |
| [Koyfin](https://www.koyfin.com/) | Free; Plus $39/month; Premium $79/month | Dashboards, financial analysis, macro and fund data, and custom charts approaching Bloomberg-lite | The best free "terminal" for individuals. Plus unlocks 10-year financials and unlimited watchlists. |
| [TIKR](https://www.tikr.com/) | Free tier; paid from about $15/month | S&P Capital IQ-sourced financials, estimates, transcripts, and superinvestor tracking for global stocks | Better global coverage and analyst estimates than most free tools; the free tier is generous. |
| [Simply Wall St](https://simplywall.st/) | Free; Premium about $10/month | Visual snapshot of a company's valuation, growth, health, and dividend, plus portfolio tracking | Good for beginners who want to understand a stock quickly. Its "fair value" figures are automated DCFs; treat them as a starting point, not an answer. |
| [Seeking Alpha](https://seekingalpha.com/) | Free (limited); Premium about $300/year | Crowd-sourced analysis, earnings call transcripts, and dividend data | Transcripts and news are the value; the articles range from excellent to promotional, so check the author's history. |
| [Morningstar](https://www.morningstar.com/) | Free articles and basic data; Investor about $250/year | Fund and ETF research, star ratings, portfolio X-Ray, and the annual "Mind the Gap" investor-return study | The standard for fund analysis. Free data covers expense ratios, holdings, and basic performance; the paid tier adds analyst reports and X-Ray. |
| [GuruFocus](https://www.gurufocus.com/) | Free (limited); Premium from about $500/year | Guru portfolio tracking, 30-year financials, and dozens of value-investing screens and scores | Aimed at value investors. Pricey; useful mainly for the guru and insider data and long financial histories. |
| [Fiscal.ai (formerly FinChat)](https://fiscal.ai/) | Free tier; paid from about $25/month | Segment-level KPIs (subscribers, stores, units), financials, and an AI assistant for research questions | Its edge is company-specific operating metrics that are hard to find elsewhere. |

## Following the professionals: 13F and insider data

| Tool | Cost | Best for | Notes |
|---|---|---|---|
| [Dataroma](https://www.dataroma.com/) | Free | Holdings of 80+ "superinvestors" (Buffett, Ackman, Klarman, Einhorn) from 13F filings, plus insider buys | Simple and free. 13Fs are filed up to 45 days after quarter-end, so positions can be stale; use them for ideas, not for copying. |
| [WhaleWisdom](https://whalewisdom.com/) | Free basics; premium tiers | 13F, 13D, and Form 4 data for every filer, with backtesting of hedge-fund clone portfolios | More complete than Dataroma, harder to read. The free tier covers most needs. |
| [OpenInsider](http://www.openinsider.com/) | Free | Screening SEC Form 4 insider purchases and sales in real time | The fastest way to see cluster buying by executives. Plain-text site, no frills. |

## Backtesting, planning, and retirement calculators

| Tool | Cost | Best for | Notes |
|---|---|---|---|
| [Portfolio Visualizer](https://www.portfoliovisualizer.com/) | Free tier (limited history and features); Basic from about $30–40/month | Backtesting asset allocations and tickers, Monte Carlo, factor regression, and efficient frontiers | The standard tool for a decade. In 2024 it moved most features behind a paywall, which is why the two alternatives below exist. |
| [Portfolio Charts](https://portfoliocharts.com/) | Free, no ads | Comparing asset allocations on long-term risk and return, safe withdrawal rates, and "how long to financial independence" charts | A labor of love by one investor. The Portfolio Matrix and Withdrawal Rates tools are unusually clear, and it covers non-US home currencies. |
| [testfol.io](https://testfol.io/) | Free | Backtesting tickers and allocations with rebalancing, cashflows, and leverage, using synthetic long histories | Fast, free, and increasingly the community favorite since Portfolio Visualizer went paid. Check the data notes on synthetic history before trusting pre-inception returns. |
| [FI Calc](https://ficalc.app/) | Free | Historical retirement simulations with flexible withdrawal strategies (constant dollar, percentage, Guyton-Klinger, and more) | The cleanest free retirement calculator. Pairs well with the Early Retirement Now safe-withdrawal series. |
| [cFIREsim](https://www.cfiresim.com/) | Free | Historical-cycle retirement simulation with detailed income and spending inputs | Older and more configurable than FI Calc; both use Shiller-style data since 1871. |
| [FINRA Fund Analyzer](https://tools.finra.org/fund_analyzer/) | Free | Comparing the total cost of any mutual funds and ETFs over time, including loads and expense ratios | Type in two funds and see the dollar difference over 10 or 20 years. Nothing else makes fees this concrete. |
| [Empower Personal Dashboard](https://www.empower.com/tools/net-worth) | Free (expect a sales call for their advisory service) | Aggregating every account into one net-worth view, fee analyzer, retirement planner | The former Personal Capital dashboard. The free tools are good; decline the advisory pitch unless you want it. |
| [Bogleheads wiki tools and calculators](https://www.bogleheads.org/wiki/Tools_and_calculators) | Free | Spreadsheets for asset allocation, tax-efficient placement, Social Security timing, and the Simba backtesting spreadsheet | Volunteer-built and unglamorous, but the Simba spreadsheet (returns since 1871 for dozens of asset classes) is a research tool in its own right. |

## Your broker's tools (already paid for)

If you have an account at [Fidelity](https://www.fidelity.com/), [Schwab](https://www.schwab.com/), or [Vanguard](https://investor.vanguard.com/), you already have a research library, screeners, Morningstar and other third-party reports, and retirement planners at no extra cost. Fidelity's and Schwab's screeners are as good as most paid tools for US stocks and funds. Check them before subscribing to anything.

## Professional platforms (for context, not a recommendation)

| Tool | Cost | Best for | Notes |
|---|---|---|---|
| [Bloomberg Terminal](https://www.bloomberg.com/professional/products/bloomberg-terminal/) | About $25,000–30,000/year | Everything, in real time, plus the chat network that runs Wall Street | Listed so you know what the pros use. Koyfin, TIKR, and Fiscal.ai now cover most of what an individual would use it for. |
| [FactSet](https://www.factset.com/) and [S&P Capital IQ](https://www.spglobal.com/marketintelligence/en/solutions/sp-capital-iq-pro) | Five figures per year | Institutional fundamentals, estimates, and screening | TIKR licenses Capital IQ data, which is the cheap way in. |
| [YCharts](https://ycharts.com/) | From about $300/month | Advisor-grade charting, fund comparison, and client reports | Good product for advisors; overkill for individuals, who get most of it from Koyfin. |

## APIs and data for tinkerers

| Source | Cost | Best for | Notes |
|---|---|---|---|
| [FRED API](https://fred.stlouisfed.org/docs/api/fred/) | Free | Pulling any FRED series into Python, R, or a spreadsheet | The `fredapi` Python package makes this a few lines. |
| [SEC EDGAR APIs](https://www.sec.gov/search-filings/edgar-application-programming-interfaces) | Free | Company facts, XBRL financial data, and filing indexes as JSON | Requires a user-agent header and a 10-requests-per-second limit; otherwise open. The `edgartools` and `sec-api` packages wrap it. |
| [Alpha Vantage](https://www.alphavantage.co/) | Free (25 requests/day); premium from about $50/month | Daily and intraday prices, fundamentals, forex, and technical indicators | The classic hobbyist API. The free rate limit is tight; fine for a personal dashboard, not for scanning the market. |
| [Massive (formerly Polygon.io)](https://massive.com/) | Free (5 calls/minute, 2 years history); Starter $29/month | Real-time and historical US stocks, options, forex, and crypto with WebSocket streaming | Polygon rebranded as Massive in early 2026. The best-documented market data API for developers; paid tiers add years of history and real-time access. |
| [Financial Modeling Prep](https://site.financialmodelingprep.com/) | Free tier (about 250 requests/day); paid from about $20/month | 30 years of financial statements, ratios, DCF inputs, and quotes for global stocks | The broadest cheap fundamentals API. Check data quality on smaller companies. |
| [Tiingo](https://www.tiingo.com/) | Free tier; paid from about $10/month | End-of-day prices, fundamentals, and news, with a reputation for clean data | Popular with quant hobbyists for its price-history accuracy. |
| [EOD Historical Data](https://eodhd.com/) | From about $20/month | Global end-of-day prices, fundamentals, and options across 60+ exchanges | Best value for non-US coverage. |
| [OpenBB](https://openbb.co/) | Free, open source | An open-source terminal and Python platform that unifies dozens of the data sources above into one interface | OpenBB open-sourced its full product suite in 2026. If you code, this is the place to start building. |
| [yfinance (Python)](https://github.com/ranaroussi/yfinance) | Free | Pulling Yahoo Finance prices and fundamentals into pandas | Unofficial and occasionally breaks when Yahoo changes its site, but it is what most tutorials use. |

## Which to use for what

- **"Is this macro claim true?"** → FRED.
- **"What does the company say about itself?"** → EDGAR full-text search, then the 10-K.
- **"Show me 10 years of this company's financials."** → StockAnalysis.com (free) or Koyfin/TIKR (deeper).
- **"Screen for cheap, profitable companies."** → Finviz (quick) or your broker's screener (deeper).
- **"Would this allocation have worked?"** → Portfolio Charts or testfol.io (free), Portfolio Visualizer (paid).
- **"Can I retire on this?"** → FI Calc, then read Early Retirement Now.
- **"What are the good investors buying?"** → Dataroma.
- **"What does this fund really cost?"** → FINRA Fund Analyzer.
- **"I want to build something."** → FRED API, EDGAR APIs, Massive or FMP, OpenBB.

## Key takeaways

- The primary sources — FRED, EDGAR, Shiller, French, Damodaran — are free, authoritative, and underused; go to them before any commercial site.
- For fundamentals, StockAnalysis.com (free) and Koyfin or TIKR (freemium) now cover what individual investors used to pay hundreds a month for.
- Portfolio Visualizer went mostly paid in 2024; Portfolio Charts and testfol.io are free and good enough for almost everyone.
- Your brokerage already includes screeners, research, and planners; check them before subscribing to anything.
- If you write code, FRED, EDGAR, and Massive/FMP APIs plus OpenBB give you a research stack that would have cost a fund six figures fifteen years ago.
