# DeFi Protocol Safety Checklist

**In one sentence:** Before depositing into any decentralized finance (DeFi) protocol — a lending pool, exchange, yield vault, or bridge — check its audits, age and size, admin powers, oracle design, bridge exposure, where the yield actually comes from, insurance, and your own wallet setup, and simulate the transaction before signing.

**The core idea:** DeFi replaces a company you could sue with code you cannot. That code can be wrong (protocol logic bugs), can be lied to (oracle manipulation), can be upgraded by whoever holds the admin key (access control), or can be reached through a bridge that gets drained. DefiLlama's hacks database counts more than $9 billion lost from DeFi protocols and nearly $4 billion from bridges. Almost all of it was avoidable with the questions below.

**Wallet rule that comes before everything else:** you interact with DeFi from a **separate hot wallet** holding only what you are deploying, never from the wallet that holds your long-term stack.

---

## 0. Before you even look at the protocol: wallet segregation

- [ ] You have **three tiers of wallet**: a **vault** (hardware wallet, never connects to any site), a **DeFi wallet** (hardware-backed if possible, used only with protocols you have vetted), and a **burner** (software wallet with pocket money, for anything experimental, new, or airdrop-related).
- [ ] The wallet you are about to use holds **only the amount you are deploying plus gas**. If the site turns out to be a drainer, that is the ceiling of your loss.
- [ ] The wallet has no valuable NFTs or tokens sitting in it from earlier activity. Sweep them to the vault first.
- [ ] You are using a **dedicated browser profile** for DeFi with a minimal, vetted extension set.

## 1. Audits and code maturity

**Why this matters:** Audits do not make code safe; they make *some* classes of bugs less likely. What you want is multiple independent reviews of the version that is actually deployed, plus time in production.

- [ ] At least **two independent audits** by recognized firms, linked from the official docs, with public reports.
- [ ] The audits cover the **currently deployed contracts** (compare the audited commit or contract address with what is live). A protocol that upgraded after its audit is effectively unaudited for the changes.
- [ ] All **critical and high** findings are marked resolved and re-verified, not "acknowledged" or "won't fix."
- [ ] Contracts are **verified on the block explorer** (source code published and matching the bytecode).
- [ ] A **bug bounty** (e.g., Immunefi) is live with a payout large enough to matter to a professional (six figures or more for a protocol holding serious TVL).
- [ ] For forks: you know what the protocol forked from, what it changed, and whether the *changes* were audited — many exploits hit "battle-tested" forks in the parts that were modified.

## 2. Age, size, and track record

**Why this matters:** Time in production with real money at stake is the only test that finds the bugs auditors missed. TVL (total value locked — how much money users have deposited) signals both trust and target size.

- [ ] Live on mainnet for **at least 6–12 months** with meaningful TVL the whole time. Newer than that = burner wallet only.
- [ ] TVL is large enough that a bug would already have been worth exploiting (tens of millions at minimum), and is **not** mostly the team's own money or a single whale.
- [ ] You checked **DefiLlama's hacks list** for the protocol *and* for its forks/parent. If it was exploited, the post-mortem was honest, the fix was audited, and users were compensated.
- [ ] TVL trend is stable or growing and not entirely driven by a token-incentive program that is scheduled to end.
- [ ] The team is still shipping and communicating (GitHub activity, governance forum, incident-response history).

## 3. Admin keys, upgradeability, and timelocks

**Why this matters:** If a contract can be upgraded, paused, or have its parameters changed, the "decentralized" protocol is exactly as safe as whoever controls that power. Access-control failures and key compromises are the largest category of losses.

- [ ] You know whether the contracts are **upgradeable** (proxy pattern) or immutable. Immutable is safer against admin abuse but cannot be patched if a bug is found; upgradeable needs the controls below.
- [ ] Admin powers are held by a **multisig** with a stated threshold (e.g., 4-of-7) and **publicly identified signers** from more than one organization — not a single address, and not a 2-of-3 controlled by the founders.
- [ ] Sensitive actions (upgrades, parameter changes, treasury moves) go through a **timelock** of at least 24–48 hours, so you can exit before a malicious or mistaken change executes.
- [ ] Emergency **pause** powers, if they exist, are limited in scope and cannot be used to withdraw user funds.
- [ ] The protocol's docs (or a third-party rating like DefiSafety or DeFiScan) explain the trust assumptions in plain language. If the protocol does not talk about its admin risk, assume the worst.
- [ ] Governance token voting cannot cheaply push through a change that drains the treasury or user deposits (check quorum, voting delay, and whether a large holder could act alone).

## 4. Oracle design

**Why this matters:** An **oracle** is how the contract learns prices. If it reads a price a trader can move — such as the spot price in one thin pool — an attacker can make the contract believe collateral is worth far more than it is, borrow against it, and vanish. Oracle manipulation is one of the most repeated exploit patterns.

- [ ] Prices come from a **decentralized oracle network** (e.g., Chainlink, Pyth) or a **time-weighted average** across deep liquidity, not the instantaneous spot price of a single pool.
- [ ] Assets accepted as collateral are **liquid enough** that their price cannot be moved a lot with a flash loan.
- [ ] The protocol has **circuit breakers** or sanity bounds on price moves, and a documented plan for when an oracle goes stale.
- [ ] For lending protocols: **liquidation** parameters (collateral factors, liquidation thresholds) are conservative for volatile assets, and the liquidator ecosystem is active (bad debt does not pile up in crashes).

## 5. Bridge and cross-chain exposure

**Why this matters:** Bridges hold locked assets on one chain and issue IOUs on another. They are the single most-drained category in DeFi, and a bridge failure makes every "wrapped" asset issued through it worthless — even if the protocol you deposited into is fine.

- [ ] You know which **bridge** the asset you hold or the chain you are using depends on, and you have looked up that bridge's audits, TVL, and hack history.
- [ ] You prefer **native assets** (ETH on Ethereum, SOL on Solana, USDC issued natively on that chain) over bridged/wrapped versions where possible.
- [ ] You keep the amount sitting on a young or low-TVL chain or L2 small, because withdrawing back to mainnet may take days (optimistic rollups) or depend on a bridge under stress.
- [ ] If the protocol itself is cross-chain, you understand what happens to your position if one chain's contracts are paused or exploited.

## 6. Where the yield actually comes from

**Why this matters:** Yield is either paid by someone who is using your capital (borrowers, traders, validators) or it is paid in newly printed tokens (emissions) — or it is paid from new depositors (a Ponzi). Only the first is sustainable. "20% APY on a stablecoin" always has an answer to *who is paying that*, and you need to know it.

- [ ] You can write one sentence: "The yield comes from ______ (borrowers paying interest / trading fees / staking rewards / token emissions)."
- [ ] For emissions-based yield, you have separated **real yield** (fees earned in an asset with independent value) from **token rewards** (which you will be selling into the same market as everyone else). Judge the position on the real yield.
- [ ] Yield is in line with the risk-free rate plus a plausible risk premium. Anything far above the best lending rates on blue-chip protocols is either very short-lived, very risky, or a fraud.
- [ ] For liquidity providing (LP): you have estimated **impermanent loss** for a realistic price move (see [crypto-formulas-and-rules-of-thumb.md](crypto-formulas-and-rules-of-thumb.md)) and confirmed fees are likely to exceed it.
- [ ] For "auto-compounding vaults" and aggregators: you have looked through to the underlying protocol and are running this checklist on *that* too. You now have two layers of smart contract risk.
- [ ] For stablecoins earning yield: you know how the stablecoin is backed (fiat in a bank, over-collateralized crypto, algorithmic) and you avoid the last category outright.

## 7. Insurance and recourse

**Why this matters:** Decentralized cover exists, but it is narrow, expensive, and often will not pay for the exact way you lose money. Know what you have before assuming you have anything.

- [ ] You know whether cover is available for this protocol (e.g., Nexus Mutual and similar) and what it covers — usually smart-contract exploit only, not oracle failure, not depeg, not admin rug, not your own phishing.
- [ ] If the protocol has a **safety module** or insurance fund, you know its size relative to TVL and what triggers it.
- [ ] You have priced the cover against your expected yield. If cover costs more than the extra yield you are chasing, the position was not worth it.
- [ ] You accept that in the base case, an exploit means the money is gone, and you have sized accordingly.

## 8. The transaction itself: simulation, approvals, and signing

**Why this matters:** Wallet drainers do not exploit the protocol; they exploit *you* at the moment you click "confirm." The defense is reading what you are signing.

- [ ] You reached the site from your **own bookmark**, not from a link, an ad, a DM, a Discord announcement, or a search result. Confirm the domain character by character.
- [ ] Your wallet or an extension (e.g., a transaction-simulation tool, or the wallet's built-in preview) **simulates the transaction** and shows what leaves and what arrives. If the simulation shows assets leaving that you did not intend, or "unlimited approval," stop.
- [ ] You set **approval limits** to the exact amount you are depositing, not "unlimited." It costs a bit more gas each time and it caps the damage if the contract is later compromised.
- [ ] You are not being asked to sign a message you do not understand — especially `permit`, `Permit2`, `setApprovalForAll`, or a blank-looking "Sign in" that actually authorizes transfers.
- [ ] The hardware wallet screen shows the **contract address and amount** matching the site. If your device can only blind-sign this transaction, reconsider.
- [ ] After withdrawing from a protocol, you **revoke the approval** (revoke.cash, the explorer's approval checker, or the wallet's own tool). You do a full approval review on every DeFi wallet **quarterly**.

## 9. Position management

- [ ] The total across all DeFi positions stays within the "DeFi / yield" sub-limit in your [investment policy statement](crypto-investment-policy-statement-template.md).
- [ ] You have written **exit triggers**: yield falls below X, TVL drops by Y%, an audit finding is published, admin multisig changes, the underlying stablecoin depegs more than Z%.
- [ ] You have alerts set (protocol Discord/Twitter, DefiLlama, a wallet-monitoring service) so you hear about incidents within hours, not days.
- [ ] Every deposit, reward claim, and withdrawal is logged for taxes — DeFi transactions are the hardest part of crypto tax prep (see [tax-record-keeping-checklist.md](tax-record-keeping-checklist.md)).

---

## Quick decision rule

| Situation | Maximum wallet tier | Maximum size |
|---|---|---|
| Blue-chip protocol, 2+ years, multiple audits, multisig + timelock, decentralized oracle | DeFi wallet | Within IPS DeFi limit |
| Established fork or 6–12 months old, one audit, clear admin disclosure | DeFi wallet | Half of IPS DeFi limit |
| New protocol, single audit or none, unknown admin setup, emissions-driven yield | Burner only | Money you have already written off |
| Any protocol reached via a DM, ad, or "limited time" claim page | None | Zero |

---

## Sources

- [DefiLlama — Hacks database](https://defillama.com/hacks) (loss totals by category: key compromise, oracle manipulation, protocol logic, bridge, access control)
- [Revoke.cash — What are token approvals?](https://revoke.cash/learn/approvals/what-are-token-approvals)
- [Ledger Academy — Token approvals explained; vault / trading / burner wallet segregation](https://www.ledger.com/academy/topics/security/ethereum-token-approvals-explained)
- [Ledger Academy — Security tips for hardware wallets (blind signing, trusted display)](https://www.ledger.com/academy/hardwarewallet/best-practices-when-using-a-hardware-wallet)
- [Chainalysis — 2025 Crypto Crime Report introduction](https://www.chainalysis.com/blog/2025-crypto-crime-report-introduction/) (private key compromise share of stolen funds; DeFi as largest loss venue)
- [Bitcoin.org — Securing your wallet](https://bitcoin.org/en/secure-your-wallet)
