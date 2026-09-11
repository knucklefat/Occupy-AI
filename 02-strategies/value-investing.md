# Value Investing

**In one sentence:** Buy businesses for meaningfully less than a sober estimate of what they are worth, insist on a margin of safety because your estimate will be wrong, and wait — sometimes years — for price to catch up with value.

## The lineage: Graham to Buffett to today

Benjamin Graham, a Columbia professor who lost heavily in the 1929 crash, wrote *Security Analysis* (1934) and *The Intelligent Investor* (1949) to replace speculation with something like accounting. His central ideas:

- A stock is a fractional ownership of a business, not a ticker that wiggles.
- **"Mr. Market"** is a manic-depressive partner who offers to buy or sell you his share every day at a price that reflects his mood, not the business. You are free to ignore him.
- **Margin of safety**: pay far less than your estimate of value so that errors, bad luck, and time are absorbed by the discount rather than your capital.

Graham's own method was quantitative and cheap: "net-nets" (stocks trading below net current assets minus all liabilities), low price-to-earnings, low price-to-book, diversified across dozens of names because any one could be a dud.

Warren Buffett, Graham's student, added two things under the influence of Charlie Munger and Phil Fisher: an appreciation of *quality* (a durable competitive advantage — "moat" — lets a business compound value for decades) and concentration. Buffett's summary in his 1989 letter: it is "far better to buy a wonderful company at a fair price than a fair company at a wonderful price." Modern value investing runs a spectrum from Graham's deep-value cigar butts (cheap, ugly, statistically likely to bounce) to Buffett/Munger quality-at-a-reasonable-price (good, fairly priced, held forever). Practitioners in the lineage include Seth Klarman, Howard Marks, Joel Greenblatt, Bill Nygren, and Mohnish Pabrai.

## Intrinsic value: what you are actually estimating

Intrinsic value is the present value of all the cash a business will hand its owners from now until the end of time, discounted for the time value of money and the risk you will not receive it. In practice, this is a **discounted cash flow (DCF)** model:

1. Estimate free cash flow (cash from operations minus capital spending) for the next 5–10 years.
2. Estimate a terminal value for everything after that (usually a modest perpetual growth rate, 2–3%).
3. Discount all of it back to today at a rate reflecting the risk (8%–12% for most businesses).
4. Subtract net debt, divide by shares outstanding.

NYU's Aswath Damodaran, the most widely followed valuation teacher, stresses that a DCF is a story turned into numbers, and that the story (how fast, how profitable, how long) matters more than the spreadsheet. Two honest analysts can differ by 30% on the same company. That is why the margin of safety exists.

## Valuation metrics and what each one hides

| Metric | Formula | What it tells you | Where it lies |
|---|---|---|---|
| **P/E** (price-to-earnings) | Price ÷ earnings per share | Years of current earnings you pay for | Earnings are easily distorted (one-time charges, accounting choices); meaningless for loss-makers; ignores debt |
| **P/B** (price-to-book) | Price ÷ book value per share | Price vs. accounting net assets | Book value ignores intangibles (brands, software, R&D); buybacks can make it negative; best for banks and asset-heavy firms |
| **EV/EBITDA** | (Market cap + debt − cash) ÷ earnings before interest, taxes, depreciation, amortization | Price of the whole enterprise vs. operating cash-ish profits; debt-neutral, so comparable across capital structures | EBITDA ignores capital spending — a capital-hungry business can look cheap and never generate real cash |
| **FCF yield** | Free cash flow ÷ enterprise value (or market cap) | Cash actually generated per dollar of price; hardest number to fake | Lumpy year to year; working-capital swings and deferred capex can inflate a single year |
| **EV/Sales** | Enterprise value ÷ revenue | Useful for unprofitable or cyclical-trough companies | Says nothing about whether sales will ever become profit |
| **Shiller P/E (CAPE)** | Price ÷ 10-year average real earnings | Smooths the cycle; used for whole markets | Slow-moving; has said "expensive" for most of the last 30 years |

Use several together. A stock with low P/E, low EV/EBITDA, *and* high FCF yield is far more likely to be genuinely cheap than one that screens well on a single measure.

## The value premium: evidence and the 2010s drought

Fama and French's 1992 paper showed that, from 1963 onward, stocks with high book-to-market (cheap) beat stocks with low book-to-market (expensive) by several percentage points a year, an effect since found in almost every country and back to the 1920s. The long-run U.S. "HML" (high-minus-low) factor premium has averaged roughly 3%–5% per year, though with enormous variation.

Then came the drought. From roughly 2007 to 2020, value badly trailed growth. Larry Swedroe's tally (2020) puts the value factor at about −2.6% annualized for 2010–2019, the worst decade on record, while the market itself compounded at 13%. Fama and French's 2020 paper "The Value Premium" concluded the shrinkage was real but that the data were too noisy to say whether the premium was dead or merely dormant. Explanations offered:

- **Intangibles**: book value misses R&D, software, and brands, so P/B mislabels modern winners as "expensive." Adjusting for intangibles recovers some of the premium.
- **Falling interest rates** raised the value of far-future cash flows, favoring growth stocks.
- **Mega-cap winner-take-all platforms** (the "Magnificent Seven") that value screens never own.
- **Crowding**: too many quants chasing the same cheap stocks.

Value roared back from late 2020 through 2022 (cheap stocks beat expensive ones by a wide margin as rates rose), then trailed again during the 2023–2025 AI-led rally. The lesson is not that value is dead or alive; it is that the premium arrives in violent, unpredictable bursts and requires a holding period measured in decades to harvest.

## Value traps

A value trap is a stock that is cheap because it deserves to be. Classic markers:

- Revenue and margins declining for several years (a melting ice cube: newspapers, legacy retailers, film cameras).
- Cheap on P/E but expensive on FCF yield — earnings are accounting fiction.
- Heavy debt with maturities approaching; the equity is a thin sliver on a big balance sheet.
- Management that has "restructured" three times and still promises next year.
- An industry in structural, not cyclical, decline. Cyclical cheapness (homebuilders in 2011) recovers; structural cheapness (coal in 2015) mostly does not.
- Low P/B in a company burning cash — book value is being destroyed while you wait.

The single best defense is to ask: *why* is this cheap, and what specifically has to happen for it to stop being cheap? If your answer is "the market will eventually notice," you have no thesis.

## Screening for value candidates

Free screeners (Finviz, Yahoo Finance, TradingView, GuruFocus, your broker's tools) can implement these. A starting screen in the Graham-plus-quality spirit:

| Criterion | Setting | Purpose |
|---|---|---|
| EV/EBITDA | < 10 | Cheap on an enterprise basis |
| FCF yield | > 6% | Cheap on cash generation |
| P/B | < 2.5 (< 1.5 for financials/industrials) | Asset backing |
| Net debt / EBITDA | < 2.5 | Survivability |
| Return on invested capital, 5-yr avg | > 10% | Not a junk business |
| Revenue growth, 5-yr | > 0% | Not a melting ice cube |
| Market cap | > $300 million | Enough liquidity to trade |

Then read the last three annual reports and the proxy statement for each survivor. Screening is a filter, not a decision.

## How to actually do it

1. **Define your circle of competence.** Industries you can explain to a friend — how the company makes money, who its customers are, what could kill it. Ignore everything else.
2. **Generate ideas** from a screen like the one above, the 52-week-low list, spin-offs, or 13F filings of managers you respect.
3. **Read the 10-K.** Business description, risk factors, MD&A, and the cash-flow statement. Five years of numbers minimum. Note trends in revenue, gross margin, operating margin, free cash flow, share count, and debt.
4. **Estimate intrinsic value** two ways: a simple DCF and a multiples check (what have similar businesses sold for?). If the two disagree wildly, figure out why before proceeding.
5. **Demand a margin of safety** of at least 30% below your estimate for a good business, 50% for a mediocre one.
6. **Write the thesis** in three sentences: why it's cheap, what changes that, and what would prove you wrong.
7. **Size the position** at 3%–8% of the portfolio; hold 15–25 names. Buffett-level concentration is for Buffett-level analysts.
8. **Hold until** price reaches your value estimate, the thesis breaks, or you find something clearly better. Recheck the thesis every quarter, not the price every day.
9. **Expect long stretches of underperformance.** The 2010s were a full decade. If you cannot hold through that, own a value index fund (see [factor-investing.md](factor-investing.md)) instead of picking stocks.

## Key takeaways

- Value investing is buying below intrinsic value with a margin of safety; the estimate is always imprecise, which is why the discount is mandatory.
- Graham was cheap-and-diversified; Buffett is quality-and-concentrated. Both work; the second is harder.
- No single multiple is trustworthy — triangulate P/E, EV/EBITDA, and FCF yield, and read the cash-flow statement.
- The value premium is real over a century of data but disappeared for most of 2007–2020; it revived in 2021–2022 and stalled again after.
- Value traps are cheap for a reason; always articulate the catalyst.
- Most people should harvest value through a diversified factor fund; stock-by-stock value investing demands reading 10-Ks for fun.
- Patience measured in years, not quarters, is the actual edge.

## Sources

- [The Value Premium — Fama & French (SSRN, 2020)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3525096)
- [A Lost Decade for the Fama-French Factors — Larry Swedroe, Advisor Perspectives (2020)](https://www.advisorperspectives.com/articles/2020/05/13/a-lost-decade-for-the-fama-french-factors)
- [Reports of Value's Death May Be Greatly Exaggerated — Arnott et al., Financial Analysts Journal (2021)](https://www.tandfonline.com/doi/full/10.1080/0015198X.2020.1842704)
- [It's Too Soon to Say the Value Premium Is Dead — Morningstar](https://www.morningstar.com/portfolios/its-too-soon-say-value-premium-is-dead)
- [Resurrecting the Value Premium — Alpha Architect](https://alphaarchitect.com/resurrecting-the-value-premium/)
- [Berkshire Hathaway Shareholder Letters (1977–present)](https://www.berkshirehathaway.com/letters/letters.html)
- [Aswath Damodaran — Valuation resources (NYU Stern)](https://pages.stern.nyu.edu/~adamodar/)
- [Investopedia: Value Investing](https://www.investopedia.com/terms/v/valueinvesting.asp)
- [Investopedia: Margin of Safety](https://www.investopedia.com/terms/m/marginofsafety.asp)
