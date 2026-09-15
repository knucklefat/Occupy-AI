# Occupy AI Research Catalog

This repo is a static investing knowledge library: **210 pre-existing library files, all Markdown**, no tracked code, no notebooks, and no structured datasets. It is useful as a source corpus for Dante's investing and AI research operation, especially for play generation, market-regime awareness, diligence checklists, policy/risk controls, and source discovery.

## 1) Top-level map

| Path | What it is for | Best operational use |
|---|---|---|
| [`README.md`](README.md) | Library overview, conventions, and suggested starting paths. | Orientation and routing readers to the right desk. |
| [`01-foundations/`](01-foundations/) | Core investing concepts: compounding, asset classes, risk/return, market mechanics, account types, glossary. | Common vocabulary for all desks; onboarding non-finance operators. |
| [`02-strategies/`](02-strategies/) | Investing schools: passive, value, growth, dividend, factor, momentum, quant/systematic, macro/all-weather, options, special situations, small/microcap. | Idea generation and strategy taxonomy. |
| [`03-techniques/`](03-techniques/) | Portfolio mechanics: asset allocation, DCA vs lump sum, rebalancing, position sizing, tax-loss harvesting, asset location, cash, withdrawal, performance tracking. | Portfolio construction, sizing, execution rules, and review cadence. |
| [`04-analysis/`](04-analysis/) | Security/fund analysis: financial statements, 10-Ks, ratios, valuation, moats, management, screening, technical analysis, bonds, ETF diligence. | Research Floor thesis work and pre-council diligence. |
| [`05-market-indicators/`](05-market-indicators/) | Macro, policy, credit/liquidity, valuation, sentiment, breadth, commodities, seasonality, and a market dashboard. | Weather Ops / Pred Ops regime dashboard. |
| [`06-legendary-investors/`](06-legendary-investors/) | Profiles and lessons from Buffett, Munger, Graham, Lynch, Bogle, Dalio, Marks, Klarman, Simons, Druckenmiller/Soros, Greenblatt, Fisher/Smith, Sleep, Pabrai/Spier. | Investing Council mental models and decision standards. |
| [`07-publications-and-resources/`](07-publications-and-resources/) | Books, letters, newsletters, podcasts, data tools, academic papers, courses, communities, and official guides. Includes [`book-summaries/`](07-publications-and-resources/book-summaries/). | Source map for human and AI research agents. |
| [`08-tax-and-account-hacks/`](08-tax-and-account-hacks/) | US tax/account tactics: funding order, Roth/HSA, capital gains, tax-efficient funds, fees, brokerage choice, charitable/estate tactics, common mistakes. | Policy desk, tax-aware implementation, and account-selection rules. |
| [`09-behavioral-finance/`](09-behavioral-finance/) | Behavioral errors, bias field guide, prospect theory, bubbles, IPS discipline, decision systems, crash behavior, media diet. | Risk controls and operator behavior guardrails. |
| [`10-checklists-and-templates/`](10-checklists-and-templates/) | Actionable templates: getting started, annual checkup, stock/fund research, IPS, pre-trade, crash playbook, retirement readiness, portfolio review, scam checklist, formulas. | Investing Council gatekeeping and repeatable operating procedures. |
| [`11-crypto/`](11-crypto/) | Full crypto sub-library mirroring the main library: foundations, strategies, techniques, analysis, indicators, key thinkers, resources, tax/regulation, risk/behavior, checklists. | Crypto research, token diligence, on-chain/weather monitoring, and custody/risk playbooks. |
| [`Claude outputs/`](Claude%20outputs/) | One duplicate Markdown output: `one-up-on-wall-street.md`, byte-identical to the book summary under `07-publications-and-resources/book-summaries/`. | Low-value duplicate/outlier folder; useful mainly as cleanup signal. |

## 2) Key documents to read first

### Orientation and common language

1. [`README.md`](README.md) - repo scope, section map, conventions, and original reading routes.
2. [`01-foundations/core-principles-of-investing.md`](01-foundations/core-principles-of-investing.md) - compounding, diversification, costs, time horizon, and risk/return basics.
3. [`01-foundations/asset-classes-explained.md`](01-foundations/asset-classes-explained.md) - what each asset class contributes to a portfolio.
4. [`01-foundations/glossary.md`](01-foundations/glossary.md) - shared terminology for agents and humans.

### Play seeds and strategy menus

1. [`02-strategies/README.md`](02-strategies/README.md) - comparison table across strategies.
2. [`02-strategies/quantitative-and-systematic-investing.md`](02-strategies/quantitative-and-systematic-investing.md) - systematic investing, backtesting pitfalls, and rules-based approaches.
3. [`02-strategies/momentum-and-trend-following.md`](02-strategies/momentum-and-trend-following.md) - rules for trend/momentum overlays.
4. [`02-strategies/contrarian-and-special-situations.md`](02-strategies/contrarian-and-special-situations.md) - forced-selling and unusual-situation hunting.
5. [`07-publications-and-resources/book-summaries/one-up-on-wall-street.md`](07-publications-and-resources/book-summaries/one-up-on-wall-street.md) - Lynch-style idea sourcing and company categorization.

### Research Floor diligence

1. [`04-analysis/README.md`](04-analysis/README.md) - order of operations for analyzing a stock, bond, or fund.
2. [`04-analysis/how-to-read-a-10-k-and-annual-report.md`](04-analysis/how-to-read-a-10-k-and-annual-report.md) - company primary-source workflow.
3. [`04-analysis/key-financial-ratios.md`](04-analysis/key-financial-ratios.md) - ratio reference table.
4. [`04-analysis/valuation-methods.md`](04-analysis/valuation-methods.md) - DCF, reverse DCF, comparables, and valuation errors.
5. [`04-analysis/economic-moats-and-competitive-advantage.md`](04-analysis/economic-moats-and-competitive-advantage.md) - moat taxonomy.
6. [`10-checklists-and-templates/stock-research-checklist.md`](10-checklists-and-templates/stock-research-checklist.md) - 55-item stock gate before a buy decision.
7. [`10-checklists-and-templates/etf-and-fund-selection-checklist.md`](10-checklists-and-templates/etf-and-fund-selection-checklist.md) - fund/ETF diligence.

### Weather / predictive operations

1. [`05-market-indicators/README.md`](05-market-indicators/README.md) - master table of macro/market indicators and free sources.
2. [`05-market-indicators/how-to-build-a-market-dashboard.md`](05-market-indicators/how-to-build-a-market-dashboard.md) - 15-indicator weekly/monthly dashboard, thresholds, and four-regime playbook.
3. [`05-market-indicators/credit-and-liquidity-indicators.md`](05-market-indicators/credit-and-liquidity-indicators.md) - stress and liquidity early warnings.
4. [`05-market-indicators/market-breadth-indicators.md`](05-market-indicators/market-breadth-indicators.md) - internal market health.
5. [`05-market-indicators/sentiment-indicators.md`](05-market-indicators/sentiment-indicators.md) - contrarian/extreme sentiment checks.

### Investing Council and policy controls

1. [`10-checklists-and-templates/investment-policy-statement-template.md`](10-checklists-and-templates/investment-policy-statement-template.md) - portfolio constitution and forbidden-action list.
2. [`10-checklists-and-templates/pre-trade-checklist.md`](10-checklists-and-templates/pre-trade-checklist.md) - required written gate for discretionary trades.
3. [`10-checklists-and-templates/portfolio-review-template.md`](10-checklists-and-templates/portfolio-review-template.md) - quarterly portfolio review form.
4. [`10-checklists-and-templates/market-crash-playbook.md`](10-checklists-and-templates/market-crash-playbook.md) - crisis procedure.
5. [`06-legendary-investors/common-threads.md`](06-legendary-investors/common-threads.md) - cross-investor principles.
6. [`09-behavioral-finance/decision-making-systems.md`](09-behavioral-finance/decision-making-systems.md) - decision journals, pre-mortems, base rates, inversion, and automation.

### Crypto / on-chain research

1. [`11-crypto/README.md`](11-crypto/README.md) - complete crypto sub-library map and caveats.
2. [`11-crypto/04-analysis/README.md`](11-crypto/04-analysis/README.md) - token/protocol research workflow.
3. [`11-crypto/10-checklists-and-templates/token-due-diligence-checklist.md`](11-crypto/10-checklists-and-templates/token-due-diligence-checklist.md) - 48-item token gate.
4. [`11-crypto/05-indicators/how-to-build-a-crypto-dashboard.md`](11-crypto/05-indicators/how-to-build-a-crypto-dashboard.md) - 14-indicator weekly crypto dashboard and regime labels.
5. [`11-crypto/07-publications-and-resources/data-sources-and-tools.md`](11-crypto/07-publications-and-resources/data-sources-and-tools.md) - crypto data/tool stack.
6. [`11-crypto/09-risk-and-behavior/risk-management-rules-for-crypto.md`](11-crypto/09-risk-and-behavior/risk-management-rules-for-crypto.md) - consolidated crypto rules.
7. [`11-crypto/08-tax-and-regulation/us-regulatory-landscape.md`](11-crypto/08-tax-and-regulation/us-regulatory-landscape.md) - US crypto policy status as of September 2026.

### Datasets and notebooks

No tracked datasets or notebooks are present. The repo links to external data sources (FRED, EDGAR, Shiller, French, Damodaran, Farside, DefiLlama, Glassnode, CryptoQuant, Dune, Coinglass, Tokenomist, etc.) but does not store raw data, derived datasets, spreadsheets, notebook analyses, or chart exports.

## 3) Desk mapping for Dante's operation

### Idea Bucket: play seeds

Use these files to seed potential plays before formal research:

- [`02-strategies/README.md`](02-strategies/README.md) - strategy menu and benchmark comparison.
- [`02-strategies/growth-investing.md`](02-strategies/growth-investing.md), [`value-investing.md`](02-strategies/value-investing.md), [`small-cap-and-microcap-investing.md`](02-strategies/small-cap-and-microcap-investing.md), [`contrarian-and-special-situations.md`](02-strategies/contrarian-and-special-situations.md) - equity play archetypes.
- [`02-strategies/quantitative-and-systematic-investing.md`](02-strategies/quantitative-and-systematic-investing.md) and [`momentum-and-trend-following.md`](02-strategies/momentum-and-trend-following.md) - rules-based screens and signal ideas.
- [`06-legendary-investors/peter-lynch.md`](06-legendary-investors/peter-lynch.md) and [`07-publications-and-resources/book-summaries/one-up-on-wall-street.md`](07-publications-and-resources/book-summaries/one-up-on-wall-street.md) - "notice the product, then prove it" workflow.
- [`11-crypto/02-strategies/README.md`](11-crypto/02-strategies/README.md), [`11-crypto/02-strategies/airdrops-points-and-early-participation.md`](11-crypto/02-strategies/airdrops-points-and-early-participation.md), and [`11-crypto/04-analysis/narratives-and-cycle-analysis.md`](11-crypto/04-analysis/narratives-and-cycle-analysis.md) - crypto narrative and participation ideas.

### Research Floor: World / Supply / Thesis / Policy

**World** - macro context, market structure, and source discovery:

- [`01-foundations/`](01-foundations/)
- [`05-market-indicators/macroeconomic-indicators.md`](05-market-indicators/macroeconomic-indicators.md)
- [`05-market-indicators/interest-rates-and-the-fed.md`](05-market-indicators/interest-rates-and-the-fed.md)
- [`07-publications-and-resources/data-sources-and-tools.md`](07-publications-and-resources/data-sources-and-tools.md)
- [`11-crypto/01-foundations/`](11-crypto/01-foundations/)
- [`11-crypto/06-key-thinkers/`](11-crypto/06-key-thinkers/)

**Supply** - flows, positioning, liquidity, issuance, and unlocks:

- [`05-market-indicators/credit-and-liquidity-indicators.md`](05-market-indicators/credit-and-liquidity-indicators.md)
- [`05-market-indicators/market-breadth-indicators.md`](05-market-indicators/market-breadth-indicators.md)
- [`05-market-indicators/valuation-indicators.md`](05-market-indicators/valuation-indicators.md)
- [`11-crypto/05-indicators/flows-and-supply-indicators.md`](11-crypto/05-indicators/flows-and-supply-indicators.md)
- [`11-crypto/05-indicators/market-structure-and-derivatives-indicators.md`](11-crypto/05-indicators/market-structure-and-derivatives-indicators.md)
- [`11-crypto/04-analysis/tokenomics-analysis.md`](11-crypto/04-analysis/tokenomics-analysis.md)

**Thesis** - company, fund, protocol, and token analysis:

- [`04-analysis/`](04-analysis/)
- [`10-checklists-and-templates/stock-research-checklist.md`](10-checklists-and-templates/stock-research-checklist.md)
- [`10-checklists-and-templates/etf-and-fund-selection-checklist.md`](10-checklists-and-templates/etf-and-fund-selection-checklist.md)
- [`11-crypto/04-analysis/`](11-crypto/04-analysis/)
- [`11-crypto/10-checklists-and-templates/token-due-diligence-checklist.md`](11-crypto/10-checklists-and-templates/token-due-diligence-checklist.md)
- [`11-crypto/10-checklists-and-templates/defi-protocol-safety-checklist.md`](11-crypto/10-checklists-and-templates/defi-protocol-safety-checklist.md)

**Policy** - rules, constraints, legal/tax wrappers, and compliance posture:

- [`08-tax-and-account-hacks/`](08-tax-and-account-hacks/)
- [`10-checklists-and-templates/investment-policy-statement-template.md`](10-checklists-and-templates/investment-policy-statement-template.md)
- [`10-checklists-and-templates/pre-trade-checklist.md`](10-checklists-and-templates/pre-trade-checklist.md)
- [`09-behavioral-finance/building-an-investment-policy-statement.md`](09-behavioral-finance/building-an-investment-policy-statement.md)
- [`11-crypto/08-tax-and-regulation/`](11-crypto/08-tax-and-regulation/)
- [`11-crypto/10-checklists-and-templates/crypto-investment-policy-statement-template.md`](11-crypto/10-checklists-and-templates/crypto-investment-policy-statement-template.md)

### Investing Council

Use this desk to approve, size, reject, and review plays:

- Diligence gates: [`stock-research-checklist.md`](10-checklists-and-templates/stock-research-checklist.md), [`etf-and-fund-selection-checklist.md`](10-checklists-and-templates/etf-and-fund-selection-checklist.md), [`token-due-diligence-checklist.md`](11-crypto/10-checklists-and-templates/token-due-diligence-checklist.md).
- Trade gates: [`pre-trade-checklist.md`](10-checklists-and-templates/pre-trade-checklist.md), [`pre-trade-checklist-for-crypto.md`](11-crypto/10-checklists-and-templates/pre-trade-checklist-for-crypto.md).
- Policy and sizing: [`investment-policy-statement-template.md`](10-checklists-and-templates/investment-policy-statement-template.md), [`crypto-investment-policy-statement-template.md`](11-crypto/10-checklists-and-templates/crypto-investment-policy-statement-template.md), [`03-techniques/position-sizing-and-risk-management.md`](03-techniques/position-sizing-and-risk-management.md), [`11-crypto/03-techniques/position-sizing-and-rebalancing-for-crypto.md`](11-crypto/03-techniques/position-sizing-and-rebalancing-for-crypto.md).
- Wisdom / second-level thinking: [`06-legendary-investors/common-threads.md`](06-legendary-investors/common-threads.md), [`06-legendary-investors/howard-marks.md`](06-legendary-investors/howard-marks.md), [`06-legendary-investors/charlie-munger.md`](06-legendary-investors/charlie-munger.md), [`09-behavioral-finance/decision-making-systems.md`](09-behavioral-finance/decision-making-systems.md).
- Review loop: [`portfolio-review-template.md`](10-checklists-and-templates/portfolio-review-template.md), [`annual-financial-checkup-checklist.md`](10-checklists-and-templates/annual-financial-checkup-checklist.md).

### Pred Ops / Weather Ops

Use this desk to name regimes, update signals, and decide whether the operating posture changes:

- Main market dashboard: [`05-market-indicators/how-to-build-a-market-dashboard.md`](05-market-indicators/how-to-build-a-market-dashboard.md).
- Market signal families: [`macroeconomic-indicators.md`](05-market-indicators/macroeconomic-indicators.md), [`interest-rates-and-the-fed.md`](05-market-indicators/interest-rates-and-the-fed.md), [`yield-curve-and-recession-indicators.md`](05-market-indicators/yield-curve-and-recession-indicators.md), [`credit-and-liquidity-indicators.md`](05-market-indicators/credit-and-liquidity-indicators.md), [`valuation-indicators.md`](05-market-indicators/valuation-indicators.md), [`sentiment-indicators.md`](05-market-indicators/sentiment-indicators.md), [`market-breadth-indicators.md`](05-market-indicators/market-breadth-indicators.md).
- Crypto dashboard: [`11-crypto/05-indicators/how-to-build-a-crypto-dashboard.md`](11-crypto/05-indicators/how-to-build-a-crypto-dashboard.md).
- Crypto signal families: [`on-chain-valuation-indicators.md`](11-crypto/05-indicators/on-chain-valuation-indicators.md), [`flows-and-supply-indicators.md`](11-crypto/05-indicators/flows-and-supply-indicators.md), [`market-structure-and-derivatives-indicators.md`](11-crypto/05-indicators/market-structure-and-derivatives-indicators.md), [`macro-and-liquidity-drivers.md`](11-crypto/05-indicators/macro-and-liquidity-drivers.md).
- Crisis procedures: [`market-crash-playbook.md`](10-checklists-and-templates/market-crash-playbook.md), [`11-crypto/10-checklists-and-templates/crypto-crash-playbook.md`](11-crypto/10-checklists-and-templates/crypto-crash-playbook.md), [`09-behavioral-finance/handling-market-crashes.md`](09-behavioral-finance/handling-market-crashes.md), [`11-crypto/09-risk-and-behavior/history-of-crypto-crashes-and-collapses.md`](11-crypto/09-risk-and-behavior/history-of-crypto-crashes-and-collapses.md).

## 4) Runnable scripts and data pipelines

There are **no tracked runnable scripts or pipelines** in this repository:

- No Python, shell, SQL, R, JavaScript/TypeScript, Makefile, package manifest, requirements file, notebook, CSV, JSON, or YAML files are tracked.
- The current repo has no local build, lint, test, ingestion, data-refresh, or chart-generation commands.
- All operational "runs" are manual procedures documented in Markdown.

Manual procedures that behave like lightweight pipelines:

| Procedure | Where documented | How to run manually |
|---|---|---|
| Main market dashboard | [`05-market-indicators/how-to-build-a-market-dashboard.md`](05-market-indicators/how-to-build-a-market-dashboard.md) | Create a FRED dashboard and bookmark the non-FRED sources; weekly update fast indicators, monthly update macro/valuation indicators, count flags, name regime, write a one-line log. |
| Crypto dashboard | [`11-crypto/05-indicators/how-to-build-a-crypto-dashboard.md`](11-crypto/05-indicators/how-to-build-a-crypto-dashboard.md) | Maintain a 14- or 15-row note/spreadsheet; weekly update valuation, flows, derivatives, macro, and sentiment links; count zones and assign Accumulation/Recovery/Expansion/Euphoria/Distribution/Mixed. |
| Stock research gate | [`10-checklists-and-templates/stock-research-checklist.md`](10-checklists-and-templates/stock-research-checklist.md) | Fill the checklist from company filings, financial statements, valuation work, and a written thesis before any stock enters council review. |
| Token research gate | [`11-crypto/10-checklists-and-templates/token-due-diligence-checklist.md`](11-crypto/10-checklists-and-templates/token-due-diligence-checklist.md) | Fill the 48-item checklist using docs/GitHub, CoinGecko/CoinMarketCap, DefiLlama, Token Terminal, explorers, unlock trackers, audits, and Messari-style profiles. |
| Trade approval | [`10-checklists-and-templates/pre-trade-checklist.md`](10-checklists-and-templates/pre-trade-checklist.md), [`11-crypto/10-checklists-and-templates/pre-trade-checklist-for-crypto.md`](11-crypto/10-checklists-and-templates/pre-trade-checklist-for-crypto.md) | Before discretionary trades, write thesis, sizing, tax, counterparty, emotional-state, and exit answers; if any hard-fail appears, do nothing. |
| Portfolio/council review | [`10-checklists-and-templates/portfolio-review-template.md`](10-checklists-and-templates/portfolio-review-template.md), [`10-checklists-and-templates/annual-financial-checkup-checklist.md`](10-checklists-and-templates/annual-financial-checkup-checklist.md) | Quarterly update allocation/performance/fees/decisions; annually review accounts, tax actions, beneficiaries, security, and policy documents. |

## 5) Gaps for market research use

1. **No machine-readable metadata.** Files lack frontmatter for asset class, desk, source type, date reviewed, signal family, ticker/protocol coverage, and freshness. That limits retrieval, automated routing, and staleness checks.
2. **No local datasets.** The repo cites many external data sources but stores no raw series, snapshots, historical dashboards, price data, filings, token metrics, or derived features.
3. **No notebooks or reproducible analyses.** Valuation examples, dashboard readings, backtest references, and indicator thresholds are prose-only; there are no notebooks to recompute them.
4. **No ingestion or refresh pipelines.** There are no scripts to pull FRED/EDGAR/ETF-flow/crypto/on-chain data, no scheduled jobs, and no artifact directory for generated tables/charts.
5. **No watchlist or idea ledger.** There is no canonical `ideas/`, `watchlists/`, `research-memos/`, `positions/`, or `decision-log/` structure for turning evergreen knowledge into active plays.
6. **No council memo template.** The checklists are strong, but there is no single investment memo format that packages World/Supply/Thesis/Policy, base/bull/bear cases, sizing, catalysts, kill criteria, and post-mortem hooks.
7. **No explicit AI-agent operating layer.** Despite the repo name, content is not yet packaged as prompts, agent playbooks, retrieval indexes, evals, or tool contracts for an AI research operation.
8. **No verification harness.** Links and figures were reportedly checked in September 2026, but the repo has no link checker, citation audit, data freshness checker, or CI.
9. **Static current-market readings will stale.** Many market and crypto pages include date-stamped September 2026 readings; those need a refresh cadence or separation from evergreen frameworks.
10. **Duplicate/outlier content.** [`Claude outputs/one-up-on-wall-street.md`](Claude%20outputs/one-up-on-wall-street.md) duplicates [`07-publications-and-resources/book-summaries/one-up-on-wall-street.md`](07-publications-and-resources/book-summaries/one-up-on-wall-street.md), suggesting generated outputs need an archival or promotion policy.

## Suggested next catalog increments

These are not implemented in this PR, but would make the library much more useful to Dante's market-research stack:

- Add YAML frontmatter to every Markdown file: `desk`, `asset_class`, `function`, `source_type`, `reviewed_at`, `freshness`, `inputs`, `outputs`.
- Create `research-memos/` templates for equity, fund/ETF, macro, and token/protocol decisions.
- Create `dashboards/` with CSV or Markdown logs for the market and crypto dashboards.
- Add a small `scripts/` or `notebooks/` layer for FRED, EDGAR, ETF-flow, and crypto indicator refreshes.
- Add link/freshness checks in CI once scripts exist.
