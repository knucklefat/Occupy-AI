# Valuation Methods

**In one sentence:** Every valuation method is a way of estimating what a stream of future cash is worth today, and the honest goal is not a precise number but a defensible range that tells you whether the current price is clearly cheap, clearly expensive, or somewhere in the muddy middle.

## The core idea

A business is worth the cash it will hand its owners over its life, discounted back to today because money later is worth less than money now. Everything below is a variation on that idea. The two families are:

- **Intrinsic (absolute) valuation:** estimate the cash flows and discount them (DCF, dividend discount model).
- **Relative valuation:** see what the market pays for similar assets (multiples/comparables).

Aswath Damodaran of NYU Stern, whose free lecture notes and data are the standard reference, argues that you should do both, because each catches the other's errors.

## Discounted cash flow (DCF)

**The formula.** Value today = sum over each year of (Cash flow in year t) ÷ (1 + r)^t, plus a **terminal value** for everything after your forecast window.

Where:
- **Cash flow** is usually **free cash flow to the firm (FCFF)** = operating income × (1 − tax rate) + depreciation − capex − change in working capital. This is cash available to all capital providers (debt and equity).
- **r** is the discount rate. For FCFF, use the **weighted average cost of capital (WACC)** — a blend of what equity investors demand and what lenders charge, weighted by the capital structure. For most large U.S. companies this lands between 7% and 10%.
- **Terminal value** (Gordon growth form) = FCF in the first year after the forecast ÷ (r − g), where g is a perpetual growth rate that must be at or below the long-run growth of the economy (roughly 2–4% nominal).

Then: **Enterprise value** = PV of forecast cash flows + PV of terminal value. **Equity value** = enterprise value − net debt. **Per-share value** = equity value ÷ diluted shares.

### Worked example

A company generated $100M of free cash flow last year. You expect FCF to grow 8% a year for five years, then 3% forever. Discount rate 9%. Net debt $300M, 100M diluted shares.

| Year | FCF ($M) | Discount factor (1.09^t) | Present value ($M) |
|---|---|---|---|
| 1 | 108.0 | 1.090 | 99.1 |
| 2 | 116.6 | 1.188 | 98.2 |
| 3 | 126.0 | 1.295 | 97.3 |
| 4 | 136.0 | 1.412 | 96.4 |
| 5 | 146.9 | 1.539 | 95.5 |
| **Sum of years 1–5** | | | **486.4** |

Terminal value at end of year 5 = 146.9 × 1.03 ÷ (0.09 − 0.03) = $2,522M.
Present value of terminal value = 2,522 ÷ 1.539 = $1,639M.

Enterprise value = 486 + 1,639 = **$2,126M**. Subtract net debt of $300M → equity value $1,826M → **$18.26 per share**.

Notice that 77% of the value sits in the terminal value. That is typical and is the main reason DCF outputs are so sensitive to assumptions.

### Sensitivity

| Discount rate | Value per share |
|---|---|
| 8% | $22.60 |
| 9% | $18.26 |
| 10% | $15.16 |

A one-point change in the discount rate moves the value by roughly 20%. This is why professionals present DCF results as a table or range, never a single number, and why Damodaran stresses that the story behind the numbers matters more than the spreadsheet.

## Reverse DCF

Instead of guessing inputs and getting a price, start from the market price and ask **what growth is the market already assuming?** Using the example above: if the stock trades at $25, the implied enterprise value is $2,800M. Holding the 9% discount rate and 3% terminal growth, the market is pricing in roughly 15% annual FCF growth for five years. Now your job is simpler and more honest: is 15% growth plausible for this business? Reverse DCF turns valuation from prediction into judgment.

## Comparables (multiples)

Relative valuation asks what the market pays for similar businesses. Pick a metric (earnings, EBITDA, sales, book value, FCF), find a peer group, and compare.

**Steps:**
1. Choose the multiple that fits the business: P/E for stable earners, EV/EBITDA for capital-structure-neutral comparison, P/S for high-growth or unprofitable firms, P/B for banks, P/FFO for REITs.
2. Build a peer set of 5–10 companies with similar growth, margins, and risk. Same sector is not enough — a 30%-growth software firm is not a peer of a 5%-growth one.
3. Compute the peer median and range.
4. Apply to your company, adjusting up or down for differences in growth, margins, and balance sheet strength.

**Example.** Peers trade at a median 12× EV/EBITDA. Your company has EBITDA of $200M, net debt of $300M, and 100M shares. Implied EV = $2,400M → equity $2,100M → $21 per share. If your company grows faster than peers with better margins, a premium multiple (say 14×) is defensible → $25 per share.

**The trap.** Comparables tell you whether a stock is cheap relative to peers, not whether the peers themselves are reasonably priced. In 1999, comparing one internet stock with another said nothing about the fact that all of them were absurd.

## Dividend discount model (DDM)

For companies that pay steady dividends (utilities, banks, consumer staples), value the dividends directly. The **Gordon growth model**: Value = D1 ÷ (r − g), where D1 is next year's dividend, r is the cost of equity, and g is the long-run dividend growth rate.

**Example.** A utility pays $2.00 today, expected to grow 3% a year; you require an 8% return. D1 = $2.06. Value = 2.06 ÷ (0.08 − 0.03) = **$41.20**. If the stock trades at $35, it offers a margin of safety; at $50, it does not. The DDM is very sensitive to (r − g) — if g rises to 4%, value jumps to $52.

Multi-stage DDMs allow a high-growth phase before settling into steady growth, which fits companies still ramping their payout.

## Sum-of-the-parts (SOTP)

For conglomerates or companies with distinct segments (a retailer with a credit card arm, a tech firm with a cloud business and a hardware business), value each segment separately with the multiple that fits it, add them up, subtract corporate costs and net debt. SOTP often reveals a "conglomerate discount" — the whole trading for less than the parts — which can be a source of value if management is willing to spin off or sell segments. Activist investors use SOTP constantly.

## Damodaran's approach

Damodaran's teaching, distilled:

- **Every valuation is a story plus numbers.** Write the narrative first (what does this company become?), then build the numbers to fit it, then test whether the story is possible, plausible, and probable.
- **Value the business, not the stock.** Start with operating cash flows and a cost of capital; get to equity last.
- **Be explicit about the terminal value assumptions.** Growth cannot exceed the economy's forever, and the return on capital in the terminal period should converge toward the cost of capital unless the moat is exceptional.
- **Use the market as a check, not a guide.** Compare your intrinsic value with relative pricing; large gaps demand explanation.
- **Accept uncertainty.** Run scenarios and Monte Carlo distributions rather than pretending to precision. His NYU pages offer free spreadsheets and industry data on betas, margins, and multiples.

## Common errors

| Error | Why it matters | Fix |
|---|---|---|
| Terminal growth above GDP growth | Implies the company eventually becomes the whole economy | Cap g at 2–4% nominal |
| Mismatched cash flow and discount rate | FCFF must be discounted at WACC; FCFE at cost of equity | Match them |
| Forgetting net debt or dilution | Overstates per-share value | Subtract debt, add cash, use diluted shares |
| Using adjusted, not GAAP, cash flows | SBC and "one-time" items are real costs | Subtract SBC from FCF or add shares |
| Peer group by sector name only | Wrong peers give wrong multiples | Match on growth, margin, and risk |
| Anchoring the DCF to the current price | Reverse-engineering to justify a buy | Do the reverse DCF openly instead |
| False precision | "$18.26" implies certainty that does not exist | Present a range and sensitivity table |
| Ignoring the cycle | Peak earnings at a low multiple can be the most expensive moment | Normalize earnings over a cycle |

## How to actually do it

1. Write a one-paragraph story: what does this company look like in ten years, and why?
2. Gather five to ten years of revenue, operating margin, tax rate, capex, depreciation, and working capital from the 10-K or an aggregator.
3. Project revenue and margins for five years consistent with your story. Derive FCFF.
4. Set the discount rate: use Damodaran's industry cost-of-capital data as a starting point (roughly 7–10% for most U.S. companies), adjusting up for smaller or riskier firms.
5. Set terminal growth at 2–3%. Compute terminal value and discount it.
6. Sum, subtract net debt, divide by diluted shares. Record the result.
7. Build a sensitivity table across discount rates (±1%) and terminal growth (±1%).
8. Run a reverse DCF from the current price to see the implied growth. Ask whether it is plausible.
9. Cross-check with peer multiples (EV/EBITDA, P/E, FCF yield).
10. Only act when the price is well below the *low* end of your range — that gap is your margin of safety.

## Key takeaways

- All valuation is discounting future cash; methods differ only in how they estimate the cash and the rate.
- The terminal value typically drives most of a DCF, so small changes in discount rate or terminal growth swing results by 20% or more.
- Always present a range and sensitivity table, never a single number.
- Reverse DCF is the most honest tool: it turns valuation into a question about plausibility.
- Multiples are fast and market-grounded but only tell you cheapness relative to peers.
- DDM works for steady dividend payers and is very sensitive to (r − g).
- Sum-of-the-parts uncovers hidden value in conglomerates.
- Damodaran's rule: story first, numbers second, and test the story for plausibility.

## Sources

- [Damodaran: Discounted Cash Flow Valuation: Equity and Firm Models (NYU Stern)](https://pages.stern.nyu.edu/~adamodar/pdfiles/ovhds/dam2ed/dcfveg.pdf)
- [Damodaran: The Free Cashflow to Firm Model (NYU Stern)](https://pages.stern.nyu.edu/~adamodar/pdfiles/eqnotes/fcff.pdf)
- [Damodaran: Discounted Cash Flow Valuation: The Inputs (NYU Stern)](https://pages.stern.nyu.edu/~adamodar/pdfiles/dcfinput.pdf)
- [Damodaran: Valuation Approaches and Metrics: A Survey of the Theory and Evidence](https://pages.stern.nyu.edu/~adamodar/pdfiles/papers/valuesurvey.pdf)
- [Damodaran Online: Current data (cost of capital, multiples by industry)](https://pages.stern.nyu.edu/~adamodar/New_Home_Page/datacurrent.html)
- [Investopedia: Discounted Cash Flow (DCF)](https://www.investopedia.com/terms/d/dcf.asp)
- [Investopedia: Gordon Growth Model](https://www.investopedia.com/terms/g/gordongrowthmodel.asp)
