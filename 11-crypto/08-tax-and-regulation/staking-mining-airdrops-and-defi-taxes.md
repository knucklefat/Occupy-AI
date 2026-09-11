# Staking, Mining, Airdrops, and DeFi Taxes

**In one sentence:** Anything the blockchain *gives* you (staking rewards, mined coins, airdrops) is ordinary income the moment you control it, and anything you *swap*, including entering a liquidity pool or wrapping a token, is probably a taxable disposal, with a handful of gray areas where the IRS has not spoken.

*Current as of September 11, 2026.*

## The two-step pattern that covers almost everything

Earned crypto is taxed twice, at two different moments:

1. **At receipt** — ordinary income equal to the fair market value (FMV) in USD when you gain "dominion and control" (you can sell, transfer, or otherwise use it). That FMV becomes your cost basis.
2. **At disposal** — capital gain or loss equal to sale proceeds minus that basis, short- or long-term depending on how long you held after receipt.

Get this pattern down and most of the exotic cases become bookkeeping.

## Staking rewards: Rev. Rul. 2023-14

In July 2023 the IRS ruled that a cash-method taxpayer who stakes on a proof-of-stake network must include validation rewards in gross income at FMV in the year they gain dominion and control. The ruling explicitly covers staking **through an exchange** as well as running your own validator. A lockup period delays recognition until the lockup ends; it does not eliminate it.

**Example.** You stake 32 ETH. During 2026 you receive rewards on 12 separate days totaling 1.1 ETH, with a combined FMV at each receipt of $3,850. You report **$3,850 of ordinary income** on Schedule 1 (line 8z, "other income") for 2026. Your basis in the 1.1 ETH is $3,850. If you sell that 1.1 ETH in March 2027 for $4,400, you have a $550 short-term capital gain.

**Practical points:**
- Liquid staking tokens (stETH, rETH): depositing ETH and receiving stETH is arguably a swap (taxable) or arguably a receipt-for-deposit (not taxable). Most tax software defaults to treating it as a taxable swap; conservative filers follow that. The IRS has not ruled.
- Rewards that auto-compound inside a rebasing token (stETH balance grows daily) are still income as they accrue, in practice tracked by the daily balance change.
- The *Jarrett* litigation (a Tennessee couple arguing staking rewards are newly created property not taxable until sold) is still the main legal challenge to this position; as of September 2026 it has not overturned the ruling. Both the Lummis bill and the House PARITY Act would legislatively defer staking income until sale, but neither has passed.

## Mining

Mined coins are ordinary income at FMV when received. If mining is a **trade or business** (regular, continuous, profit-motivated), you report on Schedule C, owe 15.3% self-employment tax on net profit, and can deduct electricity, hardware depreciation, hosting fees, and pool fees. Hobby miners report income on Schedule 1 and get no deductions.

**Example.** A home miner receives 0.15 BTC during 2026 with a total FMV at receipt of $16,500. Electricity and pool fees were $6,200; a $4,000 rig is depreciated $800 this year. Schedule C net profit = $16,500 − $6,200 − $800 = **$9,500**, subject to income tax plus roughly $1,342 of SE tax (92.35% × $9,500 × 15.3%). Basis in the 0.15 BTC is $16,500.

## Airdrops and hard forks

Rev. Rul. 2019-24 draws the line: a **hard fork alone** (the chain splits but you receive nothing) is not income. An **airdrop** of new tokens you can control is ordinary income at FMV on receipt. That includes tokens you did not ask for, though the IRS position is that income arises only once you have the ability to transfer or sell them.

**Example.** A protocol airdrops you 1,200 governance tokens on May 2, 2026, trading at $2.10 when they hit your wallet: **$2,520 of ordinary income**, basis $2,520. If the token is at $0.40 when you finally sell in November 2026, you have a $2,040 short-term capital loss, but you still owed income tax on $2,520. This "phantom income" trap is why many people claim airdrops promptly and sell some to cover the tax.

Worthless or unsellable airdrops: if there is no market at receipt, the FMV is arguably zero. Document it.

## Liquidity pools, yield farming, and lending

The IRS has never issued guidance on DeFi mechanics. The positions below reflect how most professionals and tax software treat them, ranked from conservative to aggressive.

**Entering a liquidity pool** (deposit ETH + USDC, receive an LP token):
- *Conservative (most common):* it is a swap of ETH and USDC for the LP token, so you realize gain/loss on both deposited assets. The LP token's basis = FMV of what you deposited.
- *Aggressive:* it is a non-taxable deposit because you retain economic ownership. Weaker after the wallet-by-wallet rules; use only with professional advice.

**Exiting the pool:** the reverse swap. Proceeds = FMV of tokens received; basis = LP token basis. The difference captures fees earned and impermanent loss in one number.

**Farming rewards** (extra tokens paid for providing liquidity) are ordinary income at FMV when claimable.

**Lending on Aave, Compound, or a centralized platform:** interest is ordinary income at FMV as it accrues or is paid. Whether *depositing* into a lending protocol (receiving aTokens or cTokens) is itself a disposal is a gray area; the Lummis bill would explicitly make crypto lending non-taxable like securities lending, but that is not law yet.

**Borrowing** against crypto is not taxable (a loan is not income). Being **liquidated** is a forced sale: proceeds = debt extinguished, basis = your collateral's basis.

**Wrapping** (ETH to WETH, BTC to WBTC) and **bridging**: no IRS guidance. Notice 2024-57 deferred *broker reporting* of wrapping and unwrapping, which is not the same as declaring it non-taxable. Many filers treat like-for-like wraps as non-taxable and cross-chain bridges that change the asset as taxable. Pick a position, apply it consistently, disclose if material.

## NFTs and the collectibles question

Under Notice 2023-27 the IRS uses a **look-through** test: an NFT is a collectible if the thing it represents is a collectible under section 408(m) (art, gems, coins, antiques, etc.). Consequences:
- Long-term gains on collectibles are taxed at up to **28%**, not 20%.
- An IRA that buys a collectible NFT has a deemed distribution equal to its cost.
The IRS acknowledged it is not certain whether a digital image counts as a "work of art"; virtual land generally would not. Treat art-like PFP NFTs as collectibles unless you have a reason not to.

**Example.** You buy an NFT for 2 ETH when ETH is $2,500 (basis $5,000; the ETH you spent was itself a disposal with its own gain). Fourteen months later you sell it for 4 ETH at $3,000 = $12,000 proceeds. Gain = $7,000 long-term. If it is a collectible and you are in the 35% bracket, tax is 28% × $7,000 = $1,960 plus NIIT if applicable, versus $1,400 at 20%.

Minting and selling NFTs as a creator is ordinary (usually Schedule C) income; royalties are ordinary income.

## Gas fees and basis

- **Fees to buy or swap** are added to the basis of the asset acquired.
- **Fees to sell** reduce proceeds.
- **Fees on transfers between your own wallets** are the gray one. Since the fee is paid *in* crypto, paying it is a disposal of that crypto (usually a trivial gain/loss). Whether the fee then adds to the basis of the transferred coins is unsettled; the cautious approach treats it as a non-deductible personal expense, the common software approach adds it to basis.
- A failed transaction that still burned gas: capital loss on the gas spent is the usual treatment, but the amount is small enough that many ignore it.

**Example.** You swap 1 ETH (basis $2,000) for 25 LINK when ETH is $3,000 and pay 0.005 ETH ($15) gas. Disposal of 1.005 ETH: proceeds $3,015, basis $2,010 → $1,005 gain. LINK basis = $3,000 + $15 = $3,015.

## Stablecoins are not exempt

Selling USDC for dollars at exactly $1.00 produces a $0 gain, but it is still a disposal that must appear on Form 8949 (brokers do not need to report stablecoin sales under $10,000 in a year on Form 1099-DA, but you still must report them). Using stablecoins to buy other crypto is a disposal of the stablecoin. Fractional-cent gains and losses add up over thousands of trades; tax software handles it. Proposals to treat stablecoins as cash-equivalents (PARITY Act) would fix this but have not passed.

## How to actually do it

1. Tag every incoming reward in your tax software as income (staking, mining, airdrop, interest) so it flows to Schedule 1 or Schedule C, not Form 8949.
2. Set aside cash for tax on rewards as they arrive; roughly 25–40% of the USD value depending on your bracket and state.
3. For DeFi, choose a consistent position on LP deposits and wrapping, write it down, and keep the wallet addresses and block explorer links.
4. For NFTs, decide collectible vs. not at purchase and keep a note of why.
5. If your DeFi activity is large or unusual, consider attaching Form 8275 (disclosure statement) to explain a reasonable but unsettled position; it reduces penalty exposure.
6. Talk to a crypto-specialized CPA if annual reward income exceeds a few thousand dollars or you run a validator.

## Key takeaways

- Staking rewards are ordinary income when you can control them (Rev. Rul. 2023-14), including exchange staking; that FMV becomes your basis.
- Mining as a business goes on Schedule C with SE tax but allows deductions; hobby mining does not.
- Hard forks alone are not income; airdrops you can access are, even if they later collapse in value.
- Most professionals treat entering and exiting liquidity pools as taxable swaps and farming rewards as income; the IRS has issued no DeFi guidance.
- Wrapping and bridging are gray; be consistent and document.
- Art-like NFTs are likely collectibles: 28% max long-term rate and off-limits in IRAs.
- Gas fees adjust basis or proceeds, and paying gas in ETH is itself a tiny disposal.
- Stablecoin trades are reportable even when the gain is zero.

## Sources

- [IRS: Rev. Rul. 2023-14 (staking rewards)](https://www.irs.gov/pub/irs-drop/rr-23-14.pdf)
- [IRS: Rev. Rul. 2019-24 and virtual currency FAQs (hard forks, airdrops)](https://www.irs.gov/individuals/international-taxpayers/frequently-asked-questions-on-virtual-currency-transactions)
- [IRS: Notice 2023-27 (NFTs as collectibles)](https://www.irs.gov/pub/irs-drop/n-23-27.pdf)
- [IRS: Digital assets](https://www.irs.gov/filing/digital-assets)
- [The Tax Adviser: Navigating the Form 1099-DA reporting maze (Notice 2024-57 exceptions)](https://www.thetaxadviser.com/issues/2026/mar/navigating-the-form-1099-da-reporting-maze/)
- [Sen. Lummis: Digital asset tax legislation (staking deferral, lending)](https://www.lummis.senate.gov/press-releases/lummis-unveils-digital-asset-tax-legislation/)
- [House Ways and Means June 2026 digital asset tax hearing summary](https://www.spotedcrypto.com/crypto-tax-hearing-june-2026-de-minimis-staking/)
