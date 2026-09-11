# Stock Screening

**In one sentence:** A stock screen is a filter that turns 6,000 listed companies into a list of 20 worth reading about, and the skill lies in choosing criteria that reflect what actually predicts returns rather than what merely looks good on a dashboard.

## What a screen is for (and is not for)

A screen is a search tool, not a decision tool. It answers "which companies match these numeric conditions right now?" It cannot tell you whether the numbers are accurate, whether earnings are about to collapse, or whether a cheap stock is cheap for a good reason. Every screen produces a mix of genuine opportunities and value traps, and the next step is always reading the filings.

Good screens have three properties: they rest on factors with academic support (value, quality, momentum, low volatility, size), they use a manageable number of criteria (three to seven), and they are run consistently so you can learn which of your screens actually produce winners.

## Building a screen: the logic

1. **Start with a thesis.** "I want profitable, growing companies that are cheaper than their growth rate" is a thesis. "P/E under 15" is not.
2. **Translate the thesis into 3–7 filters.** Too few and you get hundreds of names; too many and you overfit to a handful.
3. **Add hygiene filters.** Minimum market cap (e.g., $300M+) to avoid illiquid micro-caps, minimum average volume, and often a U.S.-listing or exchange filter to exclude OTC shells.
4. **Sort by the metric that matters most** for your thesis, not alphabetically.
5. **Export the list** and read the top 20 filings. Track which screens produced the stocks you actually bought and how they did.

## The best free screeners

| Screener | Free tier | What it does best | Limits / paid tier |
|---|---|---|---|
| **Finviz** | Yes, ad-supported, delayed data | Speed. 60+ fundamental and technical filters, instant heat maps, hover charts. Best for a quick first pass. | Elite ($39.50/mo or $299.50/yr) adds real-time data, backtests, exports |
| **TradingView** | Yes, with limits | Technical and fundamental filters across stocks, ETFs, crypto, and global exchanges; best charts of any free tool | Free tier restricts indicators and alerts; paid from about $15/mo |
| **Yahoo Finance** | Yes | Simplest interface; basic filters (cap, P/E, yield, sector); easy for beginners | Deeper screens need paid tiers |
| **Stock Rover** | Limited free tier, 14-day trial | Depth. 700–800+ metrics, 10+ years of history, equation-based screens, portfolio analytics; strongest for dividend and fundamental investors | Full features from roughly $8–$28/mo (annual plans) |
| **Koyfin** | Capable free tier | Professional-grade data and charts, global macro, estimates; good for comparing companies side by side | Fund research and advanced screens gated at paid tiers |
| **GuruFocus** | Limited free | Value-investor focus: 30 years of data, Piotroski F-Score, Altman Z, guru holdings, DCF calculator | Paid from roughly $35+/mo; expensive at top tiers |
| **Stock Analysis** | Yes | Clean, fast fundamentals and long statement history; good screener at low cost | Pro tier ~ $79/yr |
| **Zacks** | Yes | Earnings-estimate revisions, Zacks Rank; useful for earnings-momentum screens | Premium screens paid |
| **Morningstar** | Basic | Moat ratings and fair value on paid tier; fund screening | Investor subscription for full access |

(Prices are approximate as of 2026 and change often.)

Most investors do well with Finviz for speed plus one deeper tool (Stock Rover, Koyfin, or GuruFocus) for the research phase.

## Example screen recipes

### Classic value (Graham-inspired)

| Filter | Setting | Why |
|---|---|---|
| P/E (trailing) | < 15 | Cheap on earnings |
| P/B | < 1.5 | Cheap on assets (or P/E × P/B < 22.5, Graham's combined test) |
| Debt/Equity | < 0.5 | Financial strength |
| Current ratio | > 1.5 | Liquidity |
| Dividend yield | > 0 | Some cash return and evidence of real profits |
| Market cap | > $300M | Liquidity hygiene |

Expect: banks, insurers, industrials, energy. Read for: why is it cheap? Cyclicals at peak earnings will show low P/Es right before earnings fall.

### Quality value (modern)

| Filter | Setting | Why |
|---|---|---|
| EV/EBITDA | < 10 | Cheap on operating cash profit |
| ROIC | > 12% | Earns above cost of capital |
| FCF yield | > 5% | Real cash return |
| Net debt/EBITDA | < 2 | Not leveraged |
| 5-yr revenue growth | > 3%/yr | Not shrinking |

Expect: fewer names, better businesses. This approximates the "quality at a reasonable price" factor.

### Growth at a reasonable price (GARP)

| Filter | Setting | Why |
|---|---|---|
| EPS growth (5-yr historical) | > 12% | Proven growth |
| EPS growth (next year estimate) | > 12% | Expected to continue |
| PEG | < 1.5 | Not paying too much for it |
| ROE | > 15% | Profitable growth |
| Debt/Equity | < 1 | Growth not fueled by leverage |

Peter Lynch's approach. Check that growth is organic, not from acquisitions.

### Dividend growth

| Filter | Setting | Why |
|---|---|---|
| Dividend yield | 2–6% | Meaningful but not suspicious |
| Consecutive years of dividend increases | ≥ 10 | Track record |
| Payout ratio (of FCF) | < 70% | Room to keep growing |
| 5-yr dividend growth rate | > 5% | Actually growing |
| Net debt/EBITDA | < 3 | Can maintain through a downturn |

Stock Rover is particularly strong here (dividend history and payout-on-FCF are hard to get elsewhere for free).

### Quality/compounders

| Filter | Setting | Why |
|---|---|---|
| Gross margin | > 40% | Pricing power |
| ROIC (5-yr avg) | > 15% | Durable returns |
| FCF margin | > 15% | Cash-generative |
| Share count change (5-yr) | ≤ 0% | Not diluting |
| Revenue growth (5-yr) | > 8%/yr | Growing |

No valuation filter on purpose — build the watchlist first, then wait for the price.

### Momentum (technical)

| Filter | Setting | Why |
|---|---|---|
| Price vs. 200-day MA | Above | Uptrend |
| 6-month or 12-month return | Top 20% of market | Momentum factor |
| 1-month return | Not in top 10% | Avoid short-term reversal |
| Average volume | > 500k shares | Liquidity |
| Market cap | > $1B | Reduce noise |

Finviz and TradingView handle this easily. Momentum screens must be re-run monthly; they decay fast.

### Piotroski F-Score (accounting quality)

GuruFocus and Stock Rover compute the F-Score (0–9) from nine checks: positive net income, positive CFO, rising ROA, CFO > net income, falling leverage, rising current ratio, no new shares issued, rising gross margin, rising asset turnover. Screening for F-Score ≥ 7 combined with low P/B is the original academic recipe and remains a solid value-plus-quality filter.

## Common screening mistakes

- **Screening on trailing earnings for cyclicals.** Miners and homebuilders show P/Es of 5 at the top of the cycle.
- **Ignoring how the metric is calculated.** "P/E" may use GAAP or adjusted EPS; "debt" may or may not include leases.
- **Survivorship bias in backtests.** Companies that went bankrupt vanish from databases, making historical screens look better than they were.
- **Too many filters.** Every filter is a chance to eliminate a great company on a technicality.
- **Falling in love with the output.** The screen is where research starts.
- **Not tracking results.** Keep a log of what each screen produced and how it performed a year later.

## How to actually do it

1. Write your thesis in one sentence.
2. Choose one screener (Finviz for speed; Stock Rover, Koyfin, or GuruFocus for depth) and translate the thesis into 3–7 filters plus market cap and volume hygiene.
3. Run it. If you get more than 50 names, tighten the most important filter; if fewer than 10, loosen a secondary one.
4. Sort by your key metric and export to a spreadsheet with date and screen name.
5. For each of the top 20, spend ten minutes: read the business description and check five years of revenue, margins, and FCF. Cut the ones with obvious problems.
6. Take the survivors (usually 3–8) through full analysis: 10-K, ratios, moat, management, valuation.
7. Save the screen and re-run monthly (momentum) or quarterly (fundamentals).
8. Review the log annually: which screens found your winners?

## Key takeaways

- A screen is a search filter, not a buy list; every output needs reading.
- Build screens from a thesis using factors with evidence behind them: value, quality, momentum, dividend growth.
- Three to seven filters plus liquidity hygiene is the sweet spot.
- Finviz is fastest; Stock Rover, Koyfin, and GuruFocus go deeper; TradingView is best for technical screens.
- Combine value with quality (ROIC, F-Score, FCF) to reduce value traps.
- Beware cyclicals with low trailing P/Es and metrics whose definitions vary between tools.
- Keep a log of screen outputs and results so you learn which recipes work for you.

## Sources

- [StockBrokers.com: Best Stock Screeners 2026](https://www.stockbrokers.com/guides/best-free-stock-screeners)
- [Stock Rover: How Stock Rover Compares to Koyfin, Finviz, TIKR and More](https://www.stockrover.com/compare/)
- [Koyfin: Best Stock Screeners in 2026](https://www.koyfin.com/blog/best-stock-screeners/)
- [Finviz Screener](https://finviz.com/screener.ashx)
- [TradingView Stock Screener](https://www.tradingview.com/screener/)
- [GuruFocus Screener](https://www.gurufocus.com/screener)
- [Investopedia: Piotroski Score](https://www.investopedia.com/terms/p/piotroski-score.asp)
