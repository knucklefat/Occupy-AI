# DeFi Yield Farming and Liquidity Provision

**In one sentence:** Providing liquidity and "farming" yield in decentralized finance can produce real income from trading fees and lending, but the advertised percentages are usually dominated by token printing, the math of impermanent loss is unforgiving, and the 2020–2022 record shows most participants would have done better simply holding the underlying coins.

## The vocabulary

- **DeFi (decentralized finance):** lending, trading and derivatives run by smart contracts on public blockchains instead of by companies. You interact from your own wallet; no one can freeze your account, and no one can reverse your mistakes.
- **Liquidity provision (LPing):** depositing two tokens (say ETH and USDC) into an automated market maker (AMM) like Uniswap so traders can swap between them. You earn a share of the trading fees (typically 0.05–1% per trade) proportional to your share of the pool.
- **Yield farming:** doing the above — or lending, or staking an LP position — specifically to collect extra rewards a protocol pays in its own token to attract deposits. The practice took off in June 2020 when Compound began distributing COMP tokens to users.
- **TVL (total value locked):** the dollar value of assets deposited in a protocol; the industry's headline metric. DeFi TVL peaked around $177B in late 2021, collapsed below $40B in 2022, recovered to roughly $170B in October 2025, fell to about $68–72B in mid-2026, and sat near $86–88B as of September 2026 (DefiLlama).
- **Real yield:** income paid from actual protocol revenue (fees, interest) rather than from newly minted tokens.

## Where yield actually comes from

Every DeFi yield decomposes into at most four sources:

1. **Trading fees** paid by swappers. Real, but only large in pools with heavy volume relative to their size.
2. **Interest** paid by borrowers on Aave, Compound, Morpho and similar. Real, cyclical — borrowing demand (and rates) spikes when speculators want leverage in bull markets and evaporates in bear markets.
3. **Token emissions** — the protocol prints its governance token and hands it to depositors. This is where triple-digit APYs come from. The token's value depends entirely on someone else wanting it later, and recipients are usually selling it as fast as they receive it.
4. **Points and expected airdrops** — the 2023–26 variant of emissions, where the reward is a promise of future tokens (see the airdrops file).

The line to remember: **if you cannot tell where the yield comes from, you are the yield** — your deposit is the exit liquidity for whoever got in earlier or for the team's token allocation.

## Impermanent loss: a worked example

An AMM keeps a pool balanced by formula (Uniswap v2 holds x × y = constant). When one token's price moves, arbitrageurs rebalance the pool against you: it ends up holding less of the coin that went up and more of the one that went down. The gap between your pool value and what you would have had by simply holding is "impermanent loss" (IL) — impermanent only in the sense that it disappears if the price returns to where it started.

Suppose you deposit **1 ETH + 2,000 USDC** when ETH is $2,000 (total $4,000). ETH then doubles to $4,000.

- The pool constant is 1 × 2,000 = 2,000. At the new price the pool holds √(2,000 ÷ 4,000) ≈ **0.707 ETH** and √(2,000 × 4,000) ≈ **2,828 USDC**.
- Your position is worth 0.707 × $4,000 + $2,828 = **$5,657**.
- Had you held: 1 ETH ($4,000) + $2,000 = **$6,000**.
- Impermanent loss: $343, or **5.7%** of the hold value.

You still made money ($4,000 → $5,657), but you earned less than doing nothing, and you needed at least $343 in fees over the period just to break even against holding. The loss is symmetrical — a halving of ETH costs the same 5.7% — and it grows fast:

| Price change of one token vs. the other | Impermanent loss vs. holding |
|---|---|
| ±25% | 0.6% |
| ±50% | 2.0% |
| 2x or ½ | 5.7% |
| 3x | 13.4% |
| 4x | 20.0% |
| 5x | 25.5% |

Two implications. First, LPing is a bet that the two assets stay *close* to their starting ratio; stablecoin-to-stablecoin pools and ETH/stETH pools have little IL, while ETH/random-token pools have a lot. Second, in a rally your LP position systematically sells the winner, which is why LPs underperform in bull markets, and in a crash you end up holding the bag of the loser.

**Uniswap v3 and "concentrated liquidity"** let you supply liquidity only within a price range, which multiplies both fee income and impermanent loss; if the price leaves your range you earn nothing and are 100% in the losing asset. A widely cited 2021 study by Topaze Blue and Bancor found that roughly half of Uniswap v3 LPs earned less than they would have by holding, and that the gap was worst for casual, short-term positions.

## The graveyard of 2020–2022

The yield-farming era's body count is the best evidence for reading the "where does the yield come from" question literally:

- **Anchor Protocol / Terra (May 2022):** paid a "stable" 19.5% on UST, subsidized by the Luna Foundation's reserves. When the subsidy ran out and confidence broke, UST and LUNA went to zero; roughly $40B evaporated in a week.
- **Iron Finance / TITAN (June 2021):** a partially collateralized stablecoin farm collapsed from $60+ to zero in hours — the first large "bank run" on a DeFi protocol.
- **OlympusDAO (OHM) and its forks (Wonderland, KlimaDAO):** advertised staking APYs in the thousands of percent, all from emissions; OHM fell over 95% from its 2021 high.
- **Celsius, BlockFi, Voyager (2022):** centralized lenders that took retail deposits at 8–18%, lent them into DeFi and to hedge funds like Three Arrows, and went bankrupt when the loans went bad.
- **Harvest Finance, Cream, BadgerDAO, Wormhole, Ronin, Mango (2020–22):** flash-loan and bridge exploits costing $50M–$600M each; Chainalysis counted $3.1B stolen from DeFi in 2022 alone.
- **Countless "food coin" forks** (SushiSwap's early clones, Yam, Hotdog, Kimchi) that paid 1,000%+ for days and then had no users.

The survivors — Uniswap, Aave, Maker/Sky, Curve, Lido, and newer real-yield protocols like GMX and Hyperliquid — share a trait: their revenue comes from fees or interest that users actually pay.

## Evaluating a yield in five questions

1. **What pays it?** Fees, interest, emissions, or points? Find the number on DefiLlama's "Yields" page, which splits base APY from reward APY. If reward APY is most of it, the true yield is whatever you can sell those tokens for today.
2. **Volume-to-TVL ratio.** A pool with $10M TVL and $1M daily volume at 0.3% fees earns 0.3% × $1M = $3,000 a day ≈ 11% a year for LPs. The same pool with $100K daily volume earns 1.1%. Fee yield is arithmetic, not marketing.
3. **How correlated are the two assets?** Stable/stable or ETH/LST: low IL. Anything/new token: high IL plus the token's own collapse risk.
4. **Contract and protocol risk.** Age, audits, bug-bounty size, whether the code is a fork of something proven, whether the admin keys can drain the pool ("rug" risk). Newer than six months and unaudited means assume total loss is possible.
5. **What is your all-in cost?** Gas to enter and exit (trivial on Solana or Ethereum layer-2s, meaningful on Ethereum mainnet), swap fees to assemble the pair, and the tax overhead of tracking dozens of reward events.

A yield that survives these questions and still beats plain staking or T-bills by a few points is a reasonable trade for someone who already holds the assets. A yield that only looks good on question one is a trap.

## Points and airdrop farming as yield

Since 2023, many protocols stopped paying emissions up front and instead award "points" that are expected to convert into a token later. This has the same economics as emissions with worse transparency: you cannot value the reward until the airdrop, allocation rules change retroactively, and a share of your capital is stuck for months. The airdrops file covers this in detail.

## How to actually do it

1. **Do not start here.** Own the underlying assets, understand wallets and gas, and have a clear reason (income on coins you hold anyway) before providing liquidity.
2. **Use a separate wallet with only the funds you are deploying**, so an approval or contract exploit cannot reach your main holdings.
3. **Start with low-IL, high-volume, blue-chip pools:** stablecoin pools on Curve or Uniswap, ETH/stETH, or lending USDC on Aave. Expect 3–8%, not 30%.
4. **Check DefiLlama Yields for base vs. reward APY and volume/TVL** before every deposit; recheck monthly.
5. **Size it as speculative capital.** Even blue-chip DeFi has been hacked; treat the position as money you could lose.
6. **Track everything.** Each fee claim, reward token and LP token swap is a taxable event in the U.S.; use a wallet-tracking tax tool from day one.
7. **Have an exit rule.** Withdraw if the protocol changes admin keys, suffers a partial exploit, or if reward APY falls and the base yield no longer beats plain staking.
8. **Revoke token approvals** you are no longer using (revoke.cash or similar) — stale approvals are a common wallet-drain vector.

## Key takeaways

- All DeFi yield comes from fees, interest, token emissions, or points; only the first two are real, and the "real yield" share is usually a fraction of the advertised number.
- Impermanent loss is arithmetic: a 2x move in one asset costs 5.7% vs. holding, a 5x costs 25.5%; you need fees to exceed that just to tie.
- Concentrated-liquidity positions magnify both fees and losses; about half of Uniswap v3 LPs in the 2021 study underperformed holding.
- The 2020–22 graveyard (Anchor/Terra, Iron Finance, Olympus forks, Celsius, dozens of exploits worth $3B+ in 2022) is what happens when depositors do not ask where the yield comes from.
- Low-risk DeFi yield is 3–8% on stablecoins or correlated pairs; anything far above that is emissions, leverage, or a bug you have not found yet.
- Fee yield = fee rate × volume ÷ TVL. Compute it; do not trust the banner.
- Use an isolated wallet, size for total loss, and keep tax records from the first transaction.

## Sources

- [Uniswap docs: Understanding returns (impermanent loss table and formula)](https://docs.uniswap.org/contracts/v2/concepts/advanced-topics/understanding-returns)
- [Speedrun Ethereum: Impermanent loss explained — the math](https://speedrunethereum.com/guides/impermanent-loss-math-explained)
- [Auditless: Impermanent loss in Uniswap v3](https://medium.com/auditless/impermanent-loss-in-uniswap-v3-6c7161d3b445)
- [Topaze Blue / Bancor: Impermanent loss in Uniswap v3 (2021 study, PDF)](https://arxiv.org/abs/2111.09192)
- [DefiLlama: Yields dashboard (base vs reward APY)](https://defillama.com/yields)
- [Coinlaw: Where stablecoin yield actually comes from](https://coinlaw.io/stablecoin-yields/)
- [Chainalysis: 2025 crypto theft reaches $3.4 billion](https://www.chainalysis.com/blog/crypto-hacking-stolen-funds-2026/)
- [Chainalysis: 2025 crypto crime mid-year update](https://www.chainalysis.com/blog/2025-crypto-crime-mid-year-update/)
- [Eco: Ethena USDe and sUSDe 2026 — delta-neutral yield](https://eco.com/support/en/articles/15254002-ethena-usde-and-susde-2026-delta-neutral-yield)
- [BloFin Academy: Impermanent loss — the risk most LPs don't price in](https://blofin.com/en/academy/education/impermanent-loss)
