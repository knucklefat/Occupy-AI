# Position Sizing and Rebalancing for Crypto

**In one sentence:** Size a crypto position by its volatility, not your enthusiasm — a sleeve that moves three to four times as much as stocks needs to be three to four times smaller to carry the same risk — then let mechanical rebalancing bands and a pre-written profit-taking rule make the buy-low/sell-high decisions you will not make under stress.

## Start with volatility, not conviction

**Volatility** is the annualized standard deviation of returns — roughly, how wide the typical yearly swing is. Long-run figures (as of September 2026):

| Asset | Typical annualized volatility | Rough ratio to S&P 500 |
|---|---|---|
| S&P 500 | ~15–20% (long run); ~8% in calm 2024 | 1× |
| Gold | ~12–15% | ~0.8× |
| Bitcoin | ~35–60% recently; 2025 was its calmest year on record (~35–45%); 100%+ in 2017 and 2021 | ~3–4× long run (~4.8× on a ten-year basis) |
| Ethereum | ~60–80% | ~4–5× |
| Small-cap altcoins | 100%+ | 6×+ |

The rule of thumb: **crypto carries roughly three to four times the volatility of a broad stock index**, and bitcoin has had drawdowns (peak-to-trough declines) of 75–85% four separate times. A position you would happily hold at 20% of your portfolio in stocks is, in risk terms, a 5–7% crypto position.

### Volatility-scaled sizing

Pick a "risk budget" — how much of your portfolio's total volatility you are willing to let one sleeve contribute — and back into the weight:

> Crypto weight ≈ (target risk contribution) ÷ (crypto volatility ÷ portfolio volatility)

Example: you run a 60/40 portfolio with ~10% volatility. You are willing to let crypto add roughly 2 percentage points of volatility. Bitcoin at ~45% volatility is 4.5× your portfolio's. 2% ÷ 4.5 ≈ **4–5% weight**. If you hold ETH or altcoins at 70%+ volatility, the same risk budget buys **~3%**.

Sanity checks:

- Can you watch this sleeve fall 80% without selling or changing your life? If not, it is too big.
- Never fund it with money you need within five years, and never with leverage.
- Count crypto held in an ETF, an IRA, an exchange, and a hardware wallet as *one* sleeve.

## Rebalancing bands for a volatile sleeve

Calendar rebalancing (quarterly, yearly) works for stocks and bonds. For something that can double in three months, **percentage bands** work better: you act when the weight drifts outside a range, not on a date.

A common band rule is **relative ±25–50%** of target:

| Target weight | Sell down to target when above | Buy back to target when below |
|---|---|---|
| 3% | 4.0–4.5% | 2.0–2.25% |
| 5% | 6.5–7.5% | 3.5–4.0% |
| 10% | 12.5–15% | 7.0–8.0% |

Wider bands mean fewer trades (less tax, fewer fees) but bigger drift; narrower bands harvest volatility more often. Check weights monthly; trade only when a band is breached. In taxable accounts, first direct *new contributions* to the underweight asset before selling anything, and prefer selling lots held over a year.

Mathematically, rebalancing a volatile, mean-reverting asset against a stable one earns a "rebalancing bonus" — you are systematically selling strength and buying weakness. Emotionally it feels wrong every single time. That is why the rule is written down in advance.

## Taking profits systematically

Crypto cycles have historically produced both euphoric tops and ~80% drawdowns. The people who kept gains had a rule for selling on the way *up*. Three workable rules:

1. **Sell X% per doubling.** Each time the position doubles from your cost basis, sell a fixed fraction (commonly 20–25%) of the *remaining* position. After the first double you have recovered your principal; everything left is "house money" with a documented cost basis.
2. **Band rebalancing (above).** Purely mechanical; sells more the faster it rises.
3. **Ladder of limit orders.** Place resting sells at, say, +50%, +100%, +200% from cost, each for a slice. They fill without you.

Whatever the rule, write it down with dates and numbers, and pre-commit where the proceeds go (rebalance into the rest of the portfolio, pay down debt, or a cash reserve earmarked for the next drawdown).

## Avoiding "sell everything at the bottom"

The typical retail path: buy after a 100% rally, hold through a 60% drop hoping, sell at −80% when the news is worst, watch it recover. The fixes are structural:

- **Size small enough that −80% is survivable** (the volatility rule above). Panic is a function of position size.
- **Pre-decide the drawdown response.** Options: "do nothing," "rebalance up to target at −50%," or "add a fixed dollar amount monthly." Any of these beats improvising.
- **Keep a cash reserve outside the sleeve** so you are never forced to sell crypto for living expenses.
- **Turn off price alerts** on the cold-storage portion. Check monthly with the rebalancing review.
- **Never use leverage or margin** on a volatile sleeve; liquidation removes your choice to hold.

## Worked example

Investor: $500,000 portfolio, 60/40 stocks/bonds, decides on a **5% bitcoin target** ($25,000) with **±40% relative bands** (rebalance when weight is above 7% or below 3%) and a **sell-25%-per-doubling** rule.

| Event | BTC price move | BTC value | Weight | Action |
|---|---|---|---|---|
| Start | — | $25,000 | 5.0% | Buy $25,000 over 10 weekly tranches (see DCA file) |
| Year 1: rally | +120% | $55,000 | ~10.4% | Doubling rule fires (sell 25% = $13,750) *and* the 7% band is breached, so the stricter rule wins: sell down to the 5% target (~$28,000 sold). Proceeds to bonds/cash. Cost basis of the remaining lots recorded. |
| Year 2: crash | −70% from peak | ~$8,000 (from ~$27,000 remaining) | ~1.6% | Below 3% band → buy back up to 5% target: ~$17,000 purchase, funded from the cash raised in year 1 |
| Year 3: recovery | +150% | ~$63,000 | ~11% | Above band → sell down to target again |

Compare the do-nothing path: $25,000 → $55,000 → $16,500 → $41,000. The banded path ends with more bitcoin *and* ~$11,000 of net cash still parked in safer assets ($28,000 raised minus $17,000 redeployed), because the $17,000 spent at the bottom bought roughly twice as many coins as the $28,000 sold near the top. The cost is some capital-gains tax in year 1 and the discipline to buy when headlines are grim.

## How to actually do it

1. Write down your total portfolio value and its approximate volatility (60/40 ≈ 10%; all-stock ≈ 16–18%).
2. Pick a risk budget for crypto (1–3 percentage points of portfolio volatility for most people).
3. Divide by the ratio of crypto volatility to portfolio volatility to get the target weight; round down.
4. Set percentage bands (±25–50% relative) and a profit-taking rule (e.g., sell 25% per doubling). Record them in a one-page investment policy.
5. Buy in tranches over 4–12 weeks rather than all at once.
6. Review weights on the first of each month. Trade only on band breaches or doubling triggers. Use new contributions before sales in taxable accounts.
7. Log every trade with date, price, lot, and reason (see [record-keeping-and-portfolio-tracking.md](record-keeping-and-portfolio-tracking.md)).
8. Re-read the policy once a year and after any 50% move in either direction — and change it only then, never mid-panic.

## Key takeaways

- Crypto's volatility is roughly 3–4× equities; scale the position down by that ratio to hold equal risk.
- 75–85% drawdowns have happened repeatedly; size so that one is survivable without selling.
- Use percentage rebalancing bands, not calendar dates, for a sleeve that can double in a quarter.
- Pre-commit a profit-taking rule ("sell 25% per doubling") and where the proceeds go.
- Cash reserves outside the sleeve and zero leverage are what prevent forced selling at the bottom.
- Rebalancing feels wrong in the moment every time; that is the point of writing the rule down.
- Count all crypto exposure (ETFs, exchanges, cold storage) as one sleeve.

## Sources

- [Bitcoin volatility tracker: historical and realized vol (Spark, 2026)](https://www.spark.money/tools/bitcoin-volatility-tracker)
- [Fidelity Digital Assets: A closer look at bitcoin's volatility](https://www.fidelitydigitalassets.com/research-and-insights/closer-look-bitcoins-volatility)
- [S&P 500 more volatile than bitcoin in April 2025 (CoinDesk)](https://www.coindesk.com/markets/2025/04/11/s-and-p-500-more-volatile-than-bitcoin-as-u-s-assets-lose-investor-favor)
- [Bitcoin vs S&P 500 historical performance (Spark, 2026)](https://www.spark.money/tools/bitcoin-vs-sp500-returns)
