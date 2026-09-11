# Security and Self-Custody Setup

**In one sentence:** Self-custody means a hardware wallet bought straight from the maker, a seed phrase stamped in metal and stored in more than one place, a small test send before every large one, and — once the stakes are high — multiple keys so that no single mistake, thief, or house fire can take everything.

## The mental model

Crypto is a **bearer asset**: whoever holds the private key owns the coins, and there is no customer-service line to reverse a transaction. Every piece of this playbook exists to protect one thing — the **seed phrase** (12 or 24 words, also called a recovery phrase) that regenerates every key in your wallet. A hardware wallet's only job is to keep that seed on a chip that never touches the internet, and to show you on its own small screen what you are about to sign.

Think in tiers:

| Tier | Typical holdings | Setup |
|---|---|---|
| Spending | What you'd carry in cash | Phone/software wallet or exchange |
| Savings | Meaningful, would hurt to lose | Single hardware wallet + metal backup + passphrase (optional) |
| Life-changing | Would change your retirement | 2-of-3 multisig with geographically separated keys, collaborative custody or DIY |

## Step 1: Buy the hardware wallet correctly

Buy **only from the manufacturer's own site** (ledger.com, trezor.io, coldcard.com, foundation.xyz, etc.) or an authorized reseller they list. Never from Amazon third-party sellers, eBay, or marketplaces. In 2025 security researchers documented counterfeit "Ledger" devices sold through Chinese marketplaces at full retail price: the secure chip was swapped for a generic microcontroller with a hidden radio, and every PIN and seed was sent in plain text to the attacker's server. Over 50 victims lost more than $9.5 million. The packaging even carried a QR code to a cloned app with a fake "genuine check."

Rules:

- Pay with your own card and have it shipped to an address you control; some buyers use a PO box because vendor customer lists have leaked before.
- **Reject any device that arrives with a pre-filled seed card, a "starter" PIN, or instructions to enter your seed on a website.** A genuine device generates the seed on-screen, in front of you, the first time you set it up.
- Run the manufacturer's genuine check (Ledger Wallet app, Trezor Suite) on first connection, and download that software only from the official domain.

Reasonable choices in 2026: Ledger (broad coin support, closed-source secure element), Trezor (open source, Safe 3/5 add a secure element), Coldcard (bitcoin-only, air-gapped via microSD/QR), Foundation Passport (bitcoin-only, QR air-gap). Bitcoin-only devices remove whole classes of attack surface if you only hold bitcoin.

## Step 2: Generate and back up the seed

1. Initialize the device; let *it* generate the words. Never use a seed someone gives you, and never type the seed into a phone or computer — that includes "backup" apps and cloud notes.
2. Write the words on the included card first, then transfer them to **metal**. Stainless-steel plates (Cryptosteel, Billfodl, Coldcard's SEEDPLATE, or cheap stamped washers) survive fires and floods that destroy paper. Independent stress tests favour stamped or punched steel over engraved thin plates.
3. **Verify the backup**: most devices offer a "check backup" or dry-run recovery. Do it. A backup you have never tested is a hope, not a backup.
4. Store copies in at least **two geographically separate locations** you control — home safe plus a bank safe-deposit box or a trusted relative's safe. Do not split one seed into halves across locations (an attacker with 12 of 24 words can brute-force the rest); store *complete* copies, or use proper multisig (below).
5. Photograph nothing.

## Step 3: The passphrase ("25th word")

A passphrase (BIP-39 passphrase, sometimes marketed as a "hidden wallet") is an extra word or sentence combined with your seed to create a completely different wallet. Benefits: someone who finds your metal plate finds an empty (or decoy) wallet. Costs: it is case-sensitive, a single typo produces a different empty wallet, the device does not store it, and there is **no recovery if you forget it**. Trezor's own guidance is to write it down, store it separately from the seed, and test access regularly.

Use a passphrase if you are disciplined about documentation and understand that your heirs need it too. Skip it if you are not; a forgotten passphrase is one of the most common ways people lock themselves out permanently.

## Step 4: Multisig for large holdings

**Multisig** (multi-signature) requires M-of-N keys to spend — typically 2-of-3. One stolen or destroyed key does nothing; you still have two. This is how custodians and, increasingly, individuals hold serious sums.

| Route | How it works | Cost (Sept 2026) | Notes |
|---|---|---|---|
| **Casa** | 2-of-3 or 3-of-5; you hold phone key + hardware key(s), Casa holds one recovery key; supports BTC, ETH, USDC, USDT | ~$250/yr Standard to ~$2,100/yr Premium | Casa key can co-sign recovery but cannot spend alone |
| **Unchained** | 2-of-3; you hold two hardware keys, Unchained holds one; bitcoin only; IRA vaults available | ~$250/yr per vault; Signature concierge tier ~$4,500/yr | Your two keys can always spend without Unchained |
| **Nunchuk** | 2-of-3 up to 3-of-5 with optional Nunchuk key; timelock-based inheritance | Free DIY; ~$120–$2,100/yr for assisted tiers | Miniscript/timelocks, bitcoin only |
| **DIY with Sparrow Wallet** | Sparrow (desktop) coordinates 2-of-3 across three hardware wallets from different vendors | Hardware only (~$200–$500) | You must back up the *wallet descriptor/config* as well as each seed; losing the descriptor with one key can lock you out |

Collaborative custody's big advantage is a knowledgeable third party who can help recover after a lost key *without* being able to take your coins. DIY multisig is cheaper but the whole burden of documentation is on you.

## Step 5: Sending safely — test, verify, repeat

1. **Send a small test amount first** (a few dollars) to any new address. Confirm it arrives. Then send the rest. This single habit stops most fat-finger and wrong-network losses.
2. **Verify the receiving address on the hardware wallet's screen**, not just the computer, and check it character-by-character — first four, last four, *and* a chunk in the middle.
3. **Address poisoning** is the current mass scam: attackers generate addresses whose first and last characters match one you often use, then send you a dust transaction so the lookalike appears in your history. One victim lost ~$50 million in USDT in December 2025 by copying an address from transaction history. Never copy addresses from history or from block explorers; use your saved address book, a QR code, or paste fresh from the recipient.
4. **Clipboard malware** silently swaps a pasted address for the attacker's. Defence is the same: read the address on the device screen before approving.
5. Prefer wallets that support **address allowlisting** and reject **blind signing** (approving a transaction whose contents the device cannot display).
6. Do a **quarterly health check**: power on each device, confirm it still unlocks, confirm each metal backup is where it should be.

## What to do if you think you are compromised

1. If funds are still there and you have a clean device, **move them immediately** to a brand-new wallet with a brand-new seed generated on a trusted device. Fee cost is irrelevant.
2. Assume the old seed, the computer, and the phone are all burned. Do not reuse any of them.
3. Revoke smart-contract approvals from the compromised address (see [operational-security-and-scam-defense.md](operational-security-and-scam-defense.md)).
4. Change exchange passwords and 2FA from a clean device; enable withdrawal locks.
5. Report: FBI IC3 (ic3.gov), the exchange's security team, and the wallet vendor. Recovery is rare, but reports feed blacklists.
6. Write down what happened and when — you will need it for tax loss documentation.

## How to actually do it

1. Order the hardware wallet from the manufacturer's site. Inspect packaging; reject anything with a pre-written seed.
2. Set up on a clean computer with official software; let the device generate the seed; set a strong PIN.
3. Transfer the words to a metal backup; run the device's backup check; store complete copies in two separate locations.
4. Optional: add a passphrase; document it separately from the seed; test it.
5. Send $10 from the exchange to the wallet; confirm receipt on the device screen; then move the real amount.
6. Save the exchange withdrawal address in an allowlist; save the wallet's address in an address book.
7. When holdings cross your "life-changing" line, migrate to 2-of-3 multisig (collaborative or DIY) and record the wallet config with each backup.
8. Add the whole setup to your estate plan (see [estate-planning-for-crypto.md](estate-planning-for-crypto.md)).

## Key takeaways

- Buy hardware wallets only from the manufacturer; a pre-filled seed card means the device is a scam.
- The seed phrase is the asset; never type it into anything connected to the internet.
- Metal beats paper; two complete copies in two places beat one; test the backup.
- A passphrase adds protection and a new way to lose everything — document it or skip it.
- Test transactions and on-device address verification defeat address poisoning and clipboard malware.
- Above life-changing amounts, use 2-of-3 multisig so no single event can wipe you out.
- If compromised, move first and investigate later; the old seed is gone forever.

## Sources

- [Fake Ledger hardware wallets steal seeds and PINs (Cyber Security News, 2025)](https://cybersecuritynews.com/fake-ledger-hardware-wallets/)
- [Ledger: ongoing phishing campaigns and core rules](https://www.ledger.com/phishing-campaigns-status)
- [Trezor: passphrases and hidden wallets](https://trezor.io/learn/a/passphrases-and-hidden-wallets)
- [Bitcoin.org: Securing your wallet](https://bitcoin.org/en/secure-your-wallet)
- [Ethereum.org: Security and scam prevention](https://ethereum.org/en/security/)
- [Bitcoin collaborative custody comparison: Casa vs Unchained vs Nunchuk (Spark, 2026)](https://www.spark.money/tools/bitcoin-collaborative-custody-comparison)
- [Unchained pricing](https://www.unchained.com/pricing)
- [Unchained vs Casa comparison](https://www.unchained.com/compare/unchained-vs-casa)
- [Chainalysis: Anatomy of an address poisoning scam](https://www.chainalysis.com/blog/address-poisoning-scam/)
- [Crypto user loses $50M USDT in address poisoning scam (CoinDesk, Dec 2025)](https://www.coindesk.com/web3/2025/12/20/crypto-user-loses-usd50-million-in-address-poisoning-scam)
- [Billfodl metal backup](https://billfodl.com/products/the-billfodl)
