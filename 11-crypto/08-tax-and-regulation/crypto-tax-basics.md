# Crypto Tax Basics: Property, Taxable Events, Rates, and Cost Basis

**In one sentence:** The IRS treats every cryptocurrency, stablecoin, and NFT as *property*, so almost anything you do with it other than buying it with dollars and holding it is a taxable event measured in US dollars at the moment it happens.

*Current as of September 11, 2026. Figures for tax year 2026 come from the IRS inflation adjustments (Rev. Proc. 2025-32). Verify anything time-sensitive before filing.*

## Why "property" is the whole ballgame

In 2014 the IRS issued Notice 2014-21, which said virtual currency is property, not currency, for federal tax purposes. That single classification still drives everything in 2026:

- **Capital gains and losses apply.** When you dispose of a coin, you compare what you received (fair market value in USD) to your *cost basis* (what you paid, including fees) and report the difference.
- **Every disposal is its own event.** There is no "I never cashed out to dollars" exemption. Trading ETH for SOL is a sale of ETH.
- **Earning crypto is ordinary income.** Coins received for work, mining, staking, or airdrops are income at the USD value when you get control of them, and that value becomes your basis going forward.

The IRS now uses the broader term *digital asset*, defined as any digital representation of value recorded on a cryptographically secured distributed ledger. That sweeps in stablecoins and NFTs, not just bitcoin.

## Taxable vs. non-taxable events

| Action | Taxable? | What you report |
|---|---|---|
| Buy crypto with USD | No | Nothing (record basis and date) |
| Hold crypto, even if it moons | No | Nothing |
| Transfer between wallets/exchanges you own | No* | Nothing (*if you pay the network fee in crypto, that tiny fee payment is technically a disposal) |
| Sell crypto for USD | Yes | Capital gain/loss |
| Swap one crypto for another (ETH to SOL, BTC to USDC) | Yes | Capital gain/loss on the coin you gave up |
| Spend crypto on goods/services | Yes | Capital gain/loss on the coin spent |
| Get paid in crypto, mine, stake, receive an airdrop | Yes | Ordinary income at receipt |
| Receive crypto as a gift | No (recipient) | Carryover basis; donor may need Form 709 above $19,000 per recipient in 2026 |
| Donate appreciated crypto to a qualified charity | No gain | Possible itemized deduction |
| Lose crypto to a hack or exchange collapse | Complicated | Personal casualty/theft losses are mostly non-deductible through 2025 under the TCJA rules; see a professional |

## Short-term vs. long-term rates (tax year 2026)

Your holding period starts the day after you acquire a unit and ends on the day you dispose of it. Held **one year or less** = short-term, taxed at ordinary income rates. Held **more than one year** = long-term, taxed at preferential rates.

**2026 long-term capital gains brackets (taxable income):**

| Rate | Single | Married filing jointly | Head of household |
|---|---|---|---|
| 0% | up to $49,450 | up to $98,900 | up to $66,200 |
| 15% | $49,451 – $545,500 | $98,901 – $613,700 | $66,201 – $579,600 |
| 20% | above $545,500 | above $613,700 | above $579,600 |

**2026 ordinary income brackets (single / married filing jointly):** 10% to $12,400 / $24,800; 12% to $50,400 / $100,800; 22% to $105,700 / $211,400; 24% to $201,775 / $403,550; 32% to $256,225 / $512,450; 35% to $640,600 / $768,700; 37% above. The standard deduction is $16,100 single and $32,200 joint.

Two add-ons: the **3.8% Net Investment Income Tax** applies to investment income (including crypto gains) once modified AGI exceeds $200,000 single or $250,000 joint (these thresholds are not inflation-indexed). And NFTs that count as **collectibles** are capped at a 28% long-term rate rather than 20% (see the staking/DeFi file).

## Cost basis: what counts and how lots get picked

**Basis** = purchase price + acquisition fees. If you bought 1 ETH for $2,000 and paid a $10 exchange fee, your basis is $2,010. On sale, fees reduce your proceeds.

**Lot selection.** If you bought the same coin at several prices, which lot did you sell? IRS rules:

- **Specific identification** is allowed if, at the time of the sale, you identify the units (by date, basis, or wallet address) and can substantiate it. On a custodial exchange this means telling the broker before the trade settles; for 2025 the IRS allowed you to document it in your own records instead (Notice 2025-7), and many exchanges now offer HIFO or specific-lot settings in the app.
- **FIFO (first in, first out)** is the default if you do not specifically identify.
- "HIFO" (highest-in, first-out) and "LIFO" are not separate methods in the regulations; they are just specific identification applied consistently.

**Wallet-by-wallet rule (since January 1, 2025).** The 2024 broker regulations require basis tracking *per wallet or account*. You can no longer treat all your ETH everywhere as one "universal" pool. Rev. Proc. 2024-28 gave a one-time safe harbor to reasonably allocate your leftover basis to the wallets that held the coins on January 1, 2025. If you never did that allocation, you have lost the safe harbor's penalty protection, but you are still required to track wallet-by-wallet going forward; the practical fix is to use tax software that reconstructs history and document your allocation now.

## Does the wash-sale rule apply to crypto in 2026?

**No, not as of September 2026.** Section 1091 (the wash-sale rule) applies to "stock or securities." Because the IRS classifies crypto as property, you can sell bitcoin at a loss and rebuy it the next minute and the loss still counts.

What is in motion:

- Sen. Cynthia Lummis's digital-asset tax bill (introduced July 3, 2025) would extend the 30-day wash-sale rule to digital assets, alongside a $300-per-transaction de minimis exemption and deferral of staking/mining income until sale.
- The bipartisan **Digital Asset PARITY Act** (Reps. Max Miller and Steven Horsford; draft December 2025, introduced May 19, 2026) contains a similar wash-sale extension.
- The House Ways and Means Committee held a hearing on June 9, 2026; the Senate Finance Committee held one on October 1, 2025. As of mid-September 2026 nothing has been marked up or enacted. Every serious proposal has been prospective, so a loss harvested before enactment should be safe.

Two cautions: (1) **spot crypto ETFs are securities**, so wash-sale rules do apply to IBIT, FBTC, and similar shares; (2) the IRS can still attack a sale-and-immediate-rebuy under the *economic substance doctrine* if there is literally no market risk between the two legs. Waiting even a day or two, or rebuying a different coin, removes that argument.

## Worked examples

**Example 1 — crypto-to-crypto swap.** You bought 2 ETH on March 1, 2025 for $4,000 total ($2,000 each). On June 15, 2026 you swap 1 ETH for 20 SOL when ETH is $3,500. Proceeds = $3,500; basis = $2,000; **long-term gain = $1,500** (held over a year). Your 20 SOL now have a basis of $3,500 and a new holding period starting June 16, 2026.

**Example 2 — spending crypto.** You bought 0.05 BTC for $2,500 on January 10, 2026 and use it to buy a $3,200 laptop on August 20, 2026. Proceeds = $3,200; basis = $2,500; **short-term gain = $700**, taxed at your ordinary rate (say 24% = $168 of tax on a laptop purchase).

**Example 3 — lot selection matters.** You hold three lots of SOL in one wallet: 10 SOL at $20 (2023), 10 SOL at $150 (2024), 10 SOL at $240 (2025). You sell 10 SOL at $200 in 2026.
- FIFO: gain = $2,000 − $200 = **$1,800 long-term gain**.
- Specific ID choosing the $240 lot: $2,000 − $2,400 = **$400 loss**, usable against other gains.
Same trade, roughly $2,200 swing in reported gain.

**Example 4 — netting and the $3,000 rule.** In 2026 you have $9,000 of long-term crypto gains, $12,000 of short-term crypto losses, and no other investment activity. Net: $3,000 loss. You deduct $3,000 against ordinary income; if the net loss were $10,000, you would deduct $3,000 this year and carry $7,000 forward indefinitely.

## How to actually do it

1. **Export every transaction** from every exchange and wallet (CSV or API) and load it into a crypto tax tool (Koinly, CoinLedger, CoinTracker, ZenLedger). Reconcile until the tool's balances match what you actually hold.
2. **Choose a lot method per wallet** before year-end trades, and set it in your exchange account if the option exists. Document it.
3. **Convert everything to USD at the time of the transaction.** Tools do this automatically; keep the pricing source consistent.
4. **Separate income from gains.** Staking, mining, airdrops, and interest go on Schedule 1 (or Schedule C if a business); disposals go on Form 8949 and Schedule D.
5. **Check your 1099-DA** (from custodial brokers, first issued for 2025 activity) against your own records. Basis on these forms is often missing or wrong for coins you transferred in.
6. **Keep records for at least seven years**: acquisition dates, basis, disposal dates, USD values, wallet addresses, and the lot-selection rationale.

## Key takeaways

- Crypto is property: selling, swapping, and spending are all taxable; buying with USD and holding are not.
- Holding more than one year moves you from ordinary rates (up to 37%) to long-term rates (0/15/20%), plus the possible 3.8% NIIT.
- Basis = price paid plus fees; specific identification can dramatically change your reported gain, but FIFO is the default if you do not document a choice.
- Since 2025, basis must be tracked wallet-by-wallet; the universal-pool method is gone.
- The wash-sale rule does **not** apply to spot crypto as of September 2026, but it does apply to crypto ETFs, and Congress is actively considering extending it.
- Net capital losses offset gains without limit, then up to $3,000 of ordinary income per year, with the rest carried forward.
- Do not trust exchange-provided basis blindly; reconcile with your own records.

## Sources

- [IRS: Digital assets](https://www.irs.gov/filing/digital-assets)
- [IRS: Frequently asked questions on virtual currency transactions](https://www.irs.gov/individuals/international-taxpayers/frequently-asked-questions-on-virtual-currency-transactions)
- [IRS: Notice 2014-21](https://www.irs.gov/pub/irs-drop/n-14-21.pdf)
- [IRS: Rev. Proc. 2024-28 (basis allocation safe harbor)](https://www.irs.gov/pub/irs-drop/rp-24-28.pdf)
- [IRS: Frequently asked questions about broker reporting](https://www.irs.gov/filing/frequently-asked-questions-about-broker-reporting)
- [IRS: Tax year 2026 inflation adjustments](https://www.irs.gov/newsroom/irs-releases-tax-inflation-adjustments-for-tax-year-2026-including-amendments-from-the-one-big-beautiful-bill)
- [Kiplinger: 2026 capital gains thresholds](https://www.kiplinger.com/taxes/irs-updates-capital-gains-tax-thresholds)
- [Sen. Lummis: Digital asset tax legislation (July 2025)](https://www.lummis.senate.gov/press-releases/lummis-unveils-digital-asset-tax-legislation/)
- [BDO: Congress working to reform tax treatment of digital assets](https://www.bdo.com/insights/tax/congress-working-to-reform-tax-treatment-of-digital-assets)
- [Gordon Law: Crypto wash sale rule in 2026](https://gordonlaw.com/learn/crypto-wash-sale-rule-in-2026-is-the-loophole-finally-closed/)
- [CNBC: Congress renews push to end crypto wash sale loophole (July 2026)](https://www.cnbc.com/2026/07/28/congress-renews-push-to-end-crypto-wash-sale-tax-loophole.html)
