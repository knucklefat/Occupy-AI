# The US Regulatory Landscape for Crypto (September 2026)

**In one sentence:** Between January 2025 and September 2026 the US flipped from regulation-by-enforcement to regulation-by-rulebook: stablecoins got a federal law (GENIUS Act), the SEC dropped its exchange cases and wrote a token taxonomy with the CFTC, spot altcoin ETFs became routine, banks were told they may custody crypto, and the one big missing piece, a market-structure law (CLARITY Act), faces a make-or-break Senate vote on September 15, 2026.

*Current as of September 11, 2026. The CLARITY Act status below will be stale within days; check the outcome of the September 15 cloture vote.*

## Who regulates what

| Regulator | Claims jurisdiction over | 2026 posture |
|---|---|---|
| **SEC** | Tokens that are "investment contracts" (securities); exchanges, brokers, and funds dealing in them; ETFs | Crypto Task Force (Commissioner Peirce, since Jan 2025); enforcement narrowed to fraud; "Project Crypto" rulemaking; Regulation Crypto Assets proposed Aug 19, 2026 |
| **CFTC** | Commodity derivatives (BTC/ETH futures); anti-fraud in spot commodity markets; would gain spot-market authority under CLARITY | Registered several crypto derivatives venues; joint taxonomy with SEC (Mar 2026) |
| **Treasury / IRS** | Taxation, broker reporting (1099-DA) | Final broker regs in force; DeFi broker rule repealed by Congress Apr 2025 |
| **FinCEN** | Anti-money-laundering (Bank Secrecy Act), FBAR | Exchanges are money services businesses; FBAR crypto rule still not finalized |
| **OCC / Fed / FDIC** | Banks' ability to touch crypto | All three withdrew 2022–23 "caution" guidance in spring 2025; custody and stablecoin activities permitted with normal risk management |
| **DOL** | 401(k) fiduciaries | Rescinded 2022 anti-crypto guidance (May 2025); alternative-assets executive order (Aug 2025) |
| **States** | Money transmission, NYDFS BitLicense, state stablecoin regimes | Continue to license; GENIUS preempts parts of state stablecoin law |

The historical fight was SEC vs. CFTC: the SEC under Chair Gensler argued most tokens were securities and sued exchanges for listing them; the CFTC said BTC and ETH were commodities. Courts split (*Ripple* 2023: institutional sales were securities offerings, programmatic exchange sales were not). Congress never resolved it. That is what CLARITY is for.

## The 2025 shift at the SEC

- **January 21, 2025:** Crypto Task Force launched under Commissioner Hester Peirce to write rules instead of suing.
- **February–May 2025:** the SEC dismissed or closed its cases against Coinbase, Binance, Kraken, Consensys, and others; the Ripple appeals were dropped by August 2025 with the earlier programmatic-sales ruling intact. Enforcement continued against outright fraud (fake platforms, Ponzi schemes, wash trading).
- **May 29, 2025:** staff statement that protocol staking (including delegated and custodial staking with ministerial services) is not a securities offering.
- **July 31, 2025:** Chair Paul Atkins announced "Project Crypto," a rulemaking agenda to bring token issuance, custody, and trading on-chain within US rules.
- **September 17, 2025:** approval of **generic listing standards** for commodity-based ETPs on Nasdaq, NYSE Arca, and Cboe. Exchanges can now list a spot crypto ETF without a bespoke 19b-4 approval (which used to take up to 240 days) if the asset meets objective tests, such as having regulated futures trading for a set period or already being held by an existing ETF. Solana, XRP, Litecoin, Dogecoin, and multi-asset index ETFs followed within weeks; Bitwise's Solana ETF launched October 28, 2025 with staking enabled.
- **March 17, 2026:** joint **SEC–CFTC interpretive release** creating five categories: digital commodities, digital collectibles, digital tools, stablecoins, and digital securities. It named 23 assets, including BTC, ETH, SOL, XRP, ADA, DOGE, LTC, DOT, LINK, AVAX, as digital commodities and confirmed that mining, staking, and most airdrops are not securities transactions. It is an interpretation, not a statute, and courts need not defer to it after *Loper Bright*.
- **August 19, 2026:** proposed **Regulation Crypto Assets**: a startup exemption (up to $5 million over four years, no accredited-investor limit) and a larger tier (up to $75 million per year with audited financials), plus a safe harbor under which a token stops being an investment contract once the issuer certifies it has finished the managerial work it promised. Comments close around October 18, 2026.

## GENIUS Act (stablecoins) — signed July 18, 2025

The first federal crypto statute. Key provisions:

- Only **permitted payment stablecoin issuers** may issue dollar stablecoins in the US: subsidiaries of insured banks, nonbanks approved by the OCC, or issuers under a state regime certified as substantially similar (state-only path available up to roughly **$10 billion** outstanding, after which federal oversight kicks in).
- **1:1 reserves** in cash, insured deposits, short-term Treasuries, repo, or government money-market funds, with **monthly public reserve disclosures** and executive certification.
- **Issuers may not pay interest or yield** to holders simply for holding the coin. This is why exchanges' "stablecoin rewards" programs became the central fight in the CLARITY negotiations.
- Holders get **priority over all other creditors** if an issuer fails.
- Full Bank Secrecy Act/AML obligations, and the technical ability to freeze, seize, or burn coins on lawful order.
- Foreign issuers (Tether) can serve US markets only if their home regime is deemed comparable and they comply with US lawful orders.
- **Effective date:** the earlier of 18 months after enactment (**January 18, 2027**) or 120 days after primary regulators publish final rules. Treasury and the OCC have been issuing proposed rules through 2026; the exact go-live date depends on when those finalize.

**What it means:** USDC and other compliant coins get bank-like credibility; yield on idle stablecoin balances has to come from somewhere other than the issuer (which is what the CLARITY "activity-based rewards" compromise tries to define); and stablecoins are cemented as a distribution channel for Treasuries.

## CLARITY Act (market structure) — status on September 11, 2026

The Digital Asset Market Clarity Act (H.R. 3633) passed the House **294–134 on July 17, 2025**. In the Senate it cleared the Agriculture Committee (**12–11, January 29, 2026**) and the Banking Committee (**15–9, May 14, 2026**), and was placed on the Senate calendar June 1, 2026. Floor action slipped past the August recess over ethics provisions and bank lobbying. Majority Leader Thune filed cloture on the motion to proceed (Calendar No. 423) on August 8, and the **cloture vote on the motion to proceed is set for September 15, 2026 at 2:15 p.m. ET** (as reported by DeFi Rate and CoinDesk; the Senate returns September 14). It needs 60 votes; Republicans hold 53, so at least seven Democrats must join.

What the bill does:
- Defines **digital commodities** and a "mature blockchain" test (roughly: no single party controls 20% or more of supply or governance) that moves a token from SEC to CFTC oversight.
- Gives the **CFTC exclusive authority over spot digital-commodity markets**, registering exchanges, brokers, and dealers.
- Keeps the **SEC** over tokens sold as investment contracts, with a disclosure-based fundraising path and joint SEC–CFTC rules for mixed cases.
- **Exempts non-custodial DeFi developers** and node operators from money-transmitter and exchange registration.
- Restricts **yield on idle stablecoin balances** that mimic bank deposits while allowing activity-based rewards.
- Adds bank custody authority and customer-asset segregation rules.

Sticking points: an ethics provision limiting senior officials' crypto businesses (aimed at the President's family ventures), DeFi carve-outs Democrats see as too broad, illicit-finance safeguards, and the stablecoin rewards compromise. Prediction markets in early September priced passage this year at roughly 13–17%. If cloture fails, the bill is effectively dead until after the November 2026 midterms, and the agencies' interpretive approach becomes the de facto regime.

## Banking access

- **OCC Interpretive Letter 1183 (March 7, 2025):** national banks may custody crypto, engage in certain stablecoin activities, and run nodes without prior supervisory non-objection. Letter 1184 (May 2025) added that banks may outsource custody to sub-custodians.
- **FDIC (March 28, 2025)** and **Federal Reserve (April 24, 2025)** rescinded their 2022–23 letters requiring pre-notification and withdrew from the joint "crypto risk" statements. The Fed also dropped "reputational risk" as an examination factor in June 2025, which had been the tool behind de-banking of crypto firms.
- Result: Anchorage, Kraken, Ripple, Circle, and others pursued or obtained national trust charters; large banks announced custody and stablecoin projects. The "Operation Choke Point 2.0" era is over, though state-chartered crypto banks still face Fed master-account fights.

## Strategic Bitcoin Reserve

Executive Order of **March 6, 2025** created a Strategic Bitcoin Reserve (forfeited BTC, roughly 200,000 coins by most estimates, not to be sold) and a Digital Asset Stockpile for other seized assets. Additional bitcoin may be acquired only through **budget-neutral** strategies; no taxpayer purchases have occurred as of September 2026, and bills to codify the reserve (the BITCOIN Act) have not passed. Several states (Texas, New Hampshire, Arizona) passed their own reserve laws in 2025.

## State level

**New York's BitLicense** (since 2015) remains the most demanding state regime: licensing for custody, exchange, and transmission serving New York residents, minimum $500,000 surety bond, and a "greenlist" of coins (BTC, ETH, and a handful of NY-approved stablecoins) that licensees may list without separate approval. NYDFS updated custody guidance in September 2025 to protect customer assets in insolvency. Other states run money-transmitter licensing; GENIUS lets states supervise small stablecoin issuers under a certified regime. Wyoming's SPDI charters and Texas's reserve law show the opposite pole.

## What it means for investors

1. **Counterparty risk is lower, not gone.** Regulated custody, segregation rules, and stablecoin reserves reduce FTX-style blowups; hacks and self-custody mistakes are unchanged.
2. **More products, cheaper.** Generic listing standards mean spot ETFs for most large-cap tokens, some with staking yield, at 0.2–0.5% fees, inside IRAs and 401(k) windows.
3. **Stablecoin yield now comes from platforms, not issuers**, and CLARITY may restrict it further; treat "rewards" as a marketing expense that can be cut.
4. **Enforcement is about fraud.** A token being "not a security" does not make it a good investment; the SEC is no longer screening projects for you.
5. **Tax reporting is the enforcement that stuck**: 1099-DA matching is live regardless of what happens to CLARITY.
6. **Policy reversal risk is real.** Much of the 2025–26 shift is executive and interpretive, not statutory; a different administration or SEC chair could unwind it. GENIUS is law; CLARITY may not be.

## How to actually do it

1. Prefer venues that are US-registered (or NYDFS-licensed) and publish proof-of-reserves and segregation policies.
2. For stablecoins, hold GENIUS-track issuers (USDC, PayPal USD, bank-issued coins) for size; treat offshore coins as higher-risk.
3. Use the SEC–CFTC taxonomy list as a first-pass filter for "regulatory-cleared" large caps, not as a buy list.
4. Watch September 15, 2026 (CLARITY cloture), the Regulation Crypto Assets comment deadline (~October 18, 2026), and GENIUS implementation rules (effective by January 18, 2027 at the latest).
5. Keep a self-custody backup for any exposure you cannot afford to have frozen; regulation cuts both ways.

## Key takeaways

- The SEC and CFTC now agree BTC, ETH, SOL, XRP, and about 19 other tokens are commodities; staking and mining are not securities transactions (March 2026 interpretation).
- GENIUS Act (July 2025) is the first federal crypto law: 1:1 reserves, licensed issuers, no issuer-paid yield, holder priority; effective by January 2027.
- CLARITY passed the House in July 2025 and both Senate committees by May 2026; its September 15, 2026 cloture vote is the deciding moment for 2026.
- Generic ETF listing standards (September 2025) turned spot altcoin ETFs from years-long fights into routine listings.
- OCC, FDIC, and Fed all reopened bank access to crypto in spring 2025.
- The Strategic Bitcoin Reserve holds seized coins only; no taxpayer-funded buying yet.
- Most of the shift is administrative rather than statutory, so it can be reversed; tax reporting rules are the part that is here to stay.

## Sources

- [Latham & Watkins: US Crypto Policy Tracker — legislative developments](https://www.lw.com/en/us-crypto-policy-tracker/legislative-developments)
- [Congress.gov: H.R. 3633 Digital Asset Market Clarity Act](https://www.congress.gov/bill/119th-congress/house-bill/3633/text)
- [CoinDesk: Senate opens first stage of CLARITY Act voting (Aug 8, 2026)](https://www.coindesk.com/policy/2026/08/08/u-s-senate-opens-first-stage-of-crypto-clarity-act-voting-to-give-bill-a-chance-next-month)
- [DeFi Rate: CLARITY Act fact sheet and Sept 15 vote](https://defirate.com/clarity-act-fact-sheet/)
- [Bitcoin Foundation: CLARITY Act hits September 15 deadline](https://bitcoinfoundation.org/news/regulation/clarity-act-hits-a-september-15-deadline/)
- [White House: Fact sheet on GENIUS Act signing](https://www.whitehouse.gov/fact-sheets/2025/07/fact-sheet-president-donald-j-trump-signs-genius-act-into-law/)
- [Chapman: SEC and CFTC clarify crypto asset taxonomy (March 2026)](https://www.chapman.com/publication-sec-and-cftc-clarify-crypto-asset-taxonomy-and-the-application-of-federal-securities-laws)
- [crypto.news: SEC crypto enforcement in 2026](https://crypto.news/us/sec/)
- [CoinDesk: SEC approves generic listing standards (Sept 17, 2025)](https://www.coindesk.com/policy/2025/09/17/sec-makes-spot-crypto-etf-listing-process-easier-approves-grayscale-s-large-cap-crypto-fund)
- [Helius: US Solana spot ETFs](https://www.helius.dev/blog/solana-etfs)
- [OCC: Interpretive Letter 1183 news release (March 7, 2025)](https://www.occ.gov/news-issuances/news-releases/2025/nr-occ-2025-16.html)
- [White House: Strategic Bitcoin Reserve executive order (March 6, 2025)](https://www.whitehouse.gov/presidential-actions/2025/03/establishment-of-the-strategic-bitcoin-reserve-and-united-states-digital-asset-stockpile/)
- [NYDFS: Virtual currency businesses](https://www.dfs.ny.gov/virtual_currency_businesses)
- [DOL: Rescission of 2022 crypto 401(k) guidance](https://www.dol.gov/newsroom/releases/ebsa/ebsa20250528)
