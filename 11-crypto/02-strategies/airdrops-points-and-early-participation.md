# Airdrops, Points, and Early Participation

**In one sentence:** Protocols give away tokens to early users to bootstrap ownership and reward loyalty, and a handful of these giveaways have been worth thousands or tens of thousands of dollars per wallet — but the odds have worsened sharply since 2024, the tokens usually fall after launch, the effort and risks are real, and for a normal person it is a hobby with a lottery ticket attached, not a strategy.

## How airdrops work

An **airdrop** is a free distribution of a new token to wallets that meet some criteria — usually having used the protocol before a snapshot date. The economic logic: a decentralized protocol needs its governance token in the hands of real users (for regulatory, community and network-effect reasons), and giving it to the people who showed up early is cheaper marketing than paying for it. The team and investors keep the majority; a "community" allocation of 5–30% goes to users.

The process has evolved through three eras:

1. **Surprise drops (2020–22).** Uniswap dropped 400 UNI on every past user in September 2020 with no warning — about $1,200 at launch and roughly $17,000 at UNI's 2021 peak — to about 250,000 addresses. This created the expectation that using new protocols might pay.
2. **Expected drops with hidden criteria (2022–23).** Arbitrum (March 2023) distributed about 1.16 billion ARB to some 625,000 wallets, scoring them on transaction count, volume, duration and bridging; a typical recipient got 1,000–2,000 ARB, worth roughly $1,500–2,500 at launch. Users began "farming" — performing activity purely to qualify.
3. **Points programs (2023–present).** Protocols now publish a points ledger (Blur, EigenLayer, Ethena, Blast, Hyperliquid and hundreds since) that tracks user activity explicitly and converts to tokens at an announced or unannounced date. Points make farming legible and turn a surprise gift into a quasi-contractual, unpriced liability.

## The big ones, and what they were worth

| Airdrop | Date | Share of supply | Recipients | Value at launch | What happened next |
|---|---|---|---|---|---|
| Uniswap (UNI) | Sep 2020 | 15% to community; 400 UNI per user | ~250,000 | ~$1,200 per wallet | Peaked ~14x higher in 2021; still well above launch |
| Arbitrum (ARB) | Mar 2023 | ~11.6% | ~625,000 | ~$1,500–2,500 typical | Fell ~70–80% over the following two years |
| Jupiter (JUP) | Jan 2024 | 10% in first round | ~955,000 | ~$100–700 for most; more for heavy users | Roughly flat to down since |
| Hyperliquid (HYPE) | Nov 2024 | 31% | ~94,000 | ~$1.2B total; average ~$45,000 per wallet | Rose 5–10x through 2025 — the outlier |

Hyperliquid's drop is the one everyone points to, and it is the exception that explains the rule. The protocol had no venture investors, so 76% of supply went to the community; its users were high-volume perpetual-futures traders who had put real capital at risk for a year; and the token had an actual revenue stream (trading fees used for buybacks). Almost every other major 2024–26 launch — including ZKsync, LayerZero, Starknet, Scroll, Linea, EigenLayer, Blast, and most Solana and Base tokens — followed the "low float, high fully diluted valuation" pattern: a small fraction of supply trades at launch, insiders hold most of it under vesting, and the price declines 50–90% over the following year as unlocks arrive. Recipients who sold on day one did fine; recipients who held mostly did not.

## The points meta, and Sybil filtering

A **Sybil** is one person pretending to be many — spinning up hundreds or thousands of wallets to multiply an airdrop. Industrial farmers run scripted wallets across every new chain, and their share of activity on pre-token protocols is often the majority of "users." Protocols fight back with:

- **Clustering analysis** — wallets funded from the same source, acting at the same times, with identical patterns get grouped and cut (Arbitrum, Optimism, Hop pioneered this).
- **Self-report bounties** — LayerZero (2024) offered Sybils a reduced allocation for confessing and paid bounty hunters to expose others; about 800,000 addresses were flagged.
- **Volume and duration thresholds** that favor large, long-term users over many small ones — which also cuts out honest small users.
- **Proof-of-personhood** (Gitcoin Passport, World ID) requirements.
- **Retroactive rule changes.** Criteria are announced after the snapshot, so a farmer never knows whether their activity counted. Angry "I got zero" threads follow every launch.

The effect: rewards have concentrated toward wallets that deployed *real* capital for a *long* time. A person with $500 who bridges to a new chain and makes ten swaps is usually filtered out as low-value or Sybil-like; a person who kept $50,000 in a protocol's lending pool for a year is not. Points programs formalize this: points typically scale with dollars deposited times days deposited, which means the "free" airdrop is really a return on capital you locked up, paid in an illiquid, uncertain token.

## Realistic expected value for a normal person

Be arithmetic about it. As of September 2026, a serious farming effort might mean:
- Capital tied up: $5,000–20,000 across several protocols for 6–12 months (earning nothing, or a low points-augmented yield, and exposed to smart-contract risk).
- Gas and bridge fees: $100–1,000 over the year on Ethereum mainnet, far less on layer-2s and Solana.
- Time: several hours a week tracking programs, doing tasks, managing wallets.
- Outcome distribution: most protocols never launch a token or launch one worth little; some pay $100–500 per wallet; a few pay $1,000–5,000; a Hyperliquid happens once every few years and mostly to people who were already heavy traders.

Community estimates and post-mortems of the 2024 airdrop season suggested typical returns of low hundreds of dollars per protocol for retail-scale wallets, often below the opportunity cost of the capital — with a long right tail that keeps the game going. Professional farming operations with hundreds of wallets and six-figure capital can make it a business; a person doing it on evenings mostly earns a hobby wage.

The honest framing: **if you already use a protocol for its own sake — trading on it, lending on it, holding its liquid staking token — an airdrop is a pleasant bonus.** Reorganizing your money around qualifying for hypothetical tokens is speculation with poor transparency about the payoff.

## Tax treatment

In the U.S., IRS Revenue Ruling 2019-24 treats an airdrop as **ordinary income at fair market value when you gain control of the tokens** — when you can transfer or sell them, which for a claimable airdrop is the moment you claim. That value becomes your cost basis; a later sale is a capital gain or loss. Consequences: an airdrop worth $5,000 at claim that you hold while it falls 80% leaves you with $5,000 of taxable income and a $4,000 capital loss (subject to the $3,000 annual net-loss limit against ordinary income). Many recipients learned this the hard way in 2021–22. Practical rule: sell enough on receipt to cover the tax, or sell it all. Points themselves are not taxed until they convert to something you control. Other countries vary — some tax only on disposal, some treat airdrops as capital receipts with zero basis.

## The risks nobody mentions in the Discord

- **Wallet drains.** Fake "claim your airdrop" sites are the most common phishing lure in crypto. Signing a malicious approval or transaction can empty the wallet; Chainalysis counted 80,000 personal-wallet theft victims and $713M lost in 2025. Never claim from a link in a DM, a reply, or a sponsored search result; go through the protocol's official domain, verified from its documentation or its GitHub.
- **Smart-contract risk on the farm itself.** Capital deposited to earn points sits in new, lightly audited contracts by definition.
- **Wasted gas and dead protocols.** Many protocols you farm will fold, pivot, or "launch" a token at a valuation where your allocation is worth less than the gas you spent.
- **Locked capital in a crash.** Points programs encourage keeping funds deposited through market drops; the points do not offset a 60% decline in the asset.
- **Regulatory exposure.** A token distributed in an airdrop may be deemed a security in some jurisdictions; several projects have excluded U.S. or other users at claim time.
- **Opportunity cost.** Money farming for a maybe-token is not earning a known 3–7% staking yield or sitting in the bitcoin allocation that has been the actual source of most crypto returns.

## How to actually do it

1. **Use a dedicated "farming" wallet** funded with only what you would deploy, isolated from your main holdings and from any hardware-wallet seed.
2. **Prefer protocols you would use anyway** — a lending market you like, a DEX with good execution, a liquid staking token — so the activity has standalone value.
3. **Verify every claim site** through the protocol's official docs or Twitter/X account with a long history, never through search ads or messages. Bookmark the real domain.
4. **Read the criteria published by comparable past airdrops** (transaction count over months, volume, distinct days active, bridging) and behave like a real user across time rather than doing 50 transactions in one afternoon.
5. **Track the tax basis** of every token received; on claim day, decide deliberately whether to sell, hold, or sell part to cover the tax bill.
6. **Revoke approvals** after finishing with a protocol (revoke.cash or a wallet's built-in tool) and periodically audit the wallet for stale permissions.
7. **Cap the whole activity** — capital, hours and expectations — and reassess after a year against what the same money would have earned in plain staking or a bitcoin ETF.

## Key takeaways

- Airdrops are marketing spend paid in equity-like tokens; historically a few (Uniswap 2020, Hyperliquid 2024) paid thousands to tens of thousands per wallet, and most since 2024 paid hundreds and then declined 50–90%.
- Hyperliquid's ~$45,000 average was an outlier built on no venture capital, real revenue and users who had traded seriously for a year — it is not the base case.
- Points programs and Sybil filtering have shifted rewards to large, long-term capital; a small wallet doing quick tasks is usually filtered out.
- Expected value for a casual participant in 2025–26 is roughly a hobby wage with a lottery tail, and often below the return on the same capital in staking.
- In the U.S., an airdrop is ordinary income at claim-day value; the tokens usually fall afterward, so sell enough to cover the tax.
- "Claim your airdrop" phishing is the leading wallet-drain vector; isolated wallets and verified domains are non-negotiable.
- Participate in protocols you would use anyway and treat any drop as a bonus, not a plan.

## Sources

- [CoinGecko: What is Hyperliquid and what the Hyperliquid airdrop means for DeFi](https://www.coingecko.com/learn/what-is-hyperliquid-and-what-the-hyperliquid-airdrop-means-for-defi)
- [Cointelegraph via TradingView: Hyperliquid's HYPE surges after billion-dollar airdrop](https://www.tradingview.com/news/cointelegraph:a39ed2d74094b:0-hyperliquid-s-hype-token-surges-60-after-billion-dollar-airdrop/)
- [Uniswap blog: Introducing UNI (Sept 2020)](https://blog.uniswap.org/uni)
- [Arbitrum Foundation: ARB airdrop eligibility and distribution](https://docs.arbitrum.foundation/airdrop-eligibility-distribution)
- [Jupiter: Jupuary airdrop announcement](https://station.jup.ag/blog/jupuary)
- [LayerZero: Sybil self-report and Proof-of-Donkey (2024)](https://medium.com/layerzero-foundation)
- [IRS Revenue Ruling 2019-24 on hard forks and airdrops (PDF)](https://www.irs.gov/pub/irs-drop/rr-19-24.pdf)
- [Chainalysis: 2025 crypto theft reaches $3.4 billion — personal wallet drains](https://www.chainalysis.com/blog/crypto-hacking-stolen-funds-2026/)
- [Revoke.cash: token approval checker](https://revoke.cash/)
