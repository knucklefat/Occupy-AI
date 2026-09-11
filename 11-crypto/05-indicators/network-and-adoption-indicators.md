# Network and Adoption Indicators

**In one sentence:** Network indicators measure whether the underlying blockchains are actually being used and secured, which matters for long-run value but has a weak and often lagging relationship with price over any horizon shorter than a year.

## The honest framing

Adoption metrics are what a fundamental investor would want: usage, security spend, capital parked in the system. The problem is that crypto prices are driven mostly by flows and liquidity in the short run, and adoption data often follows price rather than leads it (people show up after the rally). So use this page to judge health and long-run thesis, not to time entries.

## Active addresses and transaction counts

**What it measures.** Active addresses is the number of unique addresses that sent or received coins in a day. Transaction count is the number of confirmed transactions. Both are proxies for usage, but imperfect ones: one person can control thousands of addresses, exchanges batch many payments into one transaction, and inscriptions or "dust" spam can inflate counts without any economic meaning.

**Where to get it free.** [Glassnode active addresses](https://studio.glassnode.com/charts/addresses.ActiveCount?a=BTC), [Coin Metrics Network Data Charts](https://charts.coinmetrics.io/), [blockchain.com charts](https://www.blockchain.com/explorer/charts/n-unique-addresses), [Etherscan charts for Ethereum](https://etherscan.io/charts).

**How to read it.** Look at the 30-day trend versus price. Rising price with flat or falling active addresses means the rally is being carried by a shrinking base of participants (often derivatives-driven). Rising addresses during a flat price is a quietly bullish divergence. Bitcoin's active address count has hovered in a 600,000 to 1,000,000-per-day band for most of the past five years; it has not tracked the 2024–25 price rise, largely because activity migrated to ETFs (off-chain) and to exchanges' internal ledgers.

**Track record.** Weak as a timing signal. Historically, active-address peaks came near price peaks (2017, 2021) because retail shows up late, so a sharp spike is more of a caution flag than a buy signal.

## Hash rate and mining difficulty

**What it measures.** Hash rate is the total computing power securing Bitcoin, estimated from block times. Difficulty is the protocol's automatic adjustment every 2,016 blocks (about two weeks) to keep blocks at 10 minutes. Difficulty is the cleaner number because hash rate estimates are noisy day to day.

**Where to get it free.** [mempool.space mining dashboard](https://mempool.space/mining), [CoinWarz difficulty](https://www.coinwarz.com/bitcoin-difficulty), [Hashrate Index](https://hashrateindex.com/), [blockchain.com hash rate](https://www.blockchain.com/explorer/charts/hash-rate).

**How to read it.** Hash rate follows price with a lag of months, because miners order machines when profitable and plug them in later. A falling hash rate signals miner stress (machines switched off), which historically clustered around bear-market bottoms. The popular "hash ribbons" indicator (30-day hash rate crossing back above the 60-day after a contraction) has flagged several good buying windows: early 2019, mid-2020, late 2022.

**As of September 2026.** After briefly crossing 1 zettahash (1,000 EH/s) earlier in the year, the 7-day hash rate sat near 934 EH/s and difficulty adjusted up 1.31% to 127.45T at block 965,664 on September 6, per Cryptolexicon's retarget note. Hash rate has stalled rather than collapsed: miners are squeezed but not capitulating.

**Track record.** Good for identifying miner capitulation at bottoms (contrarian buy), useless for tops. Difficulty going up is not bullish for price; it is bullish for network security and bearish for miner margins.

## Miner revenue and hashprice

**What it measures.** Hashprice is the dollar revenue a miner earns per unit of hash power per day, usually quoted per petahash per second per day ($/PH/day). It combines Bitcoin price, difficulty, block subsidy and fees into one number that tells you whether mining is profitable.

**Where to get it free.** [Hashrate Index hashprice](https://data.hashrateindex.com/chart/bitcoin-hashprice-index), [mempool.space mining](https://mempool.space/mining), [Glassnode miner revenue](https://studio.glassnode.com/charts/mining.RevenueSum?a=BTC).

**How to read it.** When hashprice falls below the operating cost of the median machine (roughly $30 to $40/PH/day for modern fleets at typical power prices, though this varies widely), inefficient miners must sell reserves or shut down. Both are short-term bearish for price and, at the extreme, mark bottoms. As of September 6, 2026, hashprice was about $39.63/PH/day, up 22% over 30 days entirely because price rose, not because fees rose. Transaction fees were only 0.43% of miner revenue, meaning miner income is now nearly a pure function of Bitcoin's price. That fee share is a long-run concern for security economics after future halvings, and it is a number worth watching once a quarter.

**Track record.** Hashprice lows have coincided with price lows; a good confirmation of bear-market capitulation.

## Lightning Network capacity

**What it measures.** Bitcoin locked in public Lightning payment channels, a proxy for real payments adoption on Bitcoin's second layer.

**Where to get it free.** [mempool.space Lightning capacity](https://mempool.space/graphs/lightning/capacity), [1ML](https://1ml.com/statistics), [Amboss](https://amboss.space/).

**How to read it.** Public capacity peaked near 5,637 BTC in December 2025 (a spike tied to exchange integrations) and sat around 4,900 BTC in mid-2026 across roughly 41,000 channels and 17,400 nodes, per Spark's 2026 report. Capacity has been flat-to-down for three years, though private channels (mobile wallets, service providers) are thought to hold two times or more the public figure. Falling public capacity with rising payment volume can mean the network is getting more efficient, not dying.

**Track record.** No relationship with price. This is a thesis-check indicator, not a trading one.

## Stablecoin supply

**What it measures.** Total dollar-pegged stablecoins in circulation. Stablecoins are the "dry powder" and settlement rail of the crypto economy; growth means dollars are entering the system, contraction means they are leaving.

**Where to get it free.** [DefiLlama stablecoins](https://defillama.com/stablecoins), [Stablecoin Beat tracker](https://stablecoinbeat.com/tracker/), [Coin Metrics](https://charts.coinmetrics.io/).

**How to read it.** The 30-day change is the useful number. Sustained expansion has preceded or accompanied every major rally since 2020; the 2022 contraction (Terra collapse, then USDC redemptions) tracked the bear market. Watch the split: USDT growth tends to reflect offshore and emerging-market demand; USDC growth tends to reflect US institutional and DeFi demand. As of September 11, 2026, total supply was roughly $305 to $310 billion depending on the tracker (DefiLlama ~$310 billion; USDT ~$183B, USDC ~$74B), essentially flat over 30 days and below the May 2026 record near $321 billion (mid-June was roughly $314B per Coinlaw). Flat stablecoin supply during a 25% price rally is a mild warning that the August move was driven by short-covering and ETF flows rather than fresh on-chain dollars.

**Track record.** One of the better medium-term adoption signals; it led the 2020–21 and 2023–24 rallies by weeks to months.

## Ethereum gas and Layer-2 activity

**What it measures.** Gas is Ethereum's transaction fee unit; the base fee (in gwei) rises with demand for block space. L2 activity is transactions and value on rollups such as Arbitrum, Base and Optimism, which settle to Ethereum. Since the 2024 Dencun upgrade moved most user activity to L2s, mainnet gas alone understates usage.

**Where to get it free.** [Etherscan gas tracker](https://etherscan.io/gastracker), [L2BEAT](https://l2beat.com/scaling/summary) (L2 value secured and activity), [growthepie](https://www.growthepie.xyz/) (L2 fees, users), [ultrasound.money](https://ultrasound.money/) (ETH issuance vs burn).

**How to read it.** Persistently high base fees (say, 30+ gwei) mean demand is outrunning supply, which usually accompanies speculative manias (NFTs 2021, memecoins 2024). Very low fees (under 5 gwei for weeks) mean quiet demand and, because of Ethereum's fee burn, net-inflationary ETH supply. L2 transactions per second and active addresses on L2BEAT are the better adoption read. For investors the key ratio is: are L2 fees paid back to Ethereum growing, or are L2s capturing the value?

**Track record.** Gas spikes are coincident-to-lagging (they confirm a mania is underway). L2 activity growth is a slow structural signal.

## DeFi Total Value Locked (TVL)

**What it measures.** The dollar value of assets deposited in DeFi protocols (lending, staking, exchanges). It is partly a usage metric and partly just a restatement of price, because most collateral is ETH and BTC.

**Where to get it free.** [DefiLlama](https://defillama.com/), [DefiLlama chain breakdown](https://defillama.com/chains).

**How to read it.** Always look at TVL in native units (ETH, BTC) or compare it to total crypto market cap, otherwise you are just watching price. Rising TVL in a flat market is real adoption; falling TVL in a rising market is capital leaving DeFi. As of September 11, 2026, DefiLlama showed total TVL around $86–88 billion, down from a January 18, 2026 peak of roughly $127 billion and up from a late-June/early-July trough near $68 billion. Lido, Aave and Morpho were the largest protocols; Ethereum still held over half of TVL.

**Track record.** Mostly a price echo. The useful signal is the TVL-to-market-cap ratio and per-chain share shifts.

## Exchange balances

**What it measures.** Coins held in wallets that analysts have tagged as belonging to centralized exchanges. Coins on exchanges are, in theory, available for sale; coins withdrawn are presumed to be going to cold storage.

**Where to get it free.** [CryptoQuant exchange reserve](https://cryptoquant.com/asset/btc/chart/exchange-flows/exchange-reserve), [Glassnode balance on exchanges](https://studio.glassnode.com/charts/distribution.BalanceExchanges?a=BTC), [Coinglass exchange balance](https://www.coinglass.com/Balance).

**How to read it.** The multi-year trend is down: Bitcoin exchange reserves fell from above 3.2 million BTC in 2023 to roughly 2.4 to 2.7 million by March 2026, per CryptoQuant-sourced reporting. Long-run declines reflect self-custody and ETF custody (Coinbase Custody holds ETF coins in wallets that are not counted as "exchange" balances), so a falling balance is not automatically bullish. Short-run spikes of inflows (tens of thousands of BTC in a day) are more useful: they often precede selling. Bear in mind tagging errors: one exchange reshuffling wallets can print a false signal.

**Track record.** The "supply shock" narrative built on falling balances has been oversold; balances fell throughout the 2022 bear market. Short-term inflow spikes have a modest record as sell warnings.

## How to use it

1. Once a month, check five numbers: stablecoin supply 30-day change, hash rate trend, hashprice versus miner break-even, DeFi TVL in ETH terms, and L2 activity. That is your "is the system healthy" scan.
2. Treat rising stablecoin supply as the one adoption metric with some lead on price. Treat everything else as confirmation.
3. Use hash rate and hashprice contractions as a contrarian bottom signal, combined with on-chain valuation readings.
4. Ignore active-address spikes as buy signals; they usually mean retail has arrived late.
5. Normalize everything: TVL in native units, exchange balances as a share of supply, fees as a share of miner revenue.

## Key takeaways

- Network usage metrics describe long-run health, not next month's price; adoption tends to follow price, not lead it.
- Stablecoin supply growth is the exception with some leading value; flat supply during a rally (as in August–September 2026) is a mild caution.
- Hash rate follows price with a lag; miner capitulation (falling hash rate, hashprice under break-even) is a bottom signal, not a top signal.
- Fees are under 1% of Bitcoin miner revenue as of September 2026, a structural issue to watch across future halvings.
- DeFi TVL in dollars is mostly a price echo; measure it in ETH or as a share of market cap.
- Exchange balances have declined for years for structural reasons (ETF custody, self-custody), so "coins leaving exchanges" is not by itself bullish.
- Lightning capacity is a thesis check on Bitcoin-as-payments and has no predictive value for price.

## Sources

- [Cryptolexicon: Difficulty up 1.31%, hashprice up 22% (September 2026)](https://cryptolexicon.org/en/blog/bitcoin-difficulty-rise-hashprice-jump-september-2026/)
- [Bitcoin.com News: Difficulty rises, hashprice rips 22% as hashrate stalls](https://news.bitcoin.com/mining/difficulty-rises-hashprice-rips-22-as-bitcoin-hashrate-stalls/)
- [mempool.space mining dashboard](https://mempool.space/mining)
- [Spark: State of the Lightning Network in 2026](https://www.spark.money/research/lightning-network-2026-state)
- [mempool.space Lightning capacity](https://mempool.space/graphs/lightning/capacity)
- [Stablecoin Beat tracker](https://stablecoinbeat.com/tracker/)
- [Coinlaw: DeFi market statistics 2026](https://coinlaw.io/decentralized-finance-market-statistics/)
- [DefiLlama](https://defillama.com/)
- [KuCoin News: Bitcoin exchange reserves hit multi-year low (March 2026)](https://www.kucoin.com/news/flash/bitcoin-exchange-reserves-hit-all-time-low-amid-shrinking-supply)
- [Coin Metrics Network Data Charts](https://charts.coinmetrics.io/)
- [L2BEAT](https://l2beat.com/scaling/summary)
