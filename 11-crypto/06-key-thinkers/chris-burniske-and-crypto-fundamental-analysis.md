# Chris Burniske and Crypto Fundamental Analysis

**In one sentence:** Chris Burniske's 2017 book *Cryptoassets* gave the industry its first serious attempt at fundamental valuation — treating tokens as a new asset class and valuing them with the equation of exchange — and the decade since has shown which parts of that toolkit survive contact with real markets and which were elegant math applied to assets that didn't behave.

## Who he is

Burniske led ARK Invest's crypto research from 2014, where he helped make ARK the first public fund manager to gain Bitcoin exposure (via the Grayscale trust in 2015). In October 2017 he and Jack Tatar published *Cryptoassets: The Innovative Investor's Guide to Bitcoin and Beyond*, and that year he co-founded **Placeholder**, a venture fund, with Joel Monegro — author of the influential "Fat Protocols" thesis (2016) that value in crypto would accrue to base-layer protocols rather than to applications built on them. Placeholder invested in projects like Decred, Zcash, Filecoin, Aave, The Graph, and Balancer. His incentives are those of a long-only crypto VC: he profits when tokens he holds appreciate, and he is candid about being a "cycle" investor who trims and re-enters.

## Core framework

**1. Cryptoassets are a new asset class, not just "currencies."** The book proposed a taxonomy: *cryptocurrencies* (money: Bitcoin, Monero), *cryptocommodities* (raw digital resources: Ethereum's compute, Filecoin's storage), and *cryptotokens* (finished goods and services). This framing — that most tokens are claims on a network's resource, not money — has aged better than almost anything else in the book.

**2. Value a network with the equation of exchange.** Borrowing from monetary economics: **M × V = P × Q**, where M is the size of the token's monetary base, V is velocity (how many times each token changes hands per year), P is the price of the resource being provisioned, and Q is the quantity provisioned. Rearranged, **M = PQ / V**. Estimate how much economic activity a network will support (PQ), estimate how often tokens turn over (V), and you get the total value the token supply must carry. Discount it back to today, and you have a "current utility value." Burniske's September 2017 essay "Cryptoasset Valuations" walked through this for a hypothetical storage network.

**3. Speculative value vs. utility value.** Any token's price equals current utility value plus a speculative premium for expected future utility. Early in a network's life, nearly all price is speculation — which Burniske called the "crypto J-curve": price rises on hype, collapses when utility disappoints, then rises again as real utility catches up.

**4. Network metrics as fundamentals.** Daily active addresses, transaction volume, developer activity, and the NVT ratio (network value divided by on-chain transaction value, proposed by Willy Woo in 2017 as a crypto P/E ratio) as the equivalent of revenue and earnings.

## What held up

- **The taxonomy.** Treating most tokens as commodity-like claims on network resources, rather than as money, is now the default framing for serious analysts and even regulators.
- **The J-curve.** Ethereum (2018–2020), Solana (2022–2024), and most surviving layer-1s traced exactly this shape.
- **Network fundamentals matter over long horizons.** Chains with real usage (Ethereum, Solana, Tron for stablecoins) retained value; chains with none (EOS, most 2017 ICOs) went to near-zero regardless of their token models.
- **Supply schedules and inflation** as inputs: analysts still start with emission rates and float.
- **Cycle awareness.** Burniske's public calls at the extremes — including his October 2025 warning that the October 10 liquidation cascade had "broken crypto for a while," and his November 2025 comment that the era of digital-asset-treasury selling had only begun — preceded a 23% drop in Bitcoin that November.

## What didn't hold up

- **MV = PQ as a pricing tool.** The "velocity problem" (raised by Vitalik Buterin and Kyle Samani in late 2017) is fatal in practice: if a token is only a medium of exchange, users hold it as briefly as possible, velocity goes toward infinity, and value goes toward zero. Velocity is unobservable in advance and endogenous — it depends on the price it is supposed to explain. Most attempts produced utility values a tiny fraction of market prices, which told you the market was speculative but not what to pay.
- **Fat Protocols.** Monegro's thesis that base layers capture most value was half right (Bitcoin, Ethereum) and half wrong: applications like Uniswap, Hyperliquid, and stablecoin issuers (Tether, Circle) generate far more revenue than most layer-1s, and Ethereum's rollups pushed fee capture *away* from the base token.
- **NVT and address counts** are easily gamed by spam transactions and exchange shuffling, and are distorted by stablecoins moving on-chain.
- **The 2017 cohort.** Many of the assets used as examples in *Cryptoassets* (and some Placeholder investments) lost 90–99% and never recovered; the framework didn't protect against picking the wrong networks.
- **Timing.** Burniske said bear-market callers were misguided in February 2025; Bitcoin fell about 25% into April before rallying to new highs in October. Being early is the occupational hazard of the framework.

## Criticisms

- **Physics envy.** Applying a macroeconomic identity to a token with no observable velocity gave a false sense of precision; some critics, including Austrian economists, argued the entire quantity-theory framing misunderstands why money is held.
- **Talking his book.** As a VC, Burniske benefits from the "new asset class" framing that justified institutional allocations to tokens his fund holds.
- **Survivorship.** The book's success stories were selected from the top of a bull market.

## Rules you can steal

1. **Classify before you value.** Money, commodity, or token-as-product? Each needs a different model; most tokens are not money.
2. **Ask what the token is *needed* for.** If users can get the service without holding the token, velocity will be high and value capture low.
3. **Estimate utility value, then measure the speculative premium.** Even a rough MV = PQ calculation tells you how much of the price is a story.
4. **Expect the J-curve.** Plan for an 80% drawdown between hype and utility, and decide in advance whether you'll hold through it.
5. **Use network metrics, but cross-check for spam.** Active addresses and transaction counts are cheap to fake; fees paid are harder.
6. **Value accrual is a design choice.** Check whether fees flow to the token (burns, buybacks, staking yield) or to a company.
7. **Fundamentals matter over years, not months.** In the short run, liquidity and narrative dominate; use fundamentals to pick survivors, not entries.

## Key takeaways

- Burniske's taxonomy — cryptocurrencies, cryptocommodities, cryptotokens — remains the most useful part of *Cryptoassets*.
- MV = PQ demonstrates that most token prices are speculative premium, but it cannot produce reliable price targets because velocity is unobservable.
- The crypto J-curve accurately describes how surviving networks trade across cycles.
- "Fat Protocols" was half right; applications and stablecoin issuers now out-earn most base layers.
- Network metrics are real fundamentals but are easily gamed; fees paid is the most robust.
- Burniske's cycle calls are worth following as sentiment signals; his 2025 record was mixed.

## Sources

- [Cryptoasset Valuations — Chris Burniske, Medium (Sept 2017)](https://medium.com/@cburniske/cryptoasset-valuations-ac83479ffca7)
- [Cryptoassets: The Innovative Investor's Guide — Wikipedia entry for Chris Burniske](https://en.wikipedia.org/wiki/Chris_Burniske)
- [Fat Protocols — Joel Monegro, Union Square Ventures (Aug 2016)](https://www.usv.com/writing/2016/08/fat-protocols/)
- [On Medium-of-Exchange Token Valuations — Vitalik Buterin (Oct 2017)](https://vitalik.eth.limo/general/2017/10/17/moe.html)
- [Understanding Token Velocity — Kyle Samani, Multicoin (Dec 2017)](https://multicoin.capital/2017/12/08/understanding-token-velocity/)
- [On the Velocity Problem for Cryptoasset Value — Wilson Lau](https://medium.com/thoughtchains/on-the-velocity-problem-for-cryptoasset-value-aad235694211)
- [What Crypto "Token Velocity Theorists" Can Learn From Austrian Economics — Mises Institute](https://mises.org/power-market/what-crypto-token-velocity-theorists-can-learn-austrian-economics)
- ["Era of Selling Has Just Begun" — Placeholder VC calls crypto top — Yahoo Finance (Nov 2025)](https://finance.yahoo.com/news/era-selling-just-begun-placeholder-092248997.html)
- [Crypto bear-market callers are misguided, says Burniske — Daily Hodl (Feb 2025)](https://dailyhodl.com/2025/02/25/crypto-bear-market-callers-are-misguided-according-to-investor-chris-burniske-heres-why/)
- [Placeholder VC](https://www.placeholder.vc/)
