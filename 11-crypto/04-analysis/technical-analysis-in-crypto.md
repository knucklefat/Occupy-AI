# Technical Analysis in Crypto

**In one sentence:** Crypto is the market where technical analysis is most heavily used and least rigorously tested, so keep the parts with evidence behind them (trend, momentum, positioning data from derivatives) and treat the rest (chart patterns, Fibonacci levels, indicator crossovers) as shared folklore that works mainly because everyone is watching it.

## How crypto markets differ from equities

- **24/7 trading.** There is no close, no gap, no weekend. Daily candles are a convention (most platforms use 00:00 UTC), and "weekly close" carries weight only because traders agree it does. Weekend volume is thinner, so weekend moves are more often reversed.
- **Fragmented venues.** Price forms across dozens of exchanges plus on-chain DEXs. Index prices (Coinbase, Binance, CME) can differ by tens of dollars, which matters for exact "support" levels.
- **Derivatives dominate.** Perpetual futures ("perps," futures with no expiry that use a funding payment to track spot) account for the majority of volume. Positioning in perps drives short-term moves more than spot flows do.
- **Retail-heavy, leverage-heavy.** Retail share is higher than in equities and leverage of 20–100× is offered freely, so forced liquidations are a structural feature.
- **Macro correlation has risen.** Bitcoin's correlation with the Nasdaq reached about 0.9 in late 2025, so crypto charts increasingly inherit equity-market rhythms including the US session open and Fed days.

## What carries over from equities

The evidence base for TA in equities is thin but not empty: time-series momentum and trend-following have decades of out-of-sample support, and volume-confirmed breakouts do somewhat better than unconfirmed ones. Both translate to crypto.

**Momentum.** Liu and Tsyvinski (Review of Financial Studies, 2021) found that a one-standard-deviation increase in Bitcoin's weekly return predicted about a 3% higher return the following week, and that cross-sectional momentum (buying recent winners among coins) earned abnormal returns in their sample. Investor attention (Google searches, social volume) predicted returns too. Later work is mixed: a 2025 study found crypto momentum "has (not) its moments," with profits concentrated in a few periods and vulnerable to transaction costs and crashes. The fair reading is that trend persistence exists in crypto, is stronger than in equities, and is also more prone to violent reversals.

**Moving averages as trend filters.** A simple rule such as "hold when price is above the 200-day (or 20-week) moving average, otherwise cash" has historically captured most of Bitcoin's upside while sidestepping the worst of its 75–85% drawdowns, at the cost of whipsaws in ranging markets. This is trend-following, not prophecy, and its value is risk management rather than return.

**The 200-week moving average.** Bitcoin's 200-week simple moving average is the most-cited long-term level in crypto. Across the 2015, 2018–19, and 2022 bear markets, price bottomed at or slightly below it, and it rose continuously because Bitcoin's four-year trailing average has never fallen. In late June 2026, Bitcoin closed weekly candles below the 200-week MA (then about $62,000) for the first time since June 2022, trading $58,000–62,000, before recovering to around $79,000 by September. In 2022 the same breach preceded a further slide to $15,500 and more than a year below the average. Whether the 2026 breach was a bottom or a 2022 repeat was the central chart debate of mid-2026, which illustrates the point: the level is a reference, not a rule.

**What doesn't carry over well.** Equity TA leans on the daily close, gaps, and session structure. Crypto has none, except CME Bitcoin futures, which do gap over weekends. The "CME gap" (price tending to revisit the level where the futures closed Friday) is one of the few crypto-specific patterns with a plausible mechanism (arbitrage between CME and spot), though it's inconsistent.

## Derivatives data as TA inputs

This is where crypto TA has an edge over equities: positioning data is public and real-time.

| Input | Definition | How it's read | Caveat |
|---|---|---|---|
| **Funding rate** | Periodic payment between perp longs and shorts that keeps the perp near spot. Positive = longs pay shorts (market leaning long). | Extreme positive funding (annualized >50–100%) marks crowded longs and precedes flushes; deeply negative funding marks crowded shorts and precedes squeezes. | Funding is the *cost* of a position, so it mean-reverts by design; it's contrarian at extremes, not directional in the middle. |
| **Open interest (OI)** | Total notional of open perp/futures contracts. | Rising OI with rising price = new longs entering (trend fuel and liquidation fuel). Rising OI with falling price = new shorts. Sharp OI drops = liquidation cascade just happened. | Denominate in coins, not dollars, or price moves masquerade as positioning changes. |
| **OI / market cap** | Leverage in the system relative to the asset. | High readings = fragile; a small move can cascade. | Threshold varies by asset. |
| **Liquidation heatmaps** | Estimated price levels where leveraged positions will be force-closed, inferred from OI and typical leverage. Coinglass and Hyblock publish them. | Dense liquidation clusters act as magnets: price often runs to them, triggers the stops, and reverses. | They are estimates, not order-book data; the estimate becomes partly self-fulfilling because traders target the clusters. |
| **Long/short ratio** | Share of accounts (or notional) long vs short. | Contrarian at extremes. | Account-based ratios overweight small retail positions. |
| **Basis (futures premium)** | Annualized spread between dated futures and spot. | High basis = bullish leverage and expensive to hold longs; negative basis (backwardation) = fear. | CME basis reflects institutional demand and is more informative than offshore basis. |

A useful combined read: price makes a new high, OI in coin terms is at a record, funding is strongly positive, and the liquidation heatmap shows a dense cluster of long liquidations 5% below. That is a market that will fall fast on any excuse. The same configuration inverted (crowded shorts, negative funding, short liquidation cluster above) precedes squeezes. Neither tells you *when*, but both tell you where the air pockets are.

## Common chart-pattern traps

- **Pattern hindsight.** Head-and-shoulders, cup-and-handle, and wedges are identified after the move and rarely tested out-of-sample. In a 24/7 market with no session structure, they're even less reliable than in equities.
- **Timeframe shopping.** Any thesis can be supported on some timeframe. Decide the timeframe before you look.
- **Round numbers and psychological levels.** They matter because everyone places orders there, which also makes them the levels most likely to be swept by a few dollars before reversing (the "stop hunt").
- **Indicator stacking.** RSI, MACD, and stochastics are all transformations of the same price series; three agreeing signals are one signal.
- **Fibonacci retracements.** No mechanism, wide levels, and enough of them that one always "works."
- **Fractal overlays** ("2021 vs 2025 chart looks identical") are the purest form of pattern-matching noise and get shared most at turning points.
- **Volume on CEXs is unreliable.** Wash trading was endemic on smaller exchanges; use a trusted-exchange volume index (CoinGecko's "trust score" filter, Kaiko, or CME volume).
- **Thin-liquidity wicks.** A single large market order on a weekend can print a wick 5% beyond the "real" range; that isn't a level.

## The evidence, summarized

| Claim | Evidence | Verdict |
|---|---|---|
| Time-series momentum / trend persistence | Academic (Liu & Tsyvinski) plus decades of trend-following results in other assets | Real, but crash-prone |
| Cross-sectional momentum among coins | Academic support, weaker after costs and post-2021 | Real but fragile |
| Attention predicts short-term returns | Academic support | Real, decays fast |
| Funding/OI extremes as contrarian signals | Mechanistic (forced deleveraging), widely observed | Real for timing risk, not direction |
| 200-week MA as a floor | Three data points | Useful reference; not a law |
| Chart patterns, Fibonacci, indicator crossovers | Mostly anecdotal | Folklore; works to the extent others trade it |
| Production cost or mining data predicting price | Academic: no predictive power | No |

## How to actually do it

1. Pick a timeframe and a rule set before opening the chart. Write both down.
2. Use a trend filter (e.g., price vs 20-week or 200-day MA) as a regime gate for how much risk you carry, not as an entry signal.
3. Check funding, OI in coin terms, and the liquidation heatmap on Coinglass before any leveraged position. If you're joining a crowded side, size down or wait.
4. Treat round numbers and prior highs as areas where stops cluster; expect sweeps.
5. Use CME futures data (OI, basis, gaps) for the institutional view and offshore perps for the retail view.
6. Never trade a pattern without a mechanism. If you can't explain why the pattern should work (forced flows, positioning, information), it's decoration.
7. Keep a journal with entry rationale and outcome. Most TA edges vanish in a journal.

## Key takeaways

- Crypto trades 24/7 on fragmented venues dominated by leveraged perps, so positioning data matters more than in equities.
- Momentum and trend persistence have academic support in crypto and are stronger than in stocks, but reverse violently.
- The 200-week MA has marked three bear-market bottoms; the June 2026 breach was the first since 2022.
- Funding rates and open interest are contrarian at extremes and tell you where the leverage is, not which way price goes.
- Liquidation heatmaps are estimates that become partly self-fulfilling.
- Chart patterns, Fibonacci, and stacked indicators are folklore; use them only as maps of where other people's orders sit.
- A trend filter for position sizing is the one TA tool most investors should actually use.

## Sources

- [Liu & Tsyvinski, Risks and Returns of Cryptocurrency (Review of Financial Studies, 2021)](https://academic.oup.com/rfs/article-abstract/34/6/2689/5912024)
- [Liu & Tsyvinski, Risks and Returns of Cryptocurrency (CEPR VoxEU summary)](https://cepr.org/voxeu/columns/risks-and-returns-cryptocurrencies)
- [Liu, Tsyvinski & Wu, Common Risk Factors in Cryptocurrency (Journal of Finance, 2022)](https://onlinelibrary.wiley.com/doi/abs/10.1111/jofi.13119)
- [Cryptocurrency momentum has (not) its moments (Financial Markets and Portfolio Management, 2025)](https://link.springer.com/article/10.1007/s11408-025-00474-9)
- [Crypto Briefing: Bitcoin drops below 200-week moving average for first time since 2022 (June 2026)](https://cryptobriefing.com/bitcoin-200-week-moving-average-breakdown/)
- [CoinDesk: Why a $58,000 bitcoin is the key number (February 2026)](https://www.coindesk.com/markets/2026/02/02/why-a-usd58-000-bitcoin-is-the-key-number-for-crypto-investors-right-now)
- [Coinglass: liquidation heatmaps, funding, open interest](https://www.coinglass.com/)
- [Spark: Is Bitcoin's Four-Year Cycle Dead? (Nasdaq correlation, volatility data)](https://www.spark.money/research/bitcoin-four-year-cycle-dead)
