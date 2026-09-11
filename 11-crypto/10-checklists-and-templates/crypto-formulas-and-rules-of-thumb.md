# Crypto Formulas and Rules of Thumb

**In one sentence:** The dozen calculations you actually need to size, value, and sanity-check crypto positions — FDV, supply ratio, MVRV, NVT, annualized funding, basis-trade yield, impermanent loss (with a worked example), real staking yield, volatility-based sizing, breakeven after a drawdown, and DCA average cost — each with the formula, a worked number, and the rule of thumb that follows from it.

**How to use it:** Keep this open next to the [pre-trade checklist](pre-trade-checklist-for-crypto.md) and the [token due diligence checklist](token-due-diligence-checklist.md). Every formula is arithmetic you can do on a phone calculator. The rules of thumb are historical tendencies, not laws; the point is to notice when a number is far outside its normal range.

---

## 1. Fully diluted valuation (FDV)

**What it is:** what the entire eventual token supply would be worth at today's price. Market cap only counts tokens that are circulating now.

```
FDV = current price × total (or max) supply
Market cap = current price × circulating supply
```

**Worked example:** Token at $2.00; circulating supply 200M; total supply 1B.
Market cap = $400M. FDV = $2.0B.

**Rule of thumb:** Compare FDV, not market cap, when judging whether a token is "cheap." If FDV is 5× market cap, the market has not yet had to absorb 80% of the supply.

## 2. Circulating-to-total supply ratio

```
Supply ratio = circulating supply ÷ total supply
Overhang = 1 − supply ratio
```

**Worked example:** 200M ÷ 1B = 20% circulating; 80% overhang.

**Rules of thumb:**
- Below ~30% circulating: expect years of sell pressure from unlocks; price needs strong demand growth just to stay flat.
- Above ~80% circulating: unlock risk is mostly behind it; valuation is closer to "what you see is what you get."
- Monthly unlock above ~5% of circulating supply = a scheduled price event; check the date before buying.

## 3. MVRV (market value to realized value)

**What it is:** a bitcoin (and ether) on-chain valuation gauge. **Realized cap** values every coin at the price it last moved on-chain — roughly the aggregate cost basis of all holders. MVRV compares today's price to that cost basis.

```
MVRV = market cap ÷ realized cap
```

**Reading it:** MVRV = 1 means the average coin is at breakeven. MVRV = 3 means the average holder is sitting on a 200% unrealized gain — historically the zone where profit-taking accelerates.

**Rules of thumb (historical, bitcoin):** readings below ~1.0 have coincided with cycle bottoms (holders under water in aggregate); readings above ~3.5 have coincided with cycle tops. Each cycle's extremes have been less extreme than the last, so treat the thresholds as fuzzy and shrinking. Available free on Glassnode, CryptoQuant, and similar dashboards.

## 4. NVT (network value to transactions)

**What it is:** crypto's rough analog to a price-to-sales ratio — network value divided by the value actually moving across the chain.

```
NVT = market cap ÷ daily on-chain transaction volume (USD)
NVT signal = market cap ÷ 90-day average of daily on-chain volume   (smoother)
```

**Reading it:** high NVT = price has run ahead of usage; low NVT = usage is high relative to price.

**Rules of thumb:** more useful for spotting *changes* than absolute levels; on-chain volume is distorted by exchange internal transfers, L2 batching, and wash activity, so compare a coin to its own history rather than across coins.

## 5. Funding rate, annualized

**What it is:** on perpetual futures ("perps"), longs pay shorts (or vice versa) a small fee every 8 hours to keep the perp price pinned to spot. Positive funding = longs are paying = crowded long.

```
Annualized funding ≈ 8-hour rate × 3 × 365
```

**Worked example:** funding of 0.01% per 8 hours → 0.01% × 3 × 365 = **10.95% per year** (this is roughly the "neutral" baseline on major exchanges). Funding of 0.10% per 8 hours → **109.5% per year** — extremely crowded long.

**Rules of thumb:** sustained funding above ~30–50% annualized means leveraged longs are paying a fortune to stay in; that is when long squeezes happen. Persistently negative funding in a rising market is the mirror image. You do not need to trade perps to use this as a sentiment gauge.

## 6. Basis (cash-and-carry) trade yield

**What it is:** the annualized return from buying spot and simultaneously selling a dated future at a higher price, locking in the gap.

```
Annualized basis yield = ((futures price − spot price) ÷ spot price) × (365 ÷ days to expiry)
```

**Worked example:** spot BTC $60,000; 90-day future $61,200.
Gap = 2.0%; annualized = 2.0% × (365 ÷ 90) = **8.1%**.

**Rules of thumb:** compare it to the risk-free rate — the basis is only worth the counterparty and operational risk if it clears T-bills by a meaningful margin. When the basis blows out to 20%+ annualized, speculative demand is extreme (and the trade gets crowded and then unwinds violently). Retail investors mostly should not run this trade; the number is still worth watching.

## 7. Impermanent loss (IL)

**What it is:** when you provide liquidity to a two-asset constant-product pool (Uniswap v2-style), the pool automatically sells the asset that rises and buys the one that falls. If prices diverge, you end up with less value than if you had simply held both assets. Trading fees are meant to compensate; they do not always.

```
Let k = (new price ÷ original price) of asset A relative to asset B.

IL = ( 2 × √k ÷ (1 + k) ) − 1
```

IL is the percentage by which your pool position underperforms holding. It is symmetric: a 2× move and a 0.5× move produce the same loss.

**Lookup table:**

| Price change of A vs B (k) | Impermanent loss |
|---|---|
| 1.25× or 0.8× | −0.6% |
| 1.5× or 0.67× | −2.0% |
| 2× or 0.5× | −5.7% |
| 3× or 0.33× | −13.4% |
| 4× or 0.25× | −20.0% |
| 5× or 0.2× | −25.5% |
| 10× or 0.1× | −42.5% |

**Worked example:**
You deposit 1 ETH at $2,000 and 2,000 USDC into an ETH/USDC pool (total $4,000). ETH doubles to $4,000 (k = 2).

- *If you had held:* 1 ETH ($4,000) + 2,000 USDC = **$6,000**.
- *In the pool:* the constant-product rule (ETH × USDC stays constant at 2,000) rebalances you to 0.7071 ETH and 2,828.43 USDC. Value = 0.7071 × $4,000 + $2,828.43 = **$5,656.85**.
- IL = $5,656.85 ÷ $6,000 − 1 = **−5.7%**, or about $343 — matching the formula: 2 × √2 ÷ 3 − 1 = −0.0572.

You still made money ($4,000 → $5,657) — just less than holding. Fees earned over the period need to exceed $343 for the LP position to have been worth it.

**Rules of thumb:** IL is small for correlated pairs (ETH/stETH, USDC/USDT) and large for volatile-vs-stable pairs. Before providing liquidity, estimate a realistic price range, read the IL off the table, and compare to the *fee* APR (not the token-emission APR). Concentrated-liquidity pools (Uniswap v3-style) amplify both fees and IL.

## 8. Real staking yield

**What it is:** staking rewards are largely paid in newly issued tokens. If the network inflates supply by 3% and pays you 4%, you are only 1% ahead of the dilution everyone else suffers.

```
Real staking yield (approx.) = nominal staking yield − supply inflation rate
Real staking yield (exact)   = (1 + nominal) ÷ (1 + inflation) − 1
```

**Worked example:** nominal yield 4.0%, inflation 1.5%.
Approximate: 2.5%. Exact: 1.04 ÷ 1.015 − 1 = **2.46%**.
Flip side: a non-staker's share of the network shrinks by 1.5% a year.

**Rules of thumb:** a "20% staking APY" on a token inflating 18% is a 2% real yield plus the price risk of a token that dilutes 18% a year. Always ask what fraction of rewards are protocol fees (real) versus emissions (dilution). Staking also carries slashing risk, lock-up/unbonding periods, and tax on rewards at receipt — subtract those mentally.

## 9. Position sizing for volatility

**What it is:** crypto's volatility is several times that of stocks, so a "small" crypto allocation carries a large share of portfolio risk. Three ways to size:

**(a) Volatility-equivalent sizing** — how much crypto carries the same risk as a given stock position.
```
Crypto weight = stock weight × (σ_stocks ÷ σ_crypto)
```
Worked: you would be comfortable with a 15% position in a diversified stock fund (σ ≈ 16%). Bitcoin σ ≈ 60%. Equivalent bitcoin weight ≈ 15% × (16 ÷ 60) = **4%**. Each 1% in bitcoin ≈ 3.75% in stocks, risk-wise; altcoins (σ 90–120%) are roughly twice that again.

**(b) Risk-budget sizing** — decide how much portfolio volatility crypto may contribute.
```
Crypto weight = target vol contribution ÷ σ_crypto
```
Worked: you allow crypto to add 3 percentage points of annualized volatility. 3% ÷ 60% = **5%** allocation.

**(c) Max-loss sizing** — decide the most you will accept losing from this sleeve.
```
Crypto weight = acceptable portfolio loss ÷ assumed drawdown
```
Worked: you can accept losing 2% of your portfolio to crypto; you assume an 80% drawdown is possible. 2% ÷ 80% = **2.5%** allocation. For a single altcoin, assume a 100% drawdown: an acceptable 0.5% portfolio loss → 0.5% position.

**Rules of thumb:** the three methods typically land in the 1–5% range for most investors, which is why that range appears throughout this library. Rebalance back to target; volatility means the weight drifts fast in both directions. See the main library's [position sizing guide](../../03-techniques/position-sizing-and-risk-management.md).

## 10. Breakeven gain after a drawdown

**What it is:** losses and gains are not symmetric. The gain required to recover a loss grows faster than the loss.

```
Gain needed to break even = 1 ÷ (1 − loss) − 1
```

| Drawdown | Gain needed to recover |
|---|---|
| −10% | +11.1% |
| −20% | +25% |
| −30% | +42.9% |
| −40% | +66.7% |
| −50% | +100% |
| −60% | +150% |
| −70% | +233% |
| −80% | +400% |
| −90% | +900% |
| −95% | +1,900% |

**Rules of thumb:** bitcoin has recovered from multiple −80% drawdowns; the overwhelming majority of altcoins have not, because +400% requires a new wave of buyers that never returns to most of them. This table is the mathematical reason for take-profit ladders, for capping single-token size, and for never averaging down into a broken thesis. It is also why leverage is forbidden in the IPS: a 2× leveraged position turns a −50% move into −100%.

## 11. Dollar-cost averaging: your average cost

**What it is:** buying a fixed *dollar* amount on a schedule buys more units when prices are low and fewer when high, so your average cost per unit is *below* the average price you paid at (it is the harmonic mean of prices, not the arithmetic mean).

```
Average cost per unit = total dollars invested ÷ total units acquired
```

**Worked example:** $100 each at prices of $50, $25, and $100.
Units: 2.0 + 4.0 + 1.0 = 7.0. Average cost = $300 ÷ 7 = **$42.86**.
The arithmetic average of the three prices was $58.33; DCA got you in 27% cheaper because it automatically bought most at the low.

**Rules of thumb:** DCA is a behavioral tool as much as a mathematical one — it removes the "is now a good time?" question. Lump-sum investing has historically beaten DCA more often than not in *rising* markets, but in an asset with 80% drawdowns the regret-minimization value of DCA is high. Keep the schedule fixed; do not pause in crashes (that is when it earns its keep) and do not accelerate in rallies.

## 12. Round-trip cost and hurdle

**What it is:** the total percentage you lose to fees and spread on a buy and a subsequent sell, which your thesis must beat before you make anything.

```
Round-trip cost ≈ buy fee + buy spread + network/withdrawal fees (as % of position) + sell fee + sell spread
```

**Worked example:** 0.4% fee + 0.3% spread on the buy, $15 withdrawal on a $2,000 position (0.75%), 0.4% + 0.3% on the sale = **~2.15%**. A "simple buy" button with a 1.5% spread each way doubles that.

**Rule of thumb:** for small positions, network and withdrawal fees dominate; for frequent trading, spread dominates. If your round-trip cost exceeds ~1%, use the exchange's pro/advanced interface and batch withdrawals.

---

## Quick reference

| Question | Formula | Sane range / rule |
|---|---|---|
| Is it cheap? | FDV = price × total supply | Judge on FDV; supply ratio < 30% = heavy overhang |
| Are holders in profit? (BTC) | MVRV = market cap ÷ realized cap | < 1 bottom-ish; > 3.5 top-ish (historical) |
| Is price ahead of usage? | NVT = market cap ÷ on-chain volume | Compare to own history |
| How crowded are longs? | 8h funding × 3 × 365 | ~11%/yr neutral; > 30–50% crowded |
| What does carry pay? | (fut − spot)/spot × 365/days | Compare to T-bills |
| What will LP cost me? | 2√k/(1+k) − 1 | 2× move = −5.7%; 4× = −20% |
| Is staking yield real? | nominal − inflation | Emissions ≠ income |
| How big a position? | stock weight × σ_stocks/σ_crypto | Usually 1–5% total crypto |
| Can it come back? | 1/(1 − loss) − 1 | −80% needs +400% |
| What did DCA cost me? | $ invested ÷ units bought | Below the average price |

---

## Sources

- [Token Terminal — Fundamentals for crypto](https://tokenterminal.com/) (FDV, circulating market cap, fees and revenue definitions)
- [Kraken — Proof of reserves](https://www.kraken.com/proof-of-reserves) (scope includes margin, futures collateral, and staking allocations — context for funding and basis)
- [DefiLlama — Hacks database](https://defillama.com/hacks) (context for LP and protocol risk)
- [IRS — Frequently asked questions on digital asset transactions](https://www.irs.gov/individuals/international-taxpayers/frequently-asked-questions-on-digital-asset-transactions) (staking rewards taxed at receipt; basis includes fees)
- Main library: [Position sizing and risk management](../../03-techniques/position-sizing-and-risk-management.md) and [Useful formulas and rules of thumb](../../10-checklists-and-templates/useful-formulas-and-rules-of-thumb.md)
