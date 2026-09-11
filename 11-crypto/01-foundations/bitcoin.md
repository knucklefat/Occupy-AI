# Bitcoin

**In one sentence:** Bitcoin is a 2009 open-source monetary network with a hard cap of 21 million coins, secured by energy-intensive mining, that its supporters view as "digital gold" and its critics view as a speculative asset with no cash flows; it is now held by U.S. spot ETFs with roughly $100 billion in assets, yet it has fallen by more than half from its peak four separate times.

## Origin

On October 31, 2008, six weeks after Lehman Brothers collapsed, someone using the name Satoshi Nakamoto posted a nine-page paper to a cryptography mailing list titled "Bitcoin: A Peer-to-Peer Electronic Cash System." The paper proposed a way for strangers to send payments online without a bank in the middle, solving the double-spend problem with proof of work (see [How Blockchains Work](how-blockchains-work.md)). The network went live on January 3, 2009. The first block contains a headline from that day's *Times* of London about a bank bailout, widely read as a statement of purpose.

Nakamoto's identity remains unknown; the person stopped communicating in 2011 and is believed to hold roughly 1 million BTC that have never moved. Bitcoin has no company, foundation with control, or CEO. Its rules are enforced by whoever runs its software.

## The 21 million cap and halvings

Bitcoin's supply schedule is written into its code. New coins enter circulation only as rewards to miners who add blocks, and that reward is cut in half every 210,000 blocks, roughly every four years.

| Halving | Date | Block reward before → after |
|---|---|---|
| Launch | Jan 3, 2009 | 50 BTC |
| 1st | Nov 28, 2012 | 50 → 25 |
| 2nd | Jul 9, 2016 | 25 → 12.5 |
| 3rd | May 11, 2020 | 12.5 → 6.25 |
| 4th | Apr 20, 2024 | 6.25 → 3.125 |
| 5th (projected) | ~April 2028 (block 1,050,000) | 3.125 → 1.5625 |

About 19.9 million of the 21 million coins already exist as of September 2026; the last fraction will not be mined until around 2140. Bitcoin's annual supply growth is now below 1%, lower than gold's roughly 1.5–2% mine supply growth. Halvings are the reason supporters call bitcoin "the hardest money ever created," and they have historically preceded price run-ups, though with only four data points the pattern is not statistically robust.

## Mining economics

Miners run warehouses of specialized chips (ASICs) that do nothing but SHA-256 hashing. They are paid in the block subsidy (3.125 BTC per block, roughly $243,000 at a $77,800 bitcoin price) plus transaction fees. As of September 2026:

- Network hashrate is about 930 exahashes per second, down from a peak near 1,160 EH/s in October 2025 as weaker prices pushed marginal miners offline.
- Transaction fees are under 1% of miner revenue. Miners live almost entirely on the subsidy, which raises a long-term question: what pays for security once the subsidy approaches zero? Supporters say fees will rise with adoption; skeptics call it an unsolved problem.
- CoinShares estimated the weighted-average *cash* cost for public miners to produce one bitcoin at roughly $80,000 in late 2025, meaning much of the industry was near or below breakeven during 2026's drawdown.
- Many large public miners (Core Scientific, TeraWulf, Hut 8, IREN) have pivoted part of their capacity to AI and high-performance-computing hosting, which tends to be more profitable per megawatt.

Mining is a brutally competitive, capital-intensive commodity business. Investing in miners is a leveraged bet on bitcoin's price plus a bet on energy costs and management execution; it is not the same as owning bitcoin.

## The "digital gold" thesis

The bull case, articulated by writers such as Lyn Alden and by Fidelity Digital Assets research, runs roughly as follows:

1. Bitcoin is scarce in a way no other asset is; its supply cannot be changed by any government, company, or miner.
2. It is portable, divisible, verifiable, and can be sent anywhere in minutes; gold cannot.
3. Governments run persistent deficits and central banks expand money supply over time, so an asset outside that system should absorb some of the demand for "hard" stores of value.
4. Gold's market value is roughly $20+ trillion; if bitcoin captured even a fraction of that "monetary premium," it would be worth multiples of today's ~$1.3 trillion.
5. Network effects: the longer it survives, the more credible it becomes (the "Lindy effect").

## The critiques

Serious skeptics are not just saying "it's a bubble." Their arguments:

- **No cash flows.** Unlike a stock, bond, or rental property, bitcoin generates nothing. Its value rests entirely on what the next buyer will pay. Warren Buffett and Charlie Munger made this case for years.
- **It has not behaved like gold.** In stress periods (March 2020, 2022) bitcoin fell alongside tech stocks rather than rising as a safe haven. Its correlation to the Nasdaq has been much higher than gold's. "Digital gold" is a thesis about the future, not a description of the past.
- **Volatility disqualifies it as money.** A currency that moves 5% in a day cannot price a coffee or a mortgage. Almost nobody prices goods in bitcoin.
- **Energy.** Bitcoin consumes on the order of 0.5% of global electricity (Cambridge estimates vary). Supporters note much of it is stranded or renewable energy; critics say the externality is unjustified for a settlement layer that handles a few transactions per second.
- **Its price is propped up by leverage and stablecoins of uncertain quality.** Zeke Faux's *Number Go Up* (2023) documents the industry's reliance on Tether, the FTX fraud, and pay-to-earn schemes preying on the poor, arguing much of crypto's "adoption" was speculation and fraud.
- **Concentration.** A small number of addresses hold a large share of supply, and early adopters received coins at fractions of a dollar.

An honest position is that bitcoin is a young, extremely volatile asset whose long-term monetary role is unproven, and whose price is driven by liquidity cycles and sentiment far more than by any fundamental you can model.

## Lightning and how bitcoin is actually used

Because the base chain handles ~7 transactions per second, the **Lightning Network** (launched 2018) lets users open payment channels and settle many small payments off-chain, touching the main chain only to open and close. It works, and is used for tips, remittances in places like El Salvador, and some merchant payments. But it has stayed niche: public channel capacity was about 4,900 BTC in mid-2026 (peak 5,637 BTC in December 2025), node counts have drifted down since 2022, and it requires managing "inbound liquidity," which most users find confusing.

In practice, bitcoin's dominant uses today are:

1. **Store of value / speculation.** The overwhelming majority of volume is trading and holding.
2. **Treasury asset.** Strategy (formerly MicroStrategy) and a wave of imitators hold bitcoin on corporate balance sheets; some U.S. states and the federal government have established strategic reserves.
3. **Collateral** in lending and derivatives markets.
4. **Cross-border value transfer** where banking is unreliable or capital controls bind.
5. Payments, but mostly through stablecoins rather than bitcoin itself.

## The ETF era

For a decade the SEC rejected spot bitcoin ETF applications. After Grayscale won a court case in 2023, the SEC approved eleven spot bitcoin ETFs on January 10, 2024; they began trading the next day. BlackRock's IBIT became the fastest ETF ever to reach $50 billion in assets.

As of early September 2026, U.S. spot bitcoin ETFs held roughly **$103 billion in net assets** with about **$55 billion in cumulative net inflows** since launch (SoSoValue data). IBIT dominates; Fidelity's FBTC and Grayscale's GBTC are next. Spot Ethereum ETFs followed in July 2024 and Solana ETFs in October 2025.

The ETFs changed who owns bitcoin: registered investment advisers, pensions, and retail brokerage accounts can now hold it with no keys to manage. Whether this "financialization" strengthens or undermines bitcoin's anti-establishment thesis is itself debated.

## Volatility history

Bitcoin's price history is a series of parabolic rises and crushing drawdowns. Approximate peak-to-trough declines (daily-average prices across major exchanges, Blockchain.com data; intraday extremes were slightly worse, e.g. the October 6, 2025 intraday high was about $126,000):

| Cycle | Peak | Trough | Drawdown |
|---|---|---|---|
| 2011 | ~$34 (Jun 2011) | ~$2 (Nov 2011) | ~-93% |
| 2013–15 | ~$1,140 (Dec 2013) | ~$170 (Jan 2015) | ~-85% |
| 2017–18 | ~$19,300 (Dec 2017) | ~$3,230 (Dec 2018) | ~-83% |
| 2021–22 | ~$67,600 (Nov 2021) | ~$15,800 (Nov 2022) | ~-77% |
| 2025–26 | ~$124,800 (Oct 2025) | ~$58,500 (Jul 1, 2026) | ~-53% so far |

As of September 10, 2026, bitcoin traded near **$77,800**, with a market capitalization around **$1.55 trillion**, roughly 38% below its October 2025 high and about 30% below its price a year earlier. Anyone allocating to bitcoin should assume a 50%+ drawdown will happen again and size the position so they can hold through it.

## Key takeaways

- Bitcoin is a fixed-supply (21 million) monetary network launched in 2009 with no controlling entity; the next halving is expected around April 2028, cutting the block reward to 1.5625 BTC.
- Miners earn almost entirely from the block subsidy; fees are under 1% of revenue, which is a long-term open question for security funding.
- The "digital gold" thesis rests on scarcity and neutrality; the critiques rest on no cash flows, stock-like correlation in crises, energy use, and dependence on leverage and stablecoins.
- Lightning works but remains small; bitcoin's real use is store-of-value speculation, corporate treasuries, and collateral.
- Spot ETFs (approved January 2024) hold roughly $103 billion as of September 2026 and have made bitcoin a standard brokerage product.
- Bitcoin has lost 77–93% in each of its four prior bear markets and is roughly 38% off its high as of September 2026. Size positions accordingly.
- Mining stocks are not bitcoin; they are leveraged, energy-cost-sensitive operating businesses.

## Sources

- [Bitcoin: A Peer-to-Peer Electronic Cash System (whitepaper)](https://bitcoin.org/bitcoin.pdf)
- [CoinWarz: Bitcoin Halving Countdown](https://www.coinwarz.com/bitcoin-halving)
- [CoinShares: Bitcoin Mining Report Q1 2026](https://coinshares.com/insights/research-data/bitcoin-mining-report-q1-2026/)
- [Cryptolexicon: Difficulty and hashprice, September 2026](https://cryptolexicon.org/en/blog/bitcoin-difficulty-rise-hashprice-jump-september-2026/)
- [HedgeCo: Spot Bitcoin ETFs Posted a $731 Million Net Inflow on September 3, 2026](https://hedgeco.net/news/09/2026/spot-bitcoin-etfs-posted-a-731-million-net-inflow-on-september-3.html)
- [Fortune: Price of Bitcoin, September 10, 2026](https://fortune.com/article/price-of-bitcoin-09-10-2026/)
- [TradingKey: Bitcoin at $65K vs October's $126K All-Time High](https://www.tradingkey.com/analysis/cryptocurrencies/btc/262050150-crypto-bitcoin-btc-etf-ath-price-iran-us-tradingkey)
- [Spark: State of the Lightning Network in 2026](https://www.spark.money/research/lightning-network-2026-state)
- [Cambridge Bitcoin Electricity Consumption Index](https://ccaf.io/cbnsi/cbeci)
- [Lyn Alden: What Is Money, Anyway?](https://www.lynalden.com/what-is-money/)
- [Fidelity Digital Assets: Bitcoin First Revisited](https://www.fidelitydigitalassets.com/research-and-insights/bitcoin-first-revisited)
- [Bits about Money: A review of Number Go Up](https://www.bitsaboutmoney.com/archive/a-review-of-number-go-up-on-crypto-shenanigans/)
- [SEC: Statement on the Approval of Spot Bitcoin Exchange-Traded Products (Jan 2024)](https://www.sec.gov/newsroom/speeches-statements/gensler-statement-spot-bitcoin-011023)
