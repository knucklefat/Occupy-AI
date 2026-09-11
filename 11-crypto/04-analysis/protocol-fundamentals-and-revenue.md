# Protocol Fundamentals and Revenue

**In one sentence:** Crypto protocols now publish real income statements on-chain, so you can analyze them like businesses, as long as you keep straight the difference between fees users pay, revenue the protocol keeps, and earnings that survive after the protocol pays for its own growth in tokens.

## The three lines that matter

Token Terminal, DefiLlama, and Artemis have converged on roughly the same vocabulary, though each has quirks. The core distinction:

| Line item | Definition | Analogy |
|---|---|---|
| **Fees** | Total amount users paid to use the protocol. Includes the part that goes to liquidity providers, lenders, validators, or sequencers. | Gross merchandise value, or a marketplace's gross bookings |
| **Revenue** | The share of fees the protocol itself (or its DAO / token holders) retains. Fees × take rate. | Net revenue |
| **Earnings** | Revenue minus what the protocol paid out in token incentives (liquidity mining, points converted to tokens, emissions to users). Some providers also subtract operating costs where known. | Operating profit, with stock-based compensation expensed |

Why the gap matters: a lending protocol might collect $100 million in interest (fees) but pass $90 million to lenders, keep $10 million (revenue), and spend $15 million in token emissions to attract those lenders, for earnings of negative $5 million. It looks huge on fees and is a money-losing business on earnings. DefiLlama separately reports **holders' revenue**, the part of revenue actually routed to token holders through burns, buybacks, or distributions, which is the number closest to a dividend.

**Take rate** is the fraction of fees the protocol keeps. Uniswap's take rate was zero until its fee switch activated in December 2025; Hyperliquid's is close to 100% because it runs its own order book rather than paying external liquidity providers; stablecoin issuers' take rate is effectively 100% of the interest on their reserves.

## Valuation multiples for tokens

Once you have revenue you can compute the same multiples used for stocks:

- **P/F (price to fees)** = market cap ÷ annualized fees. Useful for comparing protocols with different take rates, but flatters ones that keep nothing.
- **P/S (price to sales / revenue)** = market cap ÷ annualized revenue. The workhorse metric.
- **P/E (price to earnings)** = market cap ÷ annualized earnings. Often undefined because earnings are negative after incentives.
- **Fully diluted versions** of each: FDV ÷ revenue. Use these too; the gap between MC-based and FDV-based multiples is the dilution overhang (see `tokenomics-analysis.md`).

Two cautions specific to crypto. First, revenue is extremely cyclical: a DEX or perpetuals exchange can see revenue fall by 70% in a bear market without losing a single user, because volume falls. Annualizing a bull-market month produces absurdly low multiples. Use trailing twelve months where possible and look at the range. Second, revenue that accrues to a foundation or a company (Tether's and Circle's do) isn't available to token holders unless there's a mechanism. Tether has no token; Circle is a listed stock. Both appear atop DefiLlama's revenue rankings, which tells you the size of the stablecoin business, not anything about a token to buy.

## Users, and the ones who count

Active addresses are the crypto stand-in for active users, and they are easy to inflate: one person can control thousands of addresses, and airdrop farmers create them by the million. Better signals:

- **Fee-paying addresses** over a period, ideally weighted by fees paid.
- **Retention cohorts**: of addresses active in month N, how many are active in month N+3? Dune dashboards exist for most major protocols.
- **Transaction size distribution**: a protocol whose median transaction is $3 is being farmed, not used.
- **Volume per user**, and its trend.

Artemis, Token Terminal, and Dune are the best sources; Nansen labels help separate bots from humans.

## TVL and its limits

**Total value locked (TVL)** is the dollar value of assets deposited into a protocol's smart contracts. It was the first widely used DeFi metric and remains useful for lending and liquidity protocols, where deposits are the raw material of the business. Its problems:

1. **It's denominated in volatile assets.** TVL doubles when ETH doubles even if nobody deposits anything. DefiLlama lets you view TVL in ETH or BTC terms to strip this out.
2. **It's mercenary.** Capital chases incentives. A protocol paying 40% APY in its own token will have high TVL until the emissions stop.
3. **It double counts.** A deposit in a yield aggregator that deposits into a lending protocol that deposits into a staking protocol shows up in all three. DefiLlama separates "TVL" from "borrowed," "staking," "pool2," and "double-counted" categories for this reason.
4. **It measures inputs, not outputs.** A lending protocol with $10 billion TVL and 2% utilization earns less than one with $1 billion and 80% utilization.

Use TVL together with **utilization** (borrowed ÷ supplied for lending; volume ÷ TVL for DEXs, sometimes called capital efficiency). A DEX that turns its liquidity over daily is a better business than one that turns it over monthly, regardless of raw TVL.

## Comparing across categories

Different protocol types earn money differently, so compare like with like.

| Category | Fee source | Best primary metric | Key risk to fees |
|---|---|---|---|
| **L1 (Ethereum, Solana, Tron)** | Transaction fees, priority fees, MEV | Fees per day; fee-paying addresses; share burned vs paid to validators | Activity migrating to L2s or competing chains; fee compression as blockspace expands |
| **L2 (Base, Arbitrum, Optimism)** | Sequencer fees minus L1 data costs | Net sequencer revenue (the margin); transactions; app diversity | L1 data cost changes; centralized sequencer revenue may go to the company, not the token |
| **DEX / perps** | Trading fees | Volume; take rate; volume/TVL | Volume is cyclical; fee wars |
| **Lending** | Interest spread | Borrow volume; utilization; bad debt | Liquidation cascades; oracle failure |
| **Stablecoin issuer** | Yield on reserves | Supply; reserve yield; share of yield passed to holders | Rate cuts; regulation of yield-bearing coins |
| **Oracle / infrastructure (Chainlink)** | Service fees from protocols | Fees; number of integrations; secured value | Clients build in-house; commoditization |
| **Launchpads / memecoin infrastructure (Pump)** | Trading and creation fees | Fees; daily launches | Entirely narrative-dependent volume |

For L1s, a useful extra step is separating **security spend** (issuance to validators) from **fee revenue**. Ethereum's post-merge design burns a base fee and pays priority fees to validators; when burn exceeds issuance the network is net deflationary, which is the closest thing an L1 has to a buyback.

## Leading protocols by revenue, as of September 2026

Trailing 30-day protocol revenue per DefiLlama, rounded, with annualized figures multiplied by 12 for rough comparison. Fees and revenue differ; these are the retained figures.

| Protocol | Category | 30-day revenue | Rough annualized | Note |
|---|---|---|---|---|
| Tether | Stablecoin issuer | ~$480m | ~$5.8b | No token; revenue to the company |
| Circle | Stablecoin issuer | ~$194m | ~$2.3b | Listed equity, not a token |
| Hyperliquid | Perpetuals / L1 | ~$60m | ~$720m | ~99% of fees buy HYPE |
| Pump | Launchpad | ~$57m | ~$680m | Memecoin volume dependent |
| Canton | Chain | ~$50m | ~$600m | Institutional network |
| GMGN | Trading bot | ~$39m | ~$470m | |
| Robinhood Chain | L2 | ~$32m | ~$380m | Revenue to Robinhood |
| Tron | L1 | ~$24m | ~$290m | Stablecoin transfer chain |
| fomo | Trading app | ~$24m | ~$290m | |
| Axiom Pro | Trading app | ~$24m | ~$290m | |
| Grayscale | Asset manager | ~$17m | ~$200m | Fund fees |
| Uniswap | DEX | ~$13m | ~$160m | Post-fee-switch; UNI burns |
| Chainlink | Oracle | ~$6m | ~$66m | |

Three observations. Stablecoin issuance is by far the largest business in crypto, and neither leader has a token. Much of the rest of the top of the table in 2026 is trading infrastructure for speculation (perps, memecoin launchpads, trading bots), which means the revenue is highly cyclical. And the protocols with the loudest "fundamentals" narratives in prior years, general-purpose L1s and DEXs, sit well down the list.

## Worked example: valuing a perpetuals exchange

Suppose a perps DEX has a market cap of $18 billion, FDV of $82 billion, trailing-30-day revenue of $60 million, and routes 99% of revenue to buybacks.

- Annualized revenue ≈ $720 million.
- P/S on market cap ≈ 25×; on FDV ≈ 114×.
- Buyback yield ≈ $713m ÷ $18b ≈ 4% of market cap per year.
- Now stress it: in the last bear market, perps volume fell about 70%. Revenue at $216 million puts P/S at 83× on market cap and buyback yield at 1.2%, while unlocks continue on schedule.

The question the multiple poses is whether volume growth can outrun both the cyclical drawdown and dilution. That's a judgment, but it's now a judgment about two numbers rather than a vibe.

## How to actually do it

1. Open the protocol on Token Terminal or DefiLlama and record trailing 30-day and 12-month fees, revenue, and (where available) earnings and holders' revenue.
2. Compute P/S on both market cap and FDV. Note the gap.
3. Pull the same numbers for three direct competitors. Rank on P/S, revenue growth, and take rate.
4. Check TVL in native-asset terms and compute utilization or volume/TVL.
5. Look at fee-paying users and a retention cohort on Dune or Artemis.
6. Find the mechanism, if any, by which revenue reaches the token. If none, treat revenue as an interesting fact, not a valuation input.
7. Stress the revenue line with the last cycle's drawdown and re-run the multiple.

## Key takeaways

- Fees are what users pay; revenue is what the protocol keeps; earnings subtract token incentives. Use the right one.
- P/S on FDV, not just market cap, exposes the dilution overhang.
- Crypto revenue is violently cyclical; never annualize a peak month.
- TVL measures inputs, double counts, and inflates with prices. Pair it with utilization.
- As of September 2026, stablecoin issuers dominate revenue and have no token; much of the rest is speculative trading infrastructure.
- Revenue only matters to a token holder if a mechanism routes it to the token.
- Active addresses are trivially inflated; use fee-paying and retained users.

## Sources

- [Token Terminal: Revenue metric definition](https://tokenterminal.com/explorer/metrics/revenue)
- [Token Terminal: Earnings metric definition](https://tokenterminal.com/explorer/metrics/earnings)
- [DefiLlama: Protocol revenue rankings](https://defillama.com/revenue)
- [DefiLlama: Holders revenue rankings](https://defillama.com/holders-revenue)
- [DefiLlama: Protocol TVL rankings and methodology categories](https://defillama.com/protocols)
- [Artemis: on-chain fundamentals](https://www.artemis.xyz/)
- [Dune Analytics](https://dune.com/)
- [HYPE: The $18 Billion Question (Investing.com, August 2026)](https://www.investing.com/analysis/hype-the-18-billion-question--can-hyperliquid-outgrow-its-valuation-200686830)
- [Outlier Ventures: The Quantitative Components of Token Value](https://outlierventures.io/article/token-value-quantitative-components/)
