# Portfolio Construction and Diversification

**In one sentence:** Diversification works because assets that don't move in lockstep cancel out some of each other's swings — so a portfolio of imperfectly correlated holdings can earn the *average* of their returns with *less* than the average of their risk, which is the closest thing to a free lunch in investing.

## Correlation in plain language

**Correlation** measures how two things move together, on a scale from +1 (always in the same direction, proportionally) to −1 (always opposite) to 0 (no relationship). Two U.S. large-cap funds have a correlation near +1 — owning both adds nothing. U.S. stocks and long Treasuries have historically been around 0 to −0.3, though they were briefly positive in 2022 when both fell together. Gold and stocks sit near 0.

The maths of diversification: if you split money equally between two assets with the same volatility and a correlation of 0.5, the portfolio's volatility is about 87% of either asset's alone. At a correlation of 0, it's about 71%. At −0.5, about 50%. Returns average; risk drops. The lower the correlation, the bigger the drop.

Two caveats. Correlations are not stable — they tend to spike toward +1 in crises, which is exactly when you want them low. And correlation says nothing about return; a zero-correlation asset with a zero return still just dilutes you.

## The efficient frontier, without the maths

Harry Markowitz (1952) showed that for any set of assets, you can draw a curve of the portfolios that deliver the highest return for each level of risk. That curve is the **efficient frontier**. Anything below it is dominated — you could get more return for the same risk, or the same return for less risk, by mixing differently.

The practical lessons, not the formula:
- Adding a low-correlation asset to a portfolio can *raise* return and *lower* risk at the same time, up to a point.
- The frontier is built from *estimates* of future returns, risks and correlations, and it is exquisitely sensitive to them. Plug in slightly different numbers and the "optimal" portfolio changes wildly. This is why nobody sensible runs their life savings on a raw optimiser.
- The robust conclusion is qualitative: hold several asset classes with different economic drivers, weight them sensibly, and rebalance. Precision beyond that is false.

## What actually diversifies

| Layer | Diversifies against | Typical tool |
|---|---|---|
| Many stocks instead of a few | Single-company disaster | Total-market index fund |
| Stocks + bonds | Recession / growth shocks | Treasury or aggregate bond fund |
| U.S. + international stocks | Single-country stagnation, currency, valuation cycles | Total international fund |
| Nominal bonds + TIPS | Inflation surprises | TIPS fund or I bonds |
| Real assets (REITs, gold, commodities) | Inflation, currency debasement | Small allocations (5–20%) |
| Different factors (value, small, momentum) | Growth-stock-only regimes | Tilt funds |

The first two rows do the heavy lifting. Each layer beyond them helps less, and each adds complexity and behavioural risk (it's harder to hold a portfolio with six things when four of them are lagging).

## How many holdings?

For individual stocks: classic studies (Evans & Archer, 1968; Statman, 1987) found most *diversifiable* risk disappears somewhere between 20 and 40 randomly chosen stocks, though later work argued for 50–100 because individual-stock volatility has risen. But "diversified enough not to blow up" is not the same as "captures the market's return." Bessembinder (2018) showed that about 4% of listed U.S. stocks produced all the net wealth creation since 1926; a 30-stock portfolio has a real chance of missing the handful that mattered. This is the strongest argument for owning the whole market through an index fund.

For funds: **three is enough** (total U.S. stock, total international stock, total bond). Beyond about six to eight funds you are almost certainly duplicating exposures. Many "diversified" portfolios of 15 funds are 80% correlated with the S&P 500.

## International diversification and the home-bias debate

U.S. stocks are roughly 60–65% of the world's investable market, yet the average U.S. investor holds 80–90% in U.S. stocks. That gap is **home bias**, and every country has it.

**The case for going global (Vanguard, Bogleheads default):** you don't know which country will lead the next decade; U.S. and non-U.S. stocks have traded leadership in multi-year cycles (non-U.S. won 2002–07, U.S. won 2010–24); the U.S. has been the exception among developed markets in never suffering a decades-long stagnation, but Japan since 1989 shows it's possible. Vanguard's research finds the diversification benefit is meaningful up to about 20% of equities in international and mostly saturated by around 40%, which is why its target-date funds use 40%.

**The case for U.S.-only (Bogle, Buffett):** U.S. companies already earn ~40% of revenue abroad; U.S. markets have stronger shareholder protections and lower costs; international funds have higher expense ratios, dividend withholding taxes, and currency volatility; and U.S. stocks have simply won over the last 15 years.

**Reasonable landing zone:** 20–40% of your stock allocation in international. Zero is defensible; over 50% is unusual. What is not defensible is bouncing between them based on which one just outperformed.

## Core–satellite

A **core–satellite** structure holds 70–90% of the portfolio in low-cost, broadly diversified index funds (the core) and 10–30% in deliberate bets (satellites): a factor tilt, a sector, individual stocks, or an active fund you believe in. The point is discipline: the core guarantees you get the market return on most of your money, the satellite sleeve caps how badly your convictions can hurt you, and you can measure whether the satellites are actually adding anything (see [reading-a-brokerage-statement-and-tracking-performance.md](reading-a-brokerage-statement-and-tracking-performance.md)).

## Worked example: building a portfolio

Target: 70/30, moderate international, small real-asset sleeve, $200,000.

| Holding | Weight | Dollars | Role |
|---|---|---|---|
| Total U.S. stock index | 45% | $90,000 | Core growth |
| Total international stock index | 20% | $40,000 | Country/currency diversification |
| U.S. small-cap value index | 5% | $10,000 | Satellite factor tilt |
| Intermediate Treasury / total bond fund | 20% | $40,000 | Recession ballast |
| TIPS fund | 5% | $10,000 | Inflation ballast |
| REIT index | 5% | $10,000 | Real-asset satellite |

Stocks: 70% (of which ~29% international). Bonds: 25%. Real assets: 5%. Six funds, three of which are optional. The same investor could drop to three funds (45/25/30) and lose very little.

## How to actually do it

1. Fix the stock/bond split first (see [asset-allocation.md](asset-allocation.md)). This is 90% of the decision.
2. Inside stocks, choose an international share between 20% and 40% and write down why.
3. Use total-market index funds for each sleeve; check expense ratios (under 0.10% for U.S., under 0.15% international).
4. Decide whether you want any satellites (max 10–30% combined). If unsure, skip them.
5. Check overlap: don't hold an S&P 500 fund *and* a total-market fund *and* a large-cap growth fund — that's one bet three times.
6. Place holdings across accounts for tax efficiency (see [asset-location.md](asset-location.md)).
7. Set rebalancing bands and stop tinkering (see [rebalancing.md](rebalancing.md)).

## Key takeaways

- Diversification lowers risk without lowering expected return only when the assets are imperfectly correlated — and correlations rise in crises.
- The efficient frontier is a useful idea and a dangerous calculator; use the concept, not the optimiser.
- Stocks + bonds + international is where nearly all the diversification benefit lives; extra layers help at the margin.
- Owning the whole market through index funds beats 30 hand-picked stocks because the market's return comes from a few big winners you can't identify in advance.
- Hold 20–40% of stocks internationally; the exact number matters less than not chasing whichever region just won.
- Three funds is a complete portfolio; more than eight is almost certainly redundant.
- Core–satellite lets you take bets while guaranteeing most of your money earns the market return.

## Sources

- [Markowitz (1952) – Portfolio Selection (Journal of Finance)](https://www.jstor.org/stable/2975974)
- [Vanguard – Global equity investing: The benefits of diversification and sizing your allocation](https://www.vanguardmexico.com/content/dam/intl/americas/documents/mexico/en/global-equity-investing-diversification-sizing.pdf)
- [Vanguard – The role of home bias in global asset allocation decisions](https://zonavalue.com/wp-content/uploads/2017/06/vanguard.pdf)
- [Bessembinder (2018) – Do Stocks Outperform Treasury Bills?](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2900447)
- [Bogleheads wiki – Three-fund portfolio](https://www.bogleheads.org/wiki/Three-fund_portfolio)
- [Bogleheads wiki – Domestic/international](https://www.bogleheads.org/wiki/Domestic/international)
- [Bogleheads wiki – Core-satellite](https://www.bogleheads.org/wiki/Core-satellite)
- [Portfolio Charts – Portfolios](https://portfoliocharts.com/portfolios/)
