# Choosing an Exchange

**In one sentence:** Pick a regulated, U.S.-licensed venue whose *real* all-in cost (fee plus spread) is low, whose reserves are verifiable, and whose custody you plan to leave anyway — because an exchange is a place to buy, not a place to keep.

## Why this decision matters more than it looks

The exchange you use decides three things: how much you pay per dollar bought (often 0.1% to 2%+, which compounds over years of buying), how safe your coins are while they sit there, and how much paperwork you get at tax time. Most beginners pick an app because it is familiar, pay a hidden spread on every purchase, and never learn that the same company offers a "pro" interface at a fraction of the cost.

Two terms you need:

- **Maker/taker fee** – a *maker* places an order that sits on the order book (a limit order); a *taker* fills an existing order (a market order). Takers pay more because they remove liquidity.
- **Spread** – the gap between the buy and sell price the app quotes you. "Commission-free" apps earn money here. A 1% spread is a 1% fee with a different name.

## The venues compared (as of September 2026)

| Venue | Cheapest way to buy | Simple/app cost | Regulation & custody notes |
|---|---|---|---|
| **Coinbase** | Advanced Trade: 0.40% maker / 0.60% taker at base tier, falling with volume | Retail "simple buy": spread plus a variable fee that can approach ~1.5–1.9% on small orders; recurring buys ~1.49% | Public company (COIN), state money-transmitter licenses, NY BitLicense; ~98% of assets in cold storage; no cryptographic proof-of-reserves (relies on SEC filings and Deloitte audits) |
| **Kraken** | Kraken Pro: roughly 0.25–0.40% maker / 0.40–0.80% taker at base tier depending on pair schedule (verify current table) | Kraken app "Instant Buy": 1% fee plus spread; recurring buys ~0.40–1% | Quarterly proof-of-reserves attested by an independent CPA firm (The Network Firm); customers can verify their own balance in the Merkle tree; no insurance fund |
| **Gemini** | ActiveTrader: 0.20% maker / 0.40% taker at base tier | Web/mobile: 0.50% "convenience fee" *plus* a transaction fee — $0.99 to $2.99 on orders under $200, 1.49% above $200 | New York trust-company charter (NYDFS); ~$200M insurance via captive insurer; no cryptographic proof-of-reserves |
| **Fidelity Crypto** | 1% spread built into every trade (no separate commission) | Same 1% | Custody by Fidelity Digital Assets, a national trust bank; small coin list; can hold crypto inside a Fidelity IRA; on-chain transfers in/out available |
| **Robinhood** | "Commission-free" with a spread of roughly 0.35–0.85% on majors; 2026 tiered routing pricing of ~0.03–0.95% by volume | Same | Broker-dealer (SIPC does *not* cover crypto); acquired Bitstamp in 2025; withdrawals supported |
| **Binance.US** | 0% maker / 0.02% taker on spot since April 2026 (cheapest headline fee in the U.S.) | Same | Smaller footprint after 2023 regulatory actions; check state availability and banking rails before relying on it |
| **Bitstamp** | 0.30% maker / 0.40% taker at base tier | Card purchases carry a ~4% "instant service" fee plus ~1.8% spread — avoid | Founded 2011; NY BitLicense, FinCEN MSB, 50+ licenses globally; now owned by Robinhood |
| **Brokerage spot ETFs (IBIT, FBTC, ETHA, etc.)** | Zero commission at most brokers; ETF expense ratio ~0.19–0.25%/yr | Same | SIPC-covered brokerage account; no keys, no withdrawals, no on-chain use; tax-advantaged accounts allowed |

*Fee figures are base-tier, as of September 2026; every venue lowers them with 30-day volume. Always re-check the live fee page before trading.*

## What "insured" actually means

- **Coinbase's crime policy** (~$255M via Lloyd's) covers a *portion* of assets in Coinbase's own hot storage against a breach of *Coinbase*. It explicitly does **not** cover your account being emptied because your password or phone was compromised. Cash balances get pass-through FDIC coverage up to $250,000 through partner banks; crypto has no FDIC, NCUA, or SIPC protection anywhere.
- **Gemini** insures through a captive insurer; the same "our breach, not yours" logic applies.
- **Kraken** carries no insurance fund and says so — its answer is proof-of-reserves instead.
- **ETFs** sit in a brokerage account with SIPC coverage against broker failure (not against price loss).

The takeaway: exchange insurance protects the exchange's balance sheet. It is not a guarantee you get your coins back.

## Proof-of-reserves: what to ask for

A **proof-of-reserves (PoR)** is a periodic snapshot showing an exchange holds at least as much crypto as it owes customers, usually published as a **Merkle tree** — a cryptographic structure that lets *you* confirm your own balance was included without revealing anyone else's. Kraken's version is attested by an accounting firm and covers spot, staking, and margin balances in BTC, ETH, SOL, USDC, USDT, and XRP. Coinbase and Gemini do not publish cryptographic PoR; they point to audited financials and regulator exams instead.

Neither is perfect. PoR shows assets, not liabilities beyond customer balances, and a snapshot can be gamed with borrowed coins. But a venue that lets you verify your own balance is doing more than one that just says "trust us."

## What FTX, Celsius, and Voyager taught

All three failed in 2022. All three held customer coins in their own name, and all three sent customers to bankruptcy court as unsecured creditors.

- **FTX** customers were ultimately promised ~118% of their claim in *cash* — but claims were valued at the November 2022 petition date, when bitcoin was under $20,000. Someone who held 1 BTC on FTX got roughly $22,000, not a bitcoin. In bitcoin terms they recovered about a third of what they had.
- **Celsius** creditors had received roughly 65% of claim value by August 2025 across three distributions (mix of crypto, cash, and shares in a mining company), with an eventual target of 67–85%. Its founder was sentenced to prison.
- **Voyager** customers received an initial distribution of roughly 25–35% of claims in 2023, with further trickles from Three Arrows Capital and FTX settlements over subsequent years.

Lessons:

1. A "yield account" at a crypto lender is an unsecured loan *from you* to the company.
2. Even a good bankruptcy outcome freezes your value in dollars at the worst possible moment.
3. Coins in your own wallet were never part of any of these estates. Self-custody — or at least a regulated trust-company custodian — is the only real answer.

## How to actually do it

1. **Decide the account type first.** Want crypto in an IRA or alongside stocks with zero key management? Use a spot ETF at your brokerage or Fidelity Crypto. Want real coins you can withdraw? Continue.
2. **Shortlist two venues** from the table that operate in your state and support ACH deposits (free at most; wires cost ~$25).
3. **Use the pro interface, always.** Coinbase Advanced Trade, Kraken Pro, Gemini ActiveTrader. Same company, same custody, one-fifth to one-tenth the cost of the app's "buy" button.
4. **Place limit orders.** A limit order at or just below the current price usually fills within minutes and gets you the maker rate.
5. **Check the all-in cost on a test buy.** Buy $100, then compare coins received × market price to $100. The gap is your true fee.
6. **Verify their reserves.** On Kraken, open Proof of Reserves and confirm your balance in the last snapshot; on others, read the latest audited filing.
7. **Set up security before funding:** hardware or app-based 2FA (never SMS), a unique password, withdrawal address allowlisting, and a withdrawal delay if offered.
8. **Withdraw to your own wallet** once the balance exceeds what you would be upset to lose (see [security-and-self-custody-setup.md](security-and-self-custody-setup.md)).
9. **Download your transaction history** every quarter (see [record-keeping-and-portfolio-tracking.md](record-keeping-and-portfolio-tracking.md)).

## Key takeaways

- "Commission-free" means the fee is hidden in the spread; measure the all-in cost yourself.
- The pro interface of the same exchange is dramatically cheaper than the app's buy button.
- Exchange insurance covers the exchange's breach, not yours; crypto is never FDIC or SIPC insured.
- Proof-of-reserves you can verify yourself (Kraken) beats "trust our audit," but neither replaces self-custody.
- FTX/Celsius/Voyager customers became unsecured creditors and had their claims frozen in dollars at the bottom.
- ETFs trade custody risk for counterparty simplicity and lose on-chain optionality — a fair trade for many investors.
- Base-tier fees fall quickly with volume; if you trade actively, check tier thresholds.

## Sources

- [Coinbase fees explained (Datawallet, Aug 2026)](https://www.datawallet.com/crypto/coinbase-fees)
- [Kraken fee schedule](https://www.kraken.com/features/fee-schedule) and [How trading fees work on Kraken](https://support.kraken.com/articles/201893638-how-trading-fees-work-on-kraken)
- [Kraken Proof of Reserves](https://www.kraken.com/proof-of-reserves)
- [Gemini fees guide (BitDegree, Apr 2026)](https://www.bitdegree.org/crypto/tutorials/gemini-fees)
- [Fidelity Crypto review (NerdWallet, Aug 2026)](https://www.nerdwallet.com/investing/reviews/fidelity-crypto)
- [Robinhood crypto fees (Cryptsy, Jul 2026)](https://cryptsy.com/robinhood-crypto-fees/)
- [Binance.US zero-fee spot trading announcement](https://blog.binance.us/zero-fee-trading/)
- [Bitstamp exchange review (CryptoSlate, 2026)](https://cryptoslate.com/crypto-exchanges/bitstamp-exchange-review/)
- [How is Coinbase insured? (Coinbase Help)](https://help.coinbase.com/en/coinbase/other-topics/legal-policies/how-is-coinbase-insured)
- [Crypto exchange security comparison (Spark, 2026)](https://www.spark.money/tools/crypto-exchange-security-comparison)
- [FTX plans to repay customers "in full" — why they still lose (Axios, May 2024)](https://www.axios.com/2024/05/08/ftx-customers-recovery-repay-bankruptcy)
- [Celsius begins third distribution (crypto.news, Aug 2025)](https://crypto.news/celsius-220m-distribution-third-payout-round-2025/)
- [Voyager recovers ~30%, second distribution (Benzinga, Apr 2024)](https://benzinga.com/markets/cryptocurrency/24/04/38189476/voyager-digital-recovers-30-second-distribution-coming-for-crypto-creditors)
