# Operational Security and Scam Defense

**In one sentence:** Almost nobody loses crypto to a broken blockchain; they lose it to a phone call, a text, a link, a signature they did not read, or a stranger who was kind for three months — so the defenses are habits, not software.

## The size of the problem (as of September 2026)

- The FBI's Internet Crime Complaint Center (IC3) logged **181,565 crypto-related complaints in 2025 with losses above $11 billion**, out of nearly $21 billion in total reported cybercrime losses. Investment fraud (mostly crypto) was ~49% of all scam losses, and Americans over 60 lost ~$7.8 billion, up 37% in a year.
- Chainalysis estimates **$17 billion** was taken by crypto scams in 2025 (about $14 billion confirmed on-chain, up from $9.9 billion in 2024). Impersonation scams grew ~1,400% year over year, and scams run with AI tooling extracted roughly 4.5× more per operation than those without.
- Wallet-drainer phishing (malicious signatures) actually *fell* to ~$84 million across ~106,000 victims in 2025, down 83% from 2024 — better wallet warnings helped — but the largest single case was still $6.5 million from one "permit" signature.
- The February 2025 Bybit theft (~$1.5 billion) was not a user error; it was a compromised developer machine that altered what the signers saw. Even professionals get fooled by a screen.

The pattern: money lost to *persuasion* dwarfs money lost to *hacking*.

## The main attacks and the specific defense for each

| Attack | What it looks like | Defense |
|---|---|---|
| **Phishing** | Email/text/DM "from" Coinbase, Ledger, MetaMask: "verify your account," "firmware update," "suspicious login." Links to a pixel-perfect clone. | Never click links in messages. Type the URL or use a bookmark. Ledger, Trezor, and exchanges will never ask for your seed. Ledger says it will never call or text you at all. |
| **SIM swap** | Attacker convinces your carrier to move your number to their SIM, then receives your SMS codes and resets passwords. | Remove SMS as a 2FA/recovery option everywhere. Use an authenticator app or, better, a hardware security key (YubiKey). Set a carrier **port-out PIN / number-transfer PIN** and account lock; FCC rules since 2024 require carriers to authenticate SIM changes and notify you, but you must turn the locks on. |
| **Fake support** | After you post a question in Discord/Reddit/X, a "support agent" DMs offering help and asks you to "sync" or "validate" your wallet on a site. | Real support never DMs first and never needs your seed. Close the DM. |
| **Seed-phrase harvesting** | Fake wallet apps, fake "Ledger Live," physical letters with QR codes, "backup verification" pages. | There is *no* legitimate reason to type a seed into a website or app other than restoring a wallet you control on a device you trust. |
| **Wallet drainers / malicious approvals** | You connect a wallet to a "mint," "claim," or "airdrop" site and sign something. The signature is an unlimited token approval or a `permit` that lets the attacker move your tokens later. | Read every signature. Reject "blind" or unreadable requests. Use a separate hot wallet with small balances for interacting with new sites. Revoke old approvals (below). |
| **Address poisoning** | Dust transactions from lookalike addresses land in your history so you copy the wrong one later. | Never copy from history; use an address book; verify middle characters; test-send first. |
| **Pig butchering / romance-investment** | A friendly stranger (dating app, wrong-number text, LinkedIn) builds rapport over weeks, then shows a "trading platform" with fake gains. Withdrawals require "taxes" or "fees." | Anyone you have never met in person who steers you to an investment platform is running a script. There is no platform. Stop, do not pay "release fees," report. |
| **Fake airdrops / tokens** | Unknown tokens or NFTs appear in your wallet with a link to "claim" or "swap." | Ignore them. Interacting is the trap. Hide them in the wallet UI. |
| **Impersonated exchanges & "recovery" firms** | After a loss, "recovery experts" promise to retrieve funds for an upfront fee. | Recovery scams target victims twice. Law enforcement never charges a fee. |
| **Social engineering / wrench attacks** | Someone learns you hold crypto — from a post, a car sticker, a leaked customer list — and shows up. | Do not discuss holdings publicly. Keep large holdings in multisig with keys in separate places so no one at your door can force a transfer. |

## Two-factor authentication done right

Ranked from weakest to strongest:

1. SMS codes — vulnerable to SIM swap. Turn off.
2. Email codes — only as strong as your email, which is often the recovery path for everything else.
3. Authenticator app (TOTP) — good; back up the seed codes offline.
4. Hardware security key (FIDO2/WebAuthn) — best; phishing-resistant because the key checks the domain. Buy two, register both, keep one off-site.

Lock your **email** first; it is the master key to every account reset. Then the exchange, then the carrier.

## Revoking token approvals (Ethereum, L2s, Solana, Tron)

When you use a decentralized app, you often grant a smart contract permission to spend a token from your wallet — an **approval**. Many apps request *unlimited* approvals that never expire. If that contract is later exploited, or if you signed a malicious one, the attacker can drain the approved token at any time.

1. Go to **revoke.cash** (bookmark it; phishing clones exist) or the "Token Approvals" page on Etherscan/Basescan/Solscan.
2. Enter your address or connect your wallet, choose the network.
3. Sort by most recent or highest value; look for anything you do not recognize or no longer use.
4. Click **Revoke** (costs a small gas fee) or edit the allowance down to what you need.
5. Repeat on each chain you use, quarterly and immediately after any suspicious signature.

## How to actually do it

1. **Tonight:** switch every exchange, email, and wallet login from SMS 2FA to an authenticator app or hardware key. Add a port-out PIN at your carrier.
2. **Create a dedicated email** used only for crypto accounts, with its own hardware-key 2FA.
3. **Use a password manager** with unique passwords; it also protects you from typing credentials into a lookalike domain because autofill will not trigger.
4. **Bookmark** your exchanges, wallet sites, revoke.cash, and block explorers. Only enter through bookmarks.
5. **Segregate wallets**: cold wallet (never connects to any site), warm wallet (trusted DeFi only), burner (new sites, mints, airdrops) with money you can lose.
6. **Enable exchange withdrawal allowlists** and a 24–48 hour withdrawal delay on new addresses.
7. **Set a personal rule**: any unsolicited contact about crypto is a scam until proven otherwise; any urgency is a scam signal; anyone asking for a seed, a "validation," or a fee to release money is a scam, full stop.
8. **Run the checklist below** every quarter.

## The quarterly OPSEC checklist

- [ ] No SMS 2FA remains on email, exchanges, or carrier account
- [ ] Carrier port-out PIN and account lock confirmed active
- [ ] Hardware security keys registered on email and exchanges; spare key stored off-site
- [ ] Token approvals reviewed and revoked on every chain used
- [ ] Hot-wallet balances kept to "spendable" size; cold wallet has never touched a dApp
- [ ] Exchange withdrawal allowlist and delay enabled
- [ ] Bookmarks used for every crypto site; no links from messages clicked
- [ ] Software wallets, browser, OS, and device firmware updated from official sources
- [ ] No holdings discussed on social media, in public, or with new acquaintances
- [ ] Family members briefed on the "no one legitimate asks for the seed" rule

## If you have been scammed

1. Move any remaining funds to a new wallet from a clean device.
2. Revoke approvals from the affected address.
3. Report to IC3 (ic3.gov) with transaction hashes, addresses, and screenshots; also notify the exchange the funds went through, if any — exchanges can freeze deposits that land in their custody.
4. Do not pay anyone who contacts you offering recovery.
5. Document everything for a potential theft-loss position on your taxes (rules are restrictive; consult the tax section).

## Key takeaways

- Losses come from persuasion far more than from code; the FBI logged more than $11 billion in crypto-related losses in 2025.
- Kill SMS 2FA and set a carrier port-out PIN today; use hardware security keys where possible.
- Nobody legitimate ever needs your seed phrase — not Ledger, not Coinbase, not "support."
- Read every signature; use a burner wallet for anything new; revoke stale approvals quarterly.
- Never copy addresses from transaction history; test-send first.
- A stranger who steers you to an investment platform is a script; a "recovery expert" who wants a fee is the same scam again.
- Silence about holdings is a security control.

## Sources

- [FBI: Cryptocurrency and AI scams bilk Americans of billions (2025 IC3 report press release)](https://www.fbi.gov/news/press-releases/cryptocurrency-and-ai-scams-bilk-americans-of-billions)
- [2025 IC3 Annual Report (PDF)](https://www.ic3.gov/AnnualReport/Reports/2025_IC3Report.pdf)
- [Chainalysis 2026 Crypto Crime Report: Scams](https://www.chainalysis.com/blog/crypto-scams-2026/)
- [Chainalysis 2026 Crypto Crime Report: Introduction](https://www.chainalysis.com/blog/2026-crypto-crime-report-introduction/)
- [Scam Sniffer 2025: phishing losses fall 83% to $84M](https://drops.scamsniffer.io/scam-sniffer-2025-crypto-phishing-losses-fall-83-to-84-million/)
- [Chainalysis: Anatomy of an address poisoning scam](https://www.chainalysis.com/blog/address-poisoning-scam/)
- [Ledger: ongoing phishing campaigns status](https://www.ledger.com/phishing-campaigns-status)
- [Ethereum.org: Security and scam prevention](https://ethereum.org/en/security/)
- [Revoke.cash: How to revoke token approvals](https://revoke.cash/learn/approvals/how-to-revoke-token-approvals)
- [FCC: Protecting consumers from SIM-swap and port-out fraud (Federal Register)](https://www.federalregister.gov/documents/2023/12/08/2023-26338/protecting-consumers-from-sim-swap-and-port-out-fraud)
- [FCC announces effective compliance date for SIM swapping rules](https://www.fcc.gov/consumer-governmental-affairs/fcc-announces-effective-compliance-date-sim-swapping-item)
