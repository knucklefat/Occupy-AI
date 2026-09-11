# Staking and Yield

**In one sentence:** Staking pays you a few percent a year for helping secure a proof-of-stake network, which is real and mostly safe on the big chains — but every step you take beyond plain native staking (exchange staking, liquid staking, restaking, "stablecoin yield") adds a counterparty or a smart contract that can fail, and the extra yield is your compensation for that risk, not free money.

## What staking is

Proof-of-stake blockchains (Ethereum, Solana, Cardano, Polkadot, Cosmos, Avalanche and most others; not bitcoin) choose who gets to add the next block by having participants lock up ("stake") the network's coin as collateral. Stakers earn newly issued coins plus a share of transaction fees; if they misbehave or go offline, part of their stake can be destroyed ("slashing"). Anyone who holds the coin can stake, directly or by delegating to a validator who runs the hardware.

The yield is not interest in the bank sense. It is (a) new coins printed by the protocol — which dilutes non-stakers, so part of your "yield" is just not being diluted — plus (b) fees and, on some chains, MEV (value validators extract by ordering transactions). What matters is the *real* yield: nominal staking rate minus the network's inflation rate.

## Current yields (as of September 2026, approximate)

| Asset | Nominal staking yield | Network inflation | Real yield | Unstaking delay |
|---|---|---|---|---|
| Ether (ETH) | ~3–4% native; ~2.2–3% via Lido | ~0–0.5% | ~3% | Hours to days (queue varies) |
| Solana (SOL) | ~6–7% | ~4.5–5% | ~1–2% | ~2–3 days (one epoch) |
| Cardano (ADA) | ~2–3% | ~2% | ~0–1% | None |
| Polkadot (DOT) | ~10–12% | ~7–8% | ~2–4% | 28 days |
| Cosmos (ATOM) | ~15–19% | ~10–14% | ~2–8% | 21 days |
| Avalanche (AVAX) | ~5–7% | ~4–5% | ~1–2% | Fixed lock, 2 weeks to 1 year |

Take the "real yield" column seriously. A chain advertising 18% that inflates at 14% is paying you 4% in economic terms and 18% in tax terms (see below). And all of these yields are paid in the coin itself: a 7% SOL yield on a year when SOL falls 60% is a 57% loss.

## The ways to stake, from safest to most involved

**1. Native (solo or delegated) staking.** On Ethereum, running your own validator requires 32 ETH (~$80,000 at September 2026 prices) and an always-on machine. On Solana, Cardano, Cosmos and most others, you delegate any amount from your own wallet to a validator and keep custody. Risk: validator slashing (rare on major chains; on Ethereum, slashing has hit well under 0.1% of validators historically, mostly through operator misconfiguration), the unstaking delay, and your own key management.

**2. Exchange staking.** Coinbase, Kraken, Binance and others stake on your behalf. Convenient, but the exchange keeps a commission (Coinbase takes roughly 25–35% of rewards depending on the asset), you take exchange counterparty risk (FTX's staked customer assets were lost in the bankruptcy), and the exchange, not you, holds the keys. Regulatory risk is also real: Kraken shut down its U.S. staking service in 2023 under an SEC settlement and only resumed after the 2025 policy shift.

**3. Liquid staking.** You deposit ETH into Lido and receive stETH, a token that represents your staked ETH plus accruing rewards and can be traded, used as collateral, or sold instantly instead of waiting in the unstaking queue. Jito does the same on Solana (JitoSOL) and adds MEV revenue. Lido holds about $24B of ETH as of September 2026, roughly 46% of all liquid-staked assets, and keeps 10% of rewards. Risks: the protocol's smart contracts (Lido has been audited many times and has run since 2020, but "unhacked so far" is the strongest available claim for any contract); stETH trading below ETH during stress (it dipped to about 0.94 ETH in June 2022 when Celsius and Three Arrows were forced sellers); and the centralization concern that one protocol controlling a large share of Ethereum's validators creates.

**4. Restaking.** EigenLayer (now EigenCloud) lets you pledge already-staked ETH or stETH as security for other services ("AVSs" — oracles, data-availability layers, bridges) in exchange for additional rewards. Your ETH is now exposed to slashing conditions of multiple systems at once. Restaking TVL peaked near $20B in 2024 on airdrop expectations and sits around $6–7B for EigenLayer (about $10B across all restaking protocols) as of September 2026; slashing went live in 2025. The incremental yield has generally been low single digits and paid largely in project tokens; the EIGEN token itself trades about 95% below its 2024 launch levels. This is the layer where the risk/reward has been worst for ordinary participants.

**5. "Stablecoin yield."** Not staking at all, but often sold alongside it. See the next section.

## Where stablecoin yields come from

If someone offers you 5–15% on dollars, the money comes from one of five places, and you should be able to name which:

| Source | Example | Yield (Sept 2026, approx.) | What can go wrong |
|---|---|---|---|
| Treasury bills held by the issuer | Ondo USDY, BlackRock BUIDL, sUSDS (Sky) | ~3.5–4.7% | Issuer/custodian risk; redemption gates; this is the "safe" end |
| Lending to over-collateralized borrowers | Aave, Compound USDC pools | ~3–8%, spikes in bull markets | Smart-contract bug; bad-debt from oracle failure; rates collapse when nobody wants to borrow |
| Exchange or platform rewards | Coinbase USDC (3.5% with Coinbase One) | ~3–4% | The platform (counterparty) — Celsius, BlockFi, Voyager all paid 8–12% on stablecoins in 2021 and all went bankrupt in 2022 |
| Perpetual-futures funding rates ("delta-neutral") | Ethena sUSDe | 4–30% range, high single digits in 2026 | Funding goes negative in bear markets (yield falls to zero or below); the hedge sits on centralized exchanges; USDe has depegged 0.5–1% under stress |
| Token emissions | Any farm paying 40%+ | Anything | The token you are paid in goes to zero; see the DeFi file |

The rule: a stablecoin yield materially above the T-bill rate (about 4% in September 2026) is being paid for taking a risk that T-bills do not carry. Nothing is wrong with that as long as you can name the risk.

## The risk list, plainly

- **Slashing:** destroyed stake for validator misbehavior. Rare on major chains, unhedgeable, and multiplied by restaking.
- **Smart-contract risk:** liquid staking and DeFi yield run on code that can be exploited. Crypto hacks totaled about $3.4B in 2025 (the $1.5B Bybit exchange hack was the largest), and personal-wallet drains hit 80,000 victims.
- **Counterparty risk:** exchange or platform failure. The 2022 lenders paid the highest yields right up until they froze withdrawals.
- **Depeg risk:** a "stable" coin or a liquid staking token trading away from its reference. Usually temporary; catastrophic when the collateral is bad (Terra's UST went to zero in May 2022 paying 20% on its Anchor protocol).
- **Liquidity/lock-up risk:** 21–28-day unbonding periods mean you cannot sell during a crash without a liquid staking token, and liquid staking tokens trade at a discount precisely when you most want to sell.
- **Price risk dominates everything:** the yield is 3–7%; the asset moves 60–90%. Staking is a reason to earn on coins you already intend to hold, never a reason to buy a coin.
- **Regulatory risk:** staking services have been shut down by regulators before and can be again; ETFs that stake are new.

## Tax treatment (U.S.)

The IRS (Revenue Ruling 2023-14) treats staking rewards as **ordinary income at their fair market value when you gain control of them**, whether you sell or not. That value becomes your cost basis; later sales are capital gains or losses. Practical consequences: a 7% SOL yield is taxed like wages as it arrives, even in a year SOL falls 60%; rewards paid daily create hundreds of tiny tax lots (use tracking software); liquid staking tokens that accrue value in the token price (like Coinbase's cbETH) may defer the income event compared with rebasing tokens (like stETH), though guidance is unsettled. Staking inside an ETF in an IRA sidesteps all of this. Rules differ outside the U.S.; several countries tax rewards only on disposal.

## How to actually do it

1. **Only stake coins you already hold for other reasons**, and only proof-of-stake coins with large validator sets (ETH, SOL first; be wary of high-yield small chains).
2. **Choose your layer deliberately.** Simplest safe route: stake through the ETF you already own (ETHB, BSOL, etc.) or through a large exchange if you already keep coins there. Better economics: delegate from your own wallet (Solana, Cosmos) or use Lido/Jito on Ethereum/Solana.
3. **For delegation, pick a validator** with a long uptime record, moderate commission (5–10%), and a modest share of total stake (avoid concentrating on the biggest).
4. **Skip restaking and exotic yield** unless you can read the slashing conditions and are comfortable losing the position.
5. **For stablecoin yield, start with the T-bill-backed layer**, then Aave/Compound with a size you could lose; treat anything above ~8% as speculative.
6. **Record every reward** (date, amount, USD value) or use tax software that reads your wallet.
7. **Reassess quarterly:** yields, protocol news, validator performance. Unstake if anything changes that you do not understand.

## Key takeaways

- Native staking yields as of September 2026: ETH ~3–4%, SOL ~6–7%, ATOM ~15–19% nominal — but real (inflation-adjusted) yields are roughly 3%, 1–2% and 2–8% respectively.
- Yield is paid in the coin; price moves of 60–90% swamp any staking return. Stake what you would hold anyway.
- Each convenience layer adds a failure point: exchange (counterparty), liquid staking (contract + depeg), restaking (stacked slashing). Restaking has had the worst risk/reward for retail.
- Every stablecoin yield comes from T-bills, lending, platform subsidy, funding rates, or emissions; if it is well above ~4% you are being paid for a named risk, and if you cannot name it, walk away.
- 2022 was the stress test: Celsius, BlockFi, Voyager and Terra's Anchor all paid top yields until they didn't; ~$3.4B was hacked in 2025.
- U.S. tax: staking rewards are ordinary income on receipt; an ETF in an IRA is the cleanest way to capture the yield.
- Lido controls about 46% of liquid staking; the convenience is real, and so is the concentration.

## Sources

- [FinanceFeeds: Crypto staking rates compared — nominal vs real yields (Aug 2026)](https://financefeeds.com/crypto-staking-rates-compared-where-to-earn/)
- [PistachioFi: Ethereum staking yield 2026](https://www.pistachio.fi/blog/ethereum-staking-yield)
- [DefiLlama: Lido protocol data](https://defillama.com/protocol/lido)
- [DefiLlama: EigenLayer / EigenCloud protocol data](https://defillama.com/protocol/eigenlayer)
- [Coinlaw: Where stablecoin yield actually comes from, source by source](https://coinlaw.io/stablecoin-yields/)
- [Eco: Ethena USDe and sUSDe 2026 — delta-neutral yield and risks](https://eco.com/support/en/articles/15254002-ethena-usde-and-susde-2026-delta-neutral-yield)
- [Chainalysis: 2025 crypto theft reaches $3.4 billion](https://www.chainalysis.com/blog/crypto-hacking-stolen-funds-2026/)
- [IRS Revenue Ruling 2023-14 on staking rewards (PDF)](https://www.irs.gov/pub/irs-drop/rr-23-14.pdf)
- [Everstake: Ethereum staking ETFs for institutions (2026)](https://everstake.com/resources/blog/ethereum-staking-etfs-for-institutions)
- [Helius: Solana spot ETFs and staking](https://www.helius.dev/blog/solana-etfs)
