# Learnings

*The residue of the whole library in one page — the ideas that survive when everything else is forgotten, plus the numbers that justify them. Mirrored from the Omnia vault topic note (2026-09-12).*

## The ten things that matter most

1. **Costs and behavior decide outcomes more than picks.** Most active managers lose to the index after fees (85–93% over 10–20 years), and investors lose another ~1.2 points a year to their own timing. Cheap, boring, automated wins by default.
2. **Time in the market beats timing.** Lump sum beat dollar-cost averaging about two-thirds of the time; the best days cluster within days of the worst, so leaving during panics forfeits the recovery.
3. **Write the rules in calm weather.** An investment policy statement — allocation, bands, contribution plan, what you will never do — is the single most protective document an investor owns. Panic is not the time to decide policy.
4. **Order of operations for each dollar:** emergency fund → employer match → HSA → Roth/traditional IRA → max 401(k) → taxable → mega-backdoor. The account matters as much as the fund.
5. **Rebalance by bands, not by feel.** The 5/25 rule (rebalance when an asset drifts 5 points absolute or 25% relative) captures most of the benefit with minimal trading and tax.
6. **Price follows earnings.** Lynch's six stock categories (slow growers, stalwarts, fast growers, cyclicals, turnarounds, asset plays) tell you what to expect and when to sell; PEG near 1 is fair, well below 1 is interesting.
7. **Indicators predict decades, not months.** CAPE and the Buffett indicator say something about 10-year returns and nothing about next year; the yield curve inverts 6–18 months before recessions but misfired in 2022–24. Count flags across families; never act on one.
8. **The stock doesn't know you own it.** Purchase price is irrelevant to value; anchoring on it is the root of the "silliest things people say about stocks."
9. **Withdraw at ~3.9–4.7%, adjust with guardrails.** Sequence risk in the first decade of retirement is the real danger; a bond tent or bucket approach blunts it.
10. **Verify before trusting.** Track records quoted in press differ from primary documents; every number worth acting on should be traceable to a filing, a regulator, or the original paper.

## Crypto, in five lines

- It is a speculative satellite: size it so an 80% loss doesn't change your life (0–5% for most people), and only after the rest of the plan is funded.
- Every Bitcoin cycle has drawn down 53–93%; the median retail app user has lost money; the frauds (Mt. Gox, Terra, FTX, Celsius) were the largest in modern finance.
- Custody is the whole game: hardware wallet bought from the manufacturer, metal seed backup in two places, no SMS two-factor, never sign what you don't understand. An ETF is a legitimate alternative to holding keys.
- If you don't know where the yield comes from, you are the yield.
- Crypto is taxed as property: every swap and spend is a taxable event; wallet-by-wallet basis since 2025; the wash-sale rule still does not apply as of September 2026.

## Frameworks worth reusing

- [Investment policy statement](10-checklists-and-templates/investment-policy-statement-template.md) — the template and a filled example live in the library's checklists section.
- [Market dashboard](05-market-indicators/how-to-build-a-market-dashboard.md) / [crypto dashboard](11-crypto/05-indicators/how-to-build-a-crypto-dashboard.md) — 15 traditional and 14 crypto indicators with normal / caution / alarm zones, free sources, FRED series IDs.
- [Six stock categories](07-publications-and-resources/book-summaries/one-up-on-wall-street.md) — Lynch's sorting rule, from the One Up on Wall Street summary.
- [The behavior gap](09-behavioral-finance/the-behavior-gap.md) — the evidence and the countermeasures (checking frequency, automation, pre-commitment).

## Numbers to remember

| Fact | Figure | Source year |
|---|---|---|
| Active large-cap funds trailing S&P 500, 20 yrs | 92.9% | SPIVA YE2025 |
| Investor behavior gap | −1.2 pts/yr | Morningstar 2026 |
| Lump sum beats DCA | ~2/3 of the time | Vanguard |
| Safe withdrawal rate | 3.9% (Morningstar) / 4.7% (Bengen) | 2026 / 2025 |
| S&P 500 long-run nominal / real return | ~10% / ~7% | 1928–2025 |
| 401(k) / IRA / HSA limits | $24,500 / $7,500 / $4,400 | IRS 2026 |
| Bitcoin cycle drawdowns | −93 / −85 / −83 / −77 / −53% | 2011–2026 |

## How it was built (process learnings)

- Parallel research agents, one per section, each with a fixed file list and a shared format, then an independent fact-check agent that edits directly. The fact-checker caught roughly a dozen material errors per pass, including a live news story (MSCI index rules) that had moved since the writer's source.
- Primary sources over search: when the search budget ran out, direct fetches of IRS, Fed, CoinGecko, DefiLlama and company pages produced better numbers than search snippets had.
- The cloud workspace cannot reach GitHub; the Mac is the push path.
- Copyrighted books are summarized from knowledge and public sources, never ingested from third-party PDFs.

## Open Questions

- Does the four-year Bitcoin cycle survive the ETF era, or has liquidity replaced the halving as the driver?
- Will the CLARITY Act pass the Senate (cloture vote 2026-09-15), and does that change the ETF and custody landscape?
- Which of the library's dated readings should get a scheduled quarterly refresh?
