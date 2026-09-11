# Dollar-Cost Averaging Execution

**In one sentence:** A recurring buy is the easiest crypto strategy to get right and the easiest to overpay for — choose a venue whose recurring-buy fee is near zero, sweep coins to cold storage on a schedule, and keep every purchase record because the tax system now expects wallet-by-wallet cost basis.

## Why DCA and what it costs

**Dollar-cost averaging (DCA)** means buying a fixed dollar amount on a fixed schedule — $50 every Friday, $500 on the 1st — regardless of price. You automatically buy more coins when prices are low and fewer when high, and you remove the "is now a good time?" question that keeps people on the sidelines. It does not beat lump-sum investing on average (markets rise more often than they fall), but it dramatically improves the odds you actually follow through.

The problem is fees. The "recurring buy" button on the big apps is often the *most* expensive way to buy on that platform. Paying 1.5–2% every week for ten years is a permanent ~1.5–2% drag on every dollar you ever invest.

## Recurring-buy fee comparison (as of September 2026)

| Platform | Recurring-buy fee | Approx. all-in cost incl. spread | Minimum | Auto-withdraw to your wallet? |
|---|---|---|---|---|
| **River** (bitcoin only) | 0% after the first week | ~0.25% (spread) | $100 via ACH | Yes, at 0.005 BTC; one free on-chain withdrawal per month |
| **Strike** (bitcoin only) | 0% after the first week | ~0.15% (spread) | None | Yes, at 1,000,000 sats (0.01 BTC); free on-chain withdrawals |
| **Cash App** (bitcoin only) | 0% on Auto Invest | ~0% plus spread | $1 | Yes, at 100,000 sats |
| **Swan Bitcoin** (bitcoin only) | 0.99% | ~1.24% | $10 | Yes, to a saved address; custody fees waived when enabled |
| **Kraken** | ~0.40–1% depending on app vs Pro | ~0.4–1% plus spread | $1 | No (manual) |
| **Coinbase** | ~1.49% | ~2% | $10 | No (manual); Coinbase One subscription removes some fees for a monthly charge |
| **Fidelity Crypto** | 1% spread on each buy; recurring investment supported in the app | ~1% | $1 | On-chain transfers supported; verify current terms |
| **Gemini** | 0.50% convenience fee + $0.99–$2.99 flat under $200, 1.49% above | ~2–4% on small buys | ~$5 | No (manual) |

*Bitcoin-only platforms are cheaper because they do one thing. For ETH or other assets, Kraken Pro with a manual weekly limit order (~0.25–0.40% maker) is the low-cost route.*

The arithmetic: $200/week for 10 years is $104,000 invested. At 2% all-in you lose ~$2,080 outright; at 0.25% you lose ~$260. The difference buys a hardware wallet several times over — and that is before the lost compounding on the fee.

## Withdrawal cadence to cold storage

Coins sitting on an exchange are an IOU. The habit is to **sweep** to your own wallet on a schedule that balances network fees against exposure:

| Monthly DCA amount | Suggested sweep trigger | Reasoning |
|---|---|---|
| Under $200 | Every 3–6 months, or when the balance exceeds ~$1,000 | Bitcoin on-chain fees have been ~$0.30–$1 median in 2026, but a $30 withdrawal fee at a stingy exchange on a $150 balance is 20% |
| $200–$1,000 | Monthly, or at a 0.005–0.01 BTC threshold | Matches the auto-withdraw thresholds on River/Strike/Cash App |
| Over $1,000 | Every purchase, if the exchange withdrawal fee is small | Large balances on an exchange are the biggest single risk in your setup |

Check the exchange's *withdrawal* fee, which is separate from the network fee and varies wildly — some charge a fixed amount well above the real network cost. Prefer platforms that pass through network fees or offer free withdrawals.

Turn on **auto-withdraw** wherever it exists and point it at an address from your hardware wallet. Verify the address on the device screen when you save it, and do a $10 test.

## UTXO consolidation basics (bitcoin)

Each bitcoin deposit to your wallet creates a separate **UTXO** (unspent transaction output) — think of it as a separate coin in your pocket. Weekly DCA for two years leaves you with ~100 small UTXOs. When you eventually spend, the transaction must include every input it uses, and fees are charged per byte, so a spend built from 100 inputs can cost 50–100× more than one built from a single input — painful if fees spike to 100+ sat/vB during a busy period.

The fix is **consolidation**: during a quiet, low-fee period (1–3 sat/vB; check mempool.space), send all your small UTXOs to a single fresh address in your own wallet. Practical rules:

- Consolidate when fees are low, in your own wallet, to your own address; it is just a transfer to yourself.
- Use a wallet with **coin control** (Sparrow, Electrum, Coldcard) so you can see and select UTXOs.
- Consolidation links all those UTXOs on-chain as belonging to one owner — a privacy trade-off. If privacy matters, consolidate in groups by source.
- Do not consolidate more often than needed; each round costs a fee. Once or twice a year is typical for weekly DCA.
- Aim to keep UTXOs above ~0.001 BTC; "dust" below the fee needed to spend it is effectively unspendable in high-fee periods.

Ethereum and Solana use account balances, not UTXOs, so this section does not apply — deposits simply add to one balance.

## Keeping cost-basis records

Every recurring purchase is a separate tax **lot** with its own date, quantity, and cost. Since 2025 the IRS requires **wallet-by-wallet** basis tracking, and brokers report gross proceeds on **Form 1099-DA** (cost basis reporting begins for 2026 purchases held at the same broker). Coins you move to cold storage arrive at the new wallet with *no* basis in the broker's eyes — you must carry the records yourself.

Minimum practice:

1. Export the exchange's transaction CSV quarterly (buys, fees, withdrawals) and store it with the tax year's documents.
2. Connect the exchange API and your wallet's public address (xpub or receive addresses) to a tracker such as Koinly, CoinLedger, or CoinTracker so lots follow the coins when you withdraw.
3. Record withdrawals as transfers, not sales — mislabeling is the most common tracker error.
4. Note the fair market value of any fee paid in crypto.

Details and tool comparison in [record-keeping-and-portfolio-tracking.md](record-keeping-and-portfolio-tracking.md).

## How to actually do it

1. Decide the amount and frequency from your position-size target (see [position-sizing-and-rebalancing-for-crypto.md](position-sizing-and-rebalancing-for-crypto.md)). Weekly buys smooth more than monthly; fees per buy matter more when buys are small.
2. Choose the venue: for bitcoin, River, Strike, or Cash App (near-zero fee, auto-withdraw). For ETH/other, Kraken Pro with a weekly limit order, or Coinbase Advanced Trade.
3. Fund via ACH (free); avoid card purchases, which add 3–4%.
4. Set the recurring order. On Kraken/Coinbase, consider a manual weekly limit order instead of the "recurring" button to get maker pricing.
5. Add your hardware-wallet receive address to the platform's allowlist; test with $10; then enable auto-withdraw at the platform's threshold or set a calendar reminder for manual sweeps.
6. Once or twice a year, when fees are 1–3 sat/vB, consolidate small UTXOs in your own wallet.
7. Export CSVs quarterly and sync your tracker; label withdrawals as transfers.
8. Review the DCA amount once a year alongside your rebalancing review — increase it with income, never chase price.

## Key takeaways

- DCA wins by removing timing decisions, not by beating lump-sum returns.
- The app "recurring buy" button often costs 1.5–2% per purchase; bitcoin-only platforms and pro interfaces cost 0–0.4%.
- Fund by ACH, never by card.
- Sweep to cold storage on a schedule or with auto-withdraw; never let a large balance accumulate on an exchange.
- Weekly bitcoin buys create many small UTXOs; consolidate in low-fee windows to avoid an expensive spend later.
- Every buy is a tax lot; export records quarterly and track wallet-by-wallet.
- Raise the DCA amount with income, not with price.

## Sources

- [DCA platform comparison: Swan vs River vs Strike vs Coinbase vs Kraken (Spark, 2026)](https://www.spark.money/tools/dca-platform-comparison)
- [River Financial launches zero-fee recurring bitcoin purchases (Nasdaq)](https://www.nasdaq.com/articles/river-financial-launches-zero-fee-recurring-bitcoin-purchases)
- [What are Swan Bitcoin's fees? (Swan FAQ)](https://help.swanbitcoin.com/hc/en-us/articles/360045394134-What-are-Swan-Bitcoin-s-fees)
- [Coinbase fees explained (Datawallet, Aug 2026)](https://www.datawallet.com/crypto/coinbase-fees)
- [Kraken fee schedule](https://www.kraken.com/features/fee-schedule)
- [Fidelity Crypto review (NerdWallet, Aug 2026)](https://www.nerdwallet.com/investing/reviews/fidelity-crypto)
- [The complete guide to bitcoin transaction fees in 2026 (99Bitcoins)](https://99bitcoins.com/cryptocurrency/bitcoin/fees/)
- [Bitcoin fee at 1 sat/vB: consolidate your UTXOs now (CryptoTicker)](https://cryptoticker.io/en/bitcoin-network-fee-utxo-consolidation/)
- [Form 1099-DA: what US crypto investors need to know (CoinTracking, 2026)](https://cointracking.info/blog/form-1099-da/)
