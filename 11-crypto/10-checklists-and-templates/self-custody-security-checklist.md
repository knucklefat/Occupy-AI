# Self-Custody Security Checklist

**In one sentence:** The full sequence for holding your own keys safely — buying and verifying a hardware wallet, backing up the seed so that neither fire nor a single burglar can destroy it, deciding on a passphrase and multisig, proving the backup works, and the short list of things you must never do.

**The core idea:** A hardware wallet keeps your private key on a device that never touches the internet, and signs transactions inside itself. Your **seed phrase** (12 or 24 words, also called a recovery phrase) is the master backup from which every key is derived. Whoever has the words has the coins. Whoever loses the words and the device has nothing. Every item below exists to serve those two facts.

**Tiers:** Do the **Base** items for any amount. Add **Serious** items once the balance is more than you could comfortably lose. Add **Vault** items when the balance is life-changing.

---

## 1. Buying the device (Base)

- [ ] Buy **directly from the manufacturer's website** (Ledger, Trezor, Coldcard, BitBox, Keystone, etc.). Not from Amazon third-party sellers, eBay, or a "friend." Tampered and pre-seeded devices are a known attack.
- [ ] Ship to an address you accept being on a crypto vendor's customer list (vendor breaches have leaked customer addresses and led to phishing and, rarely, physical threats). A P.O. box or work address is reasonable.
- [ ] On arrival, inspect the packaging and device for tampering. Note that tamper-evident seals are not the main defense; the firmware check below is.
- [ ] **Never use a device that arrives with a seed phrase already written on a card.** Genuine devices generate the seed on first boot; a pre-filled card means someone else has your keys.

## 2. Setup and firmware (Base)

- [ ] Install the manufacturer's companion app **from the official site only** (type the URL yourself; bookmark it). Fake wallet apps in app stores and search ads are common.
- [ ] Let the app **verify the device is genuine** (Ledger's genuine check, Trezor's firmware signature check, Coldcard's anti-phishing words). Do not proceed if this fails.
- [ ] Update to the current firmware before generating a seed, then confirm the version matches the release notes on the official site.
- [ ] **Generate a new seed on the device.** Do not import a seed you generated in software, and do not let any app "help" by generating it for you.
- [ ] Set a PIN that is not your birthday, phone number, or the PIN on your phone. On devices with a wipe-after-N-attempts setting, leave it on.
- [ ] Write the seed words **by hand, in order, on the supplied card or paper**, with the word number next to each word. Double-check spelling against the on-device display.

## 3. Seed backup (Base → Serious)

- [ ] **Base:** the paper backup is stored somewhere other than the same room as the device, away from water and casual visitors.
- [ ] **Serious:** stamp or engrave the seed on a **metal backup** (stainless plates, punch kits, or capsule-style products) so it survives fire and flood. Paper is a temporary backup, not a permanent one.
- [ ] **Serious:** keep **two copies in two different locations** (home safe + bank safe-deposit box, or home + trusted family member's safe). One location means one fire, one burglary, or one eviction ends it.
- [ ] Never store the seed digitally: no photo, no cloud note, no password manager entry, no email draft, no "encrypted" text file. Any device with a camera or a network is off limits.
- [ ] Never store the seed with the device. A thief who gets both gets everything.
- [ ] Do not split a single seed across locations "for safety" unless you are using a real threshold scheme (SSS/Shamir, or multisig). Splitting 24 words into two halves makes each half dangerously easy to brute-force and makes losing one half fatal.
- [ ] Write down, separately from the seed, the **derivation path and wallet software** used (e.g., "BIP84 native segwit, m/84'/0'/0', created in Sparrow"). Recovering a seed into the wrong wallet type shows a zero balance and causes panic.

## 4. The passphrase decision (Serious)

A **passphrase** (sometimes called the "25th word") is extra text you type in addition to the seed. Every different passphrase opens a completely different, empty wallet from the same seed. It protects you if the seed is found, and it enables a "decoy" wallet with a small balance under duress.

- [ ] Decide deliberately. Benefits: seed-theft protection, duress wallet. Costs: it cannot be changed or recovered; a single-character typo or a forgotten word means the funds are gone; it must be typed every time.
- [ ] If you use one: make it long and unique, back it up **on metal, stored separately from the seed** (seed and passphrase together in one place defeats the purpose), and make sure your heirs' instructions include it.
- [ ] Test it immediately: enter the passphrase, note the receive address, wipe, restore, re-enter the passphrase, confirm the *same* address. A different address means you typed something different.
- [ ] If you are unsure, **skip the passphrase for now** and revisit at a higher balance. More people lose funds to a lost passphrase than to a stolen seed.

## 5. Prove it works: recovery and transaction tests (Base)

- [ ] **Recovery test:** before any meaningful balance, wipe the device (or use a second device) and restore from your written words. Confirm the first receive address matches the one you saw before wiping. Do this again after making a metal backup — from the metal, not the paper.
- [ ] **Small test send in:** withdraw a small amount from the exchange to the wallet. Wait for confirmation.
- [ ] **Small test send out:** send a small amount back to the exchange. You now know both directions work and how fees and confirmation times feel.
- [ ] Only after both tests succeed, move the real balance — ideally in a few tranches rather than one transaction.

## 6. Address verification on every transaction (Base)

- [ ] **Receiving:** always confirm the receive address on the **hardware wallet's own screen** matches what the computer shows before sharing or using it. Malware that swaps addresses in the clipboard is common.
- [ ] **Sending:** read the destination address and amount on the device screen before approving. Check the first 6 and last 6 characters at minimum; check the whole thing for large amounts.
- [ ] Beware "address poisoning": attackers send dust from an address whose first and last characters match one you have used, hoping you copy it from your history. Never copy addresses from transaction history; use the saved contact or the source app.
- [ ] Use the wallet's contact/allowlist feature for addresses you send to repeatedly.
- [ ] Do not "blind sign." If the device shows only a hash and cannot display what the transaction does, stop. Prefer wallets and apps that support clear-signing (human-readable transaction details on the device).

## 7. Multisig (Vault)

**Multisig** means spending requires M of N separate keys (e.g., 2-of-3). No single stolen or lost key loses the funds.

- [ ] Choose a threshold. **2-of-3** suits most individuals: one key lost is fine, one key stolen is fine, and there are only three devices and three backups to manage. **3-of-5** adds fault tolerance at the cost of more items to secure; it suits larger balances or shared/organizational custody.
- [ ] Use **different hardware wallet brands** for different keys so a firmware bug in one model cannot compromise a quorum.
- [ ] **Never keep a quorum of keys in one place**, even temporarily. Typical layout: one key at home, one at a bank box, one with a trusted party or a collaborative-custody provider (Casa, Unchained, Nunchuk, etc.).
- [ ] Back up the **wallet descriptor / output descriptor** (the file that lists all the public keys and the M-of-N configuration) with every key. Without it, seeds alone may not be enough to recover.
- [ ] Do a full recovery test of the multisig in the coordinator software (Sparrow, Nunchuk, Casa app, etc.) before funding.
- [ ] Schedule a **health check every 6 months**: confirm each device powers on, signs, and that backups are where they should be.

## 8. Approvals and DeFi exposure (Serious)

- [ ] The hardware wallet that holds your long-term balance is your **vault**: it never connects to a DeFi app, never signs a token approval, never mints an NFT. Use a separate hot or "burner" wallet for that (see [defi-protocol-safety-checklist.md](defi-protocol-safety-checklist.md)).
- [ ] For any wallet that has ever interacted with a smart contract, review and **revoke unused token approvals** (permissions you gave a contract to move your tokens) every quarter using a tool like revoke.cash or the block explorer's approval checker.
- [ ] Never sign a message or transaction you do not understand, especially "permit," "setApprovalForAll," or anything a website prompts unexpectedly.

## 9. Device and environment hygiene (Base)

- [ ] Dedicated computer or at least a dedicated browser profile for crypto, with no random extensions installed. Browser extensions are a frequent theft vector.
- [ ] Operating system and companion app kept updated; hardware wallet firmware updated *after* you have confirmed your seed backup works (a bad update with no backup is a wipe).
- [ ] Phone and computer locked with strong credentials; no crypto apps on a phone that also runs untrusted apps or has an old OS.
- [ ] A separate email address for crypto; a password manager for everything; hardware-key or app-based 2FA everywhere (never SMS).
- [ ] Do not discuss your holdings in public, on social media, or with strangers. Wrench attacks (physical coercion) start with knowing who to target.
- [ ] Keep the device itself somewhere unremarkable. It does not need a safe; the seed does.

## 10. Inheritance and emergencies (Serious)

- [ ] Write a plain-language **access letter** for your heirs: where the devices and seeds are, what a passphrase is and where it is stored, which software to use, who can help (a named trustworthy person, or a provider). Keep it with your will, not with the seed.
- [ ] Do not put the seed in the will itself — wills become public documents in probate.
- [ ] Walk one trusted person through a recovery test with a test wallet so they have done it once.
- [ ] Review the letter annually and whenever you change any device, threshold, or location.

## 11. What never to do

- **Never** type your seed into any website, app, or "verification" form. No legitimate company, wallet, or support agent will ever ask for it — a request for the seed *is* the scam.
- **Never** photograph, screenshot, or cloud-store the seed or passphrase.
- **Never** buy a hardware wallet from a reseller or accept one as a gift from a stranger.
- **Never** install a wallet app from a link in a message, an ad, or a search result.
- **Never** approve a transaction whose details you cannot read on the device screen.
- **Never** keep the only copy of anything.
- **Never** connect your vault wallet to a DeFi site, airdrop claim, or NFT mint.
- **Never** tell anyone online how much you hold.
- **Never** move a large balance without a recent, tested backup.

---

## Sources

- [Ledger Academy — Security tips for hardware wallets](https://www.ledger.com/academy/hardwarewallet/best-practices-when-using-a-hardware-wallet)
- [Ledger Academy — How to keep your seed phrase secure](https://www.ledger.com/academy/hardwarewallet/best-ways-to-protect-your-recovery-phrase)
- [Ledger Academy — Passphrase: an advanced security feature](https://www.ledger.com/academy/passphrase-an-advanced-security-feature)
- [Ledger Academy — Token approvals explained](https://www.ledger.com/academy/topics/security/ethereum-token-approvals-explained)
- [Trezor — What is a passphrase?](https://trezor.io/guides/backups-recovery/advanced-wallets/what-is-a-passphrase)
- [Trezor — Multisig wallets](https://trezor.io/learn/supported-assets/bitcoin/multisig-wallets-how-multi-key-security-protects-your-bitcoin)
- [Casa — Key distribution tips for multisig vaults](https://blog.casa.io/vault-key-distribution/)
- [Unchained — 2-of-3 vs 3-of-5 multisig](https://www.unchained.com/blog/bitcoin-multisig-2-of-3-vs-3-of-5)
- [Bitcoin.org — Securing your wallet](https://bitcoin.org/en/secure-your-wallet)
- [Revoke.cash — What are token approvals?](https://revoke.cash/learn/approvals/what-are-token-approvals)
