# Bond and Fixed-Income Analysis

**In one sentence:** A bond is a loan with a known schedule of payments, so analyzing one comes down to three questions — what yield will I actually earn, how much will the price move if rates change, and how likely is it that I get paid at all.

## The vocabulary, in plain language

- **Face (par) value:** what the issuer repays at maturity, usually $1,000.
- **Coupon:** the fixed annual interest, stated as a percentage of par. A 4% coupon pays $40 a year (typically $20 twice a year).
- **Price:** quoted as a percentage of par. A price of 95 means $950.
- **Maturity:** when the principal is repaid.
- **Yield:** the return you actually earn, which depends on the price you pay. Price and yield move in opposite directions: pay less than par and your yield exceeds the coupon.

## Yield to maturity (YTM)

YTM is the single annual rate that makes the present value of all remaining coupons plus the final principal equal to today's price. It assumes you hold to maturity and reinvest coupons at the same rate. It is the bond-world equivalent of an internal rate of return, and the standard number for comparing bonds.

**Quick approximation:** YTM ≈ (annual coupon + (par − price) ÷ years) ÷ ((par + price) ÷ 2).

**Example.** A 10-year bond, 4% coupon, priced at $950. Approximation: (40 + 50 ÷ 10) ÷ ((1,000 + 950) ÷ 2) = 45 ÷ 975 ≈ **4.6%**. You earn more than the 4% coupon because you also collect a $50 gain at maturity. (A financial calculator gives about 4.63% for semiannual coupons.)

Related yields:
- **Current yield** = annual coupon ÷ price = 40 ÷ 950 = 4.2%. Ignores the pull to par; less useful.
- **Yield to call (YTC):** for callable bonds (the issuer can repay early), the yield if called at the first call date. **Yield to worst** is the lower of YTM and YTC — use this one for callable bonds.
- **Yield spread:** the bond's yield minus a Treasury of the same maturity. This is the compensation for credit risk.

## Duration: how much price moves when rates move

**Duration** measures a bond's sensitivity to interest rates. The practical version is **modified duration**: the approximate percentage price change for a 1-percentage-point change in yield.

**Rule of thumb: price change ≈ −(modified duration) × (change in yield).**

A bond with a modified duration of 8 will fall roughly 8% if yields rise 1 point and gain roughly 8% if yields fall 1 point. Duration rises with maturity and falls with coupon: a 30-year zero-coupon bond has a duration near 30; a 2-year 5% note has a duration under 2.

Duration is also (roughly) the weighted-average number of years until you get your money back, which is why a bond fund with "duration 6" behaves like a 6-year commitment to today's rates.

**Why this matters:** In 2022, when the 10-year Treasury yield rose about 2.4 points, long-duration bond funds with durations near 17 fell more than 30% — bonds are not automatically "safe."

## Convexity: why duration is only approximately right

Duration is a straight-line estimate, but the real price/yield relationship is curved. **Convexity** measures that curve. For a normal bond, convexity is positive and works in your favor: prices rise more when yields fall than they drop when yields rise by the same amount.

**Refined estimate:** price change ≈ −D × Δy + ½ × C × (Δy)².

**Example.** Duration 8, convexity 80, yields rise 1 point (Δy = 0.01): −8 × 0.01 + 0.5 × 80 × 0.0001 = −0.080 + 0.004 = **−7.6%**, not −8%. For small rate moves the correction is tiny; for big moves or long bonds it matters. Mortgage-backed securities and callable bonds can have *negative* convexity — their upside is capped because the borrower refinances when rates fall — which is a reason they yield more.

## Credit ratings

Rating agencies (Moody's, S&P, Fitch) grade the likelihood of default.

| Grade | Moody's | S&P / Fitch | Meaning |
|---|---|---|---|
| Investment grade — highest | Aaa | AAA | Minimal risk (U.S. Treasuries, a few corporations) |
| Investment grade — high | Aa1–Aa3 | AA+ to AA− | Very strong |
| Investment grade — upper medium | A1–A3 | A+ to A− | Strong |
| Investment grade — lowest | Baa1–Baa3 | BBB+ to BBB− | Adequate; the largest bucket of corporate bonds |
| High yield ("junk") | Ba1 and below | BB+ and below | Speculative; meaningful default risk |
| Distressed | Caa–C | CCC–C | Default likely or imminent |
| In default | D / C | D | Missed payments |

The BBB−/Baa3 line matters because many funds and institutions can only hold investment grade; a downgrade below it (a "fallen angel") forces selling. Ratings lag; the market's spread often moves first. Historical default rates over five years run near 1% for investment grade and 15–20% for high yield in aggregate, with wide variation by cycle.

## Reading the yield curve

The yield curve plots Treasury yields by maturity (3-month to 30-year).

- **Normal (upward sloping):** longer bonds yield more, compensating for time and inflation uncertainty.
- **Flat:** little difference; often a late-cycle sign.
- **Inverted (short yields above long):** historically one of the more reliable recession warnings, though the lead time varies from months to two years. The most watched spreads are 10-year minus 2-year and 10-year minus 3-month.

For a bond investor the curve tells you where the reward for taking duration is. A steep curve pays you to extend maturity; a flat curve does not, so stay short and keep the option to reinvest higher.

## TIPS

**Treasury Inflation-Protected Securities** have a principal that adjusts with the Consumer Price Index; the coupon rate is fixed but paid on the adjusted principal. The quoted yield on a TIPS is a **real yield** — the return above inflation. The difference between a nominal Treasury yield and the TIPS yield of the same maturity is the **breakeven inflation rate**: if you expect inflation above the breakeven, TIPS win; below it, nominal Treasuries win. Two quirks: the inflation adjustment is taxed annually as income even though you do not receive it until maturity (so hold TIPS in tax-deferred accounts), and at maturity you receive the greater of adjusted or original principal — deflation cannot take you below par.

Series I savings bonds are the retail cousin, bought directly at TreasuryDirect with purchase limits.

## Municipal bonds

**Munis** are issued by states, cities, and agencies. Interest is generally exempt from federal tax and often from state tax if you live in the issuing state. Compare them using the **tax-equivalent yield** = muni yield ÷ (1 − your marginal tax rate). A 3.5% muni for someone in the 35% bracket is worth 3.5 ÷ 0.65 = **5.4%** taxable-equivalent. Two types: **general obligation** bonds backed by taxing power, and **revenue** bonds backed by a specific project (a toll road, a hospital) — the latter carry more risk. Muni defaults are rare but not zero; check the rating and the issuer's pension burden.

## How to evaluate a bond fund

Most individuals own bonds through funds or ETFs. Check:

1. **Duration.** This is the fund's interest-rate risk. Match it to your horizon; a 6-year duration fund is not a place for money you need next year.
2. **Credit quality.** The fact sheet gives the rating breakdown. A "core" fund is mostly investment grade; a "core-plus" or "multisector" fund adds high yield and emerging markets.
3. **SEC yield (30-day)**, not distribution yield. The SEC yield is standardized and net of expenses; distribution yields can include return of capital.
4. **Expense ratio.** Bond returns are modest, so fees bite hard. Index bond funds charge 0.03–0.10%; paying 0.5%+ for an active bond fund requires a strong reason.
5. **Yield-to-maturity vs. duration.** A crude but useful test: if the YTM roughly equals or exceeds the duration, the fund's income can absorb a 1-point rate rise in a year. A fund with 3% YTM and 8 duration cannot.
6. **What "aggregate" means.** The Bloomberg U.S. Aggregate index is roughly 40–45% Treasuries, 25% agency mortgages, 25% corporates — it is a government-heavy, intermediate-duration benchmark.
7. **Tax location.** Taxable bond interest is ordinary income; hold taxable bond funds in IRAs/401(k)s where possible, munis in taxable accounts.

## How to actually do it

1. Decide the job of the bond allocation: ballast against stock crashes (Treasuries, short-to-intermediate duration), income (investment-grade corporates, munis if in a high bracket), or inflation protection (TIPS).
2. For an individual bond: find the yield to worst, the rating, the maturity or call date, and the spread over Treasuries. Ask whether the spread pays you for the credit risk.
3. Compute the modified duration (given on any bond quote or fund fact sheet) and multiply by the rate move you fear. Can you tolerate that loss?
4. For a fund: read the fact sheet for duration, credit breakdown, SEC yield, and expense ratio. Compare with a low-cost index fund of the same category.
5. Check the yield curve. If it is flat or inverted, favor shorter maturities; if steep, extending duration is better compensated.
6. Compare TIPS real yields with nominal yields via the breakeven to decide the inflation-protected share.
7. Place bonds in the right account for tax: taxable bonds and TIPS in tax-deferred, munis in taxable.

## Key takeaways

- Price and yield move inversely; yield to maturity (or yield to worst, for callables) is the number to compare.
- Duration is your rate-risk gauge: a 1-point yield rise costs roughly duration-percent of price.
- Convexity is a small favorable correction for plain bonds and a hidden cost in callable and mortgage bonds.
- The BBB−/Baa3 line separates investment grade from junk and drives forced selling on downgrades.
- An inverted yield curve is a recession warning with variable timing; a steep curve pays you to extend maturity.
- TIPS yield a real rate; compare with nominal Treasuries via breakeven inflation, and hold them tax-deferred.
- Munis are compared on tax-equivalent yield; general obligation is safer than revenue.
- For bond funds, the four numbers that matter are duration, credit quality, SEC yield, and expense ratio.

## Sources

- [CFA Institute: Yield-Based Bond Convexity and Portfolio Properties](https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/yield-based-bond-convexity-and-portfolio-properties)
- [Investopedia: Duration and Convexity to Measure Bond Risk](https://www.investopedia.com/articles/bonds/08/duration-convexity.asp)
- [Investopedia: Yield to Maturity (YTM)](https://www.investopedia.com/terms/y/yieldtomaturity.asp)
- [Britannica Money: Bond duration — price, yield, and time to maturity](https://www.britannica.com/money/bond-duration)
- [TreasuryDirect: Treasury Inflation-Protected Securities (TIPS)](https://www.treasurydirect.gov/marketable-securities/tips/)
- [Investor.gov: Municipal Bonds](https://www.investor.gov/introduction-investing/investing-basics/investment-products/bonds-or-fixed-income-products/municipal-bonds)
- [FINRA: Bond Yield and Return](https://www.finra.org/investors/investing/investment-products/bonds)
- [Federal Reserve Bank of St. Louis (FRED): 10-Year minus 2-Year Treasury Spread](https://fred.stlouisfed.org/series/T10Y2Y)
