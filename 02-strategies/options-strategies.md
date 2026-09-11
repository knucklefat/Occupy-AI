# Options Strategies

**In one sentence:** Options are contracts that let you buy or sell insurance on stock prices — useful for generating income, limiting losses, or defining risk precisely — but they are a zero-sum game against professionals, they decay in value every day, and the strategies that sound like free income are the ones that eventually deliver the largest surprise losses.

## What an option is

A **call** gives the holder the right (not the obligation) to *buy* 100 shares at a fixed price (the **strike**) before a fixed date (**expiration**). A **put** gives the right to *sell* 100 shares at the strike. The buyer pays a **premium** for that right; the seller (writer) collects the premium and takes on the obligation.

Think of a put as an insurance policy on a stock and a call as a deposit on a future purchase. The premium reflects how likely the option is to pay off, how much time is left, and how volatile the stock is. An option is **in the money** if exercising it would be profitable right now, **out of the money** if not.

Two prices matter: the option's **intrinsic value** (how far in the money it is, never less than zero) and its **time value** (everything else — the market's price for the possibility that it moves further in the money). Time value goes to zero at expiration. Every day that passes transfers a little value from option buyers to option sellers.

## The Greeks in plain language

The Greeks measure how an option's price responds to changes in the things that drive it.

| Greek | Measures | Plain meaning | Typical use |
|---|---|---|---|
| **Delta** | Change in option price per $1 move in the stock | A 0.30-delta call gains about 30 cents when the stock rises $1. Also a rough probability the option expires in the money (30%). | Sizing hedges; picking strikes ("sell the 20-delta put") |
| **Gamma** | Change in delta per $1 move | How fast your exposure changes. High near the strike and near expiration — the source of sudden large losses for sellers. | Know when a small move becomes a big problem |
| **Theta** | Change in option price per day | Time decay. A theta of −0.05 means the option loses $5 per contract per day, all else equal. Negative for buyers, positive for sellers. | The "income" in income strategies is theta |
| **Vega** | Change in option price per 1-point change in implied volatility | Options get pricier when the market expects bigger swings. Buying before earnings and selling after is buying high vega and watching it collapse ("IV crush"). | Sell options when implied volatility is high; buy when it is low |
| **Rho** | Sensitivity to interest rates | Minor for short-dated options | Mostly ignorable for retail |

**Implied volatility (IV)** is the market's forecast of how much the stock will move, backed out of option prices. **IV rank** (where today's IV sits relative to the past year) is the single most useful number for option sellers: selling premium when IV rank is high (above 50) means being paid more for the same risk.

## The core strategies

| Strategy | Construction | Outlook | Max gain | Max loss | Who it suits |
|---|---|---|---|---|---|
| **Covered call** | Own 100 shares; sell 1 call above current price | Neutral to mildly bullish | Premium + gain up to strike | Stock falls to zero minus premium | Long-term holders willing to sell at the strike |
| **Cash-secured put** | Hold cash equal to 100 × strike; sell 1 put below current price | Neutral to bullish; happy to own the stock lower | Premium | Strike minus premium (stock goes to zero) | Investors who want to buy a stock at a discount and get paid to wait |
| **Protective put** | Own 100 shares; buy 1 put below current price | Bullish but worried | Unlimited (minus premium) | Stock price minus strike, plus premium | Concentrated positions, pre-event hedging |
| **Collar** | Own 100 shares; buy a put below, sell a call above | Want protection at low or zero cost | Capped at call strike | Limited to put strike | Executives with company stock; retirees locking in gains |
| **The wheel** | Sell cash-secured puts until assigned; then sell covered calls until called away; repeat | Neutral to bullish, on a stock you'd own anyway | Premiums + modest appreciation | Same as owning the stock, minus premiums | Patient income investors with a watch list |
| **Vertical spread** (bull call, bear put, credit spreads) | Buy one option, sell another at a different strike, same expiration | Directional with defined risk | Difference in strikes minus net cost (debit) or net premium (credit) | Net debit, or strike width minus credit | Anyone who wants a capped, known loss |
| **Iron condor** | Sell an out-of-the-money put spread and call spread simultaneously | Expect the stock to stay in a range | Net credit | Strike width minus credit | Income sellers in high-IV, range-bound markets |
| **Long call / long put** | Buy an option outright | Strongly directional | Unlimited / strike minus premium | Premium paid | Speculation; cheap leverage with defined loss |

### Covered calls in more detail

You own 100 shares of a stock at $50, and sell a one-month call with a $55 strike for $1.00 ($100 per contract). If the stock stays below $55, you keep the $100 and the shares; repeat next month. If it rises to $60, you must sell at $55 — you keep the $100 premium plus $500 of gains but forgo the additional $500. If it falls to $40, you lose $1,000 on the shares, cushioned by the $100.

The long-run evidence: the Cboe BXM index (S&P 500 with a monthly at-the-money call) returned about the same as the S&P 500 from 1988 to 2006 with two-thirds the volatility, underperforming in the late-1990s boom and outperforming in the 2000–2003 bust. Since 2009, a period of relentless rallies, buy-write indexes have lagged the S&P 500 materially. Covered calls are a *trade*: you give up the right tail in exchange for steady small payments. In a market whose returns come disproportionately from a few big up-months, that is often a losing trade — see the covered-call ETF discussion in [dividend-and-income-investing.md](dividend-and-income-investing.md).

### Cash-secured puts and the wheel

Selling a $45 put on the $50 stock for $0.80 means you collect $80 and promise to buy 100 shares at $45 if the stock falls below it. If it does not, you keep $80 (about 1.8% on the $4,500 reserved, for one month). If it falls to $40, you own shares worth $4,000 for which you paid $4,420 net — the same loss as anyone who bought at $44.20. The "wheel" then sells calls against those shares until they are called away.

This works well only on stocks you genuinely want to own at the strike. The failure mode is selling puts on volatile stocks because the premium is juicy, and then owning a collapsing stock.

### Protective puts and collars

Buying a put is paying for insurance; a 5%-out-of-the-money three-month put on an index typically costs 1%–2% of the position value, or 4%–8% a year if rolled continuously. That is expensive enough to erase most of the equity premium, so protective puts make sense for specific windows (a large concentrated position ahead of a known risk) rather than as permanent policy. A collar funds the put by selling a call — often at zero net cost — at the price of capping the upside. It is the standard tool for someone who must hold a large single-stock position (employee shares, a founder's stake) and wants to sleep.

## When options make sense

- **You would sell the stock at the call strike anyway** (covered call as an exit with a bonus).
- **You would buy the stock at the put strike anyway** (cash-secured put as a limit order that pays you).
- **You have a concentrated position you cannot or will not sell** (collar).
- **You want a leveraged directional bet with a hard cap on loss** (long call or debit spread instead of margin).
- **Implied volatility is unusually high** and you are a seller with defined risk (credit spreads, iron condors) — being paid a lot for insurance others are panicking to buy.

## When they do not

- To "generate income" on a portfolio you otherwise want to grow — the income is your upside, repackaged.
- Buying short-dated out-of-the-money calls on stocks in the news. Theta and IV crush make this a reliable way to lose money; studies of retail option trading (Bauer, Cosemans, Eichholtz 2009; more recent work on zero-days-to-expiration options) find most retail option buyers lose consistently.
- Selling naked (uncovered) calls or puts without cash backing. The loss is theoretically unlimited on calls and enormous on puts; this is how accounts blow up in a gap-down.
- Anything you cannot draw the payoff diagram for from memory.

## Risks specific to options

- **Assignment**: short options can be exercised early (especially calls before an ex-dividend date). Be ready to deliver or buy shares.
- **Liquidity**: wide bid-ask spreads on thinly traded options cost several percent per round trip. Stick to liquid names (index ETFs, mega-caps) with penny-wide spreads.
- **Taxes**: option premiums are generally short-term gains; covered calls can reset the holding period of the underlying shares if the call is "deep in the money" (IRS "qualified covered call" rules); index options (SPX, XSP) get favorable 60/40 long/short treatment under Section 1256.
- **Gamma near expiration**: a position that seemed safe at 30 days can swing violently in the last 48 hours. Close or roll short options a week or more before expiration unless you specifically want the assignment.
- **Leverage that hides**: a portfolio of "conservative" credit spreads can carry a total loss exposure many times the account's size if a crash breaches every spread simultaneously — which is precisely when they all do.

## How to actually do it

1. **Learn the payoff diagrams** for the eight strategies above until you can sketch each without looking. If you cannot, do not trade it.
2. **Get approved** at your broker for the level you need: Level 1 (covered calls, cash-secured puts) is enough for most investors; Level 2 adds long options and spreads.
3. **Paper trade for three months** using the broker's simulator. Track not just P&L but what happened at expiration and how often you were assigned.
4. **Start with covered calls or cash-secured puts on a broad index ETF** (SPY, QQQ, IWM) or a large, liquid stock you already own. Sell 30–45 days out, at a delta of roughly 0.20–0.30 (about 70%–80% chance of expiring worthless). Close when you have captured 50%–70% of the premium rather than holding to expiration.
5. **Check IV rank before selling.** Above 30–50 is a reasonable environment; below 20 means you are being underpaid.
6. **Never sell more contracts than shares (or cash) you hold.** Write this rule down.
7. **Size any long option position at 1%–2% of the portfolio**, and treat the premium as spent.
8. **Keep a trade log** with the thesis, the Greeks at entry, and the outcome. After 30 trades, compare your total P&L to what simply holding the underlying would have returned. Most people find the answer humbling.
9. **Use options in a tax-advantaged account** where practical, since almost all option gains are short-term.

## Key takeaways

- Calls are the right to buy, puts the right to sell; the buyer pays a premium that decays daily (theta) and the seller collects it in exchange for taking on the obligation.
- Delta is direction and rough probability, gamma is how fast that changes, theta is time decay, vega is sensitivity to fear; sell when implied volatility is high, buy when low.
- Covered calls and cash-secured puts are the retail workhorses — sensible when you would happily sell or buy at the strike anyway.
- "Income" from options is upside sold in advance; over long bull markets buy-write strategies have trailed the index.
- Protective puts cost 4%–8% a year rolled; use them for windows, not forever. Collars are the tool for concentrated positions.
- Never trade naked short options; never buy short-dated lottery tickets; never trade a strategy you cannot draw.
- Keep a log and compare to buy-and-hold after 30 trades before scaling up.

## Sources

- [Cboe S&P 500 BuyWrite Index (BXM) factsheet](https://cdn.cboe.com/resources/indices/factsheet/CboeGlobalIndices_BXM-Index.pdf)
- [Callan evaluation of the BXM vs S&P 500 (1988–2006)](https://www.borntosell.com/covered-call-blog/evaluation-of-buy-write-strategy)
- [Options-Based Benchmark Indexes: Performance and Risk — Wilshire/Cboe 2019 (PDF)](https://cdn.cboe.com/resources/spx/wilshire-options-based-benchmark-indexes-2019.pdf)
- [Investopedia: Options Basics](https://www.investopedia.com/options-basics-tutorial-4583012)
- [Investopedia: The Greeks](https://www.investopedia.com/trading/getting-to-know-the-greeks/)
- [Investopedia: Covered Call](https://www.investopedia.com/terms/c/coveredcall.asp)
- [Investopedia: Cash-Secured Put](https://www.investopedia.com/terms/c/cash-secured-put.asp)
- [Investopedia: Collar](https://www.investopedia.com/terms/c/collar.asp)
- [Options Industry Council (OIC) — free education from the exchanges](https://www.optionseducation.org/)
- [Covered Call ETFs Explained — Yahoo Finance](https://finance.yahoo.com/markets/options/articles/covered-call-etfs-explained-8-232105238.html)
