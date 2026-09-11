# Macro and All-Weather Investing

**In one sentence:** Instead of forecasting the economy, build a portfolio that holds something which does well in every combination of rising or falling growth and rising or falling inflation — stocks, long bonds, gold, cash, and inflation-linked assets in balanced proportions — so that no single economic surprise can wreck you.

## The problem all-weather portfolios solve

A traditional 60/40 stock/bond portfolio looks balanced by dollars but not by risk: stocks are about three times as volatile as bonds, so roughly 90% of the portfolio's risk comes from the stock side. It is really a bet on economic growth with a bond cushion. That cushion works when stocks and bonds move in opposite directions (most of 1998–2021) and fails when they fall together, as in 2022 (stocks −18%, long Treasuries −31%) and throughout the 1970s.

All-weather investing starts from a different question: what are the economic environments that drive asset prices, and what does well in each? Then it sizes positions so that each environment is covered roughly equally. The goal is not the highest return; it is a return that is acceptable in every scenario, which for most people is the return they actually keep.

## The four economic regimes

Ray Dalio's framework at Bridgewater reduces the economy to two variables — growth and inflation — each of which can come in above or below what markets expected. That gives four quadrants:

| | **Inflation rising** | **Inflation falling** |
|---|---|---|
| **Growth rising** | Commodities, gold, emerging-market stocks, real estate | Stocks (especially growth), corporate bonds |
| **Growth falling** | Gold, TIPS, commodities, cash | Long-term nominal Treasuries |

Any portfolio can be checked against this grid. A 60/40 covers the bottom-right (deflationary recession → bonds) and top-right (disinflationary growth → stocks) but has nothing for the left column. Someone who lived through 2022, or the 1970s, felt exactly that gap.

## Bridgewater's All Weather and risk parity

Dalio built All Weather in 1996 for his own family trust, aiming for a portfolio that would survive whatever the next 100 years brought. The method is **risk parity**: allocate so that each regime, and each asset class, contributes roughly equal *risk* rather than equal dollars. Because bonds are less volatile than stocks, they get a larger dollar weight; Bridgewater's institutional version also uses modest leverage on the bond side so that the balanced portfolio can reach an equity-like return.

The unleveraged retail version, as Dalio described it to Tony Robbins in *Money: Master the Game* (2014):

| Asset | Weight | Role |
|---|---|---|
| Long-term Treasuries (20+ yr) | 40% | Falling growth, falling inflation |
| U.S. stocks | 30% | Rising growth |
| Intermediate Treasuries (7–10 yr) | 15% | Ballast; falling growth |
| Gold | 7.5% | Rising inflation; currency stress |
| Broad commodities | 7.5% | Rising inflation, rising growth |

ETF implementation: TLT or VGLT, VTI, IEF or VGIT, GLD/IAU/SGOL, and a commodity fund such as PDBC or GSG. Historical results (1970s–2025 backtests by Portfolio Charts, Optimized Portfolio, and others): roughly 7%–8% annualized with volatility about half of the stock market's and a worst drawdown in the −15% to −25% range, most of it in 2022, when 55% in Treasuries was the wrong thing to hold as rates jumped.

The 2022 episode is the honest critique of All Weather: it was designed with heavy bond exposure during a forty-year bond bull market, and its "all weather" claim was tested by the first real inflation-plus-rate-hike regime since the 1970s. It survived — down around 20% at worst — but it did not shine. Risk parity funds with leverage did worse.

## Harry Browne's Permanent Portfolio

Harry Browne, a libertarian investment writer and 1996 presidential candidate, proposed the Permanent Portfolio in the early 1980s with an even simpler logic. There are four economic conditions — prosperity, recession, inflation, deflation — and one asset for each:

| Asset | Weight | Condition it protects against |
|---|---|---|
| Stocks (total market) | 25% | Prosperity |
| Long-term Treasuries (25–30 yr) | 25% | Deflation |
| Gold | 25% | Inflation, currency crisis |
| Cash / T-bills | 25% | Recession, "tight money" |

Rebalance when any asset drifts to below 15% or above 35% of the portfolio. That's the whole system. Browne's own backtest from 1970 and subsequent updates show roughly 8% annualized (about 4%–5% real) with a worst calendar-year loss of about −5% before 2022 and a maximum drawdown in the −15% range including 2022. It has trailed stocks badly in every long bull market and beaten them in every crisis; from 2000 to 2012 it outperformed the S&P 500 outright.

The critique: 25% in cash is a heavy drag over long periods, and 25% in gold — an asset with no cash flow — is a large bet that the inflation/crisis regime recurs. The defense: the cash is what let Browne-style investors buy stocks in 2009 and 2020 without selling anything at a loss.

## The Golden Butterfly

Tyler of Portfolio Charts modified the Permanent Portfolio in 2016 to tilt it toward prosperity, on the reasoning that prosperity is the most common regime. He split the stock allocation between total market and small-cap value (see [factor-investing.md](factor-investing.md)) and reduced cash and gold slightly:

| Asset | Weight | ETF examples |
|---|---|---|
| Total U.S. stock market | 20% | VTI |
| U.S. small-cap value | 20% | AVUV, VIOV, VBR |
| Long-term Treasuries | 20% | VGLT, TLT |
| Short-term Treasuries | 20% | VGSH, SHV |
| Gold | 20% | SGOL, IAU, GLDM |

Backtests from 1970 show roughly 9%–10% annualized with about half the volatility of the S&P 500 and a maximum drawdown near −18% (2022 again). The small-cap-value sleeve adds expected return and diversifies away from the mega-cap concentration of the total market. The Golden Butterfly is the most popular of these portfolios among early-retirement communities because its combination of return and shallow drawdowns supports a higher safe withdrawal rate than a 60/40 in most historical simulations.

## Comparing the three

| Portfolio | Stocks | Bonds | Gold/commodities | Cash | Approx. CAGR (since 1970s) | Approx. max drawdown | Character |
|---|---|---|---|---|---|---|---|
| All Weather | 30% | 55% | 15% | 0% | 7%–8% | −20% to −25% | Bond-heavy; best in deflation |
| Permanent Portfolio | 25% | 25% | 25% | 25% | ~8% | −15% | Maximum simplicity; cash drag |
| Golden Butterfly | 40% | 20% | 20% | 20% | 9%–10% | −18% | Prosperity tilt; best return of the three |
| 60/40 (reference) | 60% | 40% | 0% | 0% | ~9% | −30% to −35% | Growth bet with bond cushion |
| 100% stocks (reference) | 100% | 0% | 0% | 0% | ~10%–11% | −50% or worse | Highest return, deepest holes |

Numbers are rounded approximations from Portfolio Charts and similar backtesting tools and vary with the exact start date and data set. The consistent pattern: the all-weather family gives up 1–3 points of annual return versus stocks in exchange for cutting the worst drawdown by more than half.

## Discretionary global macro (the other kind of macro)

"Macro investing" also refers to hedge-fund managers — Soros, Druckenmiller, Tudor Jones, Dalio's Pure Alpha — who *forecast* regimes and bet on them through currencies, rates, and indices. That is a fundamentally different activity: concentrated, leveraged, and dependent on being right about the timing of central-bank decisions. The record of retail investors trying to do it is poor, and even the professionals' returns have been modest since 2010. The all-weather approach exists precisely so you do not have to forecast. If you find yourself adjusting the weights because you "think inflation is coming," you have left the strategy.

## Weaknesses to understand before adopting

- **Tracking error in bull markets.** From 2009 to 2021, any of these portfolios trailed a 100%-stock portfolio by 3–5 points a year. That is the price of the protection, paid up front and for a long time. Many people abandon the strategy after five years of watching the S&P 500 run.
- **Gold has no cash flow.** Its long-run real return is near zero; its value in the portfolio is what it does in crises, not what it earns.
- **Long bonds carry duration risk.** A 20+ year Treasury fund can fall 30%+ when rates rise 3 points, as 2022 proved. This is the main reason all three portfolios had their worst year then.
- **Taxes.** Gold ETFs are taxed as collectibles (28% max long-term rate) in taxable accounts. Hold gold and bonds in IRAs where possible.
- **Rebalancing discipline.** The return advantage in backtests depends on selling the winner to buy the loser, which feels wrong every single time.

## How to actually do it

1. **Decide whether shallow drawdowns are worth 1–3 points of annual return.** If you are within 10 years of drawing on the portfolio, or have proven you sell in crashes, the answer is probably yes. A 25-year-old with steady income probably wants more stocks.
2. **Choose a template**: Golden Butterfly for the best balance of return and drawdown; Permanent Portfolio for maximum simplicity; All Weather if you specifically want Dalio's bond-heavy version.
3. **Buy the five (or four) ETFs** in the weights listed. Low-cost choices: VTI, AVUV or VBR, VGLT, VGSH, SGOL or GLDM; for commodities, PDBC. Total expense ratio should land under 0.15%.
4. **Place assets by tax treatment**: gold and long bonds in an IRA/401(k); stocks in taxable if something must be.
5. **Rebalance with bands** — Browne's 15%/35% rule, or a 5-percentage-point drift from target — checked quarterly. Bands trade less than a calendar rule and capture more of the rebalancing benefit.
6. **Do not tinker with the weights based on your economic view.** Write that rule on the front page of your plan.
7. **Judge over a full cycle** including a crash. The portfolio's purpose becomes obvious only when stocks fall 40% and yours falls 12%.

## Key takeaways

- 60/40 is 90% stock risk; it fails when stocks and bonds fall together, as in 2022 and the 1970s.
- The growth/inflation quadrant grid tells you which asset covers which regime; a robust portfolio has something in every box.
- All Weather (Dalio) is bond-heavy risk parity; the Permanent Portfolio (Browne) is 25% each in stocks, long bonds, gold, cash; the Golden Butterfly adds a small-cap-value tilt for higher return.
- Expect 7%–10% long-run returns with maximum drawdowns of −15% to −25%, versus −50%+ for stocks.
- The cost is a long lag in bull markets and the discomfort of holding gold and long bonds.
- Rebalancing with bands, not forecasts, is the engine; discretionary macro forecasting is a different and much harder game.
- Hold gold and bonds in tax-advantaged accounts.

## Sources

- [Bridgewater: The All Weather Story](https://www.bridgewater.com/research-and-insights/the-all-weather-story)
- [Ray Dalio's All Weather Portfolio vs. The Golden Butterfly — comparison](https://donnaleehellmann.substack.com/p/ray-dalios-all-weather-portfolio)
- [Golden Butterfly Portfolio Review — Optimized Portfolio](https://www.optimizedportfolio.com/golden-butterfly-portfolio/)
- [PortfolioCharts' Golden Butterfly — Allocate Smartly review](https://allocatesmartly.com/portfoliocharts-golden-butterfly/)
- [Portfolio Charts — Golden Butterfly (original source)](https://portfoliocharts.com/portfolios/golden-butterfly/)
- [Portfolio Charts — Permanent Portfolio](https://portfoliocharts.com/portfolios/permanent-portfolio/)
- [Bogleheads wiki: Permanent Portfolio](https://www.bogleheads.org/wiki/Permanent_portfolio)
- [Investopedia: Risk Parity](https://www.investopedia.com/terms/r/risk-parity.asp)
- [The Golden Butterfly vs the All Weather Portfolio — Listen Money Matters](https://www.listenmoneymatters.com/all-weather-golden-butterfly/)
