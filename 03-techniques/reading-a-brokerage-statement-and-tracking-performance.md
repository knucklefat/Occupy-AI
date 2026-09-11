# Reading a Brokerage Statement and Tracking Performance

**In one sentence:** Most people have no idea what return they are actually earning — learning to read a statement, compute both time-weighted and money-weighted returns, compare them to a fair benchmark, and quantify fee drag turns investing from a feeling into something you can manage.

## Anatomy of a brokerage statement

Statements differ by broker, but the same sections appear everywhere:

| Section | What it tells you | What to check |
|---|---|---|
| **Account summary** | Beginning value, deposits/withdrawals, change in value, ending value | Does ending value − beginning value − net deposits equal the "change in investment value"? That is your dollar gain. |
| **Asset allocation** | Percent in stocks, bonds, cash, other | Compare to your target; broker categories are often crude (a balanced fund may show as 100% "mutual funds") |
| **Holdings / positions** | Each security: quantity, price, market value, cost basis, unrealised gain/loss | Cost basis is what you paid; unrealised gain is on paper. Check for lots with losses (harvesting) and positions over your concentration cap |
| **Income summary** | Dividends, interest, capital-gains distributions, year-to-date | Qualified vs. non-qualified dividends matter for taxes |
| **Activity / transactions** | Every buy, sell, dividend, fee, transfer | Look for fees you didn't expect and dividend reinvestments that could cause wash sales |
| **Realised gains/losses** | Closed positions, short- vs. long-term | Feeds Schedule D; verify the broker's lot method matches what you intended |
| **Fees and expenses** | Advisory fees, account fees, margin interest | Fund expense ratios do *not* appear here — they are deducted inside the fund's price |
| **Margin / cash balance** | Cash, money-market sweep, any borrowed amount | A negative cash balance means you are on margin, possibly by accident |

Two things statements routinely hide: **fund expense ratios** (look them up separately) and **your actual rate of return** (many brokers show only dollar change, or a return that ignores your deposits).

## Two ways to measure return — and why they differ

**Time-weighted return (TWR)** measures how the *investments* performed, ignoring when you added or withdrew money. It is what mutual funds report and what you use to judge a fund or a manager. It is computed by chaining the returns of each sub-period between cash flows.

**Money-weighted return (MWR)**, also called the internal rate of return (IRR), measures how *your dollars* performed, including the effect of your timing. It is what you use to judge your own outcome. In a spreadsheet it is the **XIRR** function.

**Worked example.** You invest $10,000 on 1 January 2024. By 30 June it has fallen 10% to $9,000. On 1 July you add $5,000 (total $14,000). By 31 December 2025 it has risen 25% to $17,500.

- **TWR**: (1 − 0.10) × (1 + 0.25) − 1 = **12.5%** over two years, or about **6.1% a year**. That's how the fund did.
- **MWR (XIRR)**: about **8.8% a year**. Higher, because you happened to add money right before the good stretch.

If you had added the $5,000 at the *top* instead, MWR would be *lower* than TWR. The gap between the two is a measure of your timing luck or skill. Morningstar's "Mind the Gap" studies find the average fund investor's MWR trails the fund's TWR by roughly 1 percentage point a year — the cost of buying after rallies and selling after crashes.

## Computing XIRR in a spreadsheet

Two columns: dates and cash flows (money in as negative, money out and the final value as positive).

| Date | Cash flow |
|---|---|
| 2024-01-01 | −10,000 |
| 2024-07-01 | −5,000 |
| 2025-12-31 | +17,500 |

`=XIRR(B1:B3, A1:A3)` returns 0.0876 → 8.8%. Works in Excel, Google Sheets and LibreOffice. For a whole portfolio, list every deposit and withdrawal across all accounts, and the current total value as the last positive row. Dividends reinvested inside the account are *not* cash flows — they never left the portfolio.

## Benchmarking: compare to something fair

A return means nothing without a comparison. The rules:

1. **Match the risk.** A 60/40 portfolio should be compared to a 60/40 blend (e.g., 60% total-market index + 40% total-bond index), not to the S&P 500. Beating bonds with stocks is not skill.
2. **Match the composition.** If you hold 30% international, your benchmark should too. Vanguard's LifeStrategy or target-date funds make convenient ready-made benchmarks for common mixes.
3. **Use TWR for the comparison** (that is what the benchmark reports), then look at MWR separately to see whether your *behaviour* added or subtracted.
4. **Judge over years, not quarters.** Any strategy can lag for three to five years; a decade of underperformance is a signal.

If your core–satellite portfolio's satellites are supposed to add value, track the satellite sleeve's TWR against the same benchmark separately. Most people discover their bets cost them.

## Fee drag: the calculation everyone should do once

Fees compound just like returns, in reverse. The formula is simply: run the growth at the gross return, then at the gross return minus fees, and compare.

**$100,000 for 30 years at a 7% gross return:**

| Annual fee | Net return | Ending value | Lost to fees |
|---|---|---|---|
| 0.05% (index fund) | 6.95% | ~$750,000 | ~$11,000 |
| 0.50% | 6.50% | ~$661,000 | ~$100,000 |
| 1.00% (typical advisor or active fund) | 6.00% | ~$574,000 | ~$187,000 |
| 2.00% (advisor + active funds) | 5.00% | ~$432,000 | ~$329,000 |

A 1% fee does not cost you 1% of your money — it costs about a **quarter of your ending wealth** over 30 years, because the fee is taken from a growing balance every year and the money taken can no longer compound. Add up every layer: fund expense ratio + advisory fee + platform fee + trading costs + (in taxable) tax drag from turnover.

## Tools

| Tool | Best for | Notes |
|---|---|---|
| **Spreadsheet (XIRR)** | Ground truth for your own MWR | Free, transparent, requires logging cash flows |
| **Portfolio Visualizer** | Backtesting allocations, factor analysis, Monte Carlo | The standard free research tool; some features now paid |
| **Empower (formerly Personal Capital) dashboard** | Aggregating accounts, allocation view, fee analyser | Free; expect sales calls for their advisory service |
| **Broker performance tab** (Fidelity, Schwab, Vanguard) | Quick TWR and MWR by account | Check whether it's TWR or MWR — they label inconsistently |
| **Morningstar Portfolio Manager / X-Ray** | Look-through allocation, overlap, fee comparison | Free tier is adequate |
| **Portfolio Charts** | Long-run behaviour of lazy portfolios | Great for drawdown and withdrawal-rate intuition |
| **Boldin (formerly NewRetirement), ProjectionLab, cFIREsim, FICalc** | Retirement projections | Useful once you're modelling withdrawals |

## How to actually do it

1. Once a month, record the total value of every account in one spreadsheet row (date, per-account value, total). Ten minutes.
2. Record every external deposit and withdrawal in a second sheet (date, amount). Ignore internal dividends and trades.
3. Once a year, compute XIRR from the cash-flow sheet plus the year-end total. That is your money-weighted return.
4. Compute TWR by chaining monthly returns: each month's return = (end value − net cash flow) ÷ start value − 1; multiply the (1 + r) terms. Or use your broker's TWR figure.
5. Compare TWR to a blended index benchmark matching your allocation. Compare MWR to TWR to see what your timing did.
6. Add up all fees as a percentage of assets; run the 30-year fee-drag table with your own numbers.
7. Read every statement's activity section for surprises: unexpected fees, margin, dividend reinvestments in taxable accounts, and positions drifting past concentration limits.
8. Keep year-end statements and every 1099 forever — you'll need cost basis for anything bought before brokers were required to track it (2011–2012).

## Key takeaways

- Your statement's "change in value" minus your deposits is your dollar gain; brokers rarely show your true percentage return.
- TWR judges the investments; MWR (XIRR) judges your dollars. The gap between them is the cost of your timing.
- The average investor trails their own funds by ~1% a year through poor timing.
- Benchmark against a blend matching your risk and composition, over years, not quarters.
- A 1% annual fee consumes roughly a quarter of ending wealth over 30 years; a 2% fee, over 40%.
- Fund expense ratios never appear on your statement — look them up and add them to every other fee.
- A monthly value log and a cash-flow log are all you need to compute everything above yourself.

## Sources

- [Bogleheads wiki – Calculating personal returns](https://www.bogleheads.org/wiki/Calculating_personal_returns)
- [Bogleheads wiki – Comparing investments (benchmarking)](https://www.bogleheads.org/wiki/Comparing_investments)
- [Morningstar – Mind the Gap: investor returns vs. fund returns](https://www.morningstar.com/lp/mind-the-gap)
- [SEC Investor.gov – How fees and expenses affect your investment portfolio](https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins/how-fees)
- [FINRA – Understanding your brokerage account statements](https://www.finra.org/investors/insights/brokerage-account-statements)
- [Portfolio Visualizer](https://www.portfoliovisualizer.com/)
- [Empower – Free financial dashboard](https://www.empower.com/personal-investors/financial-tools)
- [Microsoft – XIRR function](https://support.microsoft.com/en-us/office/xirr-function-de1242ec-6477-445b-b11b-a303ad9adc9d)
