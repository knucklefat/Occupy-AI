# Valuation Indicators

**In one sentence:** Valuation indicators (Shiller's CAPE, the Buffett indicator, forward P/E, the equity risk premium, the Fed model, and Tobin's Q) tell you what you are paying for a dollar of corporate earnings or assets; they are among the best predictors of *ten-year* stock returns that exist and among the worst predictors of what the market will do *next year*, and confusing those two horizons is the most common mistake investors make with them.

## The core idea

Long-run stock returns come from three things: the dividends and buybacks you collect, the growth in earnings, and the change in the multiple people are willing to pay for those earnings. The first two are fairly steady over decades. The third is where valuation comes in: if you buy when the market trades at 40 times cyclically adjusted earnings and sell when it trades at 20, you have lost half your money to multiple compression before earnings and dividends are counted. Valuation indicators try to measure that starting multiple in a way that is comparable across time.

The catch: multiples can stay high (or low) for a decade. Shiller's CAPE first exceeded its 1929 peak in 1996; the market then doubled before it crashed. Valuation is a strong statement about the *destination* and almost silent about the *route*.

## The indicators

| Indicator | What it measures | Free source | Frequency | Long-run range | Current (as of September 2026) |
|---|---|---|---|---|---|
| **Shiller CAPE (P/E10)** | S&P 500 price ÷ average of the last 10 years of inflation-adjusted earnings | [Robert Shiller's data](http://www.econ.yale.edu/~shiller/data.htm); [multpl.com](https://www.multpl.com/shiller-pe) | Monthly | Mean ~17, median ~16 since 1881. Lows: ~5 (1920), ~6.6 (1982), ~13 (2009). Peaks: ~33 (1929), 44 (Dec 1999), ~38–39 (late 2021). | ~40.7 (multpl.com, September 10, 2026; 40.9 at the September 1 monthly print), roughly the 99th percentile of history and second only to the 2000 peak. |
| **Buffett indicator** | Total US stock market value (Wilshire 5000) ÷ nominal GDP | [Current Market Valuation](https://www.currentmarketvaluation.com/models/buffett-indicator.php); [GuruFocus](https://www.gurufocus.com/stock-market-valuations.php); FRED `NCBEILQ027S` ÷ `GDP` for the corporate-equities version | Quarterly (GDP) | Buffett in 2001: 70–80% is favorable; "approaching 200%... you are playing with fire." Peak ~140% in 2000, ~200%+ in late 2021. | ~244% at June 30, 2026 (market $78.1T ÷ GDP $32.1T), about 2.6 standard deviations above its long-run trend. |
| **Forward P/E** | S&P 500 price ÷ analysts' consensus earnings for the next 12 months | [FactSet Earnings Insight](https://insight.factset.com/topic/earnings) (weekly PDF, free); [Yardeni](https://yardeni.com/charts/) | Weekly | 10-year average ~18.6; 5-year ~19.9; 1999 peak ~25; 2020 peak ~23; March 2009 low ~10. | Low-to-mid 20s (23.1 in October 2025, the highest in five years; roughly similar since). |
| **Equity risk premium (ERP)** | Expected stock return minus the 10-year Treasury yield; the extra return investors demand for owning equities | [Damodaran's implied ERP](https://pages.stern.nyu.edu/~adamodar/New_Home_Page/datafile/histimpl.html) (monthly) | Monthly | 1960–2025 average ~4.2%. Low of 2.05% in 1999; above 6% in 2009 and 2020. | 4.23% at January 2026 (Damodaran), near the historical average despite high P/Es, because earnings growth and buybacks have been strong. With 10-year yields now ~4.7%, the simple earnings-yield-minus-bond-yield version is near zero. |
| **Fed model** | Compares the S&P 500 forward earnings yield (1 ÷ forward P/E) to the 10-year Treasury yield | Compute from FactSet forward P/E and FRED `DGS10` | Weekly | Named by Ed Yardeni in 1997 after a Fed report. "Fair" when the two are equal. | Earnings yield ~4.3–4.5% vs. 10-year 4.73% at end-August 2026 (4.8–4.95% in the second week of September): stocks look expensive relative to bonds for the first time since 2002. |
| **Tobin's Q** | Market value of corporate equities ÷ replacement cost of their net assets | FRED `NCBEILQ027S` ÷ `TNWMVBSNNCB` (Fed Z.1 data); [Advisor Perspectives](https://www.advisorperspectives.com/dshort/updates) publishes charts | Quarterly (Z.1, ~10-week lag) | Long-run mean ~0.7–0.8. Peaks ~1.6 (2000), ~2.0+ (2021). | Above 2, near the all-time high. |
| **Market cap / GVA, price-to-sales, EV/EBITDA** | Alternatives that avoid earnings-quality issues | [Hussman Funds](https://www.hussmanfunds.com/comment/) (cap/GVA); [multpl.com](https://www.multpl.com/s-p-500-price-to-sales) | Monthly/quarterly | S&P 500 price/sales averaged ~1.5 pre-2010. | Price/sales above 3, a record. |

## What they predict, and over what horizon

The academic evidence is consistent across a century of US data and across other countries:

- **Ten years out, valuation explains a lot.** Starting CAPE explains roughly 40% of the variation in subsequent 10-year real returns in Shiller's data (Campbell and Shiller, 1998 and updates). From CAPE above 35, subsequent 10-year real returns have historically averaged near zero, with a range from about −4% to +5% per year. From CAPE below 15, they averaged around 10% per year. Similar results hold for the Buffett indicator, Tobin's Q, and cap/GVA, all of which have correlations of −0.8 or stronger with subsequent 10–12-year returns in Hussman's and Advisor Perspectives' work.
- **One year out, valuation explains almost nothing.** The correlation between CAPE and next-12-month returns is close to zero; expensive markets have gone up 30% (1997, 1998, 2021, 2024) and cheap markets have gone down 30% (1931, 1974, 2008). Vanguard's 2012 study found CAPE explained about 43% of 10-year real returns and about 0–10% of 1-year returns; even the 10-year figure means most of the variation is *not* explained.
- **Valuation is a terrible timing tool.** A rule of "sell when CAPE exceeds 30" would have had you out of stocks from 1997 to 2001, from 2017 to today with brief exceptions, and would have badly underperformed buy-and-hold. Cliff Asness's 2012 paper on CAPE reached the same conclusion: it is useful for setting expectations, not for market timing.

Two important debates about the current level:

1. **Is CAPE structurally higher now?** Arguments yes: accounting changes (FAS 142 goodwill write-downs depressed 2001–02 and 2008–09 earnings, inflating the 10-year average denominator), lower payout ratios (more buybacks means faster per-share growth), a shift toward asset-light, high-margin tech, and lower real interest rates than in most of history. Jeremy Siegel and others argue these justify a "new normal" CAPE in the mid-20s. Even granting all that, 40 is far above the adjusted normal.
2. **Does the ERP rescue high P/Es?** Damodaran's implied ERP of ~4.2% says stocks are priced for roughly average compensation over bonds *if* analysts' earnings growth forecasts (double-digit for 2026–27, driven by AI capital spending) come true. If growth disappoints, the same prices imply a very thin premium. Note that the simple Fed-model version, which ignores growth, now shows stocks yielding *less* than Treasuries.

## Reading the current picture (September 2026)

Almost every measure is at or near a record: CAPE ~40.7, Buffett indicator ~244%, price/sales above 3, Tobin's Q above 2. The one that says "roughly fair," Damodaran's implied ERP, does so only because it credits the market with strong future earnings growth. Combined with 10-year yields at 4.7% (bonds are a real alternative for the first time in 15 years) and a Fed leaning toward hikes, the honest summary is: expected *long-run* returns from here are well below the historical ~7% real, likely in the 0–4% real range over a decade, with wide error bars; but that tells you nothing about 2027.

## How to use it

1. **Set expectations, not timing.** Use CAPE or the Buffett indicator to estimate 10-year expected returns (a rough formula: expected real return ≈ 1/CAPE + ~1.5% growth adjustment, minus any assumed reversion). Plug that into retirement or savings-rate planning. Do not use it to decide whether to be in or out of the market this year.
2. **Compare across markets.** CAPE for Europe, Japan, and emerging markets (Barclays/Research Affiliates publish these) has typically been half the US level; relative valuation is a much better predictor of *relative* returns than absolute valuation is of absolute returns.
3. **Adjust risk at the margin, slowly.** A reasonable response to extreme valuations is a modest tilt (a few points less equity, more value, more international, more short bonds), rebalanced annually, not a binary call.
4. **Pair with sentiment and breadth.** Valuation tells you the downside is large *if* a bear market comes; sentiment and breadth tell you whether one is starting. Neither alone is enough.
5. **Beware the denominator.** Forward P/E depends on analyst forecasts that are routinely 5–10% too high at cycle peaks. CAPE's 10-year average is distorted by 2020's earnings collapse rolling in and out. Use several measures.

## Key takeaways

- Valuation is the best long-horizon predictor we have: starting CAPE explains roughly 40% of the variation in 10-year real returns.
- It is nearly useless over one year; expensive markets can get much more expensive.
- CAPE ~40.7, Buffett indicator ~244%, and Tobin's Q above 2 (all as of mid/late 2026) are at or near historical extremes; only the growth-adjusted ERP calls the market "roughly fair."
- With the 10-year Treasury at 4.7%, the Fed-model gap between earnings yield and bond yield has closed for the first time since 2002.
- Structural arguments (accounting, buybacks, sector mix) justify a higher "normal" CAPE, perhaps mid-20s, not 40.
- Use valuation to set expected returns and savings rates, to tilt toward cheaper markets and styles, and to size risk, not to time entries and exits.
- All the underlying data are free: Shiller's spreadsheet, FactSet's weekly PDF, Damodaran's site, and FRED's Z.1 series.

## Sources

- [Robert Shiller's online data (Yale)](http://www.econ.yale.edu/~shiller/data.htm)
- [MacroRadar: Shiller PE ratio](https://www.macroradar.io/shiller-pe-ratio)
- [GuruFocus: S&P 500 Shiller CAPE](https://www.gurufocus.com/economic_indicators/56/sp-500-shiller-cape-ratio)
- [Current Market Valuation: Buffett Indicator](https://www.currentmarketvaluation.com/models/buffett-indicator.php)
- [Advisor Perspectives: Buffett Valuation Indicator, June 2026](https://www.advisorperspectives.com/dshort/updates/2026/07/08/buffett-valuation-indicator-june-2026)
- [FactSet: Highest forward P/E in more than five years](https://insight.factset.com/highest-forward-12-month-p/e-ratio-for-the-sp-500-in-more-than-5-years)
- [Damodaran: Data Update 2 for 2026](https://aswathdamodaran.substack.com/p/data-update-2-for-2026-a-testing)
- [Damodaran: Historical implied equity risk premiums](https://pages.stern.nyu.edu/~adamodar/New_Home_Page/datafile/histimpl.html)
- [Damodaran: Equity Risk Premiums, 2026 edition (SSRN)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6361419)
- [Vanguard: Forecasting stock returns (2012)](https://corporate.vanguard.com/content/dam/corp/research/pdf/s338.pdf)
- [Asness: An Old Friend, the Stock Market's Shiller P/E (AQR, 2012)](https://www.aqr.com/Insights/Research/White-Papers/An-Old-Friend-The-Stock-Markets-Shiller-PE)
- [FRED: Nonfinancial corporate equities (NCBEILQ027S)](https://fred.stlouisfed.org/series/NCBEILQ027S)
