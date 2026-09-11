# Risk and Return

**In one sentence:** Risk is the price of return, and the investor's real job is not to avoid it but to measure it honestly — as volatility, as drawdown, as the chance of running out of money — and then take exactly as much as their goals require and their temperament allows.

## What "risk" actually means

Academics define risk as **volatility**: how much returns bounce around. Practitioners often prefer Warren Buffett's version — the chance of a **permanent loss of capital**. Both matter, for different reasons:

- Volatility is what you *feel*. A portfolio that swings 20% is one you may abandon at the bottom.
- Permanent loss is what *hurts*. A diversified index that falls 50% and recovers is volatile but not permanently impaired; a single company that goes bankrupt is.

A third definition matters most for anyone drawing income: **shortfall risk**, the probability that your money runs out before you do. A portfolio that is "too safe" (all cash) can carry enormous shortfall risk because inflation quietly wins.

## The core statistics, in plain language

| Measure | What it tells you | How to read it |
|---|---|---|
| **Standard deviation** (volatility) | How widely annual returns scatter around their average | U.S. stocks ≈ 19%/yr; bonds ≈ 8%; cash ≈ 3%. Roughly two-thirds of years land within ±1 std. dev. of the average, 95% within ±2. |
| **Maximum drawdown** | The largest peak-to-trough drop over a period | Stocks: −50% to −57% in the worst crises; −85% in 1929–32 |
| **Beta** | How much a stock or fund moves relative to the market | Beta 1.0 = moves with the market; 1.5 = amplifies it by half; 0.5 = damps it; negative = moves opposite |
| **Sharpe ratio** | Return per unit of risk: (return − risk-free rate) ÷ std. dev. | U.S. stocks long-run ≈ 0.4; anything consistently above 1.0 is exceptional; above 2 over long periods is usually a red flag |
| **Correlation** | Whether two assets move together (+1) or opposite (−1) | Diversification needs correlations well below +1 |
| **Value at Risk (VaR)** | The loss you'd expect to exceed only X% of the time | "95% one-year VaR of −25%" = one year in 20 should be worse than −25%. Underestimates tail events. |

**Standard deviation** is the workhorse. For a portfolio averaging 10% with 19% volatility, a "normal" bad year is about −9% (one std. dev. below) and a 1-in-40 year is about −28%. Real markets have fatter tails than the normal curve predicts — 2008's −37% was a roughly 2.5-standard-deviation event, and October 19, 1987 (−20% in a day) was statistically "impossible" under a normal distribution. Treat volatility as a floor on how bad things can get, not a ceiling.

**Sharpe ratio** lets you compare strategies with different risk levels: a fund returning 12% with 30% volatility (Sharpe ≈ 0.27 with 4% cash rates) is a worse deal than one returning 8% with 10% volatility (Sharpe ≈ 0.40), even though the first has the bigger headline number. The **Sortino ratio** is a cousin that counts only downside volatility, on the reasonable theory that nobody complains about upside surprises.

**Beta** matters mainly for individual stocks and sector funds. A utility stock with beta 0.5 will usually fall about half as far as the market in a crash; a semiconductor stock with beta 1.8 will fall almost twice as far. Beta captures only market-related risk; a company can have low beta and still go bankrupt.

## Drawdowns: the risk that actually tests you

A **drawdown** is the decline from a prior high. Recovery from a drawdown requires a larger percentage gain than the loss, because you're growing from a smaller base:

| Loss | Gain needed to break even |
|---|---|
| −10% | +11% |
| −20% | +25% |
| −33% | +50% |
| −50% | +100% |
| −80% | +400% |

The asymmetry is why avoiding catastrophic losses matters more than capturing every gain, and why leverage is so dangerous.

### The worst U.S. stock market drawdowns

S&P 500 price index (no dividends, nominal dollars), daily closing basis; recovery is time to regain the prior peak. Figures are rounded and match the table in [handling-market-crashes.md](../09-behavioral-finance/handling-market-crashes.md).

| Episode | Peak | Trough | Decline | Time to recover (price) | Notes |
|---|---|---|---|---|---|
| Great Depression | Sep 1929 | Jun 1932 | **−86%** | ~25 years (1954) | Roughly 15 years with dividends reinvested; shorter still after adjusting for 1930s deflation |
| 1973–74 oil shock / stagflation | Jan 1973 | Oct 1974 | **−48%** | ~7.5 years | Inflation-adjusted recovery took until the mid-1980s |
| 1987 crash | Aug 1987 | Dec 1987 | **−34%** | ~2 years | −20% in a single day (Oct 19) |
| Dot-com bust | Mar 2000 | Oct 2002 | **−49%** | ~7 years (2007) | Nasdaq fell 78% and took 15 years |
| Global Financial Crisis | Oct 2007 | Mar 2009 | **−57%** | ~5.5 years (Mar 2013); ~4 years with dividends | Deepest since the Depression |
| COVID crash | Feb 2020 | Mar 2020 | **−34%** | ~6 months | Fastest 30% drop and fastest recovery ever |
| 2022 rate-hike bear | Jan 2022 | Oct 2022 | **−25%** | ~2 years (Jan 2024) | Bonds fell simultaneously (−18% for 10-yr Treasuries) |

Averages from the full record since the 1920s: a decline of 10%+ ("correction") arrives roughly once a year; 20%+ ("bear market") about every 4–6 years; 30%+ roughly once a decade. Bear markets have lasted about a year on average from peak to trough, and most (not all) recoveries have taken 2–5 years. **Plan on living through several of these** over an investing lifetime.

Bonds have their own drawdowns. Long-term Treasuries fell more than 40% from their 2020 peak through 2023 as rates rose — worse than many stock bear markets — a reminder that "safe" describes credit risk, not price risk.

## Sequence-of-returns risk

The *order* in which returns arrive doesn't matter while you are accumulating with no withdrawals — the same set of annual returns in any order produces the same ending value. But it matters enormously once you are withdrawing.

Consider two retirees each starting with $1,000,000, withdrawing $40,000 a year (rising with inflation), and each earning the same average return over 30 years. Retiree A gets three bad years first, then good ones; Retiree B gets the good years first. Retiree A sells shares at depressed prices in the early years to fund spending, locking in losses that can never compound back; Retiree B's portfolio grows before the bad years hit. Historically, the difference between these two paths can be the difference between running out of money in year 22 and dying with more than you started with.

Defenses against sequence risk:

- Hold 1–3 years of spending in cash or short-term bonds so you never sell stocks in a crash (a "bucket" or "cash cushion" strategy).
- Use a flexible withdrawal rule — spend less after bad years.
- Delay Social Security or other guaranteed income to reduce what the portfolio must supply.
- Keep the stock allocation moderate (40–60%) in the five years before and after retirement — the "retirement red zone."

## Risk tolerance vs. risk capacity vs. risk need

Three separate questions that are constantly confused:

| Dimension | The question | Determined by |
|---|---|---|
| **Risk capacity** (ability) | How much loss can your finances absorb without derailing your goals? | Time horizon, job stability, other income, wealth relative to needs, debts |
| **Risk tolerance** (willingness) | How much loss can you endure emotionally without abandoning the plan? | Temperament, experience, how you actually behaved in 2008, 2020, 2022 |
| **Risk need** | How much risk must you take to reach your goal? | Savings rate, goal size, time — a high saver with modest goals may *need* very little |

A 28-year-old with a stable job has high capacity; whether they have high tolerance is unknown until they watch their balance fall 35%. A 63-year-old with a fat pension has moderate capacity and may need very little risk. The binding constraint is always the *lowest* of the three. Larry Swedroe's framing — "ability, willingness, and need" — is the standard one and worth memorizing.

Practical tests of tolerance:

- Translate percentages into dollars. "−40%" is abstract; "$200,000 of your $500,000 gone" is not.
- Ask what you did in March 2020 and in 2022. Behavior beats questionnaires.
- If you would sell after a 30% decline, your stock allocation is too high — regardless of what a calculator says.

## Matching risk to horizon

The longer the horizon, the more volatility you can afford, because time smooths it. From the 1928–2025 record (S&P 500 with dividends):

| Horizon | Chance of a nominal loss | Worst outcome (annualized) |
|---|---|---|
| 1 year | ~27% | −44% |
| 5 years | ~12% | −13% |
| 10 years | ~6% | −2% |
| 20 years | 0% | +2.4% |

So: money needed within 2–3 years belongs in cash and short bonds; 3–10 years, a balanced mix; 10+ years, mostly stocks. That rule is the single most useful application of everything on this page.

## Key takeaways

- Risk has three faces: volatility (what you feel), permanent loss (what hurts), and shortfall (running out). Cash is "safe" only on the first two.
- U.S. stocks: ~19% annual volatility, six years of −20% or worse since 1928, and peak-to-trough crashes of 49%, 57%, and 85%.
- A 50% loss needs a 100% gain to recover — avoiding catastrophe beats chasing upside.
- Bear markets (−20%+) arrive roughly every 4–6 years and typically take 2–5 years to recover; budget for several in a lifetime.
- Sequence-of-returns risk is irrelevant while saving and critical while withdrawing — keep a cash cushion around retirement.
- Your stock allocation is bounded by the lowest of risk capacity, tolerance, and need — not by the highest.
- Sharpe ratio (return per unit of volatility) is the fair way to compare strategies; long-run stocks are ≈ 0.4.
- Match horizon to asset: under 3 years cash, 3–10 balanced, 10+ mostly stocks.

## Sources

- [Damodaran, NYU Stern — Historical Returns on Stocks, Bonds and Bills: 1928–2025](https://pages.stern.nyu.edu/~adamodar/New_Home_Page/datafile/histretSP.html) (rolling-period and volatility figures computed from this data)
- [DQYDJ — S&P 500 Drawdown History (1871–present)](https://dqydj.com/sp-500-drawdown-history/)
- [Finlume — How Long the S&P 500 Takes to Recover After a Crash](https://finlume.net/en/blog/market-crash-recovery-time/)
- [Wikipedia — Closing milestones of the S&P 500](https://en.wikipedia.org/wiki/Closing_milestones_of_the_S&P_500)
- [Bogleheads wiki — Risk tolerance](https://www.bogleheads.org/wiki/Risk_tolerance)
- [Bogleheads wiki — Sequence of returns risk](https://www.bogleheads.org/wiki/Sequence_of_returns_risk)
- [Investopedia — Sharpe Ratio](https://www.investopedia.com/terms/s/sharperatio.asp)
- [Investopedia — Beta](https://www.investopedia.com/terms/b/beta.asp)
- [Investopedia — Maximum Drawdown (MDD)](https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp)
- [Investor.gov — Assessing your risk tolerance](https://www.investor.gov/introduction-investing/getting-started/assessing-your-risk-tolerance)
- [CFA Institute — Risk Management (Investment Foundations)](https://www.cfainstitute.org/insights/professional-learning/refresher-readings)
