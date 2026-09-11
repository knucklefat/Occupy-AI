# On-Chain Analysis Basics

**In one sentence:** Public blockchains publish every transaction and balance, which lets you measure holder behavior, exchange flows, and network usage directly instead of guessing, but only if you understand what an address is, what it isn't, and how easily the raw numbers mislead.

## What on-chain data is

Every Bitcoin or Ethereum transaction is recorded in a public ledger anyone can download or query. That ledger tells you, for each unit of the asset, when it last moved, at what price, to what kind of address, and (with labeling) roughly who controls it. No other asset class exposes its ownership ledger this way. Equity analysts wait for 13F filings months after the fact; on-chain analysts see the transfer as it confirms.

The catch is that the ledger records *addresses*, not people. One person can have thousands of addresses; one address (an exchange's cold wallet) can represent millions of people. Every metric below is an attempt to infer human behavior from address behavior, and every one of them can be fooled.

## Block explorers: the raw view

- **mempool.space** (Bitcoin): shows pending transactions waiting to be mined (the "mempool"), fee rates, block contents, and lets you look up any address or transaction. The fee-rate view is the best real-time gauge of Bitcoin network demand.
- **Etherscan** (Ethereum) and its forks (Arbiscan, Basescan, Polygonscan): address balances, token holdings, contract source code, "Holders" tabs for any token, labeled addresses for exchanges and protocols, and an "Analytics" tab per address.
- **Solscan / Solana Explorer** for Solana, **Tronscan** for Tron, and so on.

Explorers are where you verify claims: a project says its treasury holds $50 million? Look at the wallet. A token says 40% is locked? Find the vesting contract. A "burn" happened? Check the null address.

## Key metrics and what they actually measure

| Metric | Definition | What it's used for | How it misleads |
|---|---|---|---|
| **Active addresses** | Unique addresses sending or receiving in a period | Network usage trend | Bots, airdrop farmers, exchange batching; one user ≠ one address |
| **Transaction count** | Transactions per day | Usage trend | Inscriptions, spam, and consolidation transactions inflate it; batching deflates it |
| **Transfer volume (adjusted)** | Value moved, filtered for self-sends and change outputs | Economic throughput; input to NVT | Exchange internal shuffles; unadjusted figures are meaningless |
| **Realized cap / realized price** | Sum of each coin valued at its last-moved price | Aggregate cost basis; MVRV | Lost coins at ancient prices; custodial coins that never move |
| **MVRV and MVRV Z-score** | Market cap ÷ realized cap, and its standardized form | Cycle extremes (see `bitcoin-valuation-frameworks.md`) | Thresholds drift as the asset matures; 2025 peak Z was lower than prior tops |
| **SOPR** | Ratio of sale price to purchase price of coins being spent | Whether sellers are realizing profit or loss; >1 = profit | Noisy daily; use 7-day averages and short-term-holder variant |
| **HODL waves** | Supply bucketed by time since last move (1d–1w, 1w–1m, ..., 5y+) | Accumulation vs distribution; long-term holder conviction | Custody migrations (e.g., ETF inflows) reset ages without a change in beneficial owner |
| **Realized cap HODL waves** | Same, weighted by realized value | Shows when new money enters at high prices (short bands swelling near tops) | Same custody issue |
| **Long-/short-term holder supply** | Coins held more or less than 155 days | LTH distribution near tops, accumulation near bottoms | The 155-day cutoff is a convention |
| **Exchange balances / netflows** | Coins held on labeled exchange addresses; daily in/out | Rising inflows = potential sell pressure; falling balances = withdrawal to self-custody | Depends entirely on labeling quality; exchanges move cold wallets; derivative collateral distorts |
| **Whale holdings** | Supply in addresses above a threshold (e.g., 1,000 BTC) | Large-holder accumulation/distribution | Exchanges and custodians look like whales; ETF custodians hold hundreds of thousands of BTC in a few addresses |
| **Miner flows / hashrate** | Coins moving from miner-labeled addresses; network hashrate | Miner stress and capitulation | Miners often sell through OTC desks not visible as exchange inflows |
| **Stablecoin supply and exchange stablecoin balances** | Total issued; amount sitting on exchanges | "Dry powder" waiting to buy | Stablecoins on exchanges also serve derivatives margin and market makers |
| **Coin days destroyed** | Coins moved × days they'd been dormant | Old-holder activity | A single old wallet consolidating creates a spike |

## Tools, and what each is good at

- **Glassnode**: the most complete Bitcoin and Ethereum metric library, with excellent documentation in Glassnode Academy and its docs site. Free tier covers basics; the advanced metrics (cohort cost basis, SOPR variants) are paid.
- **CryptoQuant**: strongest on exchange flows and miner data; its exchange reserve and netflow charts are widely cited.
- **Coin Metrics**: institutional data provider, originators of realized cap; rigorous methodology notes and a free community feed.
- **Dune**: SQL over decoded blockchain data. Anyone can write or fork a dashboard, so it's the best source for protocol-specific questions (retention cohorts, fee breakdowns, holder distributions). Quality varies by author; check the query.
- **Nansen**: labeled wallets ("smart money," funds, exchanges) and token-flow tracking; best for seeing who is buying a token, useful mainly on EVM chains and Solana.
- **Arkham**: entity-level labeling and visualization of wallet relationships; strong for tracking foundations, governments, and hacker wallets.
- **Bubblemaps**: visual clustering of token holders to spot hidden concentration.
- **LookIntoBitcoin, Checkonchain, Bitcoin Magazine Pro**: free curated Bitcoin cycle charts.
- **DefiLlama, Artemis, Token Terminal**: protocol-level aggregates (see `protocol-fundamentals-and-revenue.md`).

## Worked example: reading an exchange-inflow spike

Suppose CryptoQuant shows 40,000 BTC (about $3.2 billion at $79,000) flowing into exchanges in a day, ten times the average. The headline reading is "whales preparing to dump." Before acting:

1. **Which exchange?** Check the per-exchange breakdown. If it's one address at one venue, it's probably an internal wallet reorganization or a custodian moving coins, not a thousand sellers.
2. **Which cohort?** Was the moving supply old (coin days destroyed spiked) or recent? Old coins moving to an exchange is more meaningful than coins bought last week.
3. **Was it sold?** Watch the next 48 hours of exchange balance. If balance rises and stays, the coins are sitting there; if it falls back, they were withdrawn, which often means a custody transfer.
4. **Did price react?** If $3.2 billion hit the order books and price didn't move, it wasn't sold on the open market.
5. **Corroborate**: check Arkham for a label on the source address; check funding rates and open interest for a derivatives-hedging explanation.

Most spikes turn out to be steps 1 or 3. The metric was true; the inference was wrong.

## How to avoid misreading on-chain data

- **Labels are guesses.** Exchange and entity labels come from heuristics and manual tagging. Different providers give different exchange balances for the same day; disagreement of 10–20% is normal.
- **Custody changes look like behavior changes.** When an ETF buys coins and moves them to Coinbase Custody, HODL waves reset and "whale addresses" grow, with no change in economic ownership.
- **Denominate correctly.** A rising dollar transfer volume in a bull market may be flat in BTC terms.
- **Don't confuse the mempool with demand.** Inscription and token-minting fads have driven Bitcoin fees and transaction counts without any change in monetary demand.
- **Beware survivorship in signals.** A metric that "called every bottom" has usually been re-parameterized after each cycle, and the version that called 2015 isn't the version that called 2022.
- **Use cohorts, not totals.** Short-term versus long-term holder behavior tells you more than aggregate flows.
- **Smart money is only smart until the label is public.** Nansen-style "smart money" wallets are followed by thousands of bots; front-running them is crowded.
- **Fee-paying activity beats address counts.** An address that pays $50 in fees is a user; ten thousand that pay $0.001 are a script.

## How to actually do it

1. Bookmark one raw explorer per chain you care about and one aggregator (Glassnode or CryptoQuant for Bitcoin; Dune plus Nansen or Arkham for tokens).
2. For Bitcoin cycle work, track four charts weekly: MVRV Z-score, short-term-holder SOPR, long-term-holder supply change, and exchange net position change. Don't act on any one alone.
3. For a token, verify treasury and vesting wallets on the explorer, run a holder-concentration check on Bubblemaps, and find a Dune dashboard for retention.
4. When a metric spikes, run the five-step exchange-inflow checklist above before drawing a conclusion.
5. Read the methodology page for any metric before using it. Glassnode's docs and Coin Metrics' notes explain the heuristics.
6. Keep a log of your on-chain calls and what happened. Most people discover they were pattern-matching noise.

## Key takeaways

- On-chain data is unique to crypto and genuinely useful, but it records addresses, not people.
- Realized cap, MVRV, SOPR, HODL waves, and holder cohorts are the core Bitcoin toolkit; exchange flows and miner data are secondary.
- Labels are heuristics and providers disagree; custody migrations masquerade as behavior.
- Verify project claims (treasury, locks, burns) directly on the explorer.
- An exchange-inflow spike is a question, not an answer; check the venue, cohort, subsequent balance, and price response.
- Prefer cohort and fee-weighted metrics over raw counts.
- Log your calls; on-chain analysis is easy to overfit in hindsight.

## Sources

- [mempool.space: Bitcoin explorer and mempool visualizer](https://mempool.space/)
- [Etherscan](https://etherscan.io/)
- [Glassnode Docs: HODL Waves](https://docs.glassnode.com/guides-and-tutorials/metric-guides/age-distribution/hodl-waves)
- [Glassnode Docs: Realized Cap HODL Waves](https://docs.glassnode.com/guides-and-tutorials/metric-guides/age-distribution/realized-cap-hodl-waves)
- [Glassnode Docs: MVRV Ratio](https://docs.glassnode.com/guides-and-tutorials/metric-guides/mvrv/mvrv-ratio)
- [Glassnode: Realized Price and MVRV chart](https://studio.glassnode.com/charts/realizedprice-mvrv?a=BTC)
- [Coin Metrics: realized cap metric definition](https://github.com/coinmetrics/docs-website/blob/master/asset-metrics/market/caprealusd.md)
- [LookIntoBitcoin: Realized Price](https://www.lookintobitcoin.com/charts/realized-price/)
- [CryptoQuant](https://cryptoquant.com/)
- [Dune Analytics](https://dune.com/)
- [Nansen](https://www.nansen.ai/)
- [Arkham Intelligence](https://www.arkhamintelligence.com/)
- [Bubblemaps](https://bubblemaps.io/)
