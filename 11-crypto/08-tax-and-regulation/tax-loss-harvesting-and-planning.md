# Tax-Loss Harvesting and Planning for Crypto

**In one sentence:** Because crypto is property and volatile, it offers unusually good tax-planning levers (harvesting losses without a wash-sale rule, picking high-basis lots, gifting or donating appreciated coins, and holding growth in a Roth), but each lever has a legal edge you should not step past.

*Current as of September 11, 2026. Wash-sale and de minimis legislation is pending; check status before relying on the no-wash-sale position for late-2026 trades.*

## Tax-loss harvesting in crypto

**The idea:** sell a position that is under water to realize the loss, use the loss to offset gains (and up to $3,000 of ordinary income per year), and keep your market exposure.

**Why crypto is special (still):** the wash-sale rule in Section 1091, which disallows a loss if you buy a "substantially identical" security within 30 days before or after the sale, applies to stock and securities. The IRS classifies crypto as property, so as of September 2026 you can sell BTC at a loss and buy it back immediately. Two active bills (the Lummis Senate bill and the bipartisan PARITY Act in the House) would extend the rule to digital assets, and a House Ways and Means hearing in June 2026 signaled interest, but nothing has passed and drafts have been prospective.

**Guardrails even now:**
- **Economic substance.** A sale and instant rebuy with zero price movement invites the argument that nothing real happened. Wait a few hours or a day, or rotate into a correlated but different asset (BTC to a BTC ETF, ETH to SOL) for a while.
- **ETFs are securities.** Spot bitcoin and ether ETFs (IBIT, FBTC, ETHA, etc.) are subject to the wash-sale rule. Selling IBIT at a loss and buying FBTC within 30 days is very likely "substantially identical." Selling IBIT and buying spot BTC is probably not, but nobody has litigated it.
- **Wallet-by-wallet basis.** Since 2025 you harvest per wallet; a loss lot on Coinbase cannot be paired with a high-basis lot in your Ledger.

**Worked example.** In 2026 you realized $30,000 of gains selling SOL. In November you hold 2 ETH bought at $4,000 each, now $2,600. Sell both: loss = $2,800 × 2 = **$5,600**. Rebuy 2 ETH the next day at $2,620. Net taxable gain drops to $24,400; at 15% plus 3.8% NIIT that saves about **$1,053**. Your new ETH basis is $5,240, so the deferred gain resurfaces on a later sale, but if you hold it more than a year it is taxed at long-term rates, and if you die holding it the gain disappears via step-up.

## Specific-identification lot selection

When you sell part of a position you can pick which units. Rules: identify the units at or before the sale (by date acquired, basis, or wallet address) and be able to prove it. On a custodial exchange, set your method (HIFO/specific lot) in the account before trading; FIFO is the default if you don't.

**Strategy:** sell high-basis lots when you want to minimize gain; sell low-basis long-term lots when you are in the 0% bracket and want to "harvest gains" for free.

**Gain-harvesting example.** A married couple with $70,000 of taxable income in 2026 has room up to $98,900 in the 0% long-term bracket. They sell BTC with a $28,000 long-term gain, pay **$0 federal tax**, and immediately rebuy (no wash-sale issue on a gain anyway). Their basis resets $28,000 higher.

## Holding-period planning

The difference between short-term (up to 37% + 3.8%) and long-term (up to 20% + 3.8%) is worth up to 17 percentage points. Before selling, check the acquisition date: if you are within a few weeks of the one-year mark and are not fearful of a crash, waiting can be worth it. Sell the lots that are already long-term first when you have a mix.

For coins received as income (staking, airdrops), the holding period starts the day after receipt, so a "long-term" sale of staking rewards requires holding those specific rewards for over a year.

## Gifting appreciated crypto

Giving crypto is not a taxable disposal. The recipient takes your basis and holding period (for gains); for losses their basis is the lower of your basis or the value at the gift. In 2026 you can give $19,000 per recipient ($38,000 from a couple) without filing a gift tax return; larger gifts require Form 709 but use up part of the $15 million lifetime exclusion rather than creating tax.

**Use case:** shift appreciated coins to an adult child in the 0% capital-gains bracket, who sells and pays nothing. Watch the "kiddie tax" for children under 19 (or full-time students under 24), which taxes their unearned income above about $2,700 at the parents' rate.

## Donating appreciated crypto

Donate coins held more than one year directly to a qualified charity and you (1) recognize no gain and (2) deduct the full fair market value, up to 30% of AGI with a five-year carryforward. This is strictly better than selling and giving cash.

**Mechanics that trip people up:**
- Over $500: Form 8283. Over **$5,000: a qualified appraisal is required**, and the IRS has said an exchange price printout does not substitute for one (Chief Counsel memo 202302012). Appraisals cost a few hundred dollars. The Lummis bill would remove this requirement for actively traded coins; not law yet.
- Donor-advised funds (Fidelity Charitable, Schwab Charitable, DAFgiving360, and crypto-native platforms such as The Giving Block and Endaoment) accept BTC, ETH, and major tokens, liquidate them, and let you grant over time. Contribute in a high-income year, grant later.
- Coins held one year or less: deduction limited to your basis, not FMV.

**Example.** You bought 1 BTC for $20,000 in 2023; it is worth $110,000 in December 2026 and you are in the 35% bracket. Sell and donate cash: $90,000 gain × (20% + 3.8%) = $21,420 tax, then an $88,580 deduction. Donate the coin: $0 tax and a **$110,000 deduction**, worth about $38,500 at 35%. Difference: roughly $29,000 of value.

## Roth accounts and crypto

If you expect an asset to compound at high rates, holding it in a **Roth** (contributions after-tax, growth and qualified withdrawals tax-free) is the single strongest structure available. Practical routes: spot crypto ETFs inside any Roth IRA at a mainstream brokerage; self-directed Roth IRAs that hold coins directly (iTrustCapital, Alto, Unchained); Roth 401(k) brokerage windows. Details, fees, and prohibited-transaction pitfalls are in the retirement-accounts file.

**Roth conversion angle:** converting a traditional IRA to Roth is taxed at today's ordinary rates on today's value. Converting *after* a drawdown, when the coins or ETF shares are cheap, means paying tax on a smaller number and letting the recovery happen tax-free. Conversions are irreversible (recharacterization ended in 2018), so size them to stay within your current bracket.

## Moving to a no-income-tax state (with realism)

Alaska, Florida, Nevada, New Hampshire, South Dakota, Tennessee, Texas, Washington (which does tax capital gains above about $270,000 at 7%, so it is not "no tax" for large crypto sales), and Wyoming have no state income tax. If you sit on a large unrealized gain, relocating before you sell can save 5–13% (California's top rate is 13.3%, New York City's combined rate is around 14.8%).

**What "realism" means:**
- Domicile is a facts-and-circumstances test: driver's license, voter registration, where your kids go to school, where your stuff is, days present. High-tax states audit high earners who "move" the year before a big sale. Keep a day log; the 183-day rule is a floor, not the whole test.
- Gains you realize *before* moving are taxed by the old state. Gains realized after a genuine move generally are not (California does not tax former residents on post-move sales of intangibles), but income earned there while resident, including staking rewards, is.
- Some states have "trailing" rules for deferred compensation and for partial-year residents; California in particular pursues people who keep a house there.
- Puerto Rico's Act 60 is the aggressive version: bona fide residents pay 0% on capital gains that accrue *after* they move (pre-move appreciation is still US-taxed if sold within 10 years, and fully at the federal level otherwise), in exchange for real residency, a property purchase, and an annual charitable contribution. It is heavily audited.

## Estate step-up

Under Section 1014, assets you own at death get a basis equal to their fair market value on the date of death. Heirs can sell immediately with no capital gain. Combined with the 2026 estate exclusion of $15 million per person ($30 million per couple), this is why very large, very appreciated crypto positions are often held rather than sold. Two practical requirements: heirs must be able to *access* the coins (seed phrases, multisig instructions, a custodian with beneficiary designations), and the estate needs a defensible valuation at date of death (exchange prices at time of death, documented).

Gifts during life do **not** get a step-up; the recipient inherits your basis. So for low-basis coins you plan never to sell, holding until death beats gifting, while for high-basis or loss positions, gifting or selling makes more sense.

## How to actually do it

1. In November, run a gain/loss report by lot and wallet. List every lot with an unrealized loss and every gain you have already realized.
2. Harvest losses to offset gains first, then up to $3,000 of ordinary income; rebuy after a short gap or via a different asset if you want exposure.
3. If you are in the 0% long-term bracket, harvest gains up to the bracket ceiling.
4. For charitable giving, donate long-term appreciated coins through a DAF; commission a qualified appraisal if over $5,000.
5. For gifts to family, stay under $19,000 per recipient or file Form 709.
6. Consider Roth conversions in drawdowns, sized to your bracket.
7. Put your seed phrases and account list in your estate plan; the step-up is worthless if nobody can find the keys.

## Key takeaways

- No wash-sale rule applies to spot crypto as of September 2026, but it applies to crypto ETFs, and legislation to change this is actively pending.
- Leave a gap or rotate assets when harvesting to avoid an economic-substance challenge.
- Specific-ID lot selection can turn a gain into a loss on the same trade; set it up before you sell.
- Holding past one year can cut the federal rate from 37% to 20%; check acquisition dates before selling.
- Donating long-term appreciated crypto avoids the gain and deducts full value; above $5,000 you need a qualified appraisal, not a screenshot.
- Roth accounts and Roth conversions during drawdowns are the most powerful structures for high-growth assets.
- Moving states works only if the move is real and precedes the sale; Washington and Puerto Rico have their own twists.
- Death resets basis to market value; gifts do not.

## Sources

- [IRS: Frequently asked questions on virtual currency transactions (gifts, donations, specific ID)](https://www.irs.gov/individuals/international-taxpayers/frequently-asked-questions-on-virtual-currency-transactions)
- [IRS: Tax year 2026 inflation adjustments (gift exclusion, estate exclusion)](https://www.irs.gov/newsroom/irs-releases-tax-inflation-adjustments-for-tax-year-2026-including-amendments-from-the-one-big-beautiful-bill)
- [Kiplinger: 2026 capital gains thresholds](https://www.kiplinger.com/taxes/irs-updates-capital-gains-tax-thresholds)
- [Sen. Lummis: Digital asset tax legislation (wash sale, appraisal repeal)](https://www.lummis.senate.gov/press-releases/lummis-unveils-digital-asset-tax-legislation/)
- [BDO: Congress working to reform tax treatment of digital assets (PARITY Act comparison)](https://www.bdo.com/insights/tax/congress-working-to-reform-tax-treatment-of-digital-assets)
- [Gordon Law: Crypto wash sale rule in 2026](https://gordonlaw.com/learn/crypto-wash-sale-rule-in-2026-is-the-loophole-finally-closed/)
- [CNBC: Congress renews push to end crypto wash sale loophole (July 2026)](https://www.cnbc.com/2026/07/28/congress-renews-push-to-end-crypto-wash-sale-tax-loophole.html)
- [IRS: Notice 2023-27 (NFT collectibles and IRAs)](https://www.irs.gov/pub/irs-drop/n-23-27.pdf)
