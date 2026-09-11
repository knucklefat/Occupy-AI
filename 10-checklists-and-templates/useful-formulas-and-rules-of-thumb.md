# Useful Formulas and Rules of Thumb

**In one sentence:** The fifteen calculations every self-directed investor actually uses — compound growth, Rule of 72, the 4% rule and 25×, real return, the true cost of fees, Kelly, Sharpe, PEG, free-cash-flow yield, a basic DCF, XIRR, and a few others — each with the formula, a plain-language explanation, and a worked example you can check with a calculator.

Nothing here requires more than a spreadsheet. Rules of thumb are labeled as such: they're fast approximations for orienting yourself, not precise answers. Where a formula has a hidden assumption that trips people up, it's called out.

---

## 1. Compound growth (future value)

**Formula:** FV = PV × (1 + r)ⁿ
where PV is what you start with, r is the annual return as a decimal, n is years.

**Plain language:** Money earns a return; next year that return also earns a return. Over long periods the growth is dominated by the returns *on returns*, which is why starting early matters far more than picking well.

**Worked example:** $10,000 at 7% for 30 years.
FV = 10,000 × 1.07³⁰ = 10,000 × 7.61 = **$76,100**. Of that, only $10,000 was your money and $21,000 is the simple interest (7% × 30 years); the remaining $45,000 is interest on interest.

**Related — future value of regular contributions:** FV = P × [((1 + r)ⁿ − 1) ÷ r], with P the contribution per period and r, n in matching periods.
$500/month at 7% (0.5833%/month) for 30 years (360 months): FV = 500 × [(1.005833³⁶⁰ − 1) ÷ 0.005833] = 500 × 1,220 ≈ **$610,000** — from $180,000 of contributions.

## 2. Compound annual growth rate (CAGR)

**Formula:** CAGR = (Ending value ÷ Starting value)^(1/n) − 1

**Plain language:** The single steady annual rate that would have taken you from the start to the end. It's how to compare investments held for different lengths of time; "it doubled" means something very different over 3 years versus 15.

**Worked example:** $50,000 grew to $120,000 in 12 years.
CAGR = (120,000 ÷ 50,000)^(1/12) − 1 = 2.4^0.0833 − 1 = 1.0757 − 1 = **7.6% per year**.

**Caveat:** CAGR ignores contributions and withdrawals. If you added money along the way, use XIRR (#14).

## 3. Rule of 72 (rule of thumb)

**Formula:** Years to double ≈ 72 ÷ annual return (in percent)

**Plain language:** A mental shortcut for compounding. Also works in reverse: 72 ÷ years = the return needed to double.

**Worked example:** At 8%, money doubles in about 72 ÷ 8 = **9 years** (exact: 9.0). At 3% inflation, prices double — and a fixed dollar loses half its purchasing power — in about **24 years**. A 1% fee, compounded over 72 years, halves what you'd otherwise have.

**Accuracy:** good between roughly 4% and 12%; use 70 for lower rates and 75–78 for higher ones.

## 4. Real return (inflation-adjusted)

**Formula (exact):** Real return = (1 + nominal) ÷ (1 + inflation) − 1
**Rule of thumb:** Real ≈ nominal − inflation

**Plain language:** What your money actually gained in purchasing power. Long-run planning should always use real returns; an 8% nominal return with 3% inflation buys about 5% more stuff, not 8%.

**Worked example:** Portfolio returned 7%, inflation was 3%.
Exact: 1.07 ÷ 1.03 − 1 = **3.88%**. Approximation: 7 − 3 = 4%. Close enough for planning.

**Historical context:** US stocks have delivered roughly 6–7% real over the last century; bonds roughly 1–2% real. Most planners use 4–5% real for a diversified portfolio going forward.

## 5. The 4% rule and the 25× rule

**Formula:** Initial annual withdrawal = 4% × starting portfolio, then increase the dollar amount with inflation each year.
**Flipped:** Portfolio needed = 25 × annual spending from the portfolio.

**Plain language:** Based on historical US data (Bengen 1994, the Trinity Study), a diversified 50–75% stock portfolio has survived 30 years of inflation-adjusted 4% withdrawals in essentially every historical starting year. It's a *planning* rule, not a law: it assumes a 30-year horizon, no flexibility, and US historical returns.

**Worked example:** You spend $60,000/year; Social Security will cover $20,000. The portfolio must supply $40,000.
Target = 25 × 40,000 = **$1,000,000**. Year-one withdrawal = 4% × 1,000,000 = $40,000. If inflation is 3%, year two is $41,200 regardless of what the market did.

**Adjustments:** for a 40+ year retirement or extra caution, use 3.3–3.5% (≈ 28–30×). If you can cut spending 10% in bad years, 4.5–5% has historically worked. Kitces' research suggests the 4% rule has been overly conservative in most historical periods — the median retiree following it ended with *more* money than they started with — which is why flexible "guardrail" rules exist.

## 6. The true cost of an expense ratio over N years

**Formula:** Ending value with fee = PV × (1 + r − f)ⁿ; cost = ending value without fee − ending value with fee.
where f is the expense ratio as a decimal.

**Plain language:** A fee isn't just the dollars taken this year — it's the dollars taken *plus everything those dollars would have earned*. A 1% fee on a 7% return isn't "1% of your money," it's about 14% of your return every single year, compounding.

**Worked example:** $100,000, 7% gross return, 30 years.
- Fund A (0.05% fee): 100,000 × 1.0695³⁰ = **$750,500**
- Fund B (1.05% fee): 100,000 × 1.0595³⁰ = **$566,100**
- Cost of the extra 1%: **$184,400 — about 25% of the ending balance.**

**Rule of thumb:** over 30 years, each 1% of annual fees consumes roughly a quarter of your final wealth; over 40 years, roughly a third. Multiply your annual fees in dollars by 25 for a rough lifetime cost in today's dollars.

## 7. Savings rate and years to financial independence (rule of thumb)

**Plain language:** Your savings rate determines your timeline far more than your returns, because it works on both sides — higher savings means more invested *and* less spending to replace. Assuming a 5% real return and the 25× target, approximate years from zero to financial independence:

| Savings rate | Years to FI (approx.) |
|---|---|
| 10% | ~51 |
| 15% | ~43 |
| 25% | ~32 |
| 40% | ~22 |
| 50% | ~17 |
| 65% | ~10 |

**Worked example:** A household saving 15% of take-home pay needs roughly four decades — which is why 15% is the standard career-long target, and why raising it to 25% cuts more than a decade off.

## 8. Kelly criterion (position sizing)

**Formula:** f* = (b × p − q) ÷ b
where f* is the fraction of your bankroll to bet, b is the net odds (win $b per $1 risked), p is the probability of winning, q = 1 − p.

**Plain language:** The bet size that maximizes long-run growth if you know the odds exactly. You never know the odds exactly in investing, and full Kelly produces stomach-churning swings, so practitioners use half-Kelly or less. Its real value is as a *ceiling* and as a reminder that even a great bet, sized too large, goes broke.

**Worked example:** You believe a stock has a 60% chance of doubling (b = 1) and a 40% chance of going to zero.
f* = (1 × 0.60 − 0.40) ÷ 1 = **0.20 → 20% of the portfolio at full Kelly; 10% at half-Kelly.**
Now suppose you're overconfident and the real probability is 50%: f* = (0.5 − 0.5) ÷ 1 = 0. The right position was zero. This is why most IPS documents cap single positions at 3–5%.

## 9. Sharpe ratio (return per unit of risk)

**Formula:** Sharpe = (portfolio return − risk-free rate) ÷ standard deviation of portfolio returns

**Plain language:** How much excess return you got for each unit of volatility you endured. Lets you compare a high-return/high-swing strategy against a lower-return/smoother one. Above ~1.0 over a long period is very good; most diversified portfolios sit around 0.3–0.6.

**Worked example:** Portfolio returned 10%, Treasury bills paid 4%, annual standard deviation was 15%.
Sharpe = (10 − 4) ÷ 15 = **0.40**.
A second portfolio returned 8% with 8% volatility: (8 − 4) ÷ 8 = 0.50 — lower return, but *better* risk-adjusted.

**Caveat:** volatility isn't the only risk, and past Sharpe ratios of strategies selling insurance (options, some "income" funds) look great right up until they don't.

## 10. Price-to-earnings (P/E) and earnings yield

**Formula:** P/E = price per share ÷ earnings per share. Earnings yield = E ÷ P = 1 ÷ (P/E).

**Plain language:** How many years of current earnings you're paying for. Flipping it gives an earnings yield you can compare to bond yields. Use *normalized* or multi-year average earnings; a single year can be distorted.

**Worked example:** Stock at $50, earnings $2.50/share. P/E = 20. Earnings yield = 2.50 ÷ 50 = **5%**. If 10-year Treasuries yield 4.5%, you're being paid only slightly more than a bond for taking equity risk — unless earnings grow.

## 11. PEG ratio (P/E relative to growth)

**Formula:** PEG = (P/E) ÷ expected annual earnings growth rate (in percent)

**Plain language:** Peter Lynch's shortcut for whether a growth stock's price is reasonable relative to its growth. Roughly: PEG under 1 is attractive, 1 is fair, over 2 is expensive. Lynch's dividend-adjusted version adds the dividend yield to the growth rate.

**Worked example:** Company A: P/E 20, expected growth 10% → PEG = 20 ÷ 10 = **2.0** (expensive). Company B: P/E 15, expected growth 15% → PEG = **1.0** (fair). Company C: P/E 30, growth 40% → PEG = 0.75 — but be skeptical of 40% growth persisting.

**Caveat:** the "G" is a forecast. A PEG built on an analyst's optimistic 5-year growth number is only as good as that number.

## 12. Free cash flow yield

**Formula:** FCF yield = free cash flow ÷ market capitalization (or ÷ enterprise value for a debt-adjusted view)
where free cash flow = operating cash flow − capital expenditures.

**Plain language:** The cash return the business generates for its owners, as a percentage of what you'd pay for the whole thing. Harder to manipulate than earnings. Compare it to bond yields and to the company's own history. Buffett-style investors often want an FCF yield well above the 10-year Treasury.

**Worked example:** Company generates $5 billion of free cash flow; market cap is $100 billion. FCF yield = **5%**. If it has $20 billion net debt, enterprise value is $120 billion and the debt-adjusted yield is 4.2%.

## 13. Discounted cash flow (DCF) basics

**Formula:** Value today = Σ [FCFₜ ÷ (1 + r)ᵗ] for the forecast years + Terminal value ÷ (1 + r)ᴺ
Terminal value (Gordon growth) = FCFₙ × (1 + g) ÷ (r − g)
where r is your required return (discount rate) and g the perpetual growth rate (must be below r; usually 2–3%).

**Plain language:** A business is worth all the cash it will ever hand its owners, converted to today's dollars at the return you demand. The output is only as good as the inputs — small changes to r or g swing the answer wildly, which is why you (a) use conservative inputs and (b) demand a margin of safety below the result. Damodaran's guidance: the story must justify the numbers, and the terminal value should not be most of the answer if you claim to understand the near term.

**Worked example:** Current free cash flow $100 million; you expect 5% growth for 5 years, then 3% forever; you require 9%.

| Year | FCF ($M) | Discount factor (1.09⁻ᵗ) | Present value ($M) |
|---|---|---|---|
| 1 | 105.0 | 0.917 | 96.3 |
| 2 | 110.3 | 0.842 | 92.8 |
| 3 | 115.8 | 0.772 | 89.4 |
| 4 | 121.6 | 0.708 | 86.1 |
| 5 | 127.6 | 0.650 | 83.0 |
| **Sum of years 1–5** | | | **447.6** |
| Terminal value at year 5 = 127.6 × 1.03 ÷ (0.09 − 0.03) = 2,191 | | × 0.650 | **1,423.9** |
| **Total value** | | | **≈ $1,871M** |

With 100 million shares, intrinsic value ≈ **$18.70/share**. With a 30% margin of safety, you'd want to pay under about **$13**. Note that 76% of the value is the terminal value — so the answer is mostly a bet on r and g. Re-run at r = 10%, g = 2%: total ≈ $1,446M, or $14.50/share — a 23% drop in value from one point of change in each input. That sensitivity *is* the lesson.

## 14. XIRR (money-weighted return with irregular cash flows)

**Formula:** Solve for r in Σ [CFᵢ ÷ (1 + r)^(dᵢ ÷ 365)] = 0, where each cash flow CFᵢ occurred dᵢ days after the first. In practice: `=XIRR(values, dates)` in Excel or Google Sheets, with contributions negative and the ending balance positive.

**Plain language:** Your *personal* annualized return, accounting for exactly when money went in and out. It's the right number for "how did *I* do," because a simple "ending ÷ total contributed" ignores that money added last month hasn't had time to grow. (Fund fact sheets report *time-weighted* returns, which strip out the effect of your cash flows — that's the right number for "how did the *fund* do.")

**Worked example:**

| Date | Cash flow |
|---|---|
| 2024-01-01 | −$10,000 (initial investment) |
| 2024-07-01 | −$5,000 (added) |
| 2025-01-01 | +$17,000 (ending value) |

Naive return: 17,000 ÷ 15,000 − 1 = 13.3%. XIRR ≈ **16.2%**, because the second $5,000 was only invested for half the year. Spreadsheet: put the three dates in A1:A3, the three amounts in B1:B3, and enter `=XIRR(B1:B3, A1:A3)`.

## 15. Quick rules of thumb (use with judgment)

| Rule | What it says | Where it breaks |
|---|---|---|
| **Age in bonds / 110 − age in stocks / 120 − age** | Starting-point stock/bond splits by age; 110 − age is the common modern version. | Ignores your actual risk tolerance, pension, and goals. A starting point only. |
| **3–6 months' expenses in cash** | Emergency fund size. | Dual stable incomes: 3 may do. Self-employed or single income: 6–12. |
| **15% of gross to retirement** | Career-long savings target, including employer match. | Starting late or aiming to retire early requires more (see #7). |
| **10–12× income in term life** | Coverage if others depend on your earnings. | Adjust for debts, existing assets, and years until dependents are independent. |
| **50/30/20** | Needs / wants / saving as a budget starting split. | High-cost areas or high incomes; the 20 is a floor, not a ceiling. |
| **Tax-equivalent yield = muni yield ÷ (1 − marginal tax rate)** | Compare a tax-free bond to a taxable one. E.g., 3% muni at a 32% bracket ≈ 4.41% taxable. | Ignores state taxes and AMT; apply your combined rate. |
| **Rebalance at ±5 percentage points** | A common drift band. | Small portfolios: just redirect contributions. Taxable accounts: mind the gains. |
| **Debt over ~7% → pay off before investing beyond the match** | The guaranteed return on debt payoff beats expected market returns net of risk. | Below that, it's a judgment call; always capture the employer match first. |
| **Never more than 5% in one stock, 10–20% in all individual stocks** | Concentration limits for non-professionals. | Only your IPS can set the real number. Lower is not a mistake. |

---

## A note on precision

Every projection above uses a single assumed return. Real returns arrive in a jagged sequence, and the order matters (see the sequence-risk section of [retirement-readiness-checklist.md](retirement-readiness-checklist.md)). Treat these formulas as tools for *orientation and comparison* — is this fund's fee a big deal, is this stock's price plausible, am I roughly on track — and not as forecasts. The plan in your IPS should survive being wrong by a couple of percentage points in either direction.

## Sources

- [Bogleheads wiki main page (4% rule / safe withdrawal rates, asset allocation, expense ratios)](https://www.bogleheads.org/wiki/Main_Page)
- [Rethinking65: Kitces on why the 4% withdrawal rate may be overkill](https://rethinking65.com/kitces-4-withdrawal-rate-still-may-be-overkill/)
- [Kitces: Understanding sequence of return risk and safe withdrawal rates](https://www.kitces.com/blog/understanding-sequence-of-return-risk-safe-withdrawal-rates-bear-market-crashes-and-bad-decades/)
- [Forbes: Peter Lynch's One Up On Wall Street–inspired screening strategy (PEG)](https://www.forbes.com/sites/investor/2021/04/16/lynchs-one-up-on-wall-street-inspired-screening-strategy/)
- [Damodaran Online: Valuation tools, data, and DCF spreadsheets (NYU Stern)](https://pages.stern.nyu.edu/~adamodar/)
- [Old School Value: Mohnish Pabrai — the checklist investor and Dhandho framework (Kelly and position sizing)](https://www.oldschoolvalue.com/investment-tools/mohnish-pabrai-checklist-investor/)
- [Morningstar: Guide to ETF investing (costs)](https://www.morningstar.com/funds/morningstars-guide-etf-investing)
- [r/personalfinance wiki: common topics (emergency fund, debt payoff thresholds, savings rate)](https://www.reddit.com/r/personalfinance/wiki/commontopics/)
