# Getting Started in Crypto Safely: A 30-Day Plan

**In one sentence:** A week-by-week sequence that takes you from "I know nothing" to a small, deliberately-sized, properly-secured crypto position with written rules and tax tracking already in place — before you have any real money at risk.

**Why the order matters:** Almost every expensive crypto mistake comes from doing the steps out of order — buying before deciding how much, holding on an exchange before learning about custody, setting up a hardware wallet after the balance is already large, or discovering taxes in April. This plan front-loads the boring parts so the exciting part (buying) happens last and small.

**Ground rule for the whole month:** Nothing you do in these 30 days should involve more than an amount you could lose entirely without it changing your life. The first buy is a rehearsal, not a position.

---

## Week 1 — Education and the allocation decision

**Goal:** Understand what you would be buying, and decide *before looking at prices* how much of your net worth is allowed to be in crypto.

- [ ] Read the foundations section of this library: [../01-foundations/how-blockchains-work.md](../01-foundations/how-blockchains-work.md). You should be able to explain, in plain words, what a private key is, what a seed phrase is, and why "not your keys, not your coins" is a real thing rather than a slogan.
- [ ] Learn the three ways to get exposure and the trade-offs of each:
  - **Spot ETF in a brokerage account** (e.g., a bitcoin or ether ETF): easiest, fits inside an IRA, no custody burden, but you hold a fund share, not the coin, and you pay an expense ratio. You cannot move it on-chain.
  - **Buying on a centralized exchange and leaving it there:** simple, but you are trusting the exchange's solvency and security (see [exchange-selection-checklist.md](exchange-selection-checklist.md)).
  - **Self-custody (hardware wallet):** you hold the keys; nobody can freeze or lose your coins but you; also nobody can help you if you lose the seed phrase.
- [ ] Decide your **maximum crypto allocation** as a percentage of investable assets. Use the volatility-based sizing method in [../../03-techniques/position-sizing-and-risk-management.md](../../03-techniques/position-sizing-and-risk-management.md) and the formula in [crypto-formulas-and-rules-of-thumb.md](crypto-formulas-and-rules-of-thumb.md). For most people the honest answer is 1–5%; write down the number and the reason.
- [ ] Do the "worst-case" test: multiply your planned allocation by 0.2 (an 80% drawdown, which bitcoin has done more than once). If that loss would change your retirement date, housing, or sleep, cut the allocation.
- [ ] Confirm the prerequisites are in place: emergency fund funded, high-interest debt gone, retirement accounts being funded. Crypto comes *after* these, never instead of them.
- [ ] Read [scam-red-flags-checklist.md](scam-red-flags-checklist.md) once now. You will be targeted the moment you join any crypto community; the tells are easier to spot when you have seen the list first.

**Output of Week 1:** One sentence — "I will hold no more than __% of investable assets in crypto, via [ETF / exchange / self-custody], because ___."

---

## Week 2 — Choose the exposure type and secure the accounts

**Goal:** Pick your on-ramp, open the accounts, and lock them down *before* any money arrives.

- [ ] **Choose your exposure type** using the Week 1 decision. If you chose ETF-only, open or use an existing brokerage account and skip to Week 4's rules-writing step; you can ignore the wallet steps.
- [ ] If buying real coins, **choose one exchange** using [exchange-selection-checklist.md](exchange-selection-checklist.md). One is enough to start; more accounts means more attack surface and more tax exports.
- [ ] Create a **dedicated email address** used only for crypto accounts. Never reuse it for social media or shopping, and never mention it publicly. This alone defeats a large share of phishing.
- [ ] Set a **unique 16+ character password** generated and stored by a password manager. Do not reuse any password from anywhere else.
- [ ] Enable **two-factor authentication (2FA)** — the extra code or key required to log in — using a **hardware security key** (FIDO2/passkey, e.g., a YubiKey) if the exchange supports it, or an **authenticator app** if not. **Never SMS 2FA**: attackers can take over your phone number through the carrier ("SIM swap") and receive your codes.
- [ ] Remove your phone number as a recovery method wherever the platform allows.
- [ ] Turn on every extra lock the exchange offers: withdrawal address allowlisting (only pre-approved addresses can receive withdrawals), withdrawal email confirmations, a settings time-lock, login alerts.
- [ ] Complete identity verification (KYC) now, not later. Verification delays during a market panic are a classic way to get stuck.
- [ ] Bookmark the exchange's real URL and only ever log in from the bookmark or the official app. Never from a search result or a link in a message.
- [ ] Tell nobody online that you are getting into crypto. Being known as a holder makes you a target.

**Output of Week 2:** A funded-with-$0 exchange account that is already harder to break into than your bank account.

---

## Week 3 — The first small buy and the hardware wallet rehearsal

**Goal:** Do one complete round trip — buy, withdraw to your own wallet, send back a small test — with an amount you would not miss.

- [ ] **Link a bank account** and make a small deposit. Note that many exchanges hold new deposits for several days before allowing withdrawal; this is normal.
- [ ] **First buy:** a small amount (think $50–$200) of bitcoin or ether — the two largest, most liquid, most scrutinized assets. Do not buy anything else this month. Log the date, amount, price, and fee; this is your first tax lot (see [tax-record-keeping-checklist.md](tax-record-keeping-checklist.md)).
- [ ] **Buy a hardware wallet directly from the manufacturer** (Ledger, Trezor, Coldcard, BitBox, etc.) — never from a marketplace reseller, and never a "pre-configured" device with a seed already written out. Ship to a name/address you are comfortable having on a crypto vendor's customer list.
- [ ] **Set it up** following [self-custody-security-checklist.md](self-custody-security-checklist.md): check packaging, verify firmware is genuine through the official app, generate a new seed on the device, write the words down by hand.
- [ ] **Test the recovery** before any meaningful money is on it: wipe the device, restore from your written words, and confirm the same receive address appears. If you skip this step you have not backed anything up — you have only written some words on paper.
- [ ] **Test transaction:** withdraw a small portion (say $20 of your buy) from the exchange to the hardware wallet. Verify the receive address on the device screen, not just the computer screen. Wait for confirmation. Then send a small amount *back* to the exchange to prove you can move funds in both directions.
- [ ] Decide on a **passphrase** ("25th word") only if you understand it creates a completely separate wallet and a lost passphrase means lost funds. Most beginners should skip it for now and revisit at a higher balance.
- [ ] Put the seed backup in a location that is not the same room as the device, and plan a second copy (metal, second location) before the balance grows.

**Output of Week 3:** You have proven, with real money, that you can buy, withdraw, recover, and send. Most people who lose crypto to custody mistakes never did this rehearsal.

---

## Week 4 — Automate, write the rules, set up tax tracking

**Goal:** Turn a one-time purchase into a boring, rule-driven process you can follow for years.

- [ ] **Set up dollar-cost averaging (DCA)** — a fixed dollar purchase on a fixed schedule (weekly or monthly) regardless of price. Most exchanges support recurring buys. Size it so that at your target allocation it takes 6–12 months to get there; you are not in a hurry.
- [ ] Decide your **exchange-to-cold-storage sweep rule**, e.g., "whenever the exchange balance exceeds $X or every quarter, whichever comes first, withdraw to the hardware wallet." Write it down.
- [ ] **Write your crypto investment policy statement** using [crypto-investment-policy-statement-template.md](crypto-investment-policy-statement-template.md). Include: max allocation, rebalance bands, what you will do in a crash, what you will *never* do (leverage, lending your coins for yield, signing contracts you do not understand).
- [ ] **Set up tax tracking now**, while there are three transactions to enter instead of three hundred. Pick a crypto tax tool, connect the exchange via read-only API or CSV, and add your hardware wallet's public address (never the seed). Follow [tax-record-keeping-checklist.md](tax-record-keeping-checklist.md).
- [ ] Open a separate savings sub-account labeled "crypto tax set-aside" and adopt the rule of thumb: when you realize a gain, move roughly 30% of it into that account the same week.
- [ ] Put a **quarterly review** on your calendar: check allocation vs. target, rebalance if outside bands, sweep exchange balance to cold storage, export transactions, confirm the seed backup is where it should be.
- [ ] Put an **annual review** on the calendar: re-read the IPS, re-test the hardware wallet recovery, update firmware, check that heirs know how to access funds.
- [ ] Re-read [crypto-crash-playbook.md](crypto-crash-playbook.md) once so you have already met the plan you will follow when prices fall 50%.

**Output of Week 4:** A written policy, an automated buy, a tax file with every transaction so far, and a calendar that will nag you so your emotions do not have to.

---

## What you should now be able to say

- I know exactly how much of my money is allowed in crypto and why.
- I know which type of exposure I chose and what I gave up by choosing it.
- My exchange account uses a unique email, a unique password, and non-SMS 2FA.
- I have restored a hardware wallet from its seed and moved coins in both directions.
- I have a written rule for when I buy, when I sell, when I sweep to cold storage, and what I will do in a crash.
- Every transaction I have made is recorded with date, amount, price, and fee.

If any of those sentences is false, that is next week's task.

---

## Sources

- [Ledger Academy — Security tips for hardware wallets](https://www.ledger.com/academy/hardwarewallet/best-practices-when-using-a-hardware-wallet)
- [Ledger Academy — How to keep your seed phrase secure](https://www.ledger.com/academy/hardwarewallet/best-ways-to-protect-your-recovery-phrase)
- [Trezor — What is a passphrase?](https://trezor.io/guides/backups-recovery/advanced-wallets/what-is-a-passphrase)
- [Coinbase — How to keep your crypto secure](https://www.coinbase.com/learn/crypto-basics/how-to-secure-crypto)
- [Kraken — Security features](https://www.kraken.com/features/security)
- [Bitcoin.org — Securing your wallet](https://bitcoin.org/en/secure-your-wallet)
- [FTC — What to know about cryptocurrency and scams](https://consumer.ftc.gov/articles/what-know-about-cryptocurrency-scams)
- [IRS — Digital assets](https://www.irs.gov/businesses/small-businesses-self-employed/digital-assets)
