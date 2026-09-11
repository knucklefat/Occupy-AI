# ETF and Fund Due Diligence

**In one sentence:** Two funds with nearly identical names can deliver very different results, so before buying any ETF or mutual fund you should know exactly what it holds (index methodology), what it costs in total (expense ratio plus tracking difference plus spread), and how it will treat you at tax time.

## Start with exposure, not cost

Schwab Asset Management's evaluation framework makes a point most investors get backwards: the choice of *what the fund holds* can swing returns by thousands of basis points, while the difference in fees between two similar funds is measured in hundredths of a percent. Get the exposure right first, then minimize cost among the funds that deliver it.

Exposure questions:
- **What index does it track, and how is the index built?** Market-cap weighted, equal weighted, factor-tilted, or rules-based ("smart beta")? Two "dividend" ETFs can hold completely different stocks depending on whether the index screens for yield, dividend growth, or payout consistency.
- **Selection rules and rebalancing.** How often does the index reconstitute? High turnover means more trading costs and taxable events.
- **Concentration.** Top-10 holdings as a share of the fund. A "technology" ETF can be 40% in three stocks.
- **Size and style breakpoints.** Index providers disagree on where "large cap" ends and what counts as "value"; check the fund's holdings against a plain cap-weighted benchmark to see the real tilt.
- **For bond ETFs:** duration, credit-quality mix, and whether it holds physical bonds or samples the index.
- **For commodity or leveraged ETFs:** whether exposure comes from futures (roll costs) and how daily resetting affects multi-day returns. Leveraged and inverse ETFs are trading tools, not holdings.

## The cost stack

The expense ratio is only the visible layer.

| Cost | What it is | Where to find it | Typical range |
|---|---|---|---|
| **Expense ratio** | Annual management fee deducted from assets | Fact sheet, prospectus | 0.03% broad index; 0.20–0.60% factor/sector; 0.5–1%+ active |
| **Tracking difference** | Fund return minus index return over a period; the real all-in cost of indexing | Fund's annual report, Morningstar | Roughly −expense ratio; can be better via securities lending, worse via cash drag |
| **Tracking error** | Standard deviation of the return gap; measures *consistency* of tracking | Morningstar, issuer site | <0.1% for large index ETFs; higher for sampled or illiquid indexes |
| **Bid-ask spread** | Difference between buying and selling price when you trade | Broker quote, issuer site | 0.01% for the largest ETFs; 0.2–0.8%+ for thinly traded ones |
| **Premium/discount to NAV** | Difference between market price and the value of holdings | Issuer site daily | Near zero for liquid ETFs; wider for bond, international, and niche funds |
| **Capital gains distributions** | Taxable gains the fund passes to you | Annual report, issuer site | Near zero for most equity ETFs; can be large for mutual funds |

**Worked example.** Fund A charges 0.05% but trails its index by 0.17% because of cash drag and poor sampling. Fund B charges 0.10% but trails by only 0.13% thanks to securities-lending income. Fund B is cheaper to own despite the higher sticker price. Always compare tracking difference over three to five years, not just the expense ratio.

**On spreads:** a 0.30% spread on a fund you hold for ten years is trivial; on one you trade monthly it exceeds most expense ratios. Use limit orders and avoid trading in the first and last fifteen minutes of the session, when spreads are widest.

## AUM and liquidity

Assets under management (AUM) matter for two reasons: funds below roughly $50–100M are at risk of closing (which forces a taxable liquidation), and very small funds tend to have wide spreads. But the deeper truth about ETF liquidity is that it depends on the *underlying holdings*, not the ETF's own trading volume, because authorized participants can create or redeem shares. A low-volume ETF holding S&P 500 stocks is perfectly liquid; a high-volume ETF holding frontier-market bonds is not.

## Tax efficiency

- **ETFs vs. mutual funds.** ETFs use in-kind redemptions that let them shed low-cost-basis shares without selling, so most equity ETFs distribute almost no capital gains. Mutual funds must sell holdings to meet redemptions and pass gains to all remaining holders — you can owe tax on gains you never enjoyed. In taxable accounts, this is a strong reason to prefer ETFs.
- **Dividend type.** Qualified dividends are taxed at lower rates than ordinary income; a fund's tax-cost ratio on Morningstar captures the drag.
- **Bond funds and REIT funds** pay ordinary income; hold them in tax-advantaged accounts when possible.
- **International funds** may withhold foreign taxes; in taxable accounts you may claim a foreign tax credit, in IRAs you cannot.
- **Fund structure.** Commodity funds structured as partnerships issue K-1s; some use a different structure to avoid this. Check before buying.

## Active vs. passive

The evidence, updated every year by S&P's SPIVA scorecard and Morningstar's Active/Passive Barometer, is consistent: over 10–15 year periods, roughly 85–90% of actively managed U.S. large-cap equity funds underperform their benchmark after fees. Results are somewhat better for active managers in less efficient corners (small caps, some bond categories, international small caps) but still below 50% success in most categories over long horizons.

When an active fund might earn its fee: a genuinely differentiated process, low fees relative to peers, manager ownership of the fund, capacity discipline (closing to new money), and a long record measured against the *right* benchmark. Morningstar's guidance on judging active ETFs emphasizes process, people, and cost, in that order. Absent those, the default should be the cheapest broad index fund that delivers the exposure you want.

## Reading a fact sheet and prospectus

**Fact sheet (two pages, updated monthly):** objective, index, expense ratio, AUM, inception date, top-10 holdings, sector/country weights, performance vs. index (look at the gap — that is tracking difference), yield, and for bond funds duration and credit breakdown.

**Summary prospectus (a few pages):** investment objective, fees table (including any 12b-1 marketing fee or load), principal strategies, principal risks, past performance, portfolio managers, purchase/sale info, and tax information. Read the "principal strategies" section — it says whether the fund may use derivatives, lend securities, or sample the index.

**Statement of additional information (SAI)** and **annual report:** detailed holdings, turnover, and the fund's own tracking commentary. The annual report is where you find the actual return gap over multiple years.

## Overlap tools

Owning three funds that hold the same ten stocks is not diversification. Free tools:

- **ETF Research Center Fund Overlap** (etfrc.com/tools/overlap.php): enter two tickers, get the percentage overlap by weight and the shared holdings.
- **Morningstar Instant X-Ray / Portfolio Manager:** shows combined stock, sector, and region exposure across all your holdings and flags concentration.
- **Issuer comparison tools** on Vanguard, iShares, and Schwab sites show side-by-side holdings.

Rule of thumb: two funds with more than 60–70% weighted overlap are effectively the same fund; keep the cheaper one.

## How to actually do it

1. Write down the exposure you want in one sentence ("U.S. total stock market," "international developed large cap," "intermediate investment-grade bonds").
2. List three to five funds that claim to deliver it. Open each fact sheet and record: index, expense ratio, AUM, inception date, top-10 weight, and (for bonds) duration and credit mix.
3. Compare the indexes. Note how each selects and weights holdings and how often it rebalances. Eliminate any whose methodology does not match your intent.
4. Pull three- and five-year tracking difference (fund return minus index return) from the fund's annual report or Morningstar. Rank the survivors by this, not by expense ratio alone.
5. Check the bid-ask spread and average premium/discount on the issuer site. For funds you will trade rarely, this matters little; for frequent trading, weigh it heavily.
6. Check the tax profile: structure (ETF vs. mutual fund), history of capital gains distributions, dividend qualification, K-1 issues.
7. Run an overlap check against what you already own.
8. Read the summary prospectus's principal strategies and risks. Confirm no leverage, derivatives, or sampling you did not expect.
9. Buy with a limit order during mid-session hours.
10. Review annually: has the index changed, the fee changed, AUM fallen, or tracking worsened?

## Key takeaways

- Exposure first: the index methodology determines returns far more than fee differences do.
- Total cost = expense ratio + tracking difference + spread + tax drag; compare funds on tracking difference, not just the sticker fee.
- Tracking difference is the size of the gap; tracking error is its consistency.
- ETF liquidity comes from the underlying holdings, not the ETF's volume, but very small funds risk closure.
- ETFs are usually more tax-efficient than mutual funds in taxable accounts because of in-kind redemptions.
- Long-run data show most active funds underperform after fees; demand a specific reason before paying for active management.
- Read the fact sheet for exposure and the summary prospectus for strategy and risks; use overlap tools to avoid owning the same stocks three times.
- Use limit orders and avoid trading at the open and close.

## Sources

- [Schwab Asset Management: How to evaluate ETFs](https://www.schwabassetmanagement.com/content/how-to-evaluate-etfs)
- [Morningstar: Tracking Difference vs. Tracking Error — How to Analyze ETFs](https://www.morningstar.com/business/insights/blog/funds/etf-tracking-difference-error)
- [Morningstar: How to Judge an Active ETF](https://www.morningstar.com/funds/how-judge-an-active-etf)
- [State Street: An ETF due diligence checklist](https://www.ssga.com/us/en/intermediary/insights/a-etf-due-diligence-checklist)
- [State Street: How to analyze total cost of ownership](https://www.ssga.com/us/en/intermediary/insights/how-to-analyze-total-cost-of-ownership)
- [S&P Dow Jones Indices: SPIVA U.S. Scorecard](https://www.spglobal.com/spdji/en/research-insights/spiva/)
- [ETF Research Center: Fund Overlap tool](https://www.etfrc.com/tools/overlap.php)
- [Investor.gov: Exchange-Traded Funds (ETFs)](https://www.investor.gov/introduction-investing/investing-basics/investment-products/mutual-funds-and-exchange-traded-funds-etfs)
