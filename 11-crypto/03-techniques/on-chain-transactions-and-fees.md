# On-Chain Transactions and Fees

**In one sentence:** Every on-chain send is final, priced by a live auction for block space, and only valid on the network it was sent on — so learn to read the fee market, pick the right chain for the job, and verify three things (address, network, amount) before you press confirm.

## How a send actually works

1. Your wallet builds a transaction: inputs (where the coins come from), outputs (recipient and change), and a fee.
2. The hardware wallet signs it offline; you approve on its screen.
3. It is broadcast to the network's **mempool** — the waiting room of unconfirmed transactions.
4. Miners/validators pick transactions for the next block, highest fee-per-byte first.
5. After enough blocks (bitcoin: ~1 for small amounts, 6 for large; Ethereum: ~15 minutes to full finality; Solana: seconds) the transfer is settled.

There is no "cancel" once a transaction is confirmed. Before confirmation there are limited tools (RBF, CPFP — below), but the safe assumption is: **once broadcast, it is gone.**

## Bitcoin fees: sat/vB

Bitcoin fees are priced in **satoshis per virtual byte (sat/vB)** — you pay for the *size* of your transaction in bytes, not the amount sent. Sending $10 million costs the same as $10 if the transaction is the same size. A typical single-input, two-output SegWit send is ~140 vB; a Taproot one is slightly smaller; one with 50 inputs is huge (see UTXO consolidation in [dollar-cost-averaging-execution.md](dollar-cost-averaging-execution.md)).

| Condition (2026) | Fee rate | Cost of a ~140 vB send at $100k BTC |
|---|---|---|
| Quiet (most weekends/nights in 2026) | 1–3 sat/vB | $0.15–$0.40 |
| Normal | 5–20 sat/vB | $0.70–$2.80 |
| Congested (inscription waves, panic selling) | 50–300+ sat/vB | $7–$40+ |

As of September 2026, the median bitcoin fee has hovered around $0.30 and the average under $1 — historically cheap. That will not always be true; 2024 saw brief spikes above $100 per transaction.

**mempool.space** is the standard dashboard: it shows the current fee needed for next-block, ~30-minute, and ~1-hour confirmation, plus the backlog. Most wallets pull the same estimates and let you pick a priority. Set "economy" for a transfer to your own cold storage; pay "high priority" only when timing matters.

Two rescue tools if you underpaid:

- **RBF (replace-by-fee):** rebroadcast the same transaction with a higher fee; your wallet must support it and the original must have been flagged replaceable.
- **CPFP (child pays for parent):** spend the unconfirmed output with a high-fee child transaction so miners take both. More advanced; use carefully.

## Ethereum fees: gas

Ethereum prices computation in **gas**. Cost = gas used × gas price, where gas price = base fee (set by the protocol, burned) + priority tip (to the validator), quoted in **gwei** (one-billionth of an ETH). A simple ETH transfer uses 21,000 gas; a token transfer ~65,000; a DeFi swap 150,000–300,000.

Mainnet gas has collapsed since activity moved to Layer 2s: mid-2026 averages around 0.5 gwei, so a simple transfer costs a few cents and a token transfer ~$0.10 — versus $5–$50 in 2021–2024 peaks. Gas still spikes during major launches; the cheapest windows are typically 02:00–06:00 UTC and weekends.

**Layer 2s (L2s)** — Base, Arbitrum, Optimism, zkSync — batch thousands of transactions and post them to Ethereum, so a transfer costs ~$0.01–$0.05. For most users, L2s are where ETH-ecosystem activity should happen; keep mainnet for large settlements and long-term storage.

Two gotchas on Ethereum-family chains:

- You must hold the chain's **native gas token** (ETH on mainnet and most L2s) to send *anything*, including stablecoins. Sending USDC to a fresh wallet with no ETH strands it until you add gas.
- **Signature requests** are not always transfers; some are approvals or `permit` messages that let a contract move tokens later. Read them (see the OPSEC file).

## Choosing a network for stablecoins

USDT and USDC exist on many chains. The *same* dollar token on a different network is a different asset for transfer purposes — send USDC on Solana to an Ethereum address and it is gone.

| Network | Typical transfer cost (2026) | Finality | Notes |
|---|---|---|---|
| **Tron (TRC-20)** | $0–$1 (fees paid in "energy"; up to ~$1–$4 if you hold no TRX/energy) | ~1 min | Dominant for USDT remittances in Asia/LatAm; heavily used by illicit flows, so some U.S. exchanges restrict it |
| **Ethereum mainnet (ERC-20)** | $0.10–$2 in 2026 lulls; $5–$15+ when busy | ~13–16 min full finality | Deepest liquidity, most exchange support; best for large amounts |
| **Solana (SPL)** | <$0.01 | ~seconds | Very cheap and fast; make sure the receiving exchange supports the token on Solana |
| **Base** | ~$0.01–$0.05 | Seconds (soft), 7-day window to withdraw to L1 | Coinbase-aligned L2; free/near-free USDC moves between Coinbase and Base |
| **Arbitrum / Optimism / Polygon** | ~$0.01–$0.10 | Seconds (soft) | Widely supported; check exchange deposit support per chain |

Decision rule: **use whichever network both the sender and the receiver explicitly support for that exact token**, then prefer the cheaper one. Exchange withdrawal pages list supported networks per asset; match them exactly. When in doubt, Ethereum mainnet is the safest default for large amounts, and an L2 or Solana for small ones.

Also note that exchanges charge their own **withdrawal fee** on top of network cost, and it differs by chain (e.g., $1 to withdraw USDT on Tron vs ~$0.10 on Solana or Arbitrum at some venues).

## Bridging: the riskiest thing most users do

A **bridge** moves value between chains, usually by locking tokens on one side and minting a wrapped version on the other. Bridges have been the single most exploited category in crypto: Ronin ($624M, 2022), BNB Bridge ($568M, 2022), Wormhole ($326M, 2022), Nomad ($190M, 2022), Harmony ($100M, 2022) — well over $2.8 billion cumulative, roughly 69% of all DeFi theft by some counts.

Risk ranking, safest to riskiest:

1. **Don't bridge.** Withdraw from an exchange directly onto the target chain. Exchanges are de facto bridges with much better security.
2. **Canonical/native bridges** (the official Arbitrum, Optimism, Base bridges) — inherit Ethereum security but L2→L1 withdrawals take ~7 days.
3. **Native token issuance** (USDC via Circle's CCTP burns and re-mints real USDC) — no wrapped IOU.
4. **Third-party bridges** with large validator sets, staked collateral, and long incident-free history.
5. Anything new, fast, and yield-boosted.

If you must bridge: small test first, verify the destination token is the *native* version (not "bridged USDC.e"), and never leave value sitting in a wrapped asset longer than needed.

## Irreversibility: the pre-send checklist

- **Address:** verified on the hardware wallet screen, character-by-character including the middle; sourced from an address book or QR, never transaction history.
- **Network:** matches what the recipient supports for this exact token.
- **Amount and asset:** correct token, correct decimals; you are not sending the entire balance including gas.
- **Memo/tag:** XRP, XLM, ATOM, and some exchange deposits require a destination tag; a missing tag can mean a support ticket and weeks of delay, or loss.
- **Gas available:** you hold enough native token for the fee.
- **Test transaction** done and confirmed for any new destination.

## How to actually do it

1. Open mempool.space (bitcoin) or your wallet's fee estimate (Ethereum/L2). Note the economy vs priority rates.
2. In the sending wallet, paste or scan the recipient address; compare on the hardware device screen.
3. Confirm the network selector matches the recipient's supported network for that token.
4. Send a small test (a few dollars); wait for confirmation on a block explorer (mempool.space, Etherscan, Solscan).
5. Send the balance with an appropriate fee: economy for self-transfers, higher when the recipient needs speed.
6. Save the transaction ID (hash) in your records with date, amount, fee, and purpose.
7. For stablecoins, prefer L2s or Solana for small transfers and mainnet for large ones; avoid third-party bridges by withdrawing from an exchange onto the destination chain directly.

## Key takeaways

- Bitcoin fees are per byte (sat/vB), not per dollar; Ethereum fees are gas × gwei; L2s cost cents.
- In 2026 both bitcoin and Ethereum mainnet fees are historically cheap, but spikes return without warning — watch mempool.space.
- Same token, different network = different asset; match the recipient's supported network exactly.
- You need the chain's native token for gas, even to send stablecoins.
- Bridges have lost more than $2.8 billion to hacks; withdraw directly to the target chain instead.
- Test transactions and on-device verification are the only undo button crypto has.
- Log the transaction hash for every send; it is your receipt for taxes and disputes.

## Sources

- [mempool.space — bitcoin mempool and fee explorer](https://mempool.space/)
- [The complete guide to bitcoin transaction fees in 2026 (99Bitcoins)](https://99bitcoins.com/cryptocurrency/bitcoin/fees/)
- [What is sats/vB? (Sazmining)](https://www.sazmining.com/blog/what-is-sats-vb)
- [Ethereum gas fees in 2026: how to cut costs with layer 2 and timing (Coinpaprika)](https://coinpaprika.com/education/ethereum-gas-fees-in-2026-how-to-cut-costs-with-layer-2-and-timing/)
- [Stablecoin transfer cost comparison by chain (Spark, 2026)](https://www.spark.money/tools/stablecoin-transfer-cost-comparison)
- [Cheapest way to send USDT: network fee comparison 2026 (Eco)](https://eco.com/support/en/articles/15010637-cheapest-way-to-send-usdt-network-fee-comparison-2026)
- [Bridge security comparison: trust models and track records (Spark, 2026)](https://www.spark.money/tools/bridge-security-comparison)
- [Chainlink: 7 cross-chain bridge vulnerabilities explained](https://chain.link/education-hub/cross-chain-bridge-vulnerabilities)
- [Ethereum.org: Security and scam prevention](https://ethereum.org/en/security/)
