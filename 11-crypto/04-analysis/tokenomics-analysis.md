# Tokenomics Analysis

**In one sentence:** Tokenomics is the study of how many tokens exist, who holds them, when new ones arrive, and whether anything the protocol does sends value back to the token, and getting these four questions right matters more than any narrative.

## Why tokenomics decides outcomes

Two protocols can have identical technology and users and produce opposite results for token holders, purely because of supply design. A token whose float doubles over 18 months through insider unlocks must attract twice the dollars just to stay flat. A token that burns a share of protocol fees has a tailwind even in a flat market. Tokenomics is not the whole story, but it is the part you can measure before you buy.

## The supply vocabulary

| Term | Definition | Why it matters |
|---|---|---|
| **Max supply** | Hard cap that can ever exist (Bitcoin: 21 million). Some tokens have none (ETH, SOL). | Scarcity claims are meaningless without one, but a cap alone doesn't create demand. |
| **Total supply** | Tokens minted so far, including locked ones. | The denominator for concentration analysis. |
| **Circulating supply** | Tokens that can actually be traded today. | Market cap = price × circulating supply. |
| **Float** | Circulating ÷ total (or ÷ max). | Low float means today's price is set by a thin slice of eventual supply. |
| **Market cap** | Price × circulating supply. | What the market is paying for the liquid piece. |
| **FDV (fully diluted valuation)** | Price × max (or total) supply. | What the market is implicitly paying for *everything*, including tokens not yet released. |
| **MC/FDV** | Market cap ÷ FDV. | The single fastest tokenomics screen. Below ~0.3 means most supply is still to come. |
| **Inflation rate** | Annual new issuance ÷ circulating supply. | Your hurdle rate: the token must grow demand by at least this much to hold price. |

Binance Research found that tokens launched in the first half of 2024 came to market with floats between roughly 6% and 20% and an average MC/FDV of 12.3%, the lowest in three years, and estimated around $155 billion of tokens would unlock from 2024 to 2030. Low float, high FDV became the defining tokenomic problem of that cycle.

## Emission schedules and unlock calendars

**Emissions** are new tokens created on a schedule: block rewards to miners or validators, liquidity-mining incentives, staking rewards. **Unlocks** are previously minted tokens that become transferable: team, investor, foundation, and airdrop tranches leaving their vesting contracts.

The typical venture-backed token has:

- A **cliff** (often 12 months) during which insiders receive nothing.
- **Linear vesting** after the cliff (often 24–36 months) during which tokens stream out daily or monthly.
- One or more **cliff unlocks** where a large tranche lands on a single day.

Cliff unlocks are the events that matter for price. Tokenomist (formerly Token Unlocks) tracks them: in August 2026 it counted roughly $876 million of cliff unlocks across tracked tokens, almost two-thirds of it in a single day when about $564 million of HYPE (Hyperliquid) unlocked on August 6. Note, though, that a scheduled unlock is not the same as a sale. Hyperliquid's March 2026 tranche saw only a small fraction of eligible tokens actually claimed, and unlocked tokens that stay in the same wallets have not hit the market. Watch the wallets, not just the calendar.

Where to find schedules:

- **Tokenomist** (tokenomist.ai): unlock calendar, allocation charts, and research.
- **CoinGecko / CoinMarketCap**: circulating vs total vs max supply, with a "tokenomics" tab on some assets.
- **DefiLlama** "Unlocks" page.
- **Messari** asset profiles for allocation tables.
- The project's own docs, which are the source of truth if they disagree with aggregators.

## Holder distribution and concentration

Open the token's block explorer page (Etherscan for ERC-20s, Solscan for Solana, and so on) and look at "Holders." You want to know:

- What share the top 10 and top 100 addresses hold, *after* excluding known exchange, bridge, staking, and vesting contracts (which the explorer usually labels).
- Whether the foundation or team wallets are identifiable and how they've moved. Arkham and Nansen label wallets; Bubblemaps visualizes clusters of connected addresses.
- Whether the "community" allocation is actually held by thousands of wallets or by a few addresses that received the airdrop then consolidated.

A rule of thumb: if the top 10 non-contract addresses hold more than a third of circulating supply, price is being set by a handful of decisions you can't see.

## Value accrual: does anything flow to the token?

This is the question tokenomics gets wrong most often. A protocol can earn hundreds of millions in fees while its token receives nothing. The main mechanisms, from strongest to weakest:

1. **Burns / buybacks funded by protocol revenue.** The protocol uses fees to buy tokens on the open market and destroys them (or holds them). Hyperliquid's Assistance Fund directs roughly 99% of protocol fees to buying HYPE, at an annualized pace of around $700 million in mid-2026; Uniswap's December 2025 "fee switch" vote turned on protocol fees and burned 100 million UNI (about $596 million at the time), with ongoing burns funded by a share of swap fees. Note that the market doesn't always reward this: UNI made a new all-time low around $2.90 in February 2026, two months after the burn, because the broader altcoin market fell and the activated fee stream (roughly $13 million a month by DefiLlama's September 2026 count) was smaller than the hype suggested.
2. **Direct fee distribution to stakers.** Fees paid in ETH, USDC, or the token itself go to those who stake. Compare this to dividends, and check whether the payout is in the native token (which is really just inflation redirected) or in an external asset.
3. **Staking that secures the network.** ETH and SOL stakers earn issuance plus fees; this is value accrual only to the extent the fee component is meaningful. Issuance-only staking yield is dilution shared among stakers.
4. **Fee discounts and access.** Holding the token gets you cheaper trading (BNB) or access to features. Real but weak: the value is capped by the discount.
5. **Governance only.** The token lets you vote. Unless votes can turn on a fee switch or direct a treasury, this is close to zero, and history shows most "governance tokens" traded as if the market agreed.

**Fee switch** is jargon for a governance-controlled parameter that redirects some fraction of fees from liquidity providers (or other supply-side participants) to the protocol or token holders. It's a switch because it's off by default, often for regulatory caution.

## A scoring rubric

Score each dimension 0–3 and sum. This is a screening tool, not a valuation.

| Dimension | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| MC/FDV | < 0.2 | 0.2–0.4 | 0.4–0.7 | > 0.7 |
| Insider share (team + investors) of total supply | > 50% | 35–50% | 20–35% | < 20% |
| Next 12 months' supply growth (unlocks + emissions) | > 50% | 25–50% | 10–25% | < 10% |
| Top-10 non-contract holder share of circulating | > 50% | 30–50% | 15–30% | < 15% |
| Value accrual | Governance only | Discounts / access | Fee share in native token | Fee share in external asset, or revenue-funded burn |
| Transparency (allocation, vesting, treasury wallets published) | None | Partial | Mostly | Full, on-chain verifiable |

Anything under 8 out of 18 deserves suspicion regardless of the story. Anything over 14 is rare.

## Worked example: Hyperliquid (HYPE), as of September 2026

Figures below are approximate and drawn from published analyses in late August 2026.

| Metric | Value |
|---|---|
| Price | ~$81–85 |
| Circulating supply | ~222 million |
| Total supply | ~955 million; max 1 billion |
| Market cap | ~$18 billion |
| FDV | ~$82 billion |
| MC/FDV | ~0.22 |
| Annualized protocol revenue | ~$570–730 million depending on methodology |
| Price / sales (on market cap) | ~25–32× |
| Value accrual | Assistance Fund buys HYPE with ~99% of fees, ~$700 million annualized pace (~3.9% of market cap per year) |
| Allocation | ~31% genesis airdrop to users, ~39% future emissions and community rewards, ~24% core contributors, ~6% foundation; no VC allocation |

Rubric: MC/FDV ~0.22 → 1. Insider share (contributors ~24%, no VCs) → 2. Twelve-month supply growth (contributor vesting plus emissions; monthly tranches around 1% of supply have been landing) → roughly 1–2. Concentration is hard to measure because much supply sits in the exchange's own contracts → call it 2 with a note. Value accrual → 3 (open-market buyback with real revenue). Transparency → 2. Total roughly 11–12 of 18: strong on accrual, weak on dilution.

The takeaway isn't "buy" or "sell." It's that the bull case rests on the buyback outrunning the unlock stream, and one analyst noted in August 2026 that trailing revenue had fallen from its February 2026 peak (around $866 million annualized) while the token traded roughly three times higher. Tokenomics tells you what to watch: monthly revenue versus monthly unlocked-and-sold supply.

## How to actually do it

1. Pull circulating, total, and max supply from the project docs and cross-check on CoinGecko. Compute MC/FDV.
2. Build a 24-month unlock table from Tokenomist and the docs: date, bucket, amount, percent of circulating on that date.
3. Add emissions (staking rewards, liquidity mining) to get total supply growth per quarter.
4. Open the explorer holders tab, label contracts, and compute top-10 and top-100 shares of circulating.
5. Identify the value accrual mechanism and quantify it: annual dollars to token holders ÷ market cap.
6. Score the rubric. Write one sentence on what would change the score.
7. Set calendar reminders for the next three cliff unlocks and check on-chain whether the recipients sold.

## Key takeaways

- Market cap is what you pay for the liquid slice; FDV is what you're implicitly paying for the whole thing. Low MC/FDV means the rest is coming.
- Unlock calendars are public. Ignoring them is choosing not to know when the seller shows up.
- A scheduled unlock is not a sale; check wallets afterward.
- Value accrual ranges from revenue-funded buybacks (strong) to governance-only (near zero). Most tokens sit near zero.
- Fee switches turned on don't guarantee price gains; UNI made new lows after its burn.
- Concentration among non-contract holders is the hidden variable in most altcoin price action.
- Score tokenomics before you read the narrative, because the narrative is designed to make you skip this step.

## Sources

- [Binance Research: Low Float & High FDV: How Did We Get Here? (May 2024)](https://public.bnbstatic.com/static/files/research/low-float-and-high-fdv-how-did-we-get-here.pdf)
- [Tokenomist: token unlock calendar and research](https://tokenomist.ai/research)
- [Tokenomist August 2026 unlock calendar (X post)](https://x.com/Tokenomist_ai/status/2086830620832100628)
- [Uniswap governance approves fee switch and 100M UNI burn (CoinMarketCap Academy)](https://coinmarketcap.com/academy/article/uniswap-governance-approves-fee-switch-and-100m-token-burn)
- [UNI after the fee switch: price hit a cycle low anyway (Bitget News)](https://www.bitget.com/news/detail/12560605397905)
- [HYPE: The $18 Billion Question (Investing.com, August 2026)](https://www.investing.com/analysis/hype-the-18-billion-question--can-hyperliquid-outgrow-its-valuation-200686830)
- [Why HYPE is different: inside Hyperliquid's buyback (crypto.news)](https://crypto.news/why-hype-is-different-inside-hyperliquids-buyback/)
- [DefiLlama: Protocol revenue rankings](https://defillama.com/revenue)
- [Messari Research](https://messari.io/research)
