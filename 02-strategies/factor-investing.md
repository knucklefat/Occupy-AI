# Factor Investing

**In one sentence:** Certain measurable characteristics of stocks — being cheap, small, recently rising, highly profitable, or low-volatility — have historically earned returns above the market, and you can tilt a diversified portfolio toward them cheaply with ETFs, provided you accept that each factor goes through long stretches of failure.

## What a "factor" is

A factor is a characteristic that explains differences in returns across a large group of stocks. The market itself is the first factor: stocks with more market exposure ("beta") earn more, on average, than cash. Academic research since the 1980s has identified a handful of additional characteristics that have earned a *premium* — extra return — persistently across decades and countries, even after adjusting for market risk. Factor investing (also called "smart beta" or "evidence-based investing") means systematically holding more of the stocks with those characteristics than a market-cap index does.

The framework comes from Eugene Fama (Nobel, 2013) and Kenneth French. Their 1992–1993 papers showed that a three-factor model — market, size, and value — explained far more of the variation in stock returns than the market alone. In 2015 they added profitability and investment for a five-factor model. Momentum, documented by Jegadeesh and Titman in 1993 and championed by Mark Carhart (1997), is usually treated as the sixth. AQR, Dimensional Fund Advisors (DFA), Research Affiliates, and Avantis built businesses on this research.

## The main factors

| Factor | Definition | Long-run U.S. premium (approx., annualized) | Why it might exist | Best-known evidence |
|---|---|---|---|---|
| **Value** | Cheap on price-to-book, earnings, or cash flow vs. expensive | 3%–5% (1927–present); negative 2007–2020 | Risk (distressed firms) and behavior (overreaction to bad news) | Fama & French 1992 |
| **Size** | Small market cap vs. large | 1%–3%; weak and unreliable alone | Illiquidity, less analyst coverage | Banz 1981; Fama & French 1992 |
| **Momentum** | Top-performing stocks over the past 12 months (skipping the last month) vs. worst | 6%–9% long-short, but with severe crashes | Under-reaction to news, herding | Jegadeesh & Titman 1993; Carhart 1997 |
| **Profitability / Quality** | High gross profits, ROE, stable earnings, low debt vs. the opposite | 3%–4% | Investors overpay for lottery-like junk | Novy-Marx 2013; Fama & French 2015; Asness et al. "Quality Minus Junk" 2019 |
| **Low volatility / minimum variance** | Lowest-beta or lowest-volatility stocks vs. highest | Comparable return to market with 20%–30% less volatility | Leverage constraints push investors into high-beta lottery stocks | Frazzini & Pedersen "Betting Against Beta" 2014 |
| **Investment** | Firms that grow assets slowly vs. aggressively | 2%–3% | Empire-building destroys value | Fama & French 2015 |

Long-short premiums (buy the top group, short the bottom) are what academic papers report; a long-only ETF captures perhaps a third to a half of that, before costs.

## The evidence, honestly stated

The case for factors rests on three legs:

1. **Persistence**: the premiums show up across most decades since the 1920s.
2. **Pervasiveness**: they appear in international developed markets, emerging markets, and (for value and momentum) in bonds, currencies, and commodities — see AQR's "Value and Momentum Everywhere" (2013).
3. **Explanation**: there is a plausible risk-based or behavioral story for each, which makes a data-mining fluke less likely.

Against this sits the "factor zoo": researchers have published 400+ claimed factors, most of which vanish after publication or transaction costs. Campbell Harvey and colleagues argue that a factor should clear a much higher statistical bar than the conventional one before you believe it. The six above are the survivors of that scrutiny.

The size factor deserves special caution. Alone, small caps have not reliably beaten large caps since the effect was published in 1981. Asness, Frazzini, Israel, Moskowitz, and Pedersen ("Size Matters, If You Control Your Junk," 2018) showed that the size premium is strong and consistent *once you exclude low-quality small companies*. In practice this means small-cap value or small-cap quality, not small-cap in general — which is exactly how AVUV and DFA's small-value funds are built.

## Factor cyclicality: the price of admission

Every factor has had a decade in which it looked dead:

- **Value**: 2007–2020 (about −2.6%/yr for the HML factor in the 2010s), then +30 points of outperformance vs. growth in 2021–2022, then lagging again in the 2023–2025 mega-cap rally.
- **Momentum**: crashes when markets reverse sharply — in 2009 the long-short momentum factor lost roughly 80% as beaten-down financials rebounded.
- **Low volatility**: lagged badly in 2020–2021 and 2023, exactly when speculative stocks soared.
- **Size**: the 1990s, and most of 2014–2024.
- **Quality**: fine in crashes, dull in melt-ups.

Usefully, the factors are weakly or negatively correlated with each other: value and momentum in particular tend to zig when the other zags. AQR's central argument is that a *multi-factor* portfolio smooths the ride enough to be holdable. The corollary is the strategy's hardest rule: you cannot switch to whichever factor worked last year. That is momentum-chasing at the factor level, and research on factor timing (Asness, "The Siren Song of Factor Timing," 2016) finds it very hard to do profitably.

## How to access factors with ETFs

| Factor | ETF | Expense ratio | Notes |
|---|---|---|---|
| U.S. value (large) | VTV (Vanguard Value) | 0.04% | Mild tilt; cheap, tax-efficient |
| U.S. value (large, deeper) | IUSV, RPV (S&P 500 Pure Value), VFVA (Vanguard U.S. Value Factor) | 0.04%–0.35% | RPV and VFVA tilt harder |
| U.S. small-cap value | AVUV (Avantis), DFSV (Dimensional), VBR (Vanguard), VIOV/IJS (S&P 600 Value) | 0.25% / 0.31% / 0.07% / 0.10%–0.18% | AVUV and DFSV screen out low-profitability "junk"; VBR is the mild, cheap version |
| International value | AVDV (int'l small value), AVIV, EFV, DFIV | 0.25%–0.36% | Non-U.S. value premium has been more consistent |
| Momentum | MTUM (iShares MSCI USA Momentum) | 0.15% | Rebalances semi-annually; high turnover |
| Quality | QUAL (iShares MSCI USA Quality), DGRW (WisdomTree Quality Dividend Growth), JQUA | 0.15% / 0.28% / 0.12% | ROE, earnings stability, low leverage |
| Low volatility | USMV (iShares MSCI USA Min Vol), SPLV (Invesco S&P 500 Low Vol) | 0.15% / 0.25% | USMV optimizes the whole portfolio; SPLV just picks 100 lowest-vol stocks |
| Multi-factor | VFMF (Vanguard U.S. Multifactor), AVUS (Avantis U.S. Equity), DFAC (Dimensional U.S. Core), LRGF | 0.18% / 0.15% / 0.17% / 0.08% | One-ticker tilt toward value, quality, small, momentum |

Expense ratios as of 2025–2026; check the current prospectus. Avantis and Dimensional funds are "systematic active" rather than pure index trackers — they follow rules but are not bound to an index, which reduces front-running and turnover costs.

## Building a factor-tilted portfolio

The standard construction is "core and tilt":

| Sleeve | Allocation (equity portion) | Example |
|---|---|---|
| U.S. total market core | 40% | VTI |
| U.S. small-cap value | 20% | AVUV |
| U.S. large value or multifactor | 10% | VTV or VFMF |
| International total market | 20% | VXUS |
| International small-cap value | 10% | AVDV |

A tilt of 30%–50% of equities toward factor funds is enough to make a difference over 20+ years without making the portfolio unrecognizable versus the market in any single year. Avoid stacking six single-factor ETFs; value and momentum funds partly cancel each other's trades, so a multi-factor fund that handles the interaction internally is more efficient.

## Costs and frictions to watch

- **Turnover**: momentum ETFs turn over 100%+ a year; in a taxable account this can generate distributions. Hold momentum in an IRA.
- **Tracking error vs. the market**: a factor portfolio *will* trail the S&P 500 for multi-year stretches; that is the definition of a tilt. Decide in advance how much you can tolerate.
- **Implementation drag**: the gap between the academic long-short premium and a real long-only ETF is large. Expect a well-built tilt to add perhaps 0.5%–1.5% a year over the very long run, not the 4%–8% seen in papers.
- **Fees**: 0.15%–0.35% for factor funds vs. 0.03% for a total-market fund. The expected premium must clear that hurdle.

## How to actually do it

1. **Own the total market first.** Factor tilts are an addition to an index core, not a replacement.
2. **Choose one or two factors you understand and believe in** — the research suggests value (especially small value), quality/profitability, and momentum are the most robust. Write down *why* you expect the premium to persist.
3. **Tilt 30%–50% of equities** using the ETFs above, or use a single multi-factor fund (AVUS, VFMF, DFAC) if you want simplicity.
4. **Put high-turnover funds (momentum) in tax-advantaged accounts**; small-value and quality funds are fine anywhere.
5. **Rebalance annually** back to target weights. This forces buying the factor after it has underperformed, which is where much of the premium is earned.
6. **Set a 10-year evaluation horizon.** Compare your tilted portfolio to a plain index portfolio after ten years, not after one. A three-year lag is normal; a fifteen-year lag would be evidence.
7. **Never rotate factors on recent performance.** If you find yourself wanting to sell value after a bad year, reread the cyclicality section.

## Key takeaways

- Factors are stock characteristics (value, size, momentum, quality, low volatility) with a long record of earning premiums across markets and decades.
- Fama-French's work is the foundation; AQR, Dimensional, and Avantis are the leading implementers.
- Size alone is weak; small-cap *value* or small-cap *quality* is where the evidence is.
- Every factor has had a lost decade — value's was 2007–2020; multi-factor diversification is the only cure.
- Access is cheap and easy: AVUV, VTV, MTUM, QUAL, USMV, VFMF cost 0.04%–0.35%.
- Real-world long-only premiums are perhaps 0.5%–1.5% a year, not the headline academic numbers.
- The strategy fails mainly through impatience; commit to a decade and rebalance mechanically.

## Sources

- [The Cross-Section of Expected Stock Returns — Fama & French (1992), Journal of Finance](https://onlinelibrary.wiley.com/doi/10.1111/j.1540-6261.1992.tb04398.x)
- [A Five-Factor Asset Pricing Model — Fama & French (2015), SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2287202)
- [Kenneth R. French Data Library (factor return data)](https://mba.tuck.dartmouth.edu/pages/faculty/ken.french/data_library.html)
- [Size Matters, If You Control Your Junk — Asness, Frazzini, Israel, Moskowitz, Pedersen (AQR)](https://www.aqr.com/Insights/Research/Working-Paper/Size-Matters-If-You-Control-Your-Junk)
- [Value and Momentum Everywhere — Asness, Moskowitz, Pedersen (2013)](https://www.aqr.com/Insights/Research/Journal-Article/Value-and-Momentum-Everywhere)
- [Quality Minus Junk — Asness, Frazzini, Pedersen (AQR)](https://www.aqr.com/Insights/Research/Journal-Article/Quality-Minus-Junk)
- [A Lost Decade for the Fama-French Factors — Advisor Perspectives](https://www.advisorperspectives.com/articles/2020/05/13/a-lost-decade-for-the-fama-french-factors)
- [Is Size a Useful Investing Factor or Not? — Alpha Architect](https://alphaarchitect.com/is-size-a-useful-factor-or-not/)
- [Best Factor ETFs — My ETF Journey](https://myetfjourney.com/best-etfs/factor-investing)
- [Avantis U.S. Small Cap Value ETF (AVUV) — fund page](https://www.avantisinvestors.com/avantis-investments/avantis-us-small-cap-value-etf/)
- [Investopedia: Factor Investing](https://www.investopedia.com/terms/f/factor-investing.asp)
