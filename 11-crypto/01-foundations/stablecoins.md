# Stablecoins

**In one sentence:** Stablecoins are blockchain tokens pegged to the dollar and backed (in the reputable cases) by cash and Treasury bills, and they are crypto's real killer app: roughly $310 billion outstanding as of September 2026, the settlement currency for almost all crypto trading, now governed in the U.S. by the GENIUS Act of July 2025, and with a history of breaking their peg often enough that "stable" deserves an asterisk.

## What a stablecoin is

A stablecoin is a token on a blockchain designed to always be worth one unit of a fiat currency, almost always the U.S. dollar. It gives traders a place to park money without leaving the crypto system, lets people in countries with weak currencies hold dollars on a phone, and moves across borders in minutes for cents.

There are three basic designs:

| Type | How the peg is held | Examples | Track record |
|---|---|---|---|
| **Fiat-backed** | Issuer holds dollars and T-bills; redeems 1:1 | USDT (Tether), USDC (Circle), PYUSD (PayPal), USD1 | Dominant; ~97% of the market |
| **Crypto-collateralized** | Over-collateralized with crypto in smart contracts | DAI/USDS (Sky, formerly MakerDAO) | Survived since 2017; relies partly on USDC and T-bills now |
| **Algorithmic** | Peg maintained by arbitrage with a sister token, little or no collateral | Terra UST (dead) | Catastrophic failure in May 2022 |

## The two giants: USDT and USDC

As of September 10, 2026, total stablecoin supply was about **$310 billion** (DefiLlama; the record was roughly $321 billion in May 2026). **Tether's USDT** accounted for roughly **$183 billion** and **Circle's USDC** for about **$74.5 billion**; the two together are 83% of the market. World Liberty Financial's USD1 (~$4.3 billion) and PayPal's PYUSD (under $3 billion) are the largest of the rest.

**USDC** is issued by Circle, a U.S.-listed public company. Reserves sit in the Circle Reserve Fund, a government money-market fund managed by BlackRock, plus cash at large banks, with monthly attestations by a Big Four auditor. USDC is the "regulated" choice and dominant in U.S. DeFi.

**USDT** is issued by Tether, based in El Salvador, and dominates trading pairs on offshore exchanges and dollar usage in emerging markets (largely on the Tron network). Tether's Q2 2026 attestation (by BDO, not a full audit) reported about $187.75 billion in total assets against $184.6 billion of USDT, with the bulk in U.S. Treasury bills and repos, plus about 146 tons of gold (~$18.8 billion), roughly 98,900 bitcoin (~$5.8 billion), and about $13.5 billion of secured loans. Its excess reserve buffer fell to $4.11 billion (2.2% of supply) from $8.23 billion the prior quarter as gold and bitcoin prices dropped. Tether earns billions a year in interest on its Treasury holdings and pays holders nothing.

The skeptical view, made at length in Zeke Faux's *Number Go Up*, is that Tether spent years claiming full backing while holding commercial paper, loans to affiliates, and other risky assets; paid a $41 million CFTC fine in 2021 for misrepresenting reserves; and has never produced a full audit. Tether's defenders note it has honored every redemption for over a decade, including $20 billion in a few weeks during 2022. Both things are true. The investor lesson: a stablecoin is an unsecured claim on its issuer, and the quality of that issuer's balance sheet is the whole game.

## How reserves work

A well-run fiat stablecoin functions like a narrow bank or a money-market fund without the yield. When you send $1 million to Circle, it mints 1 million USDC and buys T-bills. When you redeem, it sells T-bills, wires you dollars, and destroys the tokens. The issuer keeps the interest. At 4%+ short-term rates, this made Tether and Circle enormously profitable.

The risks are those of any money fund: the assets could lose value (duration or credit risk), the bank holding the cash could fail (USDC's problem in 2023), or the issuer could simply lie about what it holds. Attestations (a snapshot check by an accountant) are weaker than audits (a full examination of controls and a period of activity). As of 2026 only some issuers have moved to full audits.

## The GENIUS Act (signed July 18, 2025)

The Guiding and Establishing National Innovation for U.S. Stablecoins Act is the first U.S. federal law for "payment stablecoins." Its main requirements:

- **Who can issue:** only subsidiaries of insured banks, nonbank issuers approved by the OCC, or state-regulated issuers under a state regime certified as "substantially similar." Issuers with $10 billion or less outstanding may stay under state regulation; above that they move to federal oversight. Big Tech and other non-financial public companies are generally barred unless a review committee unanimously approves.
- **Reserves:** 1:1 backing at all times in cash, insured bank deposits, short-term Treasury bills (93 days or less), overnight repos, and government money-market funds. Reserves must be segregated and may not be re-lent or pledged ("rehypothecated").
- **Disclosure:** monthly public reports of reserve composition, certified by executives and examined by a registered accounting firm; annual audited statements for issuers above $50 billion.
- **No yield:** issuers may not pay interest or "any economically equivalent return" to holders simply for holding the coin. This protects bank deposits and is the most contested provision.
- **Redemption and priority:** issuers must honor redemptions promptly, and in an issuer bankruptcy, stablecoin holders are paid ahead of other creditors.
- **Legal status:** compliant payment stablecoins are explicitly not securities or commodities.
- **Foreign issuers** (i.e., Tether) may serve U.S. markets only if their home regime is deemed comparable and they hold reserves able to meet U.S. demand; Tether launched a separate U.S.-compliant coin (USAT) in response.
- **Timing:** effective the earlier of 18 months after enactment (January 2027) or 120 days after final regulations. Rules were still being finalized through 2026.

The Act legitimized stablecoins as a payment technology, and banks (JPMorgan, Bank of America, Citi) and fintechs began announcing their own coins.

## Depeg history

**Terra/UST, May 2022.** UST was an algorithmic stablecoin that held its peg by letting holders swap 1 UST for $1 worth of newly minted LUNA. A 20% yield from the Anchor protocol drew about $18 billion into UST. When large withdrawals began on May 7, 2022, the arbitrage mechanism minted trillions of LUNA, LUNA's price went to zero, and UST collapsed with it. Roughly $40 billion of value was destroyed in a week; the contagion bankrupted hedge fund Three Arrows Capital and lenders Celsius and Voyager, and set up FTX's collapse that November. Founder Do Kwon was later convicted of fraud in the U.S. Lesson: a stablecoin backed by its own sister token is backed by nothing.

**USDC, March 2023.** Circle disclosed on March 10 that $3.3 billion of USDC's cash reserves (about 8%) were stuck at the failing Silicon Valley Bank. Over the weekend USDC fell to roughly $0.87–0.88 on exchanges, and DAI (heavily backed by USDC) fell with it. When U.S. regulators guaranteed all SVB deposits on March 12, USDC returned to $1 within a day. Lesson: even a fully backed coin depends on the banks holding the cash, and the peg can break on a weekend when redemptions are closed.

**USDT** has traded a few cents below $1 during several panics (2018, May 2022) but always recovered. Smaller coins (IRON, USDN, USDR, and others) have failed outright.

## Yield-bearing stablecoins and tokenized Treasuries

Because GENIUS bans issuers from paying yield, the market routed around it:

- **Tokenized Treasury funds** such as BlackRock's BUIDL (about $2 billion in early 2026), Franklin Templeton's BENJI, Ondo's OUSG/USDY, and Superstate's USTB are registered or exempt securities, not payment stablecoins, so they can pass through T-bill yield (roughly 4–5% in 2026). Total tokenized Treasuries passed $10 billion in early 2026 per rwa.xyz and have become the preferred collateral for institutional DeFi.
- **Synthetic dollars** such as Ethena's USDe hold staked ETH and bitcoin hedged with short perpetual futures, earning the funding rate; yields have ranged from near zero to over 20% and can turn negative. Its peg depends on derivatives exchanges and is not a bank-like claim.
- **DeFi lending** on Aave, Morpho, and Compound pays 2–8% on stablecoin deposits, with smart-contract and borrower risk.
- **Exchange rewards:** Coinbase and others pay USDC holders a "reward" funded by their revenue share with Circle, which the Act's authors consider a loophole and banks are lobbying to close.

## Why stablecoins matter for the whole market

1. **They are the trading currency.** Almost every crypto trade is priced and settled in USDT or USDC. Stablecoin supply growth is the cleanest proxy for new money entering crypto; contraction signals outflows.
2. **They are the on-ramp and the off-ramp.** When investors "sell to cash" on an exchange, they usually sell to a stablecoin.
3. **They are collateral.** DeFi lending, perpetual futures, and tokenized-asset markets run on stablecoin collateral.
4. **They are a real product with real users.** Remittances, dollar savings in Argentina, Nigeria, or Turkey, and B2B settlement all use them. Stablecoins settled more transaction volume than Visa in 2024–25 by some measures (though much of it is bot and exchange traffic).
5. **They are a Treasury buyer.** Tether and Circle together hold well over $150 billion of T-bills, making them a policy-relevant source of demand for U.S. debt, which is one reason Washington chose to regulate rather than ban them.

## Key takeaways

- Stablecoins are dollar tokens; the reputable ones are backed by cash and T-bills, and the issuer keeps the interest.
- USDT (~$183B) and USDC (~$74.5B) dominate a ~$311 billion market as of September 2026; total stablecoin supply is the best single gauge of money entering or leaving crypto.
- A stablecoin is an unsecured claim on its issuer plus its banks; attestations are not audits, and Tether has never had a full audit.
- The GENIUS Act (July 2025) requires 1:1 liquid reserves, monthly disclosure, licensed issuers, and bans issuers from paying yield; it takes full effect by early 2027.
- Terra/UST (May 2022) proved algorithmic stablecoins fail catastrophically; USDC (March 2023) proved even fully backed coins can break on bank risk.
- Yield now comes from tokenized Treasury funds, DeFi lending, and synthetic dollars, each with different risks.
- If you hold stablecoins, prefer large, regulated issuers, understand where the reserves sit, and do not treat any of them as FDIC-insured cash.

## Sources

- [Congress.gov: S.1582 GENIUS Act, 119th Congress](https://www.congress.gov/bill/119th-congress/senate-bill/1582)
- [Covington: The GENIUS Act Becomes Law, Key Provisions](https://www.cov.com/news-and-insights/insights/2025/07/the-genius-act-becomes-law-key-provisions-from-the-federal-stablecoin-regulatory-framework)
- [Richmond Fed: Stablecoins and the GENIUS Act, An Overview](https://www.richmondfed.org/banking/banker_resources/news_flash/2025/20251118_genius_act)
- [Hokanews: USDT and USDC control $258 billion of the stablecoin market (Sept 2026)](https://www.hokanews.com/2026/09/usdt-and-usdc-control-258-billion-of.html)
- [Tether: Q2 2026 attestation announcement](https://tether.io/news/tether-posts-strong-q2-performance-generates-1-5b-net-operating-profit-maintains-4-11b-reserve-buffer-and-expands-gold-holdings-to-more-than-146-tons/)
- [SpotedCrypto: Tether Q2 2026 attestation analysis](https://www.spotedcrypto.com/tether-q2-2026-reserve-buffer-halved/)
- [Circle: USDC transparency and reserves](https://www.circle.com/transparency)
- [CNBC: USDC breaks dollar peg after $3.3 billion SVB exposure (March 2023)](https://www.cnbc.com/2023/03/11/stablecoin-usdc-breaks-dollar-peg-after-firm-reveals-it-has-3point3-billion-in-svb-exposure.html)
- [S&P Global: Stablecoins, A Deep Dive into Valuation and Depegging](https://www.spglobal.com/content/dam/spglobal/corporate/en/images/general/special-editorial/stablecoinsadeepdiveintovaluationanddepegging.pdf)
- [BlockEden: Stablecoin Yield Wars 2026](https://blockeden.xyz/blog/2026/05/07/stablecoin-yield-wars-genius-act-usdc-ousg-defi)
- [KuCoin: Tokenized U.S. Treasuries rise over $1B since 2026 began (rwa.xyz data)](https://www.kucoin.com/news/flash/tokenized-u-s-treasuries-rise-over-1b-since-2026-began)
- [rwa.xyz: Tokenized Treasuries dashboard](https://app.rwa.xyz/treasuries)
- [CFTC: Tether and Bitfinex settlement, October 2021](https://www.cftc.gov/PressRoom/PressReleases/8450-21)
- [Bits about Money: A review of Number Go Up](https://www.bitsaboutmoney.com/archive/a-review-of-number-go-up-on-crypto-shenanigans/)
