# How Markets Work

**In one sentence:** A stock market is a continuous auction where buyers and sellers meet through exchanges and market makers, your broker translates your order into a trade that settles one business day later, and the products you buy — individual stocks, mutual funds, or ETFs — differ mainly in how they are priced, traded, taxed, and what they cost.

## Exchanges: the auction floor

An **exchange** is a regulated venue where securities are bought and sold. The two big U.S. stock exchanges are the **New York Stock Exchange (NYSE)** and **Nasdaq**; together with a dozen smaller exchanges (Cboe, IEX, etc.) and off-exchange venues, they form one linked national market. Regular trading hours are 9:30 a.m. to 4:00 p.m. Eastern, Monday through Friday, excluding market holidays; pre-market and after-hours sessions exist but are thinner and jumpier.

Companies list on an exchange through an **IPO** (initial public offering) — the first sale of shares to the public. That is the **primary market**: the company receives the money. Every trade after that is the **secondary market**: shares change hands between investors, and the company gets nothing. When you "buy Apple," you are buying from another investor, not from Apple.

The **SEC** (Securities and Exchange Commission) is the federal regulator; **FINRA** is the industry self-regulator that oversees brokers. The **SIPC** insures brokerage accounts up to $500,000 against the *broker* failing (not against your investments losing value).

## Market makers and the bid/ask spread

At any moment, a stock has two prices:

- The **bid** — the highest price someone is currently willing to pay.
- The **ask** (or offer) — the lowest price someone is currently willing to sell for.

The gap is the **spread**. For Apple or an S&P 500 ETF it is a penny or less; for a thinly traded small-cap or an obscure ETF it can be 1% or more. You buy at the ask and sell at the bid, so the spread is a real (if invisible) cost — round-tripping a stock with a 1% spread costs you 1% before it moves at all.

**Market makers** are firms (Citadel Securities, Virtu, Jane Street, and others) that stand ready to buy or sell continuously, earning the spread as their profit. They provide **liquidity** — the ability to trade quickly without moving the price. Most retail broker orders never reach an exchange; they are routed to a market maker under **payment for order flow (PFOF)**, in which the market maker pays the broker for the privilege of filling your order, typically at a price slightly better than the public quote. It is why "commission-free" trading exists and why regulators keep scrutinizing it.

## Order types

| Order | What it does | When to use it | Trap |
|---|---|---|---|
| **Market** | Buy or sell immediately at the best available price | Liquid stocks and ETFs during market hours, when getting filled matters more than the exact price | Price is not guaranteed; in a fast or thin market you can fill far from the last trade. Never use before the open. |
| **Limit** | Buy at or below (or sell at or above) a price you set | Almost always, for anything less liquid than a mega-cap | May never fill if the price doesn't reach your limit |
| **Stop (stop-loss)** | Becomes a *market* order once the price touches your stop | Automating an exit you might not have the discipline to make | Fills at the next available price, which in a crash can be far below your stop; triggered by brief intraday spikes |
| **Stop-limit** | Becomes a *limit* order once the stop is hit | When you want a stop but refuse to sell below a floor | May not fill at all if the price gaps through both levels |
| **Trailing stop** | A stop that ratchets up as the price rises, set as a % or $ below the high | Locking in gains on a winner | Same execution risk as a plain stop |

Time-in-force settings: **Day** (expires at the close) or **GTC** (good-till-canceled, usually 60–90 days at most brokers). The SEC's practical advice: understand that "the last-traded price is not necessarily the price at which a market order will be executed."

## Settlement

When you trade, ownership and cash change hands on the **settlement date**, not the trade date. Since May 28, 2024, U.S. stocks, ETFs, and corporate bonds settle **T+1** — one business day after the trade. (Options and government securities already settled T+1; mutual funds settle T+1 or T+2 depending on the fund.) Practically, this means the cash from a sale is available the next business day, and in a cash account you must have settled funds before buying — selling an unsettled position bought with unsettled cash is a "good-faith violation" that can get a cash account restricted.

## Indexes

An **index** is a list of securities with a rule for combining their prices into one number. It is a measuring stick, not something you can buy directly.

- **S&P 500** — ~500 large U.S. companies, weighted by market capitalization (bigger companies count more). Represents ~80% of U.S. stock market value.
- **Dow Jones Industrial Average** — 30 large companies, weighted by *share price*, an outdated quirk that makes it a poor benchmark despite its fame.
- **Nasdaq Composite** — all ~3,000+ stocks on the Nasdaq exchange, heavily tech.
- **Russell 2000** — 2,000 small-cap U.S. stocks.
- **CRSP US Total Market / Wilshire 5000** — essentially every U.S. stock.
- **MSCI EAFE, MSCI ACWI ex-US, FTSE All-World ex-US** — developed and/or emerging markets outside the U.S.
- **Bloomberg U.S. Aggregate** ("the Agg") — the standard U.S. investment-grade bond index.

**Market-cap weighting** is the default because it is self-rebalancing (you never have to trade as prices change) and reflects the market's own bets. The downside is concentration: by 2025–26 the ten largest stocks were roughly 35–40% of the S&P 500. Equal-weight and fundamentally weighted indexes are the main alternatives.

## Individual stocks vs. mutual funds vs. ETFs

| | Individual stocks | Mutual funds | ETFs |
|---|---|---|---|
| **What you own** | One company | A pooled portfolio, priced once a day at 4 p.m. (NAV) | A pooled portfolio that trades all day like a stock |
| **Minimum** | One share (or fractional at most brokers) | Often $0–$3,000 | One share (or fractional) |
| **Pricing** | Continuous | End-of-day NAV | Continuous, at a price near NAV |
| **Diversification** | None — you build it | Built in | Built in |
| **Costs** | Spread; no expense ratio | Expense ratio; sometimes loads or 12b-1 fees | Expense ratio (usually lower); spread |
| **Tax efficiency (taxable accounts)** | You control when gains are realized | Can distribute capital gains you didn't ask for when other investors redeem | Usually far more efficient — the "in-kind" creation/redemption process lets ETFs avoid most capital gains distributions |
| **Automatic investing** | Limited | Easy (dollar amounts) | Easy at most brokers now |
| **Best for** | Concentrated bets, people who enjoy research | 401(k)s, automatic investing, some active strategies | Taxable accounts, low cost, flexibility |

**Index fund vs. active fund** is a separate axis: an index fund (mutual fund *or* ETF) simply holds what's in an index at minimal cost; an active fund pays managers to try to beat it. Over 15-year periods, roughly 85–90% of active U.S. large-cap funds trail the S&P 500 after fees (S&P's SPIVA scorecards). This is the strongest single finding in retail investing.

**Closed-end funds** and **interval funds** are cousins with fixed share counts and, for interval funds, limited redemption windows — mostly relevant for niche income strategies.

## Expense ratios and other fund costs

The **expense ratio** is the annual percentage of your assets the fund deducts to pay itself; you never see a bill, it simply lowers your return. Reference points (Morningstar, 2025):

- Asset-weighted average across all U.S. funds: **0.32%**.
- Broad index funds/ETFs from Vanguard, Fidelity, Schwab, iShares: **0.02%–0.10%**.
- Actively managed U.S. stock funds: asset-weighted ~0.58%, but equal-weighted ~1.0%.
- Anything above 1% needs a very good excuse. Anything with a **sales load** (a commission of 3–5.75% off the top) or **12b-1 fee** (a marketing charge embedded in the expense ratio) almost never has one.

Costs that don't show up in the expense ratio: the bid/ask spread on ETFs, **tracking error** (how far an index fund drifts from its index), and, for mutual funds in taxable accounts, capital gains distributions. For a buy-and-hold investor in a broad index fund, total all-in cost should be well under 0.1% per year.

## What actually moves prices

In the short run, prices move on the imbalance between buyers and sellers, which is driven by news, earnings surprises, interest-rate expectations, and sentiment — largely noise. In the long run, stock prices follow earnings and dividends; bond prices follow interest rates and credit quality. A price is not a verdict on a company's worth; it is the marginal trade between the most eager buyer and the most eager seller at 3:59 p.m. The rest of this library is about deciding when that marginal price is wrong.

## Key takeaways

- Trading is a secondary market: you buy from other investors, not the company; only IPOs raise capital.
- You buy at the ask and sell at the bid; the spread is a hidden cost that's tiny for large stocks and meaningful for small or obscure ones.
- Use **limit orders** by default; **market orders** only for very liquid securities during regular hours; treat **stop orders** as blunt instruments that can fill far below the stop in a crash.
- U.S. stocks and ETFs settle **T+1** (since May 2024); cash from a sale is spendable the next business day.
- An index is a measuring stick; an index fund is a product that tracks it. Market-cap weighting is standard but currently concentrated in a handful of mega-caps.
- ETFs are generally cheaper and more tax-efficient than mutual funds; mutual funds win for automatic investing and in 401(k)s.
- The asset-weighted average fund fee is ~0.32%; broad index funds cost 0.02–0.10%; ~85–90% of active funds trail their index over 15 years.
- Short-run prices are noise; long-run prices follow earnings, dividends, and interest rates.

## Sources

- [Investor.gov — Types of Orders](https://www.investor.gov/introduction-investing/investing-basics/how-stock-markets-work/types-orders)
- [SEC — Investor Bulletin: Stop, Stop-Limit, and Trailing Stop Orders](https://www.sec.gov/oiea/investor-alerts-bulletins/ib-stoporders)
- [Investor.gov — New "T+1" Settlement Cycle: What Investors Need to Know](https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins/new-t1-settlement-cycle-what-investors-need-know-investor-bulletin)
- [FINRA — Order Types](https://www.finra.org/investors/investing/investment-products/stocks/order-types)
- [Investor.gov — Mutual Funds and ETFs](https://www.investor.gov/introduction-investing/investing-basics/investment-products/mutual-funds-and-exchange-traded-funds-etfs)
- [Investor.gov — How Stock Markets Work](https://www.investor.gov/introduction-investing/investing-basics/how-stock-markets-work)
- [Morningstar — How Active ETFs Are Reshaping Fund Fees (2025 fee study)](https://www.morningstar.com/funds/how-active-etfs-are-reshaping-fund-fees)
- [Morningstar — Fund Fees Are Still Declining, But Not as Quickly](https://www.morningstar.com/financial-advisors/fund-fees-are-still-declining-not-quickly-they-once-were)
- [S&P Dow Jones Indices — SPIVA U.S. Scorecard](https://www.spglobal.com/spdji/en/research-insights/spiva/)
- [Bogleheads wiki — ETFs vs mutual funds](https://www.bogleheads.org/wiki/ETFs_vs_mutual_funds)
- [Bogleheads wiki — Expense ratios](https://www.bogleheads.org/wiki/Expense_ratios)
