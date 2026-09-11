# Exchange and Counterparty Risk

**In one sentence:** When you leave crypto on an exchange or in a yield account, you have usually made an unsecured loan to a company, and in every major failure so far the customers found that out only from the bankruptcy judge.

## What "custody" actually means

When a bank holds your dollars, deposit insurance (FDIC in the US) covers you up to $250,000 if the bank fails. When a broker holds your stocks, they are segregated from the broker's own assets and SIPC covers up to $500,000 if the broker fails. Neither applies to crypto. The FDIC does not insure crypto, SIPC does not cover it, and several failed platforms were formally ordered to stop implying otherwise (the Federal Reserve and FDIC sent Voyager a cease-and-desist over its insurance claims in July 2022).

What matters instead is the fine print. If the terms of service say the platform may lend, stake or rehypothecate your assets (use them as collateral for its own borrowing), then legally you handed over ownership and hold a claim, not coins. The Celsius bankruptcy court ruled exactly this in January 2023: roughly 600,000 "Earn" customers were unsecured creditors, not owners.

Jargon: an **unsecured creditor** is someone owed money with no collateral, who is paid after secured lenders and administrative costs. **Petition date** is the day a bankruptcy is filed; claims are usually frozen at that day's prices. **Proof of reserves** is an exchange publishing evidence it holds customer assets.

## The case files

| Platform | Failed | What happened to customer funds | Customer outcome (as of Sep 2026) |
|---|---|---|---|
| **Mt. Gox** (Japan) | Feb 2014 | ~850,000 BTC missing through theft over years, concealed by the operator; 200,000 later found. CEO Karpelès was convicted only of falsifying records (2019), acquitted of embezzlement. | 127,000 creditors. Claims were fixed in yen at 2014 prices but the rehabilitation plan (confirmed Nov 2021) paid in BTC and BCH starting July 2024. Creditors got a fraction of their original coins but far more fiat value than they lost, after ten years. |
| **QuadrigaCX** (Canada) | Dec 2018 – Jan 2019 | Founder Gerald Cotten died in India in December 2018, supposedly with the only keys. The Ontario Securities Commission concluded in 2020 that it was "an old-fashioned fraud": Cotten had traded fake balances against customers and lost their money. ~C$215M owed. | Tens of thousands of claimants. First interim dividend in March 2023 was about 13 cents on the dollar. |
| **Celsius** | Jul 2022 | Promised up to ~18% yield; lent customer coins to 3AC and others, ran a directional book, and the CEO manipulated the CEL token. $4.7B owed to 1.7M customers. | Earn customers ruled unsecured. Emerged Jan 2024; distributed over $3B in crypto, cash and shares of a mining company. Mashinsky pleaded guilty and was sentenced to 12 years (May 2025). |
| **Voyager** | Jul 2022 | Lent $666M to 3AC unsecured; ~$1.3B in customer assets frozen. Marketed FDIC "insurance" that only covered the bank account holding USD. | Initial recovery in 2023 was roughly a third of claim value in kind, with more from later 3AC and FTX recoveries. |
| **BlockFi** | Nov 2022 | Paid $100M to the SEC in Feb 2022 for unregistered lending products, then was sunk by exposure to FTX/Alameda. 100,000+ creditors. | Emerged Oct 2023 in wind-down; distributions to customers depended heavily on what BlockFi recovered from the FTX estate. |
| **FTX** | Nov 2022 | ~$8B of customer deposits had been diverted to sister fund Alameda for venture bets, political donations and real estate. Bankman-Fried convicted on all counts (Nov 2023), sentenced to 25 years (Mar 2024). | Claims frozen at Nov 2022 prices (BTC ~$16–17K). Five distribution rounds from Feb 2025 to Jul 2026 paid nearly $10B; customers have received ~105% of petition-date dollar value, but far less than the coins would have been worth at 2025 prices. |
| **Bybit** | Feb 2025 (hack, not insolvency) | ~$1.5B of ETH stolen by North Korea's Lazarus Group through a compromised signing interface. | Bybit covered the loss from its own treasury and loans; withdrawals continued. The exception that shows the rule: only a large, profitable exchange can absorb this. |

## Three lessons buried in the recoveries

**"Made whole" in dollars can still be a large loss in coins.** FTX's headline 105%+ recovery is real in petition-date dollars. A customer who held 1 BTC on FTX received roughly $17,000 of value plus interest across 2025–26, during which BTC traded between about $58,000 and $126,000. Mt. Gox creditors experienced the reverse (claims fixed low, paid in BTC that rose), which is why the two groups feel so differently about "recovery."

**Bankruptcy takes years, and you are unsecured.** Mt. Gox: ten years. Celsius: eighteen months to a plan. FTX: over two years to first payment. During that time the assets are frozen, legal and administrative fees come out first, and the market moves without you.

**Fraud is the common thread, not bad luck.** Mt. Gox concealed losses for years. QuadrigaCX was a one-man Ponzi. FTX moved customer money by design. Celsius's CEO manipulated his own token. External audits, VC backing, sports-stadium naming rights and lobbying in Washington were present in several cases and prevented nothing.

## Proof of reserves and its limits

After FTX, exchanges rushed to publish "proof of reserves" (PoR): a cryptographic snapshot showing wallets holding at least as much as customer balances. It is better than nothing, and a large exchange that cannot or will not publish one is a red flag. But PoR has well-known gaps:

- It shows assets, not liabilities. An exchange can borrow coins for the snapshot or hide off-chain debts.
- It is a point in time, not continuous.
- It often excludes internal loans to affiliates, which is exactly how FTX failed.
- Many PoR reports are "agreed-upon procedures" by an accounting firm, not audits; one of the most prominent firms involved stopped doing them in late 2022.
- It says nothing about operational security (Bybit had reserves; it had a compromised front end).

Treat PoR as a minimum hygiene check, not as evidence of solvency.

## How to limit exposure

| Tier | Where | Rule of thumb |
|---|---|---|
| Long-term holdings | Self-custody: hardware wallet, seed phrase backed up offline in two places; or a regulated qualified custodian or spot ETF if you accept the counterparty in exchange for simplicity | Anything you would be devastated to lose belongs here |
| Trading float | One or two large, regulated exchanges in your jurisdiction | Keep only what you will trade in the next few weeks; withdraw profits on a schedule |
| Yield accounts | Only with a documented source of yield you understand (e.g., native staking through a wallet, not a company promising a rate) | Assume the balance is an unsecured loan; size accordingly |
| Stablecoins | Prefer issuers with monthly attested reserves in T-bills and bank deposits; remember USDC still traded at ~$0.87 during the SVB weekend in March 2023 | Diversify issuers for large balances; do not treat as cash for emergencies |

Practical limits many experienced holders use: no more than 10–20% of total crypto on any single exchange; no single exchange balance above what you could lose without changing your life; withdrawals tested before they are needed; two-factor authentication with a hardware key, not SMS; a separate email address for exchange accounts.

## Countermeasures / How to apply

- Read the custody section of any platform's terms of service. If it can lend or rehypothecate your assets, you are a creditor.
- Assume no deposit insurance exists for crypto, regardless of marketing. FDIC and SIPC do not cover it.
- Move long-term holdings to self-custody or a spot ETF/qualified custodian; keep exchange balances to a trading float.
- Check proof of reserves for any exchange you use, but do not mistake it for an audit.
- Diversify across exchanges and stablecoin issuers; withdraw on a schedule, not only when scared.
- Watch the warning signs that preceded every failure: withdrawal delays, changes to terms, executives leaving, a related-party token propping up the balance sheet, and yields above what the market pays.
- If a platform freezes withdrawals, act immediately on other platforms, document your balances, and file claims early; expect years and partial recovery.

## Key takeaways

- Every failed platform's customers became unsecured creditors; the fine print made them so long before the failure.
- FDIC and SIPC do not cover crypto, and regulators have ordered platforms to stop suggesting they do.
- FTX customers got ~105% of Nov 2022 dollar claims by mid-2026 but lost most of the crypto upside; Mt. Gox creditors waited ten years.
- Fraud, not market volatility, was the root cause at Mt. Gox, QuadrigaCX, FTX and Celsius.
- Proof of reserves shows assets on one day and says nothing about liabilities or security.
- Even a solvent, large exchange can lose $1.5B in one transaction (Bybit, 2025).
- Self-custody carries its own risks (lost seeds, drainers, physical coercion) but removes counterparty risk.
- Limit any single exchange balance to a trading float you could afford to lose entirely.

## Sources

- [Wikipedia, Mt. Gox](https://en.wikipedia.org/wiki/Mt._Gox)
- [Wikipedia, Quadriga Fintech Solutions](https://en.wikipedia.org/wiki/Quadriga_Fintech_Solutions)
- [Wikipedia, Celsius Network](https://en.wikipedia.org/wiki/Celsius_Network)
- [Wikipedia, Voyager Digital](https://en.wikipedia.org/wiki/Voyager_Digital)
- [Wikipedia, BlockFi](https://en.wikipedia.org/wiki/BlockFi)
- [Wikipedia, Bankruptcy of FTX](https://en.wikipedia.org/wiki/Bankruptcy_of_FTX)
- [The Crypto Times, FTX creditors' 105% recovery](https://www.cryptotimes.io/2026/07/31/ftx-creditors-105-recovery-why-exchanges-clients-are-getting-more-than-they-lost/)
- [CoinDesk, FTX set to repay $2.2 billion](https://www.coindesk.com/business/2026/03/18/sam-bankman-fried-s-bankrupt-exchange-ftx-set-to-repay-creditors-usd2-2-billion-this-month)
- [Chainalysis, stolen funds 2025 (Bybit)](https://www.chainalysis.com/blog/crypto-hacking-stolen-funds-2026/)
- [Forbes, inside the Bybit hacking incident](https://www.forbes.com/sites/digital-assets/2025/04/01/inside-the-bybit-hacking-incident-lessons-from-the-breach/)
- [Wikipedia, Three Arrows Capital](https://en.wikipedia.org/wiki/Three_Arrows_Capital)
