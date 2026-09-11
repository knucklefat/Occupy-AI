# How to Read Financial Statements

**In one sentence:** The three core financial statements — income statement, balance sheet, and cash flow statement — are three different camera angles on the same business, and you only understand a company once you have looked through all three and checked that they agree with each other.

## Why three statements?

Each statement answers a different question:

| Statement | Question it answers | Time frame | Accounting basis |
|---|---|---|---|
| Income statement | Did the company make a profit this period? | A span of time (quarter/year) | Accrual (revenue when earned, expenses when incurred) |
| Balance sheet | What does it own and owe right now? | A single moment (period-end) | Snapshot of historical cost and estimates |
| Cash flow statement | Where did the cash actually come from and go? | A span of time | Cash only — no estimates |

Accounting is done on an **accrual** basis, meaning revenue is booked when a sale is made, not when the customer pays. That is useful but creates room for judgment. The cash flow statement is the antidote: cash is hard to fake. Experienced analysts read the cash flow statement first, then the balance sheet, then the income statement.

## The income statement

Read it top to bottom as a waterfall:

```
Revenue (sales)
– Cost of goods sold (COGS)
= Gross profit                     → Gross margin = Gross profit / Revenue
– Operating expenses (R&D, SG&A)
= Operating income (EBIT)          → Operating margin
– Interest expense
– Taxes
= Net income                       → Net margin
÷ Diluted shares outstanding
= Diluted earnings per share (EPS)
```

**What to look for:**

- **Revenue growth and its source.** Is growth from more units, higher prices, or acquisitions? The MD&A section of the 10-K usually breaks this out.
- **Margin trend.** A gross margin that is stable or rising suggests pricing power. A falling gross margin with rising revenue often means the company is buying growth with discounts.
- **Operating leverage.** If operating income grows faster than revenue, fixed costs are being spread over more sales — a good sign.
- **One-time items.** "Restructuring," "impairment," and "gain on sale" are excluded from adjusted earnings. Look at how often "one-time" items recur; if every year has them, they are not one-time.
- **Diluted vs. basic shares.** Diluted counts stock options and convertibles. Rising diluted share count means your ownership is shrinking.

**Worked example.** A company reports revenue of $1,000M, COGS of $600M, operating expenses of $250M, interest of $20M, and a 21% tax rate.
Gross profit = $400M (40% gross margin). Operating income = $150M (15% operating margin). Pre-tax = $130M; tax = $27.3M; net income = $102.7M (10.3% net margin). With 50M diluted shares, EPS = $2.05.

## The balance sheet

The balance sheet always balances: **Assets = Liabilities + Shareholders' Equity**. Equity is what would be left if you sold every asset and paid every debt — at book value, which often differs wildly from market value.

**Assets (in order of liquidity):** cash and equivalents, short-term investments, accounts receivable (money customers owe), inventory, then long-term items: property/plant/equipment (PP&E), intangibles, and goodwill (the premium paid in past acquisitions above the target's book value).

**Liabilities:** accounts payable (what the company owes suppliers), accrued expenses, short-term debt, deferred revenue (cash collected for services not yet delivered — a liability, but often a good sign), long-term debt, leases, pension obligations.

**What to look for:**

- **Net cash or net debt** = cash − total debt. A net cash position is a cushion; heavy net debt makes a company fragile in a downturn.
- **Working capital** = current assets − current liabilities. Negative working capital is fine for a business that collects before it pays (retailers, subscription software) and dangerous for one that does not.
- **Receivables and inventory growing faster than sales.** This is the classic early warning that customers are not paying or product is not selling.
- **Goodwill as a share of equity.** If goodwill is most of the equity, the "book value" is really just the memory of past acquisition prices and can be written down at any time.
- **Debt maturities.** Notes to the financial statements list when debt comes due. A wall of maturities in a bad year is a real risk.

## The cash flow statement

Three sections:

1. **Cash from operations (CFO):** starts with net income, adds back non-cash charges (depreciation, stock-based compensation), and adjusts for working capital changes.
2. **Cash from investing:** capital expenditures (capex), acquisitions, purchases/sales of securities.
3. **Cash from financing:** debt raised or repaid, shares issued or bought back, dividends paid.

The number most investors care about is **free cash flow (FCF) = CFO − capex**. It is the cash left over for shareholders after maintaining and growing the business.

**What to look for:**

- **CFO vs. net income.** Over several years, CFO should be roughly equal to or larger than net income. If net income is consistently well above CFO, earnings quality is suspect — profits are being recognized that never turn into cash.
- **Capex vs. depreciation.** Capex well above depreciation means the company is investing to grow; capex well below depreciation for years means it may be under-investing and the asset base is aging.
- **Stock-based compensation (SBC).** It is added back to CFO because it is non-cash, but it is a real cost to you via dilution. Many analysts subtract it from FCF.
- **How FCF is used.** The financing section tells you whether cash goes to buybacks, dividends, debt paydown, or acquisitions — a window into management's capital allocation.

Continuing the example: net income $102.7M, depreciation $40M, SBC $15M, working capital used $10M → CFO = $147.7M. Capex $50M → FCF = $97.7M. FCF of $97.7M versus net income of $102.7M is a healthy, cash-backed result.

## Red flags checklist

| Red flag | Where to see it | What it may mean |
|---|---|---|
| Net income rising, CFO flat or falling | Income statement vs. cash flow | Aggressive revenue recognition |
| Receivables growing faster than revenue | Balance sheet vs. income statement | Channel stuffing, loose credit |
| Inventory growing faster than revenue | Balance sheet | Weak demand, coming write-downs |
| Frequent "non-recurring" charges | Income statement | Ordinary costs disguised as unusual |
| Big gap between GAAP and "adjusted" EPS | Earnings release | Management hiding real costs |
| Change in auditor or accounting policy | 10-K Item 9, notes | Possible disagreement over numbers |
| Growing goodwill with weak returns | Balance sheet | Overpaying for acquisitions |
| Rising debt while buying back shares | Cash flow, financing | Leveraging up to prop up EPS |
| Related-party transactions | Notes, proxy statement | Insiders extracting value |

## Where to find the statements

- **SEC EDGAR** ([sec.gov/edgar](https://www.sec.gov/edgar/search/)): every U.S.-listed company's 10-K (annual) and 10-Q (quarterly) filings, free. Use "Financial Report" view for interactive data.
- **Investor relations pages:** search "[company] investor relations." Look for annual reports, earnings releases, and presentations.
- **Aggregators:** Stock Analysis, Macrotrends, Yahoo Finance, and Koyfin show 10+ years of statements in one table, which is far better for spotting trends than reading one filing at a time.

## How to actually do it

1. Pull five to ten years of all three statements from an aggregator or EDGAR.
2. Start with the cash flow statement. Compute FCF each year and compare it with net income. Ask: does this business generate cash?
3. Move to the balance sheet. Compute net debt, working capital, and goodwill as a share of equity. Ask: can it survive a bad year?
4. Read the income statement. Track revenue growth and the three margins. Ask: is the business getting better or worse?
5. Compute the ratio of receivables and inventory to revenue for each year and look for drift.
6. Read the notes to the financial statements for debt maturities, lease obligations, segment data, and revenue recognition policy.
7. Write one paragraph in plain words describing how the company makes money and where the cash goes. If you cannot, you do not understand it yet.

## Key takeaways

- The three statements are linked: net income flows into equity and into the cash flow statement; cash on the cash flow statement ends up on the balance sheet.
- Cash from operations is harder to manipulate than net income; compare them every year.
- Free cash flow (CFO − capex) is the number that ultimately funds dividends, buybacks, and growth.
- Watch receivables and inventory relative to sales — they are the earliest warning signs.
- Book value is often meaningless when goodwill dominates equity.
- Recurring "one-time" charges are ordinary expenses.
- Always read the notes; the statements are the summary, the notes are the story.
- EDGAR is free, complete, and primary — use it over any secondhand summary.

## Sources

- [SEC: Beginners' Guide to Financial Statements](https://www.sec.gov/about/reports-publications/investorpubsbegfinstmtguide)
- [SEC EDGAR Full-Text Search](https://www.sec.gov/edgar/search/)
- [Harvard Business School Online: How to Read Financial Statements](https://online.hbs.edu/blog/post/how-to-read-financial-statements)
- [The Motley Fool: Beginner's Guide to Financial Statements](https://www.fool.com/investing/how-to-invest/stocks/beginners-guide-financial-statements/)
- [Investor.gov: How to Read a 10-K/10-Q](https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-bulletins/how-read)
