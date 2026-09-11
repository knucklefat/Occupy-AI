# Asset Location

**In one sentence:** Asset location is deciding *which account* each investment lives in — putting tax-hungry assets like bonds and REITs inside IRAs and 401(k)s, and tax-friendly stock index funds in taxable accounts — and done well it can add a few tenths of a percent a year without changing your overall allocation at all.

## Allocation vs. location

**Asset allocation** is *what* you own (60% stocks, 40% bonds). **Asset location** is *where* you hold it. Two investors with identical 60/40 portfolios can pay very different tax bills depending on which account holds the bonds. Location only matters if you have money in more than one type of account; if everything is in a 401(k), skip this file.

## The three account types

| Account | Taxed going in | Taxed while growing | Taxed coming out |
|---|---|---|---|
| **Taxable** brokerage | Yes | Yes — dividends and interest every year; capital gains when sold | Only the gain, at capital-gains rates |
| **Tax-deferred** (traditional 401(k), IRA) | No (deductible) | No | Everything, as ordinary income; RMDs from age 73–75 |
| **Tax-free** (Roth 401(k), Roth IRA, HSA for medical) | Yes | No | Nothing |

RMD = required minimum distribution, the amount the IRS forces you to withdraw each year from tax-deferred accounts in your seventies.

## Which assets are tax-hungry

The question for each asset is: how much of its return gets taxed *every year* in a taxable account, and at what rate?

| Asset | Annual tax drag in taxable | Why |
|---|---|---|
| High-yield (junk) bonds | Very high | Big coupons taxed as ordinary income |
| REITs | Very high | Dividends mostly non-qualified (ordinary rates) |
| Taxable bond funds, TIPS | High | Interest at ordinary rates; TIPS also tax "phantom" inflation adjustments |
| Actively managed stock funds | Medium–high | Frequent trading throws off short-term gains |
| International stock index funds | Low–medium | Higher dividends, but you get a foreign tax credit *only* in taxable |
| U.S. total-market / S&P 500 index funds and ETFs | Low | ~1.3% qualified dividends; almost no capital-gains distributions |
| Growth / low-dividend stocks, tax-managed funds | Very low | Nearly all return is deferred capital gain |
| Municipal bonds | Low | Federally tax-exempt — meant for taxable accounts |

Bogleheads' rule of thumb: bond funds are the most important thing to shelter, because their entire return is interest taxed at your full marginal rate, whereas a broad stock index fund is already about as tax-efficient as an investment gets.

## The priority order

1. **Fill tax-advantaged space with the least tax-efficient assets first**: REITs, high-yield bonds, taxable bond funds, actively managed funds.
2. **Put the highest expected-growth assets in Roth** when you have a choice between traditional and Roth: the Roth is never taxed again and has no RMDs, so you want it to grow the most. Small-cap value, emerging markets, and total stock market are common Roth choices. (Counter-argument: a 401(k) dollar and a Roth dollar are not equal — the government "owns" part of the traditional dollar — so the after-tax risk differs. Most investors can ignore this nuance.)
3. **Put tax-efficient stock index funds in taxable.** They benefit from lower capital-gains rates, deferral until sale, tax-loss harvesting opportunities, the foreign tax credit (international funds), and a basis step-up at death.
4. **Whatever is left goes wherever there is room**, keeping the *overall* allocation on target.

## Worked example

Household with $600,000, target 60/40, 20% of stocks international:

| Account | Balance |
|---|---|
| 401(k) (traditional) | $300,000 |
| Roth IRA | $100,000 |
| Taxable brokerage | $200,000 |

Targets: $240,000 bonds, $288,000 U.S. stocks, $72,000 international stocks.

**Tax-efficient location:**

| Account | Holdings |
|---|---|
| 401(k) $300k | $240k total bond fund + $60k U.S. stock index |
| Roth $100k | $100k U.S. stock index (highest growth, tax-free forever) |
| Taxable $200k | $128k U.S. stock index + $72k international index |

The bonds are entirely sheltered, the international fund is in taxable where the foreign tax credit works, and the Roth carries all-stock exposure. The household allocation is exactly 60/40.

**Tax-inefficient version** — each account holds its own 60/40 mix — would put $120,000 of bonds in taxable and $40,000 in the Roth. At a 4.5% yield and a 32% bracket, the taxable bonds cost about $1,700 a year in tax that the efficient version avoids, and the Roth wastes tax-free space on the lowest-growth asset.

## How much is it worth?

Studies from Vanguard, Morningstar and Kitces put the value of good asset location at roughly **0.1% to 0.75% per year** depending on tax bracket, allocation and how much bond income you have. It is larger when yields are high (as in 2023–2026) and when you are in a high bracket. It is small if you are in the 12% bracket or your portfolio is mostly stocks anyway.

## Complications and judgement calls

- **Rebalancing gets harder.** If all bonds live in the 401(k), you rebalance mostly there — usually fine, since that's the tax-free place to trade.
- **Behavioural risk.** Some people can't stand seeing their Roth "all stocks" fall 40% while the 401(k) looks calm. If mirroring the allocation in every account keeps you invested, that is worth more than the location bonus.
- **Muni bonds** flip the logic for high earners: they belong in taxable and can make holding bonds outside the 401(k) sensible.
- **Roth conversions and early retirement**: if you'll convert traditional to Roth in low-income years, keep the traditional account's growth modest (bonds) so conversions stay cheap.
- **HSA**: triple tax-advantaged; if you pay medical costs out of pocket, treat the HSA as the best Roth you have and hold stocks in it.
- **Space runs out.** If tax-advantaged accounts are smaller than your bond target, hold the overflow bonds in taxable (munis or Treasuries — Treasury interest is state-tax-free) rather than abandoning your allocation.

## How to actually do it

1. Total every account and compute your target dollar amounts per asset class for the *household*.
2. List assets from least to most tax-efficient (table above).
3. Assign the worst offenders (bonds, REITs, active funds) to the 401(k)/traditional IRA until it's full.
4. Assign the highest-growth stock funds to Roth accounts and the HSA.
5. Assign broad U.S. and international index funds to taxable.
6. Check that the combined allocation hits the target. Adjust the 401(k) holdings to make the numbers work — it's the flexible account.
7. Set the taxable account to specific-ID lots and turn off dividend reinvestment (see [tax-loss-harvesting.md](tax-loss-harvesting.md)).
8. Rebalance across accounts as one portfolio (see [rebalancing.md](rebalancing.md)).

## Key takeaways

- Same allocation, different accounts, different tax bill — location is free money once you have more than one account type.
- Shelter bonds, REITs, high-yield and active funds in tax-deferred accounts first.
- Hold broad stock index funds in taxable: low dividends, deferred gains, foreign tax credit, loss-harvesting, step-up at death.
- Put your highest-expected-growth assets in Roth (and HSA) space.
- Worth roughly 0.1–0.75%/year; more when yields and your bracket are high.
- Manage the household as a single portfolio and rebalance inside the 401(k).
- If mirroring every account keeps you from panicking, that beats the location bonus.

## Sources

- [Bogleheads wiki – Tax-efficient fund placement](https://www.bogleheads.org/wiki/Tax-efficient_fund_placement)
- [Bogleheads wiki – Principles of tax-efficient fund placement (Forbes summary)](https://www.forbes.com/sites/thebogleheadsview/2011/12/01/exploring-the-bogleheads-wiki/)
- [Vanguard – Asset location can lead to lower taxes](https://investor.vanguard.com/investor-resources-education/article/asset-location-can-lead-to-lower-taxes)
- [Vanguard research – Revisiting conventional wisdom regarding asset location](https://externalcrewnet.vanguard.com/content/dam/corp/research/pdf/revisiting_conventional_wisdom_regarding_asset_location.pdf)
- [White Coat Investor – Asset location optimization](https://www.whitecoatinvestor.com/asset-location/)
- [Kitces – Asset location: the new wealth management value-add](https://www.kitces.com/blog/asset-location-the-new-wealth-management-value-add-for-optimal-portfolio-design/)
- [IRS – Retirement plan and IRA required minimum distributions FAQs](https://www.irs.gov/retirement-plans/retirement-plan-and-ira-required-minimum-distributions-faqs)
