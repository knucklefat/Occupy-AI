# Position Sizing and Risk Management

**In one sentence:** How much you put into any single position matters more than whether you were right about it — sizing rules like fixed-fractional risk, the Kelly criterion, and hard concentration caps are what keep one bad call from ending the game.

## The core idea: survive first

A 50% loss needs a 100% gain to recover. A 90% loss needs 900%. Returns compound geometrically, which means large losses are disproportionately destructive. Every sizing rule below is, at bottom, a way of keeping individual losses small enough that you are still in the game to benefit from being right later.

| Loss | Gain needed to break even |
|---|---|
| 10% | 11% |
| 25% | 33% |
| 50% | 100% |
| 75% | 300% |
| 90% | 900% |

## Kelly criterion

The Kelly criterion (John Kelly, Bell Labs, 1956) gives the bet size that maximises the long-run growth rate of your capital when you know the odds. For a bet that wins with probability *p*, loses with probability *q* = 1 − *p*, and pays *b* dollars per dollar risked:

**f\* = (b × p − q) / b**

where *f\** is the fraction of your bankroll to wager.

**Worked example.** A bet wins 60% of the time and pays even money (*b* = 1). Then *f\** = (1 × 0.6 − 0.4) / 1 = **0.20**, so bet 20% of your capital. If it paid 2-to-1 with only a 40% win rate: *f\** = (2 × 0.4 − 0.6) / 2 = 0.10, or 10%.

For continuous investments (a stock rather than a coin flip) the usual approximation is **f\* ≈ (expected excess return) / (variance)**. A stock with 5% expected return above cash and 16% volatility gives *f\** ≈ 0.05 / 0.16² ≈ 1.95 — i.e., nearly 2× leverage. That tells you something important: **full Kelly is extremely aggressive**, and it assumes you know the true odds, which in markets you never do. Overestimating your edge even slightly pushes you past the Kelly point, where growth turns *negative*.

The practical response is **half-Kelly** (or less): you give up about a quarter of the theoretical growth rate in exchange for roughly halving the volatility and drawdowns, and you get a large margin for being wrong about your edge. Most professional users treat Kelly as a ceiling, not a target.

## Fixed-fractional sizing

Simpler and more common among traders: risk a fixed percentage of your account per position, usually **1–2%**. "Risk" means the amount you would lose if your stop-loss is hit, not the position size.

**Position size = (Account × risk %) / (Entry price − Stop price)**

**Example.** $100,000 account, 1% risk ($1,000), stock at $50 with a stop at $45 ($5 risk per share) → buy **200 shares** ($10,000 position). A wider stop at $40 → 100 shares ($5,000). Notice the position *shrinks* when the stop is wider: the risk stays constant.

At 1% per position it takes many consecutive losers to do serious damage (ten straight losses ≈ −9.6%), which is why this rule is the backbone of most systematic trading.

## Volatility-based sizing

Instead of a price stop, size by how much the asset moves. Two common versions:

- **ATR sizing.** Use Average True Range (a measure of typical daily price movement). Shares = (Account × risk %) / (k × ATR), with *k* typically 2–3. A stock with a $2 daily ATR and *k* = 2 on a $100,000 account at 1% risk → $1,000 / $4 = 250 shares.
- **Volatility targeting.** Allocate so each holding contributes equal expected volatility: weight ∝ 1 / volatility. A 30%-vol crypto position gets a third the weight of a 10%-vol bond fund. This is the logic behind "risk parity" portfolios.

## Concentration limits

For long-term investors the more relevant rules are portfolio-level caps:

- **Single stock: 5% max, 10% absolute ceiling.** Beyond this, one company's idiosyncratic risk (fraud, a failed drug trial, a CEO scandal) can meaningfully dent your net worth.
- **Employer stock: under 10%,** and ideally lower — your salary already depends on that company. Enron employees held 60% of their 401(k)s in Enron.
- **Single sector: 20–25%** unless you are deliberately making a sector bet and know it.
- **Illiquid or speculative assets (private deals, crypto, options): 5–10% total.**

Hendrik Bessembinder's research found that just 4% of U.S. stocks accounted for all net stock-market wealth creation since 1926; the median stock underperformed Treasury bills. Concentrating in a few names is a bet that you have picked from the 4%.

## Stop-losses: the evidence

A **stop-loss** is a standing order to sell if price falls to a set level. A **trailing stop** moves the trigger up as the price rises (e.g., "sell if it falls 15% from its high") but never down.

**The case for:** Stops cap the worst outcome, remove emotion at the moment of decision, and enforce the fixed-fractional discipline above. Kaminski and Lo's paper "When Do Stop-Loss Rules Stop Losses?" shows that stops add value when returns exhibit **momentum** (losers keep losing) — which has been true for individual stocks over months.

**The case against:** The same paper shows stops *destroy* value when returns **mean-revert** (dips bounce back) — which is typical for broad index funds and over short horizons. A stop on an S&P 500 fund is a systematic way to sell low and buy back higher. Stops are also vulnerable to gap-downs (a stock opens 30% below your stop and you are filled there, not at your stop) and to "stop hunting" volatility around round numbers. Studies of retail traders (Barber and Odean's work) show they already sell winners too soon and hold losers too long; stops can help the second problem but worsen the first.

**Sensible synthesis:**
- Diversified index funds in a long-term portfolio: **no stop-losses.** Use rebalancing instead.
- Individual stocks or concentrated positions: a **wide** stop (20–25%) or a trailing stop is defensible as a discipline tool, especially for positions you would not have the stomach to sell manually.
- Never set stops so tight that normal noise triggers them (well inside 2× ATR).

## How to actually do it

1. Decide what kind of investor you are: buy-and-hold indexer (skip stops, use concentration caps and rebalancing) or active stock-picker/trader (use fixed-fractional risk).
2. Write hard limits: max single position, max sector, max employer stock, max speculative bucket.
3. If trading: pick a risk-per-trade (1% is standard; never above 2%), define your exit before entry, and compute shares from the formula above.
4. If using Kelly: estimate your edge conservatively, compute *f\**, and use half of it or less.
5. Set up a monthly check of concentration — winners quietly become oversized positions.
6. When a single holding breaches its cap, trim it back regardless of how good the story is. Trim in tax-advantaged accounts or with high-cost lots first.
7. Review the rules yearly; never mid-trade.

## Key takeaways

- Losses compound asymmetrically: a 50% loss needs a 100% gain to recover, so keep every single loss small.
- Kelly: *f\** = (bp − q)/b. Full Kelly is a ceiling; half-Kelly is the practical choice given you never know your true edge.
- Fixed-fractional sizing (risk 1–2% per position, size = risk ÷ distance to stop) is the workhorse of disciplined trading.
- Cap single stocks at 5–10%, employer stock under 10%, speculative assets at 5–10% total.
- Stop-losses help when losers keep losing (single stocks, momentum) and hurt when dips bounce (index funds).
- Trailing stops are a reasonable discipline for concentrated positions you might otherwise ride into the ground.
- Volatility-based sizing equalises risk across holdings with very different behaviour.

## Sources

- [Kelly, J. L. (1956) – A New Interpretation of Information Rate (Bell System Technical Journal)](https://ieeexplore.ieee.org/document/6771227)
- [Kaminski & Lo – When Do Stop-Loss Rules Stop Losses? (MIT open access)](https://dspace.mit.edu/bitstream/handle/1721.1/114876/Lo_When%20Do%20Stop-Loss.pdf)
- [Kaminski & Lo – SSRN abstract](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=968338)
- [Bessembinder (2018) – Do Stocks Outperform Treasury Bills? (SSRN)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2900447)
- [Bogleheads wiki – Kelly criterion](https://www.bogleheads.org/wiki/Kelly_criterion)
- [Investopedia – Position sizing](https://www.investopedia.com/terms/p/positionsizing.asp)
