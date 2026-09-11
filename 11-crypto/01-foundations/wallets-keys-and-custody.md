# Wallets, Keys, and Custody

**In one sentence:** Owning crypto means controlling a private key, and the only real decision is who holds that key: you (self-custody, with total control and total responsibility), an exchange (custodial, convenient but you are an unsecured creditor), or a fund manager via an ETF (no keys at all, held in a brokerage account), and the right answer depends on how much you hold, how technical you are, and what you are trying to protect against.

## Keys are the asset

A crypto "wallet" does not hold coins. Coins live on the blockchain. A wallet holds the **private key** that can sign transactions moving them (see [How Blockchains Work](how-blockchains-work.md)). Whoever has the key has the coins; whoever loses the key loses them permanently. There is no "forgot password" link and no fraud department. This single fact drives every custody decision.

## Custodial vs. self-custody

**Custodial**: an exchange (Coinbase, Kraken, Binance) or custodian holds the keys. You have an account with a username and password; your balance is an entry in their database. This feels like a bank account, but legally you are usually an unsecured creditor. When FTX collapsed in November 2022, customer deposits were gone; when Celsius, Voyager, and BlockFi failed the same year, customers waited years for partial recoveries. Reputable U.S. exchanges now segregate customer assets and are subject to state and federal oversight, and the largest use institutional-grade cold storage, but "the exchange got hacked" (Mt. Gox 2014, Bybit 2025) and "the exchange was a fraud" (FTX) remain the two biggest ways people have lost crypto.

**Self-custody**: you hold the key. Nobody can freeze, seize, or lose your coins but you. You also cannot call anyone when you send to a wrong address, get phished, or lose the backup.

The phrase **"not your keys, not your coins"** is literally true. It is also true that most self-custody losses are self-inflicted.

## Hot vs. cold wallets

| | Hot wallet | Cold wallet |
|---|---|---|
| Definition | Key lives on an internet-connected device (phone, browser extension, exchange) | Key is generated and stored offline |
| Examples | MetaMask, Phantom, Coinbase Wallet, Trust Wallet, exchange accounts | Ledger, Trezor, Coldcard, paper/steel backups |
| Convenience | High: sign transactions in seconds, use DeFi and NFTs | Lower: physically confirm each transaction on the device |
| Main risk | Malware, phishing, malicious websites, clipboard hijacking | Physical loss/theft, supply-chain tampering, losing the backup |
| Best for | Small "spending" balances, active DeFi use | Long-term holdings, anything you cannot afford to lose |

A sensible pattern mirrors cash: a small hot-wallet balance for activity, the bulk in cold storage.

## Hardware wallets

A **hardware wallet** is a small device that generates and stores the private key in a secure chip that never exposes it to the connected computer. Transactions are sent to the device, displayed on its screen, and signed only after you physically confirm. Even if your PC is infected, the key does not leave the device.

- **Ledger** (France): most popular; secure element chip; closed-source firmware; a 2020 customer-database leak exposed buyers' addresses to phishing, and its 2023 "Recover" service (optional key backup with third parties) alienated some users. Supports thousands of assets.
- **Trezor** (Czech Republic): open-source hardware and software; newer models add a secure element. Strong reputation among privacy-minded users.
- **Coldcard** (Canada): bitcoin-only, air-gapped (can operate via microSD/QR with no USB connection), favored by serious bitcoin holders.
- Others: BitBox, Keystone, Foundation Passport.

Buy directly from the manufacturer, never from a marketplace reseller (tampered devices with pre-set seed phrases are a known scam). Set the device up yourself; a device that arrives with a seed phrase already written down is compromised.

## Seed phrases

When you set up a wallet, it generates a **seed phrase** (also called a recovery phrase or mnemonic): 12 or 24 English words from a standard list (BIP-39) that encode the master key. Every address in the wallet is derived from it. Anyone with the words can recreate the wallet on any device and take everything.

Rules that account for most of the difference between people who keep their crypto and people who lose it:

1. Write the phrase on paper or stamp it into steel (fire- and flood-proof). Never type it into a computer, phone, photo, cloud note, or password manager.
2. Store copies in at least two physically separate secure locations.
3. Never enter it on any website. No legitimate service ever asks for it. "Support" asking for your seed phrase is a scammer, every time.
4. Consider an optional **passphrase** (a "25th word") that creates a hidden wallet; losing it loses the funds, so document it separately.
5. Make sure a trusted person or your estate plan can find and use it. Crypto that dies with you is gone.

## Multisig

A **multisignature** (multisig) wallet requires M of N keys to sign, such as 2-of-3. Keys can be spread across devices, locations, and people. One lost or stolen key does not lose the funds; one compromised key cannot spend them. This is how exchanges, funds, and DAOs hold treasuries, and services like Casa and Unchained offer "collaborative custody" where the company holds one key, you hold the others, and neither can move funds alone. Multisig is the best structure for large personal holdings and for inheritance planning, at the cost of setup complexity. On Ethereum the standard is the Safe (formerly Gnosis Safe) smart-contract wallet.

## The third option: ETFs and brokerage exposure

Since January 2024, U.S. investors can buy spot bitcoin ETFs (IBIT, FBTC, and others), spot Ethereum ETFs (July 2024), and Solana ETFs (October 2025) in an ordinary brokerage or retirement account. The fund's custodian (Coinbase Custody for most of them) holds the keys in cold storage; you hold fund shares.

Advantages: no keys, no seed phrases, no exchange account, works in an IRA or 401(k), simple tax reporting, insured against broker failure via SIPC (for the shares, not the underlying coins). Disadvantages: annual fees (roughly 0.2–0.25% for the large bitcoin ETFs), trading only during market hours, no ability to use the coins (Lightning, DeFi, staking, self-custody), no exposure to most altcoins, and reliance on a custodian and fund structure you do not control. Also available: shares of Strategy (MSTR) and other bitcoin-treasury companies, which are leveraged, premium-or-discount proxies rather than clean exposure, and crypto held inside brokerage apps like Robinhood or Fidelity Crypto, which is custodial.

## Which option suits whom

| Investor | Suggested approach |
|---|---|
| Wants price exposure in a retirement or brokerage account; no interest in the technology | **Spot ETF.** Simplest, cheapest to get right, hardest to lose. |
| Small allocation (a few percent), moderate technical comfort | **Reputable regulated exchange** (custodial), with two-factor authentication via an authenticator app or hardware key, never SMS. Or an ETF. |
| Meaningful holdings, willing to learn | **Hardware wallet** with steel seed backup in two locations. Keep a small hot wallet for activity. |
| Large holdings, or planning for heirs | **Multisig** (2-of-3 or 3-of-5), possibly with a collaborative-custody provider, and written instructions for the estate. |
| Active DeFi user | Hardware-wallet-backed hot wallet (Ledger + MetaMask/Rabby); separate "burner" wallet for new or risky sites; never hold the bulk in a wallet that signs DeFi transactions. |
| Lives under an unstable government or capital controls | **Self-custody** is the point; the censorship-resistance case only works if you hold the keys. |

## Operational security basics

- Use unique passwords and app-based or hardware-key two-factor authentication on exchanges; SIM-swap attacks defeat SMS codes.
- Verify the first and last several characters of every address before sending; malware swaps clipboard contents.
- Send a small test transaction first for any large transfer.
- Be paranoid about "approvals" in DeFi: signing a token approval can let a malicious contract drain that token later. Revoke unused approvals (revoke.cash).
- Assume every unsolicited message about your crypto is a scam. Bookmark exchange and wallet sites; never click links from email or social media.
- Do not talk publicly about holdings; "wrench attacks" (physical coercion) are real and rising.

## Key takeaways

- A wallet stores keys, not coins; the key is the asset, and losing it is final.
- Custodial accounts are convenient but make you an unsecured creditor; FTX, Celsius, and Mt. Gox are the cautionary tales.
- Hot wallets are for spending money; cold storage (hardware wallets) is for savings. Buy hardware wallets only from the manufacturer.
- The seed phrase is everything: write it on steel, store copies apart, never digitize it, never share it, and make sure heirs can find it.
- Multisig removes single points of failure and is the standard for large holdings and estates.
- Spot ETFs are the right answer for most investors who just want price exposure, especially in retirement accounts.
- Most crypto losses are phishing, malware, and mistakes, not blockchain failures; operational discipline is the real security.

## Sources

- [Bitcoin.org: Securing your wallet](https://bitcoin.org/en/secure-your-wallet)
- [Bitcoin.org: Choose your wallet](https://bitcoin.org/en/choose-your-wallet)
- [Ethereum.org: Wallets](https://ethereum.org/en/wallets/)
- [Coinbase Learn: What is a crypto wallet?](https://www.coinbase.com/learn/crypto-basics/what-is-a-crypto-wallet)
- [Kraken Learn: Custodial vs non-custodial wallets](https://www.kraken.com/learn/custodial-non-custodial-crypto-wallet)
- [BIP-39 specification (mnemonic seed phrases)](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki)
- [Ledger: Security model](https://www.ledger.com/academy/security)
- [Trezor: Learn and support](https://trezor.io/learn)
- [Coinkite: Coldcard documentation](https://coldcard.com/docs/)
- [Safe: Smart account documentation (multisig)](https://docs.safe.global/)
- [Investopedia: What is a hardware wallet?](https://www.investopedia.com/hardware-wallet-8749727)
- [Fidelity: Understanding crypto ETFs](https://www.fidelity.com/learning-center/trading-investing/crypto/crypto-etfs)
- [CNBC: Hackers steal $1.5 billion from Bybit (Feb 2025)](https://www.cnbc.com/2025/02/21/hackers-steal-1point5-billion-from-exchange-bybit-biggest-crypto-heist.html)
