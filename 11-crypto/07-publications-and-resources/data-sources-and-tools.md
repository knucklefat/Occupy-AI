# Data Sources and Tools

**In one sentence:** Crypto is the only asset class where a retail investor can see the full ledger, the fund flows, the exchange positioning and the insider unlock schedule for free, so there is no excuse for investing on vibes — the tools below tell you where to look and what each one costs.

## A note on data quality

Crypto data is abundant and often wrong. Exchange volumes are inflated by wash trading (a 2019 Bitwise study found most reported Bitcoin volume was fake; aggregators have since filtered, but not perfectly). "Market cap" for small tokens multiplies a thin price by a supply most of which is locked. On-chain "users" are addresses, not people. The tools below are the best available; the habit that matters is checking a number in two of them before acting on it.

Cost tags: **Free** (fully usable free), **Freemium** (real free tier, paid for depth), **Paid** (free is a teaser).

## Prices, market data and aggregators

| Tool | Cost | Best for | Notes and caveats |
|---|---|---|---|
| [CoinGecko](https://www.coingecko.com/) | Freemium | Prices, market caps, exchange listings, token supply | The default aggregator; better than CMC on small caps and exchange trust scores. Listing does not mean vetting. |
| [CoinMarketCap](https://coinmarketcap.com/) | Freemium | Prices, rankings, historical snapshots | Owned by Binance since 2020, a conflict to keep in mind for exchange rankings. Historical daily snapshots are useful for "what was the top 20 in 2017?" |
| [TradingView](https://www.tradingview.com/) | Freemium | Charting, multi-exchange price feeds, alerts | The industry-standard charting tool; free tier is adequate for most investors. Paid tiers add indicators and alerts. |
| [Kaiko](https://www.kaiko.com/) | Paid (free research) | Institutional-grade tick data, liquidity, spreads | The data vendor institutions use; retail readers should follow the free [research blog](https://research.kaiko.com/) for market-structure insight. |
| [Coinglass](https://www.coinglass.com/) | Freemium | Derivatives: open interest, funding rates, liquidations, long/short ratios | The standard free view into leverage; the liquidation heatmaps are what "the market got liquidated" headlines come from. |
| [Velo](https://velo.xyz/) | Freemium | Cross-exchange derivatives and basis data | A cleaner, more quantitative alternative to Coinglass for futures term structure. |
| [Alternative.me Fear and Greed Index](https://alternative.me/crypto/fear-and-greed-index/) | Free | Sentiment composite | A simple contrarian gauge; extreme fear has historically been a better buy signal than extreme greed a sell signal. |

## Fund flows, ETFs and unlocks

| Tool | Cost | Best for | Notes and caveats |
|---|---|---|---|
| [Farside Investors: Bitcoin ETF Flows](https://farside.co.uk/btc/) | Free | Daily US spot Bitcoin ETF net flows by issuer | The reference table for ETF flows since January 2024; also [Ether ETF flows](https://farside.co.uk/eth/). Updated after US close. |
| [Tokenomist](https://tokenomist.ai/) (formerly TokenUnlocks) | Freemium | Token vesting schedules and upcoming unlocks | The unlock calendar is the single most under-used tool in altcoin investing: large unlocks to VCs and teams are scheduled supply, and prices often weaken into them. Free tier covers the major tokens. |
| [The Block: Data Dashboard](https://www.theblock.co/data) | Free | Exchange volumes, stablecoin supply, ETF and futures data, L2 activity | Well-maintained charts drawn from multiple vendors; a good cross-check. |
| [Bitcoin Magazine Pro](https://www.bitcoinmagazinepro.com/) | Freemium | Bitcoin cycle and valuation charts (MVRV, Puell, stock-to-flow and others) | Note that Bitcoin Magazine's parent is maximalist; the charts are fine, the "models" are curve fits. |
| [Look Into Bitcoin](https://www.lookintobitcoin.com/) | Free | Bitcoin on-chain and cycle indicators, explained | Each chart has a plain-English explanation of what the indicator is and when it has and has not worked. |

## On-chain analytics

| Tool | Cost | Best for | Notes and caveats |
|---|---|---|---|
| [Glassnode](https://glassnode.com/) | Freemium | Bitcoin and Ethereum holder behaviour, supply distribution, realized metrics | The leader in on-chain metrics; the free tier (via [Glassnode Studio](https://studio.glassnode.com/)) covers the basics with a lag. Paid tiers are expensive. |
| [CryptoQuant](https://cryptoquant.com/) | Freemium | Exchange inflows/outflows, miner flows, stablecoin reserves | Strong on exchange and miner data; the community dashboards are hit-and-miss. |
| [Coin Metrics: Community Charts](https://charts.coinmetrics.io/) | Free | Network data (active addresses, fees, supply, realized cap) across many assets | The free community version of an institutional dataset; the best free source for clean, documented network metrics. |
| [Dune](https://dune.com/) | Freemium | Custom SQL queries and community dashboards on EVM, Solana and Bitcoin data | If you want to know how many wallets used a protocol last week, someone has built a Dune dashboard. Free to browse; learning to write queries is the single most useful crypto research skill. |
| [Nansen](https://www.nansen.ai/) | Paid (limited free) | Labeled wallets ("smart money"), token flows, fund holdings | Labels are the value; it is expensive, and "smart money" labels are inferred, not verified. |
| [Arkham Intelligence](https://intel.arkm.com/) | Free | Entity-labeled wallets and portfolios (exchanges, funds, governments, individuals) | Free and surprisingly deep; also runs a controversial bounty market for de-anonymizing wallets, which is an ethical issue and a signal about the company's incentives. |
| [Artemis](https://www.artemis.xyz/) | Freemium | Cross-chain fundamentals: fees, revenue, active users, developer counts | A clean "fundamentals terminal" for comparing chains; good for the "which chains actually earn fees?" question. |
| [Token Terminal](https://tokenterminal.com/) | Freemium | Protocol revenue, fees, P/S-style ratios for tokens | The closest thing to financial statements for protocols; use it to see which tokens have any cash flow at all. |
| [DefiLlama](https://defillama.com/) | Free | DeFi total value locked, protocol fees and revenue, stablecoin supply, hacks, airdrops, yields | Open-source, ad-free, no token; the most trusted free DeFi data source. The [hacks page](https://defillama.com/hacks) and [stablecoins page](https://defillama.com/stablecoins) are references in their own right. |
| [L2Beat](https://l2beat.com/) | Free | Ethereum layer-2 TVL, risk assessment, decentralization stage | The honest scorecard on how "trustless" each rollup actually is; the risk framework is more useful than the TVL number. |
| [growthepie](https://growthepie.xyz/) | Free | Layer-2 usage, fees and economics, visualized | Complements L2Beat with activity and revenue data. |
| [ultrasound.money](https://ultrasound.money/) | Free | Ethereum issuance, burn and supply | Built by Ethereum advocates (the name is a meme), but the numbers are on-chain facts. |
| [rated.network](https://rated.network/) | Free | Ethereum validator and staking-operator performance | For anyone staking or evaluating a staking provider. |
| [CryptoFees](https://cryptofees.info/) | Free | Daily fees paid on each chain and protocol | A one-page answer to "which of these things do people pay to use?" |

## Block explorers and network monitors

| Tool | Cost | Best for | Notes and caveats |
|---|---|---|---|
| [mempool.space](https://mempool.space/) | Free | Bitcoin mempool, fee estimation, block visualization, [Lightning network explorer](https://mempool.space/lightning) | Open-source and self-hostable; the Bitcoin explorer to use. Shows you why your fee estimate was wrong. |
| [Etherscan](https://etherscan.io/) | Free | Ethereum transactions, contracts, token holders, [gas tracker](https://etherscan.io/gastracker) | The standard EVM explorer; verify contract source, read token-holder distribution before buying. Sister sites: [Arbiscan](https://arbiscan.io/), [Basescan](https://basescan.org/). |
| [Solscan](https://solscan.io/) | Free | Solana transactions, tokens, accounts | The main Solana explorer. |
| [Blockchain.com Explorer](https://www.blockchain.com/explorer) | Free | Multi-chain lookups, long historical Bitcoin charts | Fine as a second opinion; mempool.space is better for Bitcoin. |
| [OKLink](https://www.oklink.com/) | Free | Multi-chain explorer | Owned by the OKX exchange; broad chain coverage. |
| [Bitnodes](https://bitnodes.io/) | Free | Reachable Bitcoin nodes by country and version | For "how decentralized is it, really?" arguments. |
| [Clark Moody Bitcoin Dashboard](https://bitcoin.clarkmoody.com/dashboard/) | Free | Everything about Bitcoin's current state on one page | Price, mempool, hashrate, Lightning capacity, difficulty; a Bitcoiner's terminal. |
| [Timechain Index](https://timechainindex.com/) | Free | Bitcoin entity and wallet clustering | Independent alternative to Arkham for Bitcoin address labels. |
| [Amboss](https://amboss.space/) and [1ML](https://1ml.com/) | Free | Lightning Network nodes and channels | For running or evaluating Lightning liquidity. |
| [BTC Map](https://www.btcmap.org/) | Free | Merchants accepting Bitcoin, worldwide | The best answer to "does anyone actually spend it?" (Answer: some, unevenly.) |
| [beaconcha.in](https://beaconcha.in/) | Free | Ethereum consensus-layer (validators, epochs, slashings) | The explorer for the staking side of Ethereum. |
| [Chainlist](https://chainlist.org/) | Free | Verified RPC endpoints for adding networks to a wallet | Use this instead of copying RPC details from a random tweet; maintained by DefiLlama. |

## Portfolio, wallet safety and scam checks

| Tool | Cost | Best for | Notes and caveats |
|---|---|---|---|
| [revoke.cash](https://revoke.cash/) | Free | Viewing and revoking token approvals on EVM chains | Old approvals are how drained wallets get drained; check monthly and after using any new dapp. |
| [DeBank](https://debank.com/) | Free | Multi-chain portfolio view, wallet history, protocol positions | The cleanest free portfolio tracker for EVM wallets; also a social layer you can ignore. |
| [Zapper](https://zapper.xyz/) | Free | Portfolio tracking and DeFi position management | Similar to DeBank; use whichever reads your positions correctly. |
| [Rugcheck](https://rugcheck.xyz/) | Free | Solana token risk report (mint authority, freeze authority, top-holder concentration, LP lock) | Run every Solana memecoin through this before buying; a bad score is disqualifying, a good score is not an endorsement. |
| [GoPlus Token Security](https://gopluslabs.io/token-security) | Free | EVM token contract risk scan (honeypot, hidden mint, tax, blacklist) | Automated; catches the obvious traps. |
| [Honeypot.is](https://honeypot.is/) | Free | Simulates whether a token can be sold after buying | The single question that matters for a new token contract. |
| [De.Fi Scanner](https://de.fi/scanner) | Free | Contract and wallet risk scanner | Another automated check; use more than one. |
| [Token Sniffer](https://tokensniffer.com/) | Free | EVM token audit scores and similar-contract detection | Good at flagging copy-paste scam contracts. |
| [SlowMist Hacked](https://hacked.slowmist.io/) | Free | Database of every major hack and exploit | Check a protocol's history before depositing. |
| [Chainabuse](https://www.chainabuse.com/) | Free | Report and look up scam addresses | Run by TRM Labs; check a payment address before sending. |
| [CryptoScamDB](https://cryptoscamdb.org/) | Free | Blacklist of scam domains and addresses | Older and less maintained, still useful. |
| [ScamSniffer](https://scamsniffer.io/) | Free | Phishing-site detection, wallet-drainer tracking | Publishes the running total of funds lost to wallet drainers; a browser extension is available. |
| [DEX Screener](https://dexscreener.com/) | Free | Real-time DEX pair charts and liquidity across chains | Where new-token trading actually shows up; the "liquidity" and "top holders" panels are the risk check. |
| [GeckoTerminal](https://www.geckoterminal.com/) | Free | DEX pair data (CoinGecko's on-chain product) | Alternative to DEX Screener. |
| [Bitcoin Who's Who](https://bitcoinwhoswho.com/) | Free | Bitcoin address reputation and scam reports | Check an address before paying an invoice. |

## Research terminals

| Tool | Cost | Best for | Notes and caveats |
|---|---|---|---|
| [Messari](https://messari.io/) | Freemium | Asset profiles, fundraising data, governance trackers, research | The profiles are the best quick overview of a token's supply, team and history; note that some reports are commissioned by the projects. |
| [CoinGecko Learn](https://www.coingecko.com/learn) and [CoinMarketCap Alexandria](https://coinmarketcap.com/alexandria/) | Free | Beginner explainers | Aggregator-written; fine for definitions, promotional for products. |
| [Rekt Leaderboard](https://rekt.news/leaderboard/) | Free | Ranked list of DeFi exploits by size | Read the post-mortems before trusting a protocol category. |

## Suggested daily and weekly routine

- **Daily (five minutes):** Coinglass funding and open interest; Farside ETF flows; Fear and Greed.
- **Weekly (thirty minutes):** DefiLlama TVL and fees; Tokenomist unlocks for anything you hold; revoke.cash if you used a new dapp; Coin Metrics or Glassnode weekly.
- **Before buying any token:** CoinGecko supply and exchange listing; Etherscan or Solscan holder distribution; Tokenomist unlock schedule; Rugcheck or GoPlus scan; Rekt and SlowMist history; Messari profile for team and raise.
- **Before sending money anywhere:** Chainabuse and Bitcoin Who's Who on the address; ScamSniffer on the domain.

## Key takeaways

- The best free data stack is DefiLlama, Coin Metrics community charts, Dune, mempool.space, Etherscan and Farside; paid tools add labels and depth, not truth.
- Token unlock schedules (Tokenomist) and holder concentration (explorers) are the two data points retail investors most often skip and most often regret skipping.
- Check volumes and market caps in two aggregators; wash trading and locked supply make single-source numbers unreliable.
- Approval hygiene (revoke.cash) and pre-trade contract scans (Rugcheck, GoPlus, Honeypot.is) prevent most of the losses that no amount of market analysis would.
- Ownership matters: CoinMarketCap belongs to Binance, OKLink to OKX, Bitcoin Magazine Pro to a maximalist publisher; know who runs the tool you trust.
