# Estate Planning for Crypto

**In one sentence:** If you die with your keys and no plan, your coins are gone as surely as if you had burned them — the fix is a written letter of instruction kept outside the will, a way for a trusted person to reach the keys without holding them today, and a dry run to prove it works.

## The "dying with your keys" problem

Self-custody has no forgot-password link. Estimates of permanently lost bitcoin — from early miners, crashed drives, and holders who died without telling anyone — run into the millions of coins, and the pattern repeats at household scale every week: a spouse finds a hardware wallet and a PIN-locked phone and no idea what either means. Even with exchange accounts, an executor needs to know the accounts exist; exchanges do not go looking for heirs.

Three separate things must survive you:

1. **Knowledge** that the assets exist and where (exchanges, wallets, ETFs, IRAs).
2. **Access** — the seed phrases, passphrases, PINs, multisig configurations, and device locations.
3. **Authority** — the legal right of an executor or trustee to take control, and instructions on who gets what.

Most plans fail at 2. A few fail at 1. Almost none fail at 3, because wills are good at authority and terrible at secrets.

## Why not to put seed phrases in a will

A will becomes a **public court record** when it enters probate. Anyone can read it. A seed phrase in a will is a seed phrase published to the world — and a will is typically drafted years before death and photocopied to lawyers, witnesses, and family. Trusts are private but are still read by multiple people and stored in law-firm systems that get breached.

Rule: the will and trust say **who** inherits and **that** crypto exists; a separate, secured document says **how** to access it.

## The letter of instruction

A **letter of instruction** is a plain-language, non-binding document kept with your important papers (or with the metal backups themselves) that tells a technically ordinary person what to do. Contents:

| Section | What to include |
|---|---|
| Inventory | Every exchange account (name, email used, approximate value), every wallet (type, where the device is), ETFs/IRAs at brokerages, any collaborative-custody provider |
| Access map | Where each seed backup is stored (not the words themselves unless the letter is itself in a safe), which backup pairs with which device, any passphrase and where *it* is stored, PINs, the multisig config/descriptor file location |
| Step-by-step | "Take the Ledger from the safe. Install the app from ledger.com only. Enter the PIN written on card B. To move funds, contact [named helper]." Written for someone who has never used crypto |
| Who to call | A trusted technical friend, the custody provider's inheritance line, your estate attorney, your CPA (with the tax-tool login for basis records) |
| Warnings | "Nobody legitimate will ever ask for the 24 words. Do not pay anyone claiming to recover funds. Do not type words into a website." |
| Wishes | Sell vs. hold, who receives what, in what proportions — cross-referenced to the will/trust |

Update it yearly and after any change in wallets, devices, or custody. Date each version.

## Inheritance protocols that actually work

| Approach | How it works | Who holds what today | Cost (Sept 2026) |
|---|---|---|---|
| **Casa Inheritance** | You name a recipient in the app. After your death they request access; Casa notifies you repeatedly; if you do not deny the request within 6 months, Casa co-signs with the recipient's key to unlock the vault. Supports BTC, ETH, USDC, USDT. No death certificate required. | You: 2 or 4 keys; Casa: 1 recovery key; recipient: their own Casa key | Included in plans from ~$250/yr to ~$2,100/yr |
| **Unchained Inheritance Protocol** | 2-of-3 multisig where you hold two keys and Unchained holds one. You complete inheritance documents; on death, your executor locates one of your keys and follows the protocol with Unchained's concierge. Your two keys can spend without Unchained at all. Transfer-on-death vaults and trust vaults can bypass probate. Bitcoin only. | You: 2 keys; Unchained: 1 | ~$250/yr per vault; Signature concierge tier ~$4,500/yr |
| **Nunchuk (timelock inheritance)** | Uses bitcoin timelocks: the beneficiary's key cannot spend until a date you set (1–2 years out); you refresh the timelock each year. If you stop refreshing, the beneficiary's key becomes valid automatically — no company needed. | You: keys; beneficiary: a key that "activates" on expiry | Free DIY to ~$2,100/yr assisted |
| **DIY multisig with a trusted party** | 2-of-3 with one key held by a lawyer, sibling, or adult child in a sealed envelope, plus your two. They cannot spend alone; with your documented second key after death, they can. | You: 2; trusted party: 1 | Hardware cost only |
| **Single-sig + sealed seed** | Seed in a bank safe-deposit box; executor gets access through probate. Simple but the box may be sealed for weeks, and anyone with box access has everything. | You (and whoever can open the box) | Box rental |
| **Exchange / ETF only** | Beneficiary designations (where offered), or the estate claims the account with a death certificate and letters testamentary. No keys to manage; still needs the inventory. | Custodian | Nothing extra |

Multisig with a trusted party is the pattern that solves the core tension: the helper can *assist* recovery but cannot *steal* while you are alive.

## What executors need

- **Legal authority**: a will or trust with a **digital-assets clause** granting the fiduciary power over digital property and online accounts. Nearly every U.S. state has adopted RUFADAA (Revised Uniform Fiduciary Access to Digital Assets Act), but exchanges still demand explicit authority plus a death certificate.
- **The inventory and letter of instruction** — location known to the executor in advance.
- **A technical helper** named in the letter, ideally someone who has practiced the recovery with you.
- **Tax records**: the cost basis of every lot (your tracker login), because heirs generally receive a **stepped-up basis** to the date-of-death value — but they need documentation of that value, and the estate may need the original basis for the final return.
- **Time**: they should not rush. Coins are not going anywhere; scammers who contact grieving families are.

## How to actually do it

1. **Inventory** every account and wallet in a single document; store it encrypted and in a sealed physical copy with your estate papers.
2. **Add a digital-assets clause** to your will or trust (any estate attorney can do this) naming an executor and, if you like, a separate "digital executor."
3. **Choose an inheritance protocol** from the table matching your holdings: under a few thousand dollars, exchange beneficiary designation plus the letter is enough; life-changing amounts justify collaborative custody or DIY multisig.
4. **Write the letter of instruction** for a non-technical reader; keep it *out* of the will; store copies with the seed backups and with the executor's sealed envelope.
5. **Split knowledge from access**: the executor knows where things are; the seed and passphrase sit in a safe or with the custody provider's protocol — nobody but you holds everything until you are gone.
6. **Do a dry run**: have your executor or helper walk through the letter with a test wallet holding $20. Fix every point where they got stuck.
7. **Review yearly** and after any change in holdings, devices, marriage, or death of a named helper; date each version and destroy superseded copies.
8. **Tell your executor the letter exists** and where. A plan nobody knows about is not a plan.

## Key takeaways

- Without a plan, self-custodied crypto dies with you; exchanges and brokerages need the inventory too.
- Wills become public in probate — never put seed phrases or passphrases in them.
- Keep three things separate: the will (authority), the letter of instruction (how), and the secrets (where).
- Collaborative custody (Casa, Unchained) or DIY 2-of-3 multisig lets a trusted person help recover without being able to steal.
- Executors need a digital-assets clause, the inventory, a named technical helper, and your basis records.
- Rehearse the recovery with a test wallet; the first time should not be the real time.
- Update the plan every year and after every change in wallets or people.

## Sources

- [Casa Inheritance: recipient FAQs](https://support.casa.io/knowledge/inheritance-faqs-recipient)
- [Casa expands self-custody inheritance to bitcoin, ether and stablecoins (The Block)](https://www.theblock.co/post/285090/casa-expands-self-custody-inheritance-solution-globally-bitcoin-ether-stablecoins)
- [Unchained Inheritance Protocol (PDF)](https://help.unchained.com/hubfs/Unchained%20Inheritance%20Protocol.pdf)
- [Unchained vs Casa: multisig custody, inheritance, and key control](https://www.unchained.com/compare/unchained-vs-casa)
- [Unchained pricing](https://www.unchained.com/pricing)
- [Inheritance planning: Casa vs Nunchuk (Nunchuk blog, 2026)](https://nunchuk.io/blog/casa)
- [Bitcoin collaborative custody comparison (Spark, 2026)](https://www.spark.money/tools/bitcoin-collaborative-custody-comparison)
- [Bitcoin.org: Securing your wallet — plan for your testament](https://bitcoin.org/en/secure-your-wallet)
- [Digital estate plan for cryptocurrency: a practical 2026 guide (Ironclad Family)](https://www.ironcladfamily.com/blog/digital-estate-plan-for-cryptocurrency-a-practical-2026-guide)
- [Estate planning for digital assets and crypto (LegalClarity)](https://legalclarity.org/estate-planning-for-digital-assets-and-crypto-what-to-know/)
