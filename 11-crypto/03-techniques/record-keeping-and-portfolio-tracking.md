# Record-Keeping and Portfolio Tracking

**In one sentence:** Crypto generates a taxable event every time you sell, swap, spend, or earn, the IRS now receives broker forms that show your proceeds but not your cost, and the only person who can prove what you paid — across every exchange and wallet — is you.

## Why this is harder than stocks

At a stock brokerage, one firm sees every buy and sell and hands you a clean 1099-B. In crypto you might buy on Coinbase, move to a hardware wallet, swap on a decentralized exchange, earn staking rewards, and sell on Kraken. No single party sees the chain of custody, so:

- **Cost basis** (what you paid, including fees) has to travel with the coins from wallet to wallet in *your* records.
- Since the 2025 tax year, basis must be tracked **wallet-by-wallet** (per account or address), not in one blended pool. Rev. Proc. 2024-28 gave a one-time safe harbor to allocate old basis to specific wallets; if you missed it, you still must track by wallet going forward.
- Every crypto-to-crypto swap is a sale of the first asset, and every purchase with crypto (a coffee, an NFT, gas paid in ETH) is a disposal.
- Staking, mining, airdrop, and interest income is ordinary income at fair market value when received, and that value becomes the basis of the new coins.

## Form 1099-DA: what brokers now report (as of September 2026)

| Tax year | What U.S. brokers (exchanges, custodial wallets, payment processors) report on Form 1099-DA |
|---|---|
| 2025 (forms sent early 2026) | **Gross proceeds** of sales; cost basis optional. Many exchanges missed the mid-February deadline and sent forms in March or later. |
| 2026 (forms sent early 2027) | Gross proceeds **and cost basis**, but only for "covered" assets — bought on or after Jan 1, 2026 and held at the same broker continuously. |
| Any year | Coins you *transferred in* from another exchange or your own wallet show proceeds with **no basis** — the IRS may treat unreported basis as zero, taxing the whole sale as gain unless you document it. |
| Any year | Decentralized exchanges and non-custodial wallets are outside the 1099-DA regime; you report those yourself. |

The practical consequence: the IRS will know you sold $50,000 of bitcoin. Whether they think you made $50,000 or $5,000 of profit depends on the records you kept.

## Tools compared (as of September 2026)

| Tool | Best for | Price (entry tier) | Notes |
|---|---|---|---|
| **Koinly** | All-round tax + tracking; 800+ integrations | Free tracking; ~$49/tax year for 100 transactions, higher tiers for more | Good wallet-by-wallet support; exports IRS Form 8949 and TurboTax files |
| **CoinLedger** | Simple US tax filing | ~$49/tax year for 100 transactions | Clean UI; strong exchange coverage; less depth for DeFi |
| **CoinTracker** | Coinbase/TurboTax users | ~$59 for 100 transactions; ~$199/yr premium | Official Coinbase and TurboTax partner; tracks performance |
| **CoinTracking** | Power users, long histories | ~$49/tax year for 200 transactions; unlimited ~$839/yr | Oldest tool, most accounting methods, steeper learning curve |
| **ZenLedger / TokenTax** | CPA-assisted filing | ~$49–$65+ | TokenTax offers full-service preparation at higher tiers |
| **Kubera** | Net-worth tracking across everything (stocks, real estate, crypto) | ~$150/yr | Not a tax tool; excellent for a whole-portfolio view and beneficiary access |
| **CoinStats** | Mobile portfolio tracking | Free / paid tiers | Price tracking and DeFi view; pair with a tax tool |
| **Spreadsheet** | Under ~50 transactions a year | Free | Perfectly acceptable; columns below |

Whichever tool you pick, connect it *before* you have years of history. Reconstructing 2021 DeFi activity in 2027 is where people give up and guess.

## Wallet-address tracking

Tax tools and trackers read public blockchains, so you can add your own addresses without giving them any control:

- **Bitcoin:** add the wallet's **xpub/zpub** (extended public key) so the tool sees every address the wallet generates. It cannot spend; it can see everything, so treat it as private information.
- **Ethereum/L2s/Solana:** add the public address; the tool pulls token transfers, swaps, and gas.
- Label each address (e.g., "Cold storage – Ledger", "Burner – mints") so transfers between your own wallets are recognized as **transfers, not sales**. Mislabeled internal transfers are the number-one cause of phantom gains in these tools.

## Exporting exchange history

Every exchange offers a CSV (and usually a read-only API key). Read-only keys let the tax tool pull data continuously but must be created with **no withdrawal or trade permissions**. Export:

1. Trade history (buys, sells, swaps)
2. Deposits and withdrawals (with transaction IDs)
3. Fees, rewards, staking income, interest
4. Any 1099-DA, 1099-MISC, or annual statement the exchange issues

Do this **quarterly**, not once a year: exchanges shut down (FTX, Voyager), delist regions, or limit history windows, and a closed account can mean lost records.

## The minimum spreadsheet

If you keep it yourself, one row per event:

| Date | Type (buy/sell/swap/transfer/income/spend) | Asset | Quantity | Price per unit (USD) | Fee (USD) | Venue/wallet from | Venue/wallet to | Tx hash | Cost basis of lot used | Proceeds | Gain/loss | Notes |

Use **specific identification** (choose which lot you sold) if your records support it — it lets you pick high-basis lots to reduce gains — otherwise FIFO (first in, first out) is the default. Record the method you use and keep it consistent within each wallet.

## How to actually do it

1. **Pick one tool now** (Koinly, CoinLedger, or CoinTracker for most people) and open a free account.
2. **Connect every exchange** by read-only API; upload CSVs for any that lack API support or are closed.
3. **Add every wallet address** (xpub for bitcoin, public addresses elsewhere) and label them as your own.
4. **Reconcile**: the tool's balances should match what each exchange and wallet actually holds today. Chase down every mismatch — missing deposits, unlabeled transfers, unknown tokens (airdrop spam can be marked as ignored).
5. **Set your wallet-by-wallet basis** for pre-2025 holdings per your safe-harbor allocation (if made) or a documented reasonable allocation; keep the memo.
6. **Quarterly:** export CSVs, re-sync, re-reconcile, archive the files with the tax year.
7. **At year-end:** generate Form 8949 / Schedule D output, compare the proceeds total to every 1099-DA you receive, and resolve differences before filing. Transfers-in that show zero basis on the 1099-DA must be supported by your own lot records.
8. **Keep records seven years** (some advisers say indefinitely for crypto): CSVs, tax-tool reports, transaction hashes, and screenshots of any wallet that no longer exists.
9. Coordinate with the tax section of this library for treatment of staking, NFTs, losses, and the wash-sale rule's status.

## Key takeaways

- Every sale, swap, spend, and reward is a taxable event; only you can trace basis across venues and wallets.
- Form 1099-DA reports your gross proceeds (from tax year 2025) and basis only for coins bought and held at one broker from 2026 — transfers-in show no basis.
- Wallet-by-wallet basis tracking is now mandatory; label internal transfers correctly or the tool will invent gains.
- Connect read-only APIs and public addresses to a tracker before the history gets long.
- Export exchange CSVs quarterly; closed exchanges take their records with them.
- Reconcile tool balances to real balances; unexplained gaps are future audit questions.
- Keep everything for at least seven years, including transaction hashes.

## Sources

- [Form 1099-DA: what US crypto investors need to know for 2026 (CoinTracking)](https://cointracking.info/blog/form-1099-da/)
- [Navigating the Form 1099-DA reporting maze (The Tax Adviser, Mar 2026)](https://www.thetaxadviser.com/issues/2026/mar/navigating-the-form-1099-da-reporting-maze/)
- [The coming changes to crypto compliance: Rev. Proc. 2024-28 and Form 1099-DA (Wolf & Co.)](https://www.wolfandco.com/resources/insights/coming-changes-crypto-compliance-rev-proc-2024-28-form-1099-da-reporting/)
- [10 best crypto tax software in 2026 (Koinly, Jun 2026)](https://koinly.io/blog/compare-crypto-tax-software/)
- [Koinly vs CoinTracker comparison](https://koinly.io/compare/cointracker-vs-koinly/)
- [CoinLedger vs CoinTracker (Koinly blog)](https://koinly.io/blog/coinledger-vs-cointracker/)
- [Preparing for new 1099 digital asset reporting rules (Thomson Reuters)](https://tax.thomsonreuters.com/news/preparing-for-new-1099-digital-asset-reporting-rules/)
