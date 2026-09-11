# Bitcoin Valuation Frameworks

**In one sentence:** Bitcoin has no cash flows, so every valuation model is really a story about adoption or scarcity dressed in numbers, and the useful ones (realized cap, MVRV, liquidity, production cost) describe where the market *is* rather than predicting where it *goes*.

## Why this is hard

A stock can be valued by discounting the cash it will pay you. Bitcoin pays nothing. Its value rests entirely on what others will pay for it in the future, which depends on how many people want a scarce, censorship-resistant, bearer digital asset and how much of their wealth they want in it. That's an adoption question, not an accounting one, and every framework below is an attempt to make adoption measurable. Keep two things in mind throughout: correlation with past prices is not prediction, and the models that fit best historically are often the ones that failed hardest afterward.

Context as of September 2026: Bitcoin trades in the high $70,000s with a market cap of roughly $1.55 trillion, about 38% below its all-time high of roughly $126,000 (intraday) set on October 6, 2025. It fell below its 200-week moving average (then roughly $62,000) in late June 2026 and has since recovered above it.

## 1. Digital gold and the market-cap-of-gold comparison

The oldest framework. If Bitcoin is a better store of value than gold (more scarce, more portable, more verifiable, more divisible), it should eventually capture some share of gold's monetary premium. Gold's above-ground stock is worth roughly $30 trillion at September 2026 prices (~$4,390/oz across ~216,000 tonnes), so:

| Share of gold's market cap | Implied BTC market cap | Implied price (~19.9m BTC) |
|---|---|---|
| 5% (roughly today) | $1.5t | ~$75,000 |
| 10% | $3t | ~$150,000 |
| 25% | $7.6t | ~$380,000 |
| 100% | $30t | ~$1.5m |

This is the framework behind most large-institution price targets, including ARK's and various sell-side notes. Its strength is that it names the thing you're betting on: monetary premium migration. Its weaknesses are that gold's market cap isn't fixed (gold roughly doubled in dollar terms between 2023 and 2026, moving the goalposts), that the share Bitcoin "should" capture is entirely a matter of opinion, and that it says nothing about timing.

## 2. Metcalfe's law and network-value models

Metcalfe's law says a network's value scales with the square of its users. Ken Alabi (2017) and Timothy Peterson (2018) fit Bitcoin's market cap to the square of active addresses and found tight historical fits; Peterson's version treated the halving-driven supply schedule as an input and produced a formula that tracked price well through 2017. Later analysts fit variants using unique addresses, transaction counts, or a "network value to transactions" (NVT) ratio, which is market cap divided by daily on-chain transaction value and is used like a P/E: high NVT means price has run ahead of usage.

What these models capture: Bitcoin's value has grown with its user base, and NVT spikes have flagged some tops. What they miss: active addresses are a poor proxy for users (one exchange can be millions of users behind one address; one person can be thousands of addresses), the "n²" exponent is an assumption that later work found closer to 1.5 for real networks, and the fits are in-sample. Metcalfe models tell you Bitcoin is a network good; they don't tell you the next user's arrival date.

## 3. Stock-to-flow, and why it failed

Stock-to-flow (S2F) is the ratio of existing supply to annual new supply. Gold's is about 60; Bitcoin's doubles each halving and was around 120 after April 2024. In 2019 the pseudonymous analyst PlanB regressed Bitcoin's market cap on S2F and found a striking log-linear fit, then extrapolated: an average price above $100,000 during the 2020–2024 halving epoch, and in the "S2FX" cross-asset version, $288,000.

What happened: Bitcoin did reach $69,000 in November 2021 and then fell to $15,500 in 2022, spending the entire epoch far below the model's band. The model's 2021 year-end target above $100,000 was missed, and by late 2022 price was roughly 90% below the model line. PlanB later reset the model's parameters; critics noted that a model which needs re-fitting after each miss has no predictive content.

The deeper critiques, made before the failure by Nico Cordeiro (Strix Leviathan), Vitalik Buterin, and others: supply is only half a price; demand is the other half, and S2F ignores it entirely. The regression has few effective data points (three halvings) and a spurious-regression problem because both series trend. It implies price rises forever regardless of what anyone does, which is a claim about the world, not a model. And gold's stable S2F has coexisted with decades of flat real prices, which the model can't explain.

The "power law" model (Giovanni Santostasi and others), which fits log price against log time, is the current successor: it has a good in-sample fit and a similar structure of unfalsifiable-until-it-isn't. Treat both as descriptions of the past.

## 4. Realized cap, MVRV, and cost-basis models

**Realized capitalization**, introduced by Coin Metrics' Nic Carter and Antoine Le Calvez in 2018, values every coin at the price when it last moved on-chain rather than at today's price. It approximates the aggregate cost basis of all holders and is far less volatile than market cap. **Realized price** is realized cap divided by supply.

**MVRV** = market cap ÷ realized cap. Above 1, the average holder is in profit; below 1, in loss. The **MVRV Z-score** standardizes the gap by historical volatility. Historically, Z-scores above roughly 7 coincided with cycle tops (2013, 2017, 2021) and below 0 with cycle bottoms (2015, 2018–19, March 2020, late 2022). The 2025 top produced a lower peak Z-score than prior cycles, which some read as a maturing asset and others as the indicator losing power.

Related metrics from the same family: **short-term and long-term holder realized price** (cost basis of coins moved within/beyond 155 days), **SOPR** (spent output profit ratio, whether coins being sold are in profit), and **net unrealized profit/loss**. These are the metrics Lyn Alden and most on-chain analysts actually use, because they describe holder behavior rather than assert a price target. See `on-chain-analysis-basics.md`.

Limits: realized cap is distorted by lost coins (valued at ancient prices), by exchange internal transfers, and by ETF custody (coins that move once into a custodian and never again). Thresholds drift as the asset matures.

## 5. Production cost and miner models

Miners spend electricity and hardware to produce coins, so production cost should act as a soft floor: when price falls below marginal cost, inefficient miners shut off, hashrate falls, and selling pressure from miners drops. Charles Edwards' "hash ribbons" and various "miner cost basis" estimates formalize this.

The evidence: bear-market bottoms in 2015, 2018, 2020, and 2022 came near or below estimated average production cost, and miner capitulation (hashrate dropping sharply) has been a decent bottom signal. But causality runs the wrong way for prediction: production cost adjusts *to* price via difficulty, with a lag. Liu and Tsyvinski's academic study found production-cost measures had no predictive power for returns. Use miner data to gauge stress, not to set a floor.

## 6. Lyn Alden's frameworks

Alden's work combines three lenses rather than one model:

1. **Global liquidity.** A study she commissioned (Sam Callahan, 2024) found Bitcoin moved in the same direction as global M2 in 83% of rolling 12-month periods, more than any other major asset (the S&P 500 was about 73%), with a long-run correlation of 0.94 from 2013 to 2024 but much weaker correlations over 6-month windows. Bitcoin, in this view, is a "liquidity barometer," and the times it decouples are idiosyncratic shocks (exchange collapses, regulatory hits) or valuation extremes.
2. **MVRV Z-score as the override.** When the Z-score is stretched, internal dynamics (profit-taking or capitulation) dominate macro. She uses on-chain valuation to know when to distrust the liquidity signal.
3. **Adoption as an S-curve**, with Bitcoin still in the early-majority phase by global ownership metrics, which frames the long-run bet as adoption, not scarcity.

This is the most defensible framework in this file precisely because it's not a price model. It tells you what regime you're in.

## 7. Adoption curves

Compare Bitcoin's user growth to the internet's or mobile phones'. Depending on the survey, somewhere between 4% and 7% of the world's adults own some crypto as of the mid-2020s, which on a technology S-curve puts it around where the internet was in the late 1990s. Spot ETFs (approved January 2024; roughly $55 billion of cumulative net inflows and about $103 billion of assets by early September 2026, with BlackRock's IBIT the largest) and corporate treasuries are the current adoption channels, and their flows explain much of 2024–25 price action.

The framework is honest about what it is: a bet that adoption continues. It offers no help on price within a cycle.

## What none of them can tell you

- **Timing.** Every model above is either a long-run trend or a regime descriptor. None has predicted a cycle top or bottom out-of-sample with usable precision.
- **Whether the adoption thesis is right.** Bitcoin could stall at 5% of gold or reach 100%; the models just multiply your assumption.
- **What happens when structure changes.** ETFs, corporate holders, and lower volatility have already altered the amplitude of cycles (the 2025 peak was a ~240% year-over-year gain versus 1,000%+ in earlier cycles). Models fit to the old regime may be quietly wrong.
- **Tail risks.** A protocol bug, a quantum-computing breakthrough, or a coordinated ban wouldn't appear in any of these frameworks until after the fact.

## How to actually do it

1. Decide what you believe about adoption: what share of gold's monetary premium, or what share of global portfolios, over what horizon. Write it down; that's your thesis.
2. Use realized price, MVRV Z-score, and long-/short-term holder cost basis to locate the current price within the cycle. Free versions are on LookIntoBitcoin and Glassnode's public charts.
3. Check the liquidity regime: is global M2 expanding or contracting? Alden's and CrossBorder Capital's work is the reference.
4. Note miner stress (hashrate trend, hash ribbons) as a secondary bottom signal.
5. Ignore S2F and power-law price targets except as a reminder of how confident wrong models sound.
6. Size the position for the possibility that the adoption thesis is wrong, because no framework here rules it out.

## Key takeaways

- Bitcoin has no cash flows; every model is an adoption or scarcity story in disguise.
- The gold comparison names the bet clearly but can't tell you the share or the timing.
- Stock-to-flow made a specific forecast, missed by more than half, and was re-fit; that's disqualifying for a predictive model.
- Realized cap and MVRV describe holder cost basis and have flagged prior extremes, but thresholds drift.
- Production cost adjusts to price, not the other way round; miner stress is a sentiment gauge.
- Alden's liquidity-plus-MVRV approach is a regime detector, and that's the most any of these can honestly claim.
- As of September 2026: high $70,000s, ~$1.55 trillion, roughly 38% below the October 2025 high, ETF assets ~$103 billion.

## Sources

- [Lyn Alden: Bitcoin, A Global Liquidity Barometer](https://www.lynalden.com/bitcoin-a-global-liquidity-barometer/)
- [Coin Metrics realized cap metric documentation (GitHub)](https://github.com/coinmetrics/docs-website/blob/master/asset-metrics/market/caprealusd.md)
- [Glassnode: Bitcoin MVRV Z-Score chart](https://studio.glassnode.com/charts/market.MvrvZScore?a=BTC)
- [LookIntoBitcoin: MVRV Z-Score](https://www.lookintobitcoin.com/charts/mvrv-zscore/)
- [CoinGecko: Bitcoin Stock-to-Flow Model Explained](https://www.coingecko.com/learn/bitcoin-stock-to-flow-model-explained)
- [FXStreet: Stock-to-flow model invalidated as BTC closes 2021 below $100,000](https://www.fxstreet.com/cryptocurrencies/news/bitcoin-stock-to-flow-model-invalidated-as-btc-closes-2021-below-100-000-202201010939)
- [CryptoRank: Does the Bitcoin power law model still hold after S2F failed?](https://cryptorank.io/news/feed/868ab-does-the-bitcoin-power-law-model-still-hold-after-stock-to-flow-failed)
- [Giovanni Santostasi: The Bitcoin Power Law Theory](https://giovannisantostasi.medium.com/the-bitcoin-power-law-theory-962dfaf99ee9)
- [Liu & Tsyvinski, Risks and Returns of Cryptocurrency (CEPR summary)](https://cepr.org/voxeu/columns/risks-and-returns-cryptocurrencies)
- [Gold market capitalization (companiesmarketcap.com)](https://companiesmarketcap.com/gold/marketcap/)
- [World Gold Council: Gold market size and structure](https://www.gold.org/goldhub/research/market-primer/gold-market-primer-market-size-and-structure)
- [Fortune: Price of Bitcoin, September 9, 2026](https://fortune.com/article/price-of-bitcoin-09-09-2026/)
- [Spark: Is Bitcoin's Four-Year Cycle Dead?](https://www.spark.money/research/bitcoin-four-year-cycle-dead)
- [Crypto Briefing: Bitcoin drops below 200-week moving average (June 2026)](https://cryptobriefing.com/bitcoin-200-week-moving-average-breakdown/)
- [HedgeCo: Spot Bitcoin ETF flows, September 3, 2026](https://hedgeco.net/news/09/2026/spot-bitcoin-etfs-posted-a-731-million-net-inflow-on-september-3.html)
