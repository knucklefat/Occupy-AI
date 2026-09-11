# Tax-Loss Harvesting

**In one sentence:** Tax-loss harvesting means selling an investment that has dropped, booking the loss to offset taxable gains (and up to $3,000 of ordinary income a year), and immediately buying a similar-but-not-identical fund so you stay invested — it is mostly a tax *deferral*, worth roughly 0.2–0.5% a year to the right investor and nothing to the wrong one.

## Mechanics

You bought a total-market index fund for $50,000. It is now worth $40,000. You sell, realising a **$10,000 capital loss**, and the same day buy $40,000 of a different broad U.S. stock fund (say, an S&P 500 fund). Your market exposure is essentially unchanged, but you now hold a $10,000 loss you can use on your tax return.

What the loss does, in order:

1. Offsets capital gains of the same type first (short-term losses against short-term gains, long-term against long-term), then across types.
2. Any excess offsets up to **$3,000 of ordinary income** per year ($1,500 if married filing separately).
3. Anything left **carries forward indefinitely** to future years.

**Short-term** means held one year or less (gains taxed as ordinary income, up to 37% federal); **long-term** means held more than one year (0%, 15% or 20% federal, plus 3.8% net investment income tax for high earners).

## The wash-sale rule

The IRS disallows a loss if you buy the same or a "substantially identical" security within **30 days before or 30 days after** the sale — a 61-day window. Key points people get wrong:

- **It covers all your accounts**, including IRAs (Revenue Ruling 2008-5) and your spouse's accounts. Buying the fund you just sold inside your 401(k) — via automatic contributions or dividend reinvestment — triggers it.
- The disallowed loss is not gone forever; it is **added to the cost basis** of the replacement shares. But if the wash happens in an IRA, the loss is lost permanently.
- "Substantially identical" is not defined by statute. The conservative consensus: two funds tracking the **same index** (e.g., two S&P 500 ETFs) are risky; two funds tracking **different indexes** with similar exposure (S&P 500 vs. total market vs. Russell 1000) are widely treated as fine. Individual stocks are only identical to themselves (and their options/convertibles).
- Automatic dividend reinvestment is the most common accidental wash. Turn it off in taxable accounts if you harvest.

## Tax-lot selection: specific ID vs. FIFO

Every purchase creates a **tax lot** with its own cost basis. When you sell, your broker's default method — usually **FIFO** (first in, first out) or average cost for mutual funds — decides which lot goes. FIFO sells your oldest, usually lowest-cost, shares: the *worst* choice for harvesting.

Set your account to **specific identification** (Fidelity, Schwab and Vanguard all allow this; on Vanguard it's "SpecID"). Then you can sell exactly the lots that show a loss while leaving the gains alone.

| Lot | Bought | Cost | Value today | Gain/Loss |
|---|---|---|---|---|
| A | 2019 | $20,000 | $34,000 | +$14,000 |
| B | Jan 2025 | $15,000 | $13,500 | −$1,500 |
| C | Mar 2025 | $15,000 | $12,000 | −$3,000 |

With specific ID you sell lots B and C, book a $4,500 loss and keep lot A untouched. Under FIFO you would sell lot A and *owe* tax on $14,000.

## Partner funds

Keep a written list of pairs so you can act quickly on a down day:

| Sold | Replacement (different index) |
|---|---|
| Total U.S. market (VTI/VTSAX) | S&P 500 (VOO) or Russell 1000 (IWB) |
| S&P 500 (VOO/IVV) | Total market (ITOT) or large-cap (SCHX) |
| Total international (VXUS) | FTSE developed + emerging split (VEA + VWO), or IXUS |
| U.S. small-cap value (VBR) | S&P 600 value (VIOV) or Russell 2000 value (VTWV) |
| Total bond (BND) | Intermediate core bond (SCHZ) or AGG |

Ideally hold the replacement for 31+ days, then either keep it or switch back if you prefer the original (only if the replacement hasn't gained enough to make switching back costly).

## Why it's deferral, not free money

When you harvest, you reset your cost basis lower. In the example above, you owned shares with a $50,000 basis; now you own shares with a $40,000 basis. When you eventually sell, you will have $10,000 *more* gain than you otherwise would. As Michael Kitces puts it, the net tax is often "the exact same as would have occurred if the loss was never harvested." What you actually gain:

- **Time value**: an interest-free loan of the tax saved, invested for years. Kitces estimates this is worth roughly **0.2–0.3% per year** of extra return for a typical case.
- **Rate arbitrage**: harvest a *short-term* loss to offset ordinary income at 32–37% today, and pay 15–20% long-term rates on the recovery gain later. This is where most of the real value lives.
- **Permanent escape**: if you hold the replacement shares until death (basis steps up to market value) or donate them to charity, the deferred gain is never taxed. Then harvesting is pure gain.

## When it's worth it — and when it isn't

**Worth it:** you have a taxable account with meaningful lots showing losses; you are in a high bracket now and expect a lower one in retirement; you have capital gains to offset (from other sales, fund distributions, or a business); you plan to donate or bequeath appreciated shares.

**Not worth it / harmful:**
- You are in the **0% long-term capital gains bracket** (taxable income under roughly $48,000 single / $97,000 married in 2025). Harvesting *lowers* your basis for no benefit — you should be harvesting *gains* instead.
- You expect to be in a **higher** bracket when you sell.
- The loss is small (under ~$500) and the transaction costs or complexity aren't worth it.
- Your only holdings are in IRAs/401(k)s — there is nothing to harvest.

## Robo-advisor TLH

Wealthfront, Betterment, Schwab Intelligent Portfolios and others harvest daily and advertise large "tax alpha" — Wealthfront has claimed a median benefit several times its 0.25% fee. Kitces' analysis of these claims finds that once you remove favourable assumptions (constant new contributions, short-term/long-term rate arbitrage, always having gains to offset), the realistic figure drops to roughly **0.2–0.7% a year**, and can fall below the advisory fee for investors without contributions or gains. Wealthfront was fined by the SEC in 2018 after wash sales occurred in a large share of client accounts — software cannot see your 401(k) or your spouse's IRA. If you use one, keep all your taxable and retirement accounts consistent with its fund list, and turn off outside dividend reinvestment.

## How to actually do it

1. Switch every taxable account's cost-basis method to **specific identification** today, before you need it.
2. Turn off automatic dividend reinvestment in taxable accounts (reinvest manually into whichever fund is underweight).
3. Write down your partner-fund pairs and check that none of them appear in your 401(k) contributions.
4. On a down day, open the lot view. Sell only lots with losses larger than ~$500 or ~5%, preferring **short-term** losses if you have short-term gains or high ordinary income.
5. Buy the partner fund with the proceeds the same day.
6. Note the date; no purchases of the sold fund in any account for 31 days.
7. At tax time, enter the loss on Form 8949 / Schedule D; track the carryforward.
8. Don't obsess. A few harvests in bear markets (2008, 2020, 2022) capture most of the lifetime value.

## Key takeaways

- TLH turns paper losses into tax deductions while keeping you invested through a similar replacement fund.
- Losses offset gains first, then $3,000/year of ordinary income, and carry forward indefinitely.
- The wash-sale window is 30 days before and after, across *all* your and your spouse's accounts, IRAs included.
- Use specific-ID lot selection; FIFO sells your best lots.
- It is mostly deferral, worth ~0.2–0.5%/year; real value comes from rate arbitrage, donation, or step-up at death.
- Useless or harmful in the 0% capital-gains bracket — harvest gains there instead.
- Robo-advisor "tax alpha" claims are inflated; realistic figures are a fraction of a percent.

## Sources

- [IRS Publication 550 – Investment Income and Expenses (wash sales, capital losses)](https://www.irs.gov/publications/p550)
- [IRS – Topic No. 409, Capital Gains and Losses](https://www.irs.gov/taxtopics/tc409)
- [Kitces – Calculating the True Benefits of Tax Loss Harvesting](https://www.kitces.com/blog/evaluating-the-tax-deferral-and-tax-bracket-arbitrage-benefits-of-tax-loss-harvesting/)
- [Kitces – Is Automated Tax-Loss Harvesting Software Worth It?](https://www.kitces.com/blog/automated-tax-loss-harvesting-technology-software-value-risks-gaps-benefits/)
- [Bogleheads wiki – Tax loss harvesting](https://www.bogleheads.org/wiki/Tax_loss_harvesting)
- [Bogleheads wiki – Wash sale](https://www.bogleheads.org/wiki/Wash_sale)
