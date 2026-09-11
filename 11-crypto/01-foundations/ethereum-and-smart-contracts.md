# Ethereum and Smart Contracts

**In one sentence:** Ethereum is a blockchain that runs programs ("smart contracts") as well as moving money, which makes it the settlement layer for most of stablecoins, DeFi, and tokenized assets; it switched to proof of stake in 2022, pushed most user activity to cheaper "Layer 2" networks, and now competes with faster, more centralized chains like Solana on the question of whether the base layer or the apps on top capture the value.

## What a smart contract is

Bitcoin's ledger records one thing: who owns how many coins. Ethereum, launched in July 2015 by Vitalik Buterin and others, generalized the idea. Its ledger can store small programs, and anyone can call those programs by sending a transaction. Once deployed, the code runs exactly as written on every node in the network, and nobody, including its author, can stop it or change it unless the code itself allows for that.

A "smart contract" is therefore neither smart nor a contract in the legal sense. It is an automated escrow agent: "if X happens, move Y." Practical examples:

- A **token contract** keeps a table of balances and lets holders transfer them. USDC, USDT, and nearly every "altcoin" on Ethereum are just token contracts (the ERC-20 standard).
- An **exchange contract** (Uniswap) holds two tokens in a pool and lets anyone swap one for the other at a formula-set price.
- A **lending contract** (Aave) accepts deposits, lends them out against collateral, and liquidates borrowers automatically if collateral falls too far.

The upside is that financial plumbing becomes open, composable, and available 24/7 without intermediaries. The downside is that code bugs are irreversible: the 2016 DAO hack drained about $60 million and forced a chain split; the February 2025 Bybit theft (~$1.5 billion, attributed to North Korea's Lazarus Group) exploited a signing interface, not the blockchain, but it illustrates that the surrounding software is as important as the chain.

## Gas: paying for computation

Every operation on Ethereum costs **gas**, a unit of computational work. Users pay gas in ETH. The price of gas floats with demand: a simple transfer might cost under a dollar on a quiet day and $50+ during a frenzy (2021 NFT mania, memecoin spikes). Gas is what stops someone from spamming the network with an infinite loop; the program runs out of fuel and stops.

For an investor, gas fees are Ethereum's revenue. When the network is busy, fees rise, and (since 2021) most of that fee is destroyed, benefiting all ETH holders.

## EIP-1559 and the fee burn (August 2021)

Before 2021, fees were a blind auction paid entirely to miners. EIP-1559 (Ethereum Improvement Proposal 1559) introduced a protocol-set **base fee** that rises and falls with demand and is **burned** (permanently removed from supply), plus an optional tip to the block producer. About 4.6 million ETH had been burned cumulatively by mid-2026.

## The Merge (September 15, 2022) and staking

The Merge switched Ethereum from proof of work to proof of stake. Mining stopped; issuance of new ETH fell by roughly 88% overnight. Security is now provided by validators who lock 32 ETH each.

As of August 2026:

- About **34% of all ETH is staked** (roughly 42.6 million ETH, per ethereum.org), up from roughly 29% at the start of the year, spread across roughly a million validator slots (the exact count changes daily and has been falling as large stakers consolidate under Pectra's 2,048 ETH cap).
- Base staking yield is about **2.6–2.7%**, or roughly 3.1–3.3% including tips and MEV (value extracted by ordering transactions). Yields fall as more ETH is staked because the reward pool is shared more widely.
- **Lido**, a liquid-staking protocol, controls about 23% of staked ETH (down from a 32% peak in 2023); Binance and Coinbase hold roughly 3.7 million and 2.9 million ETH respectively. Critics point out that a few operators controlling a third of stake is not the decentralization the design promised.
- A proposal (EIP-8361, August 2026) would taper rewards as staking participation rises to discourage over-staking; if adopted, yields could fall toward 1.2%.

Staking is the closest thing crypto has to a dividend: ETH holders can earn a yield paid in ETH for securing the network. But it is paid partly by inflation, and staked ETH carries slashing risk, smart-contract risk (if done via Lido), and liquidity risk (unstaking queues have run 50 days or more).

## "Ultrasound money" and its unraveling

After the Merge, supporters argued ETH had become "ultrasound money": with issuance cut and fees burned, ETH supply would shrink whenever the network was busy, making it deflationary while still paying a yield. For about 18 months (September 2022 to March 2024) it worked; supply fell by roughly 450,000 ETH.

Then the **Dencun upgrade (March 13, 2024)** gave Layer 2 networks a cheap way to post their data ("blobs"), and activity migrated off the base chain. Base fees collapsed to under 1 gwei, the burn dried up, and ETH turned inflationary from April 2024 onward. Supply now grows about 0.2% a year (about 120.5+ million ETH in 2026). Validator rewards create close to a million ETH a year against a burn of only a few tens of ETH per day on quiet days.

The critique from investors like those at Bankless and elsewhere is sharp: Ethereum deliberately gave away its fee revenue to Layer 2s to scale, and the L2s (Base is owned by Coinbase; Arbitrum and Optimism by venture-backed foundations) keep the sequencer fees. ETH the asset benefits from L2 activity only indirectly, through blob fees and the demand to hold ETH as collateral. Whether this "L2-centric roadmap" was a strategic masterstroke or a value-accrual mistake is the central debate about ETH as an investment.

## Layer 2s: rollups

A **rollup** processes transactions on its own chain, then posts compressed data and either a fraud proof or a validity proof back to Ethereum. Users get fees of a fraction of a cent to a few cents while inheriting (most of) Ethereum's security.

| Rollup | Type | Operator | Notes |
|---|---|---|---|
| **Base** | Optimistic | Coinbase | ~47% of L2 DeFi TVL (Feb 2026); over 1 million daily active addresses; no token |
| **Arbitrum One** | Optimistic | Offchain Labs / Arbitrum DAO | ~31% of L2 DeFi TVL; ARB token |
| **OP Mainnet** | Optimistic | Optimism Foundation | ~6%; OP token; its "OP Stack" software powers Base and others |
| **zkSync Era, Starknet, Linea, Scroll** | ZK (validity proofs) | Various | Faster withdrawals, harder engineering; smaller TVL |

"Optimistic" rollups assume transactions are valid and allow a ~7-day challenge window; "ZK" rollups prove validity with cryptography up front. In January 2026, Arbitrum, OP Mainnet, and Base all reached "Stage 1" on L2Beat's decentralization ladder, meaning working fraud proofs with a security council backstop. Most L2s still run a single "sequencer" (the computer ordering transactions), a centralization risk. Of 50+ rollups launched, only a handful have meaningful usage; Base and Arbitrum together account for roughly three-quarters of L2 activity.

## Ethereum vs. Solana and other Layer 1s

Solana (launched 2020) made the opposite design choice: one fast base chain with higher hardware requirements, no Layer 2s. It became the home of memecoin trading and much retail activity in 2024–25.

| | Ethereum (L1) | Solana | Notes on others |
|---|---|---|---|
| Consensus | Proof of stake | Proof of stake + proof of history | Avalanche, Sui, Aptos, Cardano all PoS |
| Real-world throughput | ~15–20 TPS on L1; thousands across L2s | ~600–700 TPS actual (65,000 theoretical) | Sui/Aptos claim high TPS, less proven |
| Typical fee | Variable; L2s $0.01–$1 | ~$0.00025 | BNB Chain low fees, Binance-controlled |
| Validators | roughly 1 million-plus validator slots (about 42.6 million ETH staked; the slot count has been falling since Pectra allowed consolidation up to 2,048 ETH), run by tens of thousands of operators | ~675 active vote accounts (Solana RPC, September 2026), down from ~800 in early 2026 and 2,500+ in 2023 | Fewer validators = faster but more centralized |
| Hardware to validate | Consumer machine | High-end server | Barrier to entry is the tradeoff for speed |
| DeFi TVL | ~$38 billion L1 (June 2026), plus L2s | ~$8 billion (April 2026) | Tron is large in stablecoin transfers |
| Staking rate / yield | ~34% staked; ~2.6–3.3% | ~65% staked; ~6–7% (higher inflation) | |
| Outage history | No halts since 2022 | Several full outages 2021–24; last major one Feb 6, 2024 (~5 hours) | |
| Spot ETF | Yes (July 2024) | Yes (October 2025) | |
| Bull case | Most secure, most liquidity, institutional default | Speed and cost enable consumer apps | |
| Bear case | Value leaks to L2s; slow governance | Centralization; reliance on a few clients; memecoin-driven activity | |

Other L1s worth knowing: **BNB Chain** (Binance's chain, high volume, centralized), **Tron** (dominant for USDT transfers in emerging markets), **Avalanche**, **Sui**, **Aptos**, **Cardano**, and **Hyperliquid** (an app-specific chain for derivatives; see [DeFi Explained](defi-explained.md)). History suggests most "Ethereum killers" fail: roughly 65% of the July 2021 top-100 tokens that dropped out were L1/L2 chains marketed as alternatives.

## How to think about ETH as an investment

ETH is priced as a hybrid: part commodity (needed to pay gas), part capital asset (staking yield), part monetary asset (collateral in DeFi). Unlike bitcoin, it has a plausible cash-flow story via fees and burn, but that story weakened after Dencun. The bull case is that tokenized stocks, stablecoins, and institutional settlement all land on Ethereum and its L2s, bringing fees back. The bear case is that Ethereum becomes a low-margin data-availability utility while apps and L2s capture the profits, and that Solana or a newer chain takes the consumer activity. ETH traded around $2,460 on September 10, 2026, well below its November 2021 high near $4,900.

## Key takeaways

- Smart contracts are self-executing programs on the blockchain; tokens, exchanges, and lending protocols are all just contracts. Bugs are irreversible.
- Gas is Ethereum's fee mechanism and, via EIP-1559, most fees are burned, benefiting ETH holders.
- The Merge (Sept 2022) moved Ethereum to proof of stake; about 34% of ETH is staked earning ~2.6–3.3% as of 2026, with Lido and exchanges holding a concerning share.
- "Ultrasound money" held for 18 months, then the Dencun upgrade (March 2024) pushed activity to L2s and ETH turned mildly inflationary again.
- Rollups (Base, Arbitrum, Optimism, plus ZK chains) are where most users transact; Base and Arbitrum dominate, and most L2s have a centralized sequencer.
- Solana trades decentralization for speed and cost; it has fewer validators and a history of outages but far cheaper transactions.
- Whether value accrues to ETH or leaks to L2s and apps is the central unresolved question for ETH investors.

## Sources

- [Ethereum.org: Introduction to smart contracts](https://ethereum.org/en/developers/docs/smart-contracts/)
- [Ethereum.org: Gas and fees](https://ethereum.org/en/developers/docs/gas/)
- [Ethereum.org: The Merge](https://ethereum.org/en/roadmap/merge/)
- [Ethereum.org: Layer 2 rollups](https://ethereum.org/en/developers/docs/scaling/)
- [EIP-1559 specification](https://eips.ethereum.org/EIPS/eip-1559)
- [The Block: Ethereum staking climbs to 34% (Aug 2026)](https://www.theblock.co/news/ecosystems/2026-08-12-ethereum-staking-climbs-34-proposal-targets-validator-rewards-eth-treasury-firm-yields-411312)
- [Datawallet: Ethereum Staking Statistics (2026)](https://www.datawallet.com/crypto/ethereum-staking-statistics-and-trends)
- [BloFin Academy: ETH and ultrasound money, the honest 2026 status](https://blofin.com/academy/education/eth-ultrasound-money)
- [BlockEden: Layer 2 Consolidation War (Feb 2026)](https://blockeden.xyz/blog/2026/02/11/layer-2-consolidation-war-base-arbitrum/)
- [L2Beat: Layer 2 risk analysis](https://l2beat.com/scaling/summary)
- [CoinLaw: Solana vs Ethereum Statistics 2026](https://coinlaw.io/solana-vs-ethereum-statistics/)
- [BeInCrypto: Nearly 3 in 4 tokens that ever cracked the top 100 are dead (CryptoRank)](https://beincrypto.com/top-100-crypto-tokens-dead/)
- [Fortune: Price of Bitcoin, September 10, 2026 (includes ETH)](https://fortune.com/article/price-of-bitcoin-09-10-2026/)
- [CNBC: Hackers steal $1.5 billion from Bybit (Feb 2025)](https://www.cnbc.com/2025/02/21/hackers-steal-1point5-billion-from-exchange-bybit-biggest-crypto-heist.html)
