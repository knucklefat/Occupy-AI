# Academic Papers and Research

**In one sentence:** The peer-reviewed literature on crypto is small enough to actually read, and it is far more skeptical than the industry, so the twenty-odd papers below are the best antidote to both the bull-market narrative and the lazy "it's all a scam" dismissal.

## Why bother with papers

Industry research (see [research-desks-and-reports.md](research-desks-and-reports.md)) is paid for by people selling crypto. Academic finance is paid for by tenure, which has its own distortions but does not depend on token prices. The papers below are where you find out whether Bitcoin returns are explained by stock factors (mostly not), whether Tether printing moved the 2017 price (the evidence says yes), how concentrated ownership really is (very), and why a proof-of-work chain's security budget may not scale (Budish). Every link is to a free version or to the journal page; where the journal is paywalled, the working-paper version is usually free on SSRN, NBER or arXiv.

Difficulty: *Readable* means a non-economist can follow the argument from the introduction and conclusion; *Technical* means the model or econometrics matter and you will need some background.

## The founding documents

**[Bitcoin: A Peer-to-Peer Electronic Cash System](https://bitcoin.org/bitcoin.pdf)** — Satoshi Nakamoto, 2008. *Readable, 9 pages.* Still the clearest statement of the problem (double-spending without a trusted party) and the solution (proof-of-work chain, longest-chain rule). Read it before anything else; notice what it does not say (nothing about "digital gold").

**[Ethereum Whitepaper](https://ethereum.org/en/whitepaper/)** — Vitalik Buterin, 2014. *Readable.* The original proposal for a general-purpose blockchain, with the "world computer" framing and a candid section on scalability limits. The page notes which parts are now out of date.

## Returns, risk and pricing

**[Risks and Returns of Cryptocurrency](https://doi.org/10.1093/rfs/hhaa113)** — Yukun Liu and Aleh Tsyvinski, *Review of Financial Studies*, 2021. *Technical, but the tables speak for themselves.* The first top-journal test of whether crypto returns are explained by equity, currency or commodity factors: they are not, and the only reliable predictors are crypto-specific momentum and investor-attention measures. Foundational for anyone treating crypto as a portfolio asset.

**[Equilibrium Bitcoin Pricing](https://doi.org/10.1111/jofi.13206)** — Bruno Biais, Christophe Bisière, Matthieu Bouvard, Catherine Casamatta and Albert Menkveld, *Journal of Finance*, 2023. *Technical.* A model where Bitcoin's price reflects its transactional benefits net of risks (hacks, regulatory bans), estimated on real data. The empirical finding that "crypto-specific" risk explains a large share of returns is a rigorous version of what every trader knows.

**[Trading and Arbitrage in Cryptocurrency Markets](https://doi.org/10.1016/j.jfineco.2019.07.001)** — Igor Makarov and Antoinette Schoar, *Journal of Financial Economics*, 2020. *Readable.* Documents large, persistent price differences for the same coin across exchanges and countries (the "Kimchi premium" and its cousins), and attributes them to capital controls and slow fiat rails. Explains why crypto markets were, and partly still are, less efficient than they look.

**[Cryptocurrencies: Stylized Facts on a New Investible Instrument](https://doi.org/10.1111/fima.12300)** — Albert Hu, Christine Parlour and Uday Rajan, *Financial Management*, 2019. *Readable.* Early, plain-language evidence that nearly all altcoins are just leveraged Bitcoin: returns are highly correlated with BTC and mostly uncorrelated with stocks. Useful for diversification arguments.

## Market manipulation and integrity

**[Is Bitcoin Really Untethered?](https://doi.org/10.1111/jofi.12903)** — John Griffin and Amin Shams, *Journal of Finance*, 2020. *Readable.* Blockchain forensics showing that Tether issuance in 2017 was used to buy Bitcoin at price dips from a single large Bitfinex-linked account, consistent with manipulation rather than organic demand. Tether disputes the findings; the paper survived peer review at the field's top journal. Required reading on stablecoins and market integrity.

**[Sex, Drugs, and Bitcoin: How Much Illegal Activity Is Financed through Cryptocurrencies?](https://doi.org/10.1093/rfs/hhz015)** — Sean Foley, Jonathan Karlsen and Tālis Putniņš, *Review of Financial Studies*, 2019. *Readable.* Estimates that around a quarter of Bitcoin users and nearly half of transactions (by 2017) were associated with illegal activity, though the share was falling as mainstream interest grew. The number is contested (Chainalysis puts illicit share far lower with different methods); read both.

## Ownership, concentration and who actually uses this

**[Blockchain Analysis of the Bitcoin Market](https://www.nber.org/papers/w29396)** — Igor Makarov and Antoinette Schoar, NBER Working Paper 29396, 2021. *Readable.* The definitive study of who holds and moves Bitcoin: the top 10,000 individual holders control about a third of supply, mining is highly concentrated, and most volume is exchange-to-exchange rather than payments. Deflates the "decentralized" claim at the ownership layer. Free PDF; also on [SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3942181).

**[Crypto trading and Bitcoin prices: evidence from a new database of retail adoption](https://www.bis.org/publ/work1049.htm)** — Raphael Auer, Giulio Cornelli, Sebastian Doerr, Jon Frost and Leonardo Gambacorta, BIS Working Paper 1049, 2022. *Readable.* Exchange-app downloads across 95 countries show retail investors pile in after prices rise, and the typical buyer is a man under 35; most retail participants who bought after 2015 were likely underwater by the 2022 crash. The best evidence on the "retail buys the top" pattern.

**[The 2025 Geography of Cryptocurrency / Global Adoption Index](https://www.chainalysis.com/blog/2025-global-crypto-adoption-index/)** — Chainalysis, 2025 (annual). *Readable; industry, not peer-reviewed.* Ranks countries by grassroots adoption adjusted for purchasing power; consistently shows the heaviest real-world use in India, Nigeria, Vietnam, Indonesia and other emerging markets rather than the US. Included here because there is no academic equivalent.

## Stablecoins and runs

**[Taming Wildcat Stablecoins](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3888752)** — Gary Gorton and Jeffery Zhang, *University of Chicago Law Review*, 2023 (SSRN 2021). *Readable.* A Yale banking historian and a Fed lawyer argue stablecoins are privately issued money of the kind that failed repeatedly in the 19th-century "free banking" era, and should be regulated as bank deposits. The intellectual basis for much of the 2025 GENIUS Act debate.

**[Anatomy of a Run: The Terra Luna Crash](https://www.nber.org/papers/w31160)** — Jiageng Liu, Igor Makarov and Antoinette Schoar, NBER Working Paper 31160, 2023. *Readable.* Uses on-chain data to reconstruct the May 2022 collapse of the UST stablecoin block by block: large, sophisticated holders got out first, retail was left holding the bag, and the blockchain's transparency did not prevent a classic bank run. The best case study of a crypto run in existence.

**[Will the real stablecoin please stand up?](https://www.bis.org/publ/bppdf/bispap141.htm)** — Anneke Kosse, Marc Glowka, Ilaria Mattei and Tara Rice, BIS Papers 141, 2023. *Readable.* Examines 68 stablecoins and finds not one held its peg at all times; the fiat-backed ones did best, the algorithmic ones worst. Short, and an efficient corrective to "stablecoins are just digital dollars."

**[Stablecoins: Growth Potential and Impact on Banking](https://www.federalreserve.gov/econres/ifdp/stablecoins-growth-potential-and-impact-on-banking.htm)** — Gordon Liao and John Caramichael, Federal Reserve IFDP, 2022. *Readable.* Works through what happens to bank credit if stablecoins scale under different reserve designs (narrow bank, deposits, securities). The framework regulators used when drafting reserve rules.

**[Stablecoins: risks, potential and regulation](https://www.bis.org/publ/work905.htm)** — Douglas Arner, Raphael Auer and Jon Frost, BIS Working Paper 905, 2020. *Readable.* An early but still-cited map of stablecoin designs and the regulatory questions each raises.

## Economics of blockchains and tokens

**[The Economic Limits of Bitcoin and the Blockchain](https://www.nber.org/papers/w24717)** — Eric Budish, NBER Working Paper 24717, 2018; expanded as [Trust at Scale: The Economic Limits of Cryptocurrencies and Blockchains](https://bfi.uchicago.edu/working-paper/the-economic-limits-of-bitcoin-and-anonymous-decentralized-trust-on-the-blockchain/), Becker Friedman Institute, 2022–2025. *Readable, one key equation.* Argues that proof-of-work security is a flow cost that must be paid forever and must scale with the value of what an attacker could gain, which makes a very valuable Bitcoin either very expensive to secure or vulnerable. The most cited economic critique of Bitcoin's design; Bitcoiners have replies (attack costs are higher than the model assumes), but every serious investor should know the argument.

**[Tokenomics: Dynamic Adoption and Valuation](https://doi.org/10.1093/rfs/hhaa089)** — Lin William Cong, Ye Li and Neng Wang, *Review of Financial Studies*, 2021. *Technical.* A model in which a platform's token accelerates adoption because users anticipate future price gains, and which derives a token value from platform usage. The academic foundation of "tokenomics" as a discipline; also explains why token prices are so much more volatile than the platforms they represent.

**[Some Simple Economics of the Blockchain](https://www.nber.org/papers/w22952)** — Christian Catalini and Joshua Gans, NBER Working Paper 22952, 2016 (later in *Communications of the ACM*). *Readable.* Frames blockchains as reducing two costs, verification and networking, and asks where that actually matters. The clearest "what is this technology economically good for" paper; the answer is narrower than the hype.

**[Some Simple Bitcoin Economics](https://doi.org/10.1016/j.jmoneco.2019.07.002)** — Linda Schilling and Harald Uhlig, *Journal of Monetary Economics*, 2019. *Technical.* A monetary model where Bitcoin and dollars coexist; derives that Bitcoin's expected return should equal the dollar's under certain conditions, and analyzes how central-bank policy interacts with a fixed-supply competitor.

**[The Blockchain Folk Theorem](https://doi.org/10.1093/rfs/hhy095)** — Bruno Biais, Christophe Bisière, Matthieu Bouvard and Catherine Casamatta, *Review of Financial Studies*, 2019. *Technical.* A game-theoretic analysis of proof-of-work mining showing that the "longest chain" rule is an equilibrium, but so are persistent forks; the consensus is a coordination outcome, not a mathematical guarantee.

**[The Microeconomics of Cryptocurrencies](https://doi.org/10.1257/jel.20201593)** — Hanna Halaburda, Guillaume Haeringer, Joshua Gans and Neil Gandal, *Journal of Economic Literature*, 2022. *Readable survey.* If you read one paper to understand what economists have concluded about crypto, read this one: it summarizes the literature on mining, consensus, pricing, tokens and platform economics with a professional's skepticism.

**[Is Bitcoin a Real Currency? An Economic Appraisal](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2361599)** — David Yermack, NBER/SSRN, 2013 (later in the *Handbook of Digital Currency*). *Readable.* The first mainstream finance paper on Bitcoin, concluding it fails all three tests of money (medium of exchange, unit of account, store of value) and behaves like a speculative asset. A decade on, the judgment holds on two of three counts.

## The critics' side, formally

**[Bitcoin, Currencies, and Fragility](https://arxiv.org/abs/2106.14204)** — Nassim Nicholas Taleb, arXiv, 2021 (the "Black Paper"). *Technical in parts, polemical throughout.* Argues that an asset with no cash flow and a non-zero probability of going to zero has an expected present value of zero, and that Bitcoin fails as a currency, an inflation hedge and a safe haven. Overstated (the same argument would condemn gold and art) but the fragility framing is worth engaging.

**[Bitcoin's last stand](https://www.ecb.europa.eu/press/blog/date/2022/html/ecb.blog221130~5301eecd19.en.html)** — Ulrich Bindseil and Jürgen Schaaf, European Central Bank blog, November 2022. *Readable, short.* The ECB's argument, published at the bottom of the 2022 bear market, that Bitcoin was on "the road to irrelevance." The price then quadrupled. Read it as a specimen of institutional skepticism and a reminder that timing is hard for everyone.

**[Banking in the shadow of Bitcoin? The institutional adoption of cryptocurrencies](https://www.bis.org/publ/work1013.htm)** — Raphael Auer, Marc Farag, Ulf Lewrick, Lovrenc Orazem and Markus Zoss, BIS Working Paper 1013, 2022. *Readable.* Finds banks hold almost no crypto and most activity sits in lightly regulated exchanges, and characterizes the result as a shadow financial system.

**[The Financial Stability Implications of Digital Assets](https://www.newyorkfed.org/research/staff_reports/sr1034)** — Pablo Azar, Garth Baughman, Francesca Carapella et al., Federal Reserve Bank of New York Staff Report 1034, 2022. *Readable.* Maps how crypto risk could transmit to the traditional system (stablecoin runs, leverage, exchange failures) months before FTX demonstrated it.

**[BIS Annual Economic Report 2022, Chapter III: The future monetary system](https://www.bis.org/publ/arpdf/ar2022e3.htm)** — Bank for International Settlements, 2022. *Readable.* The central-bank case that crypto's fragmentation, congestion and lack of a nominal anchor are structural, and that the right future is tokenized central-bank money. The industry's most important institutional opponent, stating its position plainly.

## How to find more

- **SSRN** ([papers.ssrn.com](https://papers.ssrn.com/sol3/DisplayAbstractSearch.cfm)) hosts nearly every finance working paper before publication. Search the exact title, or the author (Makarov, Schoar, Griffin, Shams, Cong, Tsyvinski, Auer) — the crypto literature is concentrated in a few dozen people. Sort by "downloads" to find what practitioners read.
- **NBER** ([nber.org/papers](https://www.nber.org/papers?page=1&perPage=50&q=cryptocurrency)) is the prestige working-paper series; new crypto papers appear here a year or two before the journal version. Free PDFs.
- **arXiv q-fin** ([arxiv.org/list/q-fin/recent](https://arxiv.org/list/q-fin/recent)) and the cs.CR (cryptography) list are where the technical and computer-science papers appear; quality varies more than on SSRN.
- **Google Scholar** ([scholar.google.com](https://scholar.google.com/)) — search a paper's title and click "Cited by" to find the replies; for Griffin and Shams, Budish and Foley et al., the rebuttals are as instructive as the originals.
- **Central-bank research**: the BIS working papers, Fed [FEDS Notes](https://www.federalreserve.gov/econres/notes/feds-notes/default.htm), NY Fed [Liberty Street Economics](https://libertystreeteconomics.newyorkfed.org/), and the [FSB's crypto framework](https://www.fsb.org/2023/07/fsb-global-regulatory-framework-for-crypto-asset-activities/) are free, empirical and institutionally skeptical.
- Reading tip: for any empirical paper, read the abstract, the introduction's last two paragraphs (the contribution), the main table, and the conclusion. That is 20 minutes and gets you 80% of the value.

## Key takeaways

- The best peer-reviewed evidence says crypto returns are a distinct factor, not a stock or gold proxy (Liu and Tsyvinski), which is the honest basis for a small diversifying allocation, if any.
- Ownership is highly concentrated (Makarov and Schoar), retail tends to buy after rallies (BIS), and stablecoins have all broken their pegs at some point (BIS Papers 141); the data undercuts the "decentralized, democratized money" story even if the technology works.
- Griffin and Shams on Tether and Liu, Makarov and Schoar on Terra are the two papers to read before trusting any stablecoin.
- Budish's security-cost argument is the strongest economic critique of proof-of-work; know it and know the replies.
- Every paper here is free in some version; use SSRN, NBER and Google Scholar's "Cited by" to follow the argument forward.
