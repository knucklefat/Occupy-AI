# Crypto Tax Record-Keeping Checklist

**In one sentence:** What to write down for every transaction, how often to export it, why basis must now be tracked wallet-by-wallet, which tools do the work, what to do at year-end, how to reconcile the new Form 1099-DA, and a simple rule for setting aside tax money as you go.

**The core idea:** In the US (and most countries), crypto is property. Every sale, every crypto-to-crypto swap, every purchase of a coffee with bitcoin, and every reward you receive is a taxable event that you — not the exchange — are responsible for reporting. The IRS now receives broker reports (Form 1099-DA) and expects your return to match. The only way this is painless is to keep records as you go; reconstructing three years of DeFi activity in March is a nightmare that costs real money in professional fees and lost basis.

**This is a record-keeping checklist, not tax advice.** Rules differ by country and change often; the US specifics below reflect IRS guidance at the time of writing. Confirm with a professional for your situation.

---

## 1. What counts as a taxable event (so you know what to record)

**Taxable — gain or loss to calculate:**
- [ ] Selling crypto for cash (fiat).
- [ ] **Trading one crypto for another** — including stablecoins. ETH → USDC is a sale of ETH.
- [ ] **Spending** crypto on goods or services.
- [ ] Converting crypto inside a platform ("swap," "convert," "bridge" in many cases).
- [ ] Providing or withdrawing DeFi liquidity, where the position token is treated as an exchange (treatment varies; record everything).

**Taxable — ordinary income at fair market value when received:**
- [ ] Staking rewards, mining rewards, lending interest, liquidity-mining rewards.
- [ ] Airdrops (when you have control of them), hard-fork coins received.
- [ ] Payment for work or services in crypto; referral bonuses; "learn and earn" rewards.

**Not taxable (but still record):**
- [ ] Buying crypto with cash.
- [ ] **Transferring between wallets or accounts you own** (exchange → hardware wallet). Not taxable, but the *fee* may be, and you must record the transfer so your tool does not think you sold.
- [ ] Holding through price changes.
- [ ] Receiving a bona fide gift (you inherit the giver's basis in most cases); giving a gift (may require a gift-tax form above the annual exclusion).
- [ ] Donating appreciated crypto to a qualified charity (generally no gain, possible deduction).

**Form 1040 question:** every US return asks whether you received, sold, exchanged, or otherwise disposed of a digital asset during the year. Answer honestly; "just held" is the only situation where "No" applies.

---

## 2. What to record for every transaction

Your tool captures most of this automatically from exchanges; you must fill gaps for wallets, DeFi, and off-platform events.

- [ ] **Date and time** (with time zone) of the transaction.
- [ ] **Type:** buy / sell / trade / transfer / income (staking, airdrop, etc.) / spend / gift / fee.
- [ ] **Asset(s)** and **quantity** in, quantity out.
- [ ] **Fair market value in USD** at the time (for income events and for the received side of a crypto-to-crypto trade).
- [ ] **Fees** paid, in what asset, and their USD value (fees on purchases add to basis; fees on sales reduce proceeds).
- [ ] **Venue and wallet:** which exchange account or which wallet address the asset left from and arrived in. This is now essential (see section 3).
- [ ] **Transaction ID / hash** for on-chain transactions.
- [ ] **Counterparty or purpose** note for anything unusual ("paid contractor," "moved to cold storage," "Aave deposit," "NFT mint").
- [ ] **For sales:** which specific lot(s) were sold (see specific identification, section 3).
- [ ] **Cost basis** of what was disposed and the resulting gain/loss, short- or long-term (held more than one year = long-term in the US).

**Example entry:**
> 2026-05-14 09:32 ET · Trade · Sold 0.10 ETH → received 310.00 USDC · FMV $3,105.00 · fee 0.0004 ETH ($1.24) · Kraken spot account · lot sold: ETH bought 2025-02-03 @ $2,600 (basis $260.00 + $0.95 fee) · gain $48.81 · long-term.

---

## 3. Wallet-by-wallet basis (the 2025 change that trips people up)

Under the IRS regulations that took effect January 1, 2025, cost basis must be tracked **per wallet or per account**, not pooled across everything you own ("universal" method is no longer allowed).

- [ ] Every wallet address and every exchange account is set up as a **separate account** in your tax tool.
- [ ] Transfers between your own accounts are marked as **transfers**, and the tool carries the *original basis and purchase date* to the destination wallet. (A transfer is not a sale, but the units keep their history.)
- [ ] You know your **default lot method.** If you do not specifically identify which units you are selling, the IRS default is **FIFO (first in, first out) within that wallet** — usually the oldest, cheapest lots, meaning the largest gains.
- [ ] If you want to use **specific identification** (choosing which lot to sell, e.g., the highest-cost lot to minimize gain), you must identify the units **before or at the time of the sale**: at a broker, by telling the broker; in a self-custody wallet, by keeping your own contemporaneous records. Your tax tool's "HIFO" setting only counts if you actually made the identification when you sold, so decide the method in advance and document it.
- [ ] You did the **one-time allocation** of pre-2025 basis to specific wallets (the IRS allowed a transition allocation for units held on January 1, 2025). If you have not, do it now with your tool or a professional, and keep the allocation record.
- [ ] Hardware wallet, mobile wallet, DeFi wallet, burner: each added by **public address only**. A tax tool never needs your seed phrase; one that asks for it is a scam.

---

## 4. Tools and setup

- [ ] Choose one crypto tax platform (commonly used: Koinly, CoinTracker, CoinLedger, TokenTax, ZenLedger, Crypto Tax Calculator, Awaken for DeFi-heavy users). Criteria: supports every chain and exchange you use; supports per-wallet basis and specific identification; exports Form 8949; keeps history if you stop paying.
- [ ] Connect exchanges via **read-only API keys** (never keys with trade or withdraw permission), or CSV export where APIs are unavailable.
- [ ] Add every wallet by public address, on every chain you have used (including L2s, Solana, etc.).
- [ ] Reconcile the starting balances: the tool's calculated balance for each account should match the actual balance. Every mismatch is a missing transaction; find it now, not in April.
- [ ] Keep a **separate spreadsheet or note** for things tools miss: off-platform trades, gifts, lost/stolen assets, NFT mints, bridge transactions that appear as a "sale" and "buy," staking rewards on validators the tool does not read.
- [ ] Keep **your own copies** of all exchange CSV exports and statements — exchanges close, delist you, or lose history.

---

## 5. Export and review cadence

- [ ] **Monthly** (or whenever you make more than a handful of transactions): sync the tool, resolve flagged/unmatched transactions, label transfers, note the running realized gain figure.
- [ ] **Quarterly:** export a full transaction CSV from every exchange and store it in your own cloud/drive folder ("Crypto tax / 2026 / Q3 / Kraken.csv"). Check the tool's account balances against reality. Move estimated tax money (section 8).
- [ ] **Before any large sale:** confirm which lots will be sold and their holding period; identify the lot in writing (screenshot or note with date/time) if using specific identification.
- [ ] **After any DeFi activity:** immediately annotate what happened in plain English — tools misclassify DeFi constantly, and you will not remember in nine months what a "0x…a3f2 contract interaction" was.
- [ ] **Annually:** everything in section 6.

---

## 6. Year-end steps (December)

- [ ] Sync every account and resolve all flagged items so the tool shows **zero unmatched transactions**.
- [ ] Review **realized gains and losses year-to-date**, split short-term / long-term.
- [ ] **Tax-loss harvest** if useful: sell lots that are underwater to realize losses that offset gains (and up to $3,000 of ordinary income, with the remainder carried forward). Record the lots sold. At the time of writing, the wash-sale rule does not apply to crypto in the US, but legislation has been proposed repeatedly — **confirm the current rule before repurchasing immediately.**
- [ ] Consider **holding-period timing**: if a lot is close to the one-year mark and you plan to sell, waiting can move the gain from short-term (ordinary rates) to long-term (lower rates).
- [ ] Consider **donating appreciated crypto** held more than a year directly to charity (no capital gain, potential deduction) instead of selling and donating cash.
- [ ] Tally **income events** (staking, airdrops, interest) and their USD values at receipt; these go on Schedule 1 (or Schedule C if a business), not Schedule D.
- [ ] Note any **worthless or stolen** assets and gather documentation; discuss treatment with a professional (rules are specific and unfavorable for personal theft losses in many years).
- [ ] Download the tool's year-end **Form 8949 / Schedule D** export and a full-year transaction ledger. Archive both.

---

## 7. Reconciling Form 1099-DA (January–March)

Brokers (US exchanges and some other platforms) now issue **Form 1099-DA** for digital asset sales: gross proceeds for 2025 transactions onward, and **cost basis** for covered transactions from 2026 onward. Copies go to the IRS.

- [ ] Collect every 1099-DA you receive (and any 1099-MISC/NEC for rewards or income).
- [ ] **Match gross proceeds** on each 1099-DA to the sales your tool shows for that exchange for the year. Differences usually come from: transfers the exchange treated as sales, fees, timing across year-end, or transactions you failed to import.
- [ ] **Check the basis** the broker reports. It can be wrong or missing — especially for coins you transferred *in* from another wallet, where the broker has no purchase record. If the broker's basis is blank or wrong, you still report the correct basis on Form 8949 using your own records, with the appropriate adjustment code. Your records are the authority, which is why you keep them.
- [ ] Understand that the broker's default lot method (usually FIFO within that account) may differ from the identification you made; document your identification so your 8949 can reflect it.
- [ ] Report **all** dispositions, including those from self-custody wallets and DEXs that produce no 1099-DA. The IRS position is that reporting is required whether or not you received a form.
- [ ] Keep every 1099-DA with the year's archive. If a form is wrong, request a corrected one from the broker, but do not delay filing correctly on account of it.

---

## 8. Estimated-tax set-aside rule of thumb

Crypto gains are not withheld at source. If you realize meaningful gains, you may owe **quarterly estimated taxes** (US due dates roughly mid-April, mid-June, mid-September, mid-January), and underpayment penalties apply if you wait until April.

- [ ] **When you realize a gain, move a set percentage of the gain into a separate savings account the same week.** Rule of thumb:
  - **Short-term gains** (held ≤ 1 year): set aside **30–40%** (federal ordinary rates up to 37%, plus possible 3.8% net investment income tax, plus state).
  - **Long-term gains** (held > 1 year): set aside **20–25%** (federal 15–20% plus NIIT plus state).
  - **Income events** (staking, airdrops): treat like short-term — 30–40% of the USD value at receipt, even though you received tokens, not cash. Consider selling enough of the reward to cover the tax at receipt.
  - If unsure, **30% of every realized gain** is a reasonable single number for most people; residents of high-tax states or top brackets should use 40%.
- [ ] Never spend, reinvest, or "let ride" the set-aside. In 2021–22, many people owed tax on 2021 gains with portfolios that had since fallen 70%; the set-aside is what prevents that.
- [ ] Check with your tool or professional each quarter whether your year-to-date gains push you above the safe-harbor thresholds (paying at least 100–110% of last year's tax, or 90% of this year's) and make the estimated payment if so.

---

## 9. Retention

- [ ] Keep all records for **at least 7 years** after the return that used them (the IRS can look back 3 years normally, 6 for substantial under-reporting, indefinitely for no return). For basis, keep records as long as you hold the asset **plus** 7 years.
- [ ] Archive per year: exchange CSVs, wallet transaction ledgers, tax-tool exports (8949, full ledger, per-wallet basis report), 1099 forms, lot identification notes, and your plain-English DeFi annotations.
- [ ] Store in two places (local + cloud), encrypted. Public addresses and transaction records are fine to store digitally; seed phrases are never in this archive.

---

## Sources

- [IRS — Digital assets](https://www.irs.gov/businesses/small-businesses-self-employed/digital-assets) (Form 1040 question, Form 1099-DA timeline, which forms to use, record-keeping)
- [IRS — Frequently asked questions on digital asset transactions](https://www.irs.gov/individuals/international-taxpayers/frequently-asked-questions-on-digital-asset-transactions) (basis rules, per-wallet identification, FIFO default, taxable vs non-taxable events)
- [IRS — Frequently asked questions on virtual currency transactions](https://www.irs.gov/individuals/international-taxpayers/frequently-asked-questions-on-virtual-currency-transactions)
- [Kraken — Security features (read-only API keys; account statements)](https://www.kraken.com/features/security)
- Main library: [Tax and account hacks](../../08-tax-and-account-hacks/) and [Annual financial checkup checklist](../../10-checklists-and-templates/annual-financial-checkup-checklist.md)
