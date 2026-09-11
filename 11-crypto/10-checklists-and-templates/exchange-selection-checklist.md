# Exchange Selection Checklist

**In one sentence:** Twenty-four questions to ask before trusting a centralized exchange with your money — licensing, solvency proof, insurance, fees, withdrawals, account security, incident history, jurisdiction, asset segregation, and support — plus a US comparison table to fill in and verify.

**The core idea:** When you hold coins on an exchange you are an unsecured creditor of that company. FTX, Celsius, Voyager, Mt. Gox, and QuadrigaCX customers all learned that a balance on a screen is a promise, not a possession. The checklist is about finding exchanges whose promises are regulated, verifiable, and insured — and then keeping as little on them as possible anyway.

**How to use it:** Score each exchange. Any "no" in section 1 or 2 should disqualify it for anything beyond a quick on-ramp. Re-check annually; regulatory status and ownership change.

---

## 1. Licensing and legal standing (5 items)

**Why this matters:** A licensed exchange has a regulator who can inspect its books, a legal entity you can name, and (usually) capital and consumer-protection requirements. An unlicensed one has your money and a Telegram channel.

- [ ] 1. The exchange names its **legal entity and headquarters jurisdiction** clearly in its terms of service — and it is a jurisdiction with a functioning legal system you could actually pursue a claim in.
- [ ] 2. **US users:** the entity is registered with FinCEN as a Money Services Business (searchable at msb.fincen.gov) and holds **state money-transmitter licenses** for your state (look for a "licenses" page listing state license numbers, or search the NMLS Consumer Access site).
- [ ] 3. For New York residents, or as a quality signal for anyone: holds a **NYDFS BitLicense or trust charter**, widely regarded as the strictest US state regime.
- [ ] 4. **Non-US users:** registered with your national regulator (e.g., FCA in the UK, MiCA authorization in the EU, AUSTRAC in Australia, FINTRAC in Canada), not merely "registered as a company."
- [ ] 5. No current enforcement action, unresolved lawsuit about customer funds, or regulator warning against the entity you would be contracting with. (Search "[exchange] SEC," "[exchange] CFTC," "[exchange] consent order.")

## 2. Solvency and custody of customer assets (5 items)

**Why this matters:** The failures that hurt customers most were not hacks; they were exchanges secretly lending out or losing customer deposits. You want proof the coins exist and a legal structure that keeps them yours if the company fails.

- [ ] 6. Publishes **proof of reserves** (PoR): a cryptographic snapshot in which an independent auditor confirms on-chain holdings at least equal the sum of customer balances, typically via a Merkle tree so you can verify your own balance is included. Ask: how recent, how frequent, which assets, which auditor.
- [ ] 7. You understand what PoR **does not** prove: that keys are not shared or duplicated, that assets were not borrowed for the snapshot, or that nothing has happened since. Treat it as necessary, not sufficient.
- [ ] 8. **Liabilities are covered too:** either the PoR includes a liabilities attestation, or the company is public / files audited financial statements you can read.
- [ ] 9. **Customer-asset segregation:** the terms of service say customer crypto is held in trust or otherwise segregated from corporate assets, and is not lent, rehypothecated, or used for the company's own trading unless you opt in. Read the custody clause; if it says your assets may be "used," that is a loan you are making.
- [ ] 10. The bulk of customer crypto is stated to be in **cold storage** (offline keys), with hot-wallet balances kept to operating needs.

## 3. Insurance and loss history (3 items)

**Why this matters:** "Insured" in exchange marketing usually means the exchange's *hot wallet* against *their* breach — not your account against phishing, not cold storage, and not insolvency. Read the fine print.

- [ ] 11. Insurance coverage is described specifically: what is covered (hot wallet theft? cash balances via pass-through FDIC at partner banks?), the policy limit, and what is excluded (your credentials being compromised is almost always excluded).
- [ ] 12. **Incident history:** search "[exchange] hack," "[exchange] breach," "[exchange] outage." A past incident is not disqualifying; how it was handled is. Were customers reimbursed in full and promptly? Was the disclosure honest?
- [ ] 13. Operates a public **bug bounty** and holds recognized security certifications (e.g., SOC 2, ISO 27001).

## 4. Account security features (5 items)

**Why this matters:** Most individual losses on reputable exchanges come from account takeover — SIM swaps, phishing, credential stuffing — not from the exchange being hacked. The exchange's security toolbox is your toolbox.

- [ ] 14. Supports **hardware security keys / passkeys (FIDO2)** for login 2FA, or at minimum authenticator apps. Any exchange that only offers **SMS 2FA** is a hard no.
- [ ] 15. Lets you **remove your phone number** as a recovery factor once stronger 2FA is set up.
- [ ] 16. Supports **withdrawal address allowlisting** (only pre-approved addresses can receive withdrawals, with a delay to add new ones), plus email/2FA confirmation on every withdrawal.
- [ ] 17. Offers a **settings lock / time-lock** or "vault" feature that delays sensitive changes and large withdrawals by 24–72 hours.
- [ ] 18. Provides login and withdrawal alerts, session management (see and kill active sessions), and anti-phishing codes in emails.

## 5. Fees, limits, and practicalities (4 items)

**Why this matters:** Fees compound just like returns. A 1.5% "convenience" spread on every recurring buy over ten years is a large drag, and hidden withdrawal fees can trap small balances.

- [ ] 19. You know the **all-in cost of a buy**: trading fee *plus* spread (the gap between the price you pay and the mid-market price). Check by comparing the quoted price with a price site at the same moment. Prefer the exchange's "advanced" or "pro" interface if it exists — often much cheaper than the simple buy button.
- [ ] 20. **Withdrawal fees and limits** are published, reasonable, and support the network you need. Some exchanges charge a flat fee that makes small withdrawals uneconomical; some cap daily withdrawals low until you pass extra verification.
- [ ] 21. **Deposit holds** are understood: how long after a bank deposit before you can withdraw crypto? (Multi-day holds are normal; multi-week is a warning.)
- [ ] 22. Supports the **on-ramp method you actually use** (ACH, wire, debit) at an acceptable cost, and — for later — offers **tax exports** (CSV and/or read-only API) and, for US users, issues Form 1099-DA.

## 6. Support and reputation (2 items)

**Why this matters:** You will need support exactly once — when something has gone wrong and the clock is running. That is the wrong time to discover it is a chatbot.

- [ ] 23. Support is reachable by a human through an official channel with a published response time. Confirm the official support URL and note it: scammers impersonating exchange support are one of the most common frauds. **No exchange will ever DM you first on Telegram, X, or Discord.**
- [ ] 24. Reputation check: recent reviews on independent sites, the exchange's subreddit or forum, and any pattern of "account frozen with no explanation" complaints. Every exchange has some; a flood in the last three months is a signal.

---

## Fill-in scorecard

| Exchange | Sec 1 (of 5) | Sec 2 (of 5) | Sec 3 (of 3) | Sec 4 (of 5) | Sec 5 (of 4) | Sec 6 (of 2) | Total (of 24) | Decision |
|---|---|---|---|---|---|---|---|---|
| ______ | | | | | | | | |
| ______ | | | | | | | | |

**Suggested thresholds:** 20+ = suitable as primary on-ramp and short-term holding; 15–19 = on-ramp only, sweep to self-custody promptly; below 15 or any zero in sections 1–2 = do not use.

---

## US exchange comparison table (starting point — verify before relying on it)

The table below is a *template with typical answers* as of the time of writing. Regulatory status, PoR practices, fees, and features change frequently. **Confirm each cell on the exchange's own site before using it to decide anything.** Empty cells are deliberately left for you to fill in.

| Criterion | Coinbase | Kraken | Gemini | Fidelity Crypto | Robinhood Crypto |
|---|---|---|---|---|---|
| US legal entity / public company? | Yes; publicly traded (audited financials) | Yes; check current listing status | Yes; check current listing status | Subsidiary of Fidelity; custody via Fidelity Digital Assets | Yes; publicly traded (parent) |
| FinCEN MSB + state MTLs? | Yes (verify your state) | Yes (verify your state) | Yes (verify your state) | Verify | Yes (verify your state) |
| NYDFS BitLicense / trust charter? | BitLicense | Verify current NY status | NY limited-purpose trust | NY trust (FDA) | BitLicense |
| Proof of reserves published? | Relies on public-company audits rather than Merkle PoR; verify | Periodic Merkle-tree PoR with independent auditor; you can verify your own balance | Verify | No Merkle PoR; verify custody disclosures | Verify |
| Customer asset segregation stated? | Verify terms (custody clause) | Verify terms | Verify terms | Verify terms | Verify terms |
| Hardware-key / passkey 2FA? | Yes | Yes (FIDO2 / passkeys) | Yes | Fidelity login security; verify | Verify |
| Withdrawal allowlisting? | Yes | Yes (new addresses need email confirmation; settings lock available) | Yes | Withdrawals limited; verify | Verify |
| Time-lock / vault feature? | Vault (delayed withdrawal) | Global settings lock | Verify | N/A | N/A |
| Withdraw coins to self-custody? | Yes | Yes | Yes | Limited; verify current policy | Yes (Robinhood Wallet); verify |
| Coins supported | Broad | Broad | Moderate | Very few (BTC, ETH, and a few others) | Moderate |
| Typical all-in fee, simple buy | ~1–2% incl. spread; lower on Advanced | Lower on Pro; simple buy has spread | Lower on ActiveTrader | ~1% spread | "Commission-free" but spread applies |
| Tax export / 1099-DA | CSV + API; 1099-DA | CSV + API; 1099-DA | CSV; 1099-DA | Integrated with Fidelity tax docs | 1099-DA |
| Notable incidents | Verify recent | Verify recent | Verify recent | Verify recent | Verify recent |
| Your score (of 24) | | | | | |

**Reading the table:** For someone who only wants bitcoin or ether inside an existing brokerage relationship, a brokerage-integrated option may be simplest. For someone who wants to withdraw to self-custody and use a broad set of assets, the dedicated exchanges with strong 2FA, allowlisting, and PoR are the standard choice. In every case the correct amount to *leave* on the exchange long-term is close to zero.

---

## Sources

- [Kraken — Proof of reserves](https://www.kraken.com/proof-of-reserves) (how Merkle-tree PoR works, what it does and does not prove)
- [Kraken — Security features](https://www.kraken.com/features/security) (FIDO2/passkeys, settings lock, withdrawal confirmations, SOC 2 / ISO 27001)
- [Kraken — Most secure crypto exchange](https://www.kraken.com/learn/most-secure-crypto-exchange)
- [Coinbase — How to keep your crypto secure](https://www.coinbase.com/learn/crypto-basics/how-to-secure-crypto) (2FA hierarchy, SIM swap, support impersonation)
- [Coinbase — A guide to Coinbase account security](https://www.coinbase.com/blog/a-guide-to-coinbase-account-security)
- [FinCEN — MSB registrant search](https://www.fincen.gov/msb-state-selector)
- [FTC — What to know about cryptocurrency and scams](https://consumer.ftc.gov/articles/what-know-about-cryptocurrency-scams)
- [IRS — Digital assets (Form 1099-DA reporting timeline)](https://www.irs.gov/businesses/small-businesses-self-employed/digital-assets)
