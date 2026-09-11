# Reporting and Forms: 8949, Schedule D, 1099-DA, FBAR, and Fixing Past Years

**In one sentence:** Crypto disposals go on Form 8949 and Schedule D, crypto income goes on Schedule 1 or Schedule C, everyone answers the digital-asset question on page 1 of Form 1040, and starting with 2025 activity the IRS is receiving a copy of your exchange trades on Form 1099-DA, so your return needs to match.

*Current as of September 11, 2026.*

## The map of forms

| What happened | Where it goes |
|---|---|
| Sold, swapped, or spent crypto | Form 8949 (each lot) → totals to Schedule D |
| Staking, airdrop, interest, hobby mining, other reward income | Schedule 1, line 8z ("other income") |
| Mining, validating, or trading as a business; NFT creator sales | Schedule C (plus Schedule SE for self-employment tax) |
| Paid in crypto by an employer | W-2 wages, as usual |
| Paid in crypto as a contractor | 1099-NEC → Schedule C |
| Gave crypto worth more than $19,000 (2026) to one person | Form 709 (gift tax return; usually no tax due) |
| Donated crypto worth more than $500 | Form 8283 (Section B and a qualified appraisal above $5,000) |
| Net investment income above $200k/$250k MAGI | Form 8960 (3.8% NIIT) |
| Foreign account holding crypto **and** fiat over $10,000 | FinCEN Form 114 (FBAR), filed separately from the 1040 |
| Possibly: foreign financial assets over $50k/$100k | Form 8938 (unsettled for pure crypto; see below) |

## The digital-asset question on Form 1040

Near the top of the 1040 (and 1040-SR, 1040-NR, 1041, 1065, 1120, 1120-S) is a yes/no box: *At any time during the tax year, did you (a) receive (as a reward, award, or payment for property or services); or (b) sell, exchange, or otherwise dispose of a digital asset (or a financial interest in a digital asset)?*

Answer **Yes** if you received crypto as payment, reward, mining, staking, or an airdrop; sold or swapped it; spent it; or paid transfer fees with it. Answer **No** if you only bought with USD, held, or moved coins between your own wallets (fee nuance aside). Leaving it blank or answering falsely is signed under penalty of perjury and is the IRS's cleanest hook for a willfulness argument later.

## Form 8949 and Schedule D, line by line

Each disposal is a row on Form 8949: description (e.g., "0.5 BTC"), date acquired, date sold, proceeds, cost basis, adjustment code if any, gain/loss. Rows are sorted into boxes:

- **Box A/D:** broker reported the sale *and* basis to the IRS (long-term is D). Most 1099-DA rows for 2026 activity should land here.
- **Box B/E:** broker reported proceeds but not basis. Most 2025-activity 1099-DA rows.
- **Box C/F:** not reported to the IRS at all (self-custody wallets, DeFi, foreign exchanges).

Totals flow to Schedule D, which nets short-term against short-term, long-term against long-term, then the two against each other. If you have thousands of rows, you may attach a summary statement per box with the detail on a separate schedule (tax software produces this).

**Worked example.** Three 2026 disposals:

| Lot | Acquired | Sold | Proceeds | Basis | Gain |
|---|---|---|---|---|---|
| 0.2 BTC | 2024-02-10 | 2026-03-05 | $22,000 | $9,000 | +$13,000 LT |
| 5 ETH | 2026-01-15 | 2026-04-20 | $14,000 | $16,500 | −$2,500 ST |
| 300 SOL | 2025-11-01 | 2026-08-30 | $48,000 | $60,000 | −$12,000 ST |

Schedule D: short-term net = −$14,500; long-term net = +$13,000; overall net = −$1,500. You deduct $1,500 against ordinary income and carry nothing forward. Had the BTC gain been $20,000, net would be +$5,500 and, because short-term losses absorb long-term gain, the remaining $5,500 is taxed at long-term rates.

## Form 1099-DA: what brokers now send the IRS

The 2024 final broker regulations (T.D. 10000) created Form 1099-DA. The rollout:

- **2025 transactions (forms issued early 2026):** custodial brokers (Coinbase, Kraken, Robinhood, Gemini, PayPal, etc.) report **gross proceeds** only. Basis is optional and mostly absent.
- **2026 transactions (forms issued early 2027):** brokers must also report **cost basis** and acquisition dates for "covered" assets bought and held at that same broker.
- Certain hard cases (wrapping, liquidity provision, staking, lending, short sales) were carved out of reporting by Notice 2024-57 pending further study.
- Notices 2024-56 and 2025-33 give brokers penalty relief for good-faith errors through 2027, and some brokers may issue 2025 forms up to a year late.
- **DeFi front-ends are not brokers.** The separate December 2024 rule that would have made them brokers was repealed by Congress under the Congressional Review Act (H.J.Res. 25, signed April 10, 2025).
- Small carve-outs: brokers need not report stablecoin sales under $10,000 per year or NFT sales under $600. You still must.

**Why basis on 1099-DA is often wrong.** The regulations forbid a broker from using basis passed along from another broker when you transfer coins in. So if you bought ETH on Kraken, moved it to Coinbase, and sold there, Coinbase reports proceeds with **no basis** (Box B/E). If you do nothing, the IRS's automated matching will assume basis is zero and treat the whole proceeds as gain. Your 8949 fixes this by entering your real basis with adjustment code B if the 1099-DA showed an incorrect figure.

**Lot selection with a broker.** The default for broker reporting is FIFO unless you identified specific units to the broker at or before the sale. Set your preferred method (HIFO or specific lot) in the exchange's tax settings before you trade; for 2025 activity, Notice 2025-7 let you document the choice in your own records instead.

## FBAR and FATCA for foreign exchanges

**FBAR (FinCEN 114):** FinCEN Notice 2020-2 said a foreign account holding *only* virtual currency is not currently reportable, but announced plans to change that. As of September 2026, **no final rule has been issued**, so pure-crypto foreign accounts remain outside FBAR. If the account also holds fiat, securities, or anything else reportable and the aggregate of all your foreign accounts exceeds $10,000 at any point in the year, the whole account is reportable. Penalties for non-willful failures run about $10,000 per violation (inflation-adjusted higher), and willful penalties are far worse, so most advisers say: if you are near the threshold on Binance.com, Bybit, or a non-US Kraken entity, file anyway. It is free and there is no downside to over-reporting.

**Form 8938 (FATCA):** the statute's "specified foreign financial asset" language is broad enough to reach crypto held with a foreign financial institution, and the IRS has never said it does not. Thresholds for a US resident are $50,000 at year-end or $75,000 at any time (single) and double that for joint filers. Conservative practice: file it.

Self-custody wallets (Ledger, MetaMask) are not "foreign accounts" regardless of where the nodes are; there is nobody holding the asset for you.

## Record-keeping

Keep for at least seven years after filing: exchange CSV exports and API history, wallet addresses and transaction hashes, USD pricing source, lot-selection method and any specific-ID elections, 1099-DA, 1099-MISC, and 1099-NEC forms, receipts for goods bought with crypto, the Rev. Proc. 2024-28 basis allocation you made as of January 1, 2025, and a written explanation of any DeFi position you took. Exchanges shut down (FTX, Voyager, Celsius); export while you can.

## What if you did not report in prior years

The IRS has the data. It has run John Doe summonses on Coinbase, Kraken, and others, sends "educational" and compliance letters (6173, 6174, 6174-A), and will now match 1099-DA proceeds automatically. Options depend on *why* you did not report:

**Non-willful mistakes** (you didn't know a swap was taxable, forgot an exchange): file **Form 1040-X** for each open year. You generally have three years from the original due date to claim a refund, but there is no deadline to amend to pay more. The IRS has three years to audit a filed return, six years if you omitted more than 25% of gross income, and forever if you never filed or the return was fraudulent. Penalties for amended returns are typically the 20% accuracy-related penalty on the additional tax plus interest, and sometimes no penalty at all if you come forward before contact.

**Willful concealment** (you knew and hid it, used mixers, structured withdrawals): consider the **IRS Criminal Investigation Voluntary Disclosure Practice**. You file Form 14457 Part I for preclearance, then Part II within 45 days, pay all tax, interest, and penalties (generally a 75% civil fraud penalty on the highest-tax year plus 20% accuracy penalties on the others, and FBAR penalties if relevant), and in exchange the IRS normally recommends no prosecution. It only works if you apply *before* the IRS has your name from a summons, informant, or exam. This is a lawyer's job, not a CPA's.

A **Digital Assets Voluntary Disclosure Program Act** offering a two-year amnesty window was discussed at the June 2026 House hearing but has not been enacted.

**Example.** In 2023 you swapped $40,000 of ETH for SOL without reporting; basis was $15,000, so you omitted $25,000 of long-term gain. If your total 2023 gross income was $90,000, the omission exceeds 25%, giving the IRS six years (to April 2030). Amending now: extra tax at 15% ≈ $3,750, plus interest (roughly 8% compounded since April 2024 ≈ $800), plus a possible 20% penalty ≈ $750. Total ≈ $5,300, versus far more if the IRS finds it first and argues willfulness.

## How to actually do it

1. In January, download every 1099-DA, 1099-MISC (staking/rewards), and 1099-NEC you receive, and compare to your tax-software output. Investigate every mismatch.
2. Enter true basis on Form 8949 for any Box B/E rows; use adjustment code B where the 1099-DA figure is wrong.
3. Answer the digital-asset question honestly; "Yes" is not an audit trigger by itself.
4. If you have foreign-exchange accounts, file FBAR (due April 15 with automatic extension to October 15) and consider Form 8938.
5. If you discover unreported prior years, quantify the exposure first, then choose between 1040-X and the Voluntary Disclosure Practice with a professional.
6. Archive everything in a folder you will still have in 2033.

## Key takeaways

- Disposals → Form 8949/Schedule D; income → Schedule 1 or Schedule C; the 1040 digital-asset question must be answered.
- Form 1099-DA reports gross proceeds for 2025 activity and adds cost basis for 2026 activity; the IRS matches these to your return.
- Broker-reported basis is often missing or wrong for transferred-in coins; your 8949 must supply the truth.
- DeFi front-ends are not brokers (rule repealed April 2025), so on-chain activity is self-reported in Box C/F.
- Pure-crypto foreign accounts are not yet FBAR-reportable (no final rule as of September 2026), but mixed accounts are, and filing anyway is the safe play.
- Non-willful omissions: amend with 1040-X. Willful ones: the Voluntary Disclosure Practice, before the IRS contacts you.
- Keep seven years of records and export from exchanges before they disappear.

## Sources

- [IRS: Digital assets (forms and the 1040 question)](https://www.irs.gov/filing/digital-assets)
- [IRS: Final regulations and related guidance for broker reporting of digital assets](https://www.irs.gov/newsroom/final-regulations-and-related-irs-guidance-for-reporting-by-brokers-on-sales-and-exchanges-of-digital-assets)
- [IRS: Frequently asked questions about broker reporting](https://www.irs.gov/filing/frequently-asked-questions-about-broker-reporting)
- [The Tax Adviser: Navigating the Form 1099-DA reporting maze](https://www.thetaxadviser.com/issues/2026/mar/navigating-the-form-1099-da-reporting-maze/)
- [Thomson Reuters: Form 1099-DA debut will test broker, taxpayer readiness](https://tax.thomsonreuters.com/news/form-1099-da-debut-will-test-broker-taxpayer-readiness-in-transition-year/)
- [IRS Criminal Investigation: Voluntary Disclosure Practice](https://www.irs.gov/compliance/criminal-investigation/irs-criminal-investigation-voluntary-disclosure-practice)
- [TokenTax: FBAR for crypto (FinCEN Notice 2020-2 status)](https://tokentax.co/blog/how-to-file-a-crypto-fbar)
- [Taxes for Expats: Crypto FBAR requirements 2026](https://www.taxesforexpats.com/articles/fbar-fatca/crypto-fbar.html)
- [House Ways and Means June 2026 hearing (voluntary disclosure bill)](https://www.spotedcrypto.com/crypto-tax-hearing-june-2026-de-minimis-staking/)
