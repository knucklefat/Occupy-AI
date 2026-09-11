# Token Due Diligence Checklist

**In one sentence:** A 48-item checklist for investigating any token beyond bitcoin and ether — team, supply, value accrual, product, security, liquidity, ownership, listings, narrative, and your own exit — with a scoring guide that turns the answers into a buy / small / pass decision.

**How to use it:** Work through every section before buying. Write the answer, not just a tick. An item you cannot answer counts as a *no*. Most tokens fail this checklist, which is the point: the base rate for altcoins going to roughly zero over a full cycle is very high, and the tokens that survive usually pass most of these items.

**Where to look:** the project's docs and GitHub; the token's page on CoinGecko or CoinMarketCap (contract address, supply, exchanges); DefiLlama (TVL, fees, revenue, hacks); Token Terminal or the project's own dashboards (fees, revenue, users); a block explorer such as Etherscan or Solscan (holders, contract, admin functions); unlock trackers such as Tokenomist (formerly TokenUnlocks) or CryptoRank; audit reports linked from the docs; and Messari or similar research for governance and disclosure quality.

---

## 1. Team and organization (6 items)

**Why this matters:** In crypto there is often no legal entity to sue, no board, and no regulator standing between you and the people who wrote the code. Their identity, track record, and incentives are most of your protection.

- [ ] 1. Core team members are publicly identified (real names, verifiable work history), or — if pseudonymous — have a multi-year public track record under that pseudonym.
- [ ] 2. At least one team member has shipped a previous product (in crypto or elsewhere) that still exists.
- [ ] 3. No team member has been associated with a prior rug pull, exploit cover-up, or enforcement action (search names + "SEC", "lawsuit", "rug", "exploit").
- [ ] 4. There is a legal entity or foundation you can name, and its jurisdiction is stated.
- [ ] 5. The team's own token allocation is disclosed, and it vests over at least 2–4 years with a cliff (a period, usually 12 months, before any of it unlocks).
- [ ] 6. Development is active: GitHub shows meaningful commits from multiple contributors in the last 90 days, not just README edits.

## 2. Tokenomics: supply, unlocks, inflation (9 items)

**Why this matters:** A token's price is set by the tiny fraction of supply that trades each day. If far more supply is scheduled to arrive than the market is absorbing, price falls regardless of how good the product is. Fully diluted valuation (FDV) — price × total eventual supply — tells you what you are really paying.

- [ ] 7. You know the **circulating supply**, **total supply**, and **max supply** (if any), and where each number came from.
- [ ] 8. You have calculated **FDV** and the **circulating-to-total ratio** (see [crypto-formulas-and-rules-of-thumb.md](crypto-formulas-and-rules-of-thumb.md)). A ratio below ~30% means most of the supply has not hit the market yet.
- [ ] 9. You have looked at the **unlock schedule** for the next 12 months and know the largest single monthly unlock as a percentage of circulating supply. Anything above ~5% in a month is a price event.
- [ ] 10. You know who receives those unlocks (team, investors, foundation, community) and at what cost basis. Investors who bought at 1/20th of today's price will sell.
- [ ] 11. You know the **annual inflation rate** from emissions (new tokens minted for staking rewards, liquidity incentives, etc.) and have compared it to the staking yield. If staking yield ≈ inflation, the "yield" is just dilution protection, not income.
- [ ] 12. The allocation is not lopsided: insiders (team + investors) hold less than ~40–50% of total supply. Above that, the token was designed to be sold to you.
- [ ] 13. The token contract cannot be minted beyond the stated schedule without a governance vote, or the mint function is renounced/burned. (For Solana tokens: mint authority and freeze authority are revoked.)
- [ ] 14. There is no hidden supply: check the top holders on the block explorer for large unlabeled wallets that could be undisclosed team or market-maker inventory.
- [ ] 15. Market-maker agreements (loans of tokens to trading firms) are disclosed, including how many tokens and whether the market maker has a cheap call option on them.

## 3. Value accrual (6 items)

**Why this matters:** A protocol can be wildly successful while its token is worthless, if nothing about the protocol's success flows to token holders. Ask: *why does this token need to exist, and what does it capture?*

- [ ] 16. You can write one sentence explaining why the token must exist for the protocol to work (gas, security/staking, collateral, governance with real economic rights). "It's the governance token" alone is a weak answer.
- [ ] 17. There is a concrete mechanism by which protocol usage benefits holders: fee sharing, buybacks, burns, staking that earns real fees (not just emissions), or a required use in the product.
- [ ] 18. That mechanism is live today, not "planned" or "subject to a future governance vote." If it is planned, discount it heavily.
- [ ] 19. Protocol **revenue** (the portion of fees kept by the protocol/token holders, as opposed to paid to liquidity providers or validators) is positive and you know the number.
- [ ] 20. Revenue exceeds token incentives paid out. If the protocol spends $10M in emissions to earn $1M in fees, it is buying growth with your dilution.
- [ ] 21. You have compared FDV to annualized revenue (the "price-to-sales" ratio) against a few peers in the same category. Extreme outliers need a strong reason.

## 4. Product, users, and traction (6 items)

**Why this matters:** Narrative and price feed each other in crypto; usage is the one thing that is hard to fake for long. Look for organic activity by people who are not being paid in tokens to show up.

- [ ] 22. The product is live on mainnet and you have personally used it (or watched someone use it) end to end.
- [ ] 23. Daily/monthly active addresses, transactions, or volume are trending flat-to-up over 6+ months, not spiking around airdrop announcements and collapsing after.
- [ ] 24. TVL (total value locked — assets deposited in the protocol) is meaningful relative to FDV and relative to competitors, and did not arrive mostly through incentive programs that are about to end.
- [ ] 25. You can name the competitors and explain what this protocol does better, cheaper, or first.
- [ ] 26. The addressable market is large enough that the token's current FDV represents a plausible share of it.
- [ ] 27. The roadmap has dated milestones, and at least two past milestones were hit within a reasonable window of the promised date.

## 5. Security: audits, admin keys, contract risk (7 items)

**Why this matters:** Private key compromises and access-control flaws account for the largest share of stolen funds each year. A token you hold can be minted to infinity, frozen, or drained by whoever holds the admin key — audit or not.

- [ ] 28. At least one audit by a recognized firm (e.g., Trail of Bits, OpenZeppelin, Spearbit, Cantina, Halborn, Zellic, Certora) is linked from the official docs and the report is public.
- [ ] 29. The audit covers the *currently deployed* contract version, and critical/high findings were fixed and re-verified, not "acknowledged."
- [ ] 30. You know what the **admin keys** can do: upgrade contracts, pause, mint, change fees, drain treasury. This is listed in the docs or discoverable on the explorer (look for `owner`, `admin`, `upgradeTo`, `pause`, `mint`).
- [ ] 31. Admin powers are behind a **multisig** (multiple independent signers required) with a stated threshold and signer list, not a single externally owned account.
- [ ] 32. Sensitive admin actions are behind a **timelock** (a mandatory delay, ideally 24–72 hours, between proposing and executing a change) so users can exit before a malicious change takes effect.
- [ ] 33. There is an active bug bounty (e.g., on Immunefi) with a meaningful maximum payout.
- [ ] 34. The project has not been exploited before — or, if it has, the post-mortem was honest and users were made whole. Check DefiLlama's hacks database.

## 6. Liquidity, holders, and listings (7 items)

**Why this matters:** You are not investing in a token; you are investing in the ability to sell it later. Thin liquidity and concentrated ownership mean you may not be able to exit at anything near the quoted price — and that a few wallets can decide the price for you.

- [ ] 35. **Liquidity depth:** you have checked how much a $10k (or your position size × 5) market sell would move the price on the deepest venue. Above 1–2% slippage for a modest size is a thin market.
- [ ] 36. On-chain liquidity is **locked or owned by the protocol**, not sitting in a wallet the deployer can pull (the classic rug). Tools like rugcheck (Solana) or the DEX's pool page show this.
- [ ] 37. **Holder concentration:** the top 10 non-contract, non-exchange wallets hold less than ~30–40% of circulating supply. Label exchange and contract addresses before judging.
- [ ] 38. Holder count is growing and the distribution is not dominated by wallets created on the same day (a tell for sybil farming or insider splitting).
- [ ] 39. The token is listed on at least one major regulated exchange (or a top-tier DEX with deep liquidity). A listing is not endorsement, but delistings are a meaningful negative signal.
- [ ] 40. Trading volume is not fake: volume/market cap ratio is in a sane range, and volume is spread across venues rather than one obscure exchange reporting most of it.
- [ ] 41. The contract address you plan to buy is the one listed on the project's official site *and* CoinGecko/CoinMarketCap. Copycat tokens with the same ticker are common.

## 7. Narrative and cycle risk (4 items)

**Why this matters:** Most altcoin returns are explained by *when* in the cycle you bought and which narrative was hot, not by the project. Knowing which narrative you are riding lets you plan for its end.

- [ ] 42. You can name the narrative this token belongs to (L1, L2, DeFi, AI, memecoin, RWA, DePIN, gaming, etc.) and where you think that narrative is in its hype cycle.
- [ ] 43. Price is not already up 5–10× in the last few months on the narrative alone. If it is, you are buying the exit liquidity of earlier holders.
- [ ] 44. You have a view on how the token behaves in a broad crypto drawdown (most altcoins fall 70–95% and many never recover), and you are sized for that.
- [ ] 45. Regulatory exposure is understood: is this likely to be treated as a security in your jurisdiction, and what happens to the listing if so?

## 8. Your exit plan (3 items)

**Why this matters:** Without a written exit, you will sell at the worst time — either panicking at the bottom or holding a 10× all the way back down.

- [ ] 46. You have written the **thesis** in one paragraph and the **conditions that would prove it wrong** (e.g., "revenue stops growing," "unlock arrives and team wallets sell," "a competitor takes share").
- [ ] 47. You have written **take-profit rules** (e.g., sell 25% at 2×, 25% at 4×, recover initial cost) and a **stop rule** (a price or thesis-break at which you exit regardless of feelings).
- [ ] 48. Position size follows [pre-trade-checklist-for-crypto.md](pre-trade-checklist-for-crypto.md): small enough that a 100% loss is survivable, and within the altcoin sub-limit in your [investment policy statement](crypto-investment-policy-statement-template.md).

---

## Scoring guide

Count the checked items. Treat any unchecked item in **bold** as an automatic disqualifier regardless of score: **13 (uncontrolled mint)**, **31 (single-key admin)**, **36 (unlocked liquidity)**, **41 (wrong contract address)**.

| Score | Interpretation | Suggested action |
|---|---|---|
| 42–48 | Institutional-grade for crypto. Rare. | Eligible for a full position within your altcoin limit. |
| 34–41 | Solid project with known gaps. | Half position; list the gaps and re-check quarterly. |
| 26–33 | Speculative. Several important unknowns. | "Lottery ticket" size only (≤1% of crypto allocation), or pass. |
| Below 26 | You are guessing. | Pass. Revisit only if the score changes. |

**Section weighting for tie-breaks:** if two tokens score the same, prefer the one stronger in sections 2 (tokenomics), 5 (security), and 6 (liquidity). Those are where money is lost quickly; sections 1, 4, and 7 are where money is lost slowly.

**Re-check triggers:** a major unlock, a governance change to fees or emissions, a change in admin key setup, a hack anywhere in the same category, or the token doubling or halving since your last review.

---

## Sources

- [Token Terminal — Fundamentals for crypto](https://tokenterminal.com/) (fees, revenue, user metrics; standardized KPIs)
- [DefiLlama — Hacks database](https://defillama.com/hacks) (exploit categories: key compromise, oracle manipulation, access control, bridge)
- [RugCheck](https://rugcheck.xyz/) (Solana token risk: holder concentration, liquidity, insider activity, metadata)
- [Revoke.cash — What are token approvals?](https://revoke.cash/learn/approvals/what-are-token-approvals)
- [Chainalysis — 2025 Crypto Crime Report introduction](https://www.chainalysis.com/blog/2025-crypto-crime-report-introduction/) (private key compromises as the largest share of stolen funds)
- [Ledger Academy — Token approvals explained](https://www.ledger.com/academy/topics/security/ethereum-token-approvals-explained)
- [FTC — What to know about cryptocurrency and scams](https://consumer.ftc.gov/articles/what-know-about-cryptocurrency-scams)
