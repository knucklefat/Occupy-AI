# Altcoins and Tokenomics

**In one sentence:** Every crypto asset other than bitcoin is an "altcoin," and whether one is worth anything depends on its tokenomics (how many tokens exist, how fast new ones are released, who got them cheaply, and whether the token has any claim on the project's success), which is why most of the tokens that ever reached the top 100 are now dead and why buying a freshly listed "low float, high FDV" token is usually a way to become someone else's exit liquidity.

## Token categories

"Altcoin" covers wildly different things. A rough taxonomy:

| Category | What the token does | Examples | How it might earn value |
|---|---|---|---|
| **Layer 1 (L1)** | Native coin of a base blockchain; pays fees, secures the chain via staking | ETH, SOL, BNB, AVAX, SUI, TRX | Fee burn, staking demand, collateral use |
| **Layer 2 (L2)** | Governance or fee token of a rollup on Ethereum | ARB, OP, STRK, ZK | Mostly governance; fee capture is rare so far |
| **DeFi** | Governance of a protocol; sometimes fee share | UNI, AAVE, LDO, MKR/SKY, HYPE | Buybacks, fee switches, staking discounts |
| **Utility** | Pays for a specific service | LINK (oracles), FIL (storage), RENDER (GPU) | Demand for the service |
| **Governance** | Votes on protocol parameters and treasury | Many DeFi tokens | Weak unless votes control cash |
| **Memecoin** | Nothing; pure attention and community | DOGE, SHIB, PEPE, WIF, TRUMP | None; price is a popularity contest |
| **RWA (real-world assets)** | Represents or governs tokenized Treasuries, credit, real estate | ONDO, tokenized funds like BUIDL | Fees on tokenized assets |
| **AI tokens** | Tokens attached to AI compute, agents, or data projects | TAO, FET, RENDER, VIRTUAL | Mostly narrative; some compute demand |
| **Exchange tokens** | Fee discounts and buybacks at a centralized exchange | BNB, OKB, CRO | Buybacks from exchange profits |

The critical question for any token: **does owning it entitle you to anything?** A share of stock is a claim on profits and assets. Most tokens are not. They are, at best, a claim on future governance votes, and the project's revenue may flow to a company or foundation rather than to token holders. Regulatory fear (the SEC's position through 2024 that revenue-sharing tokens are securities) is why so many tokens were designed to be "valueless governance tokens." That stance loosened in 2025–26, and more protocols have turned on fee sharing or buybacks; Hyperliquid's HYPE, which routes about 99% of trading fees into buying and burning the token, is the model now being copied.

## Supply schedules: the three numbers you must know

1. **Circulating supply**: tokens actually tradable today.
2. **Total / max supply**: the ceiling (bitcoin: 21 million) or, for many tokens, "uncapped" with an inflation rate.
3. **Emission or inflation rate**: how fast new tokens are created and to whom (stakers, miners, treasury, team, investors).

**Market cap** = price × circulating supply. **Fully diluted valuation (FDV)** = price × total supply. When a token has 10% of its supply circulating and FDV is $10 billion, its market cap is $1 billion, and $9 billion of tokens are waiting to be released onto the market.

## Vesting, cliffs, and unlocks

Tokens allocated to founders, employees, and venture investors are typically locked and then released ("vested") over time. A common structure: a **cliff** of 12 months during which nothing unlocks, then linear monthly unlocks over the next 24–36 months. **Token unlock calendars** (TokenUnlocks, CryptoRank, DefiLlama) publish these schedules.

Unlocks matter because they are scheduled supply shocks. A 2024 study by market maker Keyrock of more than 16,000 unlock events found that roughly **90% created negative price pressure**, that prices tend to weaken from about **30 days before** the unlock as traders front-run it, and that **team unlocks were the most damaging** (average declines around 25%) because insiders sell without coordination. Investor unlocks were less harmful because VCs often hedge or sell over-the-counter in advance. Ecosystem-fund unlocks were roughly neutral.

## Why "low float, high FDV" hurts buyers

The 2023–24 launch cycle produced a wave of tokens that listed with a tiny share of supply circulating (Binance Research found the average float at listing was about 13% for 2024 launches) at fully diluted valuations of $5–20 billion. The mechanics work against the public buyer:

1. Venture funds bought in private rounds at valuations often 10–100x below the listing FDV.
2. A small float plus airdrop hype creates a high initial price with little real supply to absorb it.
3. Over the next 2–4 years, unlocks release 5–10x the initial float. Even if the project succeeds, the price must rise enough to absorb that supply just to stay flat.
4. Retail buyers at listing therefore underwrite insiders' exit; most 2024 low-float launches traded 60–90% below listing price within a year.

The reaction was a swing toward memecoins ("at least the float is 100% and nobody has a cheaper cost basis than me"), which then produced its own carnage. The lesson is not "avoid all new tokens," it is: **always look at FDV, not market cap; check the unlock schedule; and assume that a 13% float means the true valuation is the FDV and the sellers are already lined up.** Some newer launches ("fair launch," high-float, or auction-priced) have tried to fix this.

## How value accrues (or doesn't)

Mechanisms that actually route economic value to a token:

- **Fee burn**: fees destroy tokens, reducing supply for all holders (ETH base fee, BNB quarterly burns).
- **Buyback and burn / buyback and distribute**: protocol revenue buys tokens on the open market (HYPE, MKR/SKY, some DEXs).
- **Staking with real yield**: fees, not inflation, are paid to stakers (see [DeFi Explained](defi-explained.md)).
- **Required use**: you must hold or spend the token to use the service (gas on an L1; LINK for oracle payments).
- **Fee switch**: governance turns on a share of protocol revenue for token holders (Uniswap debated this for years before moving forward in 2025).

Mechanisms that sound like value but usually are not:

- **Governance alone**: voting rights without control of cash flows.
- **Inflationary staking rewards**: a 20% "yield" paid in newly printed tokens is dilution, not income.
- **"Utility" that could be replaced by a stablecoin**: if users would rather pay in USDC, the token is a friction, not a moat.
- **Treasury size**: a foundation holding $1 billion of its own token has $1 billion only if it can sell without crashing the price, which it cannot.

## Survivorship: the base rate is brutal

Data compiled by CryptoRank (2026) on the 1,539 tokens that have ever been in CoinMarketCap's top 100:

- **71.9% are operationally dead** (delisted by major exchanges and under $10,000 daily volume for 90+ days).
- The **median top-100 token survives 2 years and 4 months**.
- About **62% die within five years**; roughly 85% within ten.

Cohort views:

- **December 2017 top 100:** by early 2021, only 21 had made a new all-time high, about 68 remained below their 2017 peak, and 27 showed no signs of activity at all (analysis by @0xdavanai). Only three (BNB, LINK, DOGE) had improved their rank.
- **July 2021 top 100:** five years later, 41 were still in the top 100, 46 had fallen out, and 13 had ceased operations. Tokens that dropped out lost a median of 93% of their value, and about 65% of the dropouts were "Ethereum killer" L1s and L2s.
- **Memecoins:** of 18.67 million tokens launched on Solana's pump.fun between January 2024 and June 2026, about 69% had their last trade the same day they were created, only about 4.5% survived 90 days, and roughly 1% "graduated" to a real exchange listing.

The implication is that an equal-weighted basket of altcoins is a strategy for losing money, even in a bull market. Bitcoin and, to a lesser extent, Ethereum have remained in the top two since 2015; almost nothing else has held its rank across two cycles.

## A tokenomics checklist

Before buying any altcoin, answer these:

1. What is the FDV, and what share is circulating?
2. Who holds the non-circulating supply, at what cost basis, and when does it unlock?
3. Is issuance inflationary? If so, what is the annual rate, and who receives it?
4. Does the token have any claim on revenue, or is it governance only?
5. What does the project earn today (DefiLlama "fees" and "revenue" pages), and what multiple of that is the FDV?
6. Could the product work just as well with no token at all? If yes, why does the token exist?
7. What is the base rate of survival for this category?

## Key takeaways

- "Altcoin" spans L1 coins with real fee economics to memecoins with none; the category tells you how, if at all, the token might capture value.
- Always value tokens on FDV, not market cap. A 13% float means 87% of the supply is coming to market.
- Unlocks are scheduled supply shocks: about 90% are followed by price weakness, starting a month early, and team unlocks are the worst.
- Value accrues through burns, buybacks, real-yield staking, and required use; governance alone and inflationary "yield" usually do not.
- Roughly 72% of tokens that ever reached the top 100 are dead; the median survives just over two years; most memecoins die the day they launch.
- Insiders (VCs, teams) buy at private valuations far below listing prices; the public buyer at listing is typically the exit liquidity.
- If you must own altcoins, own few, know their revenue and unlock schedules, and size them as venture bets that will mostly go to zero.

## Sources

- [BeInCrypto: Nearly 3 in 4 tokens that ever cracked the top 100 are operationally dead (CryptoRank)](https://beincrypto.com/top-100-crypto-tokens-dead/)
- [U.Today: Top 100 cryptos of 2017: 27 scams, 79 will never update ATH](https://u.today/top-100-cryptos-of-2017-27-scams-79-will-never-update-ath-analyst-says)
- [CoinGecko Research: The average lifespan of pump.fun memecoins is less than a day](https://www.coingecko.com/research/publications/average-lifespan-of-pumpfun-tokens)
- [Keyrock: From Locked to Liquidity, what 16,000+ token unlocks teach us](https://keyrock.com/from-locked-to-liquidity-what-16000-token-unlocks-teach-us/)
- [StoneX: High FDV and Low Float Criticism (citing Binance Research)](https://www.stonex.com/en/insights/stonex-digital-asset-weekly-commentary---high-fdv-and-low-float-criticism-1499185/)
- [Binance Research: Low Float and High FDV, How Did We Get Here?](https://www.binance.com/en/research/analysis/low-float-and-high-fdv-how-did-we-get-here)
- [Gate Learn: Time-scheduled token unlocks, the low float high FDV problem](https://www.gate.com/learn/articles/time-scheduled-token-unlocks-an-elephant-in-the-room/4895)
- [a16z crypto: Token design guidance](https://a16zcrypto.com/posts/article/token-design-mental-frameworks-and-tools/)
- [DefiLlama: Fees and revenue by protocol](https://defillama.com/fees)
- [Motley Fool: Hyperliquid has now generated $1 billion in revenue (buyback mechanism)](https://www.fool.com/investing/2026/07/09/hyperliquid-has-now-generated-1-billion-in-revenue/)
- [CoinMarketCap: Evolution of top-10 coins in CMC's history (2013–2023)](https://coinmarketcap.com/academy/article/evolution-of-top-10-coins-in-cmcs-history)
