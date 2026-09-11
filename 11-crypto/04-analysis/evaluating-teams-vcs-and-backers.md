# Evaluating Teams, VCs, and Backers

**In one sentence:** In crypto, the people behind a token and the terms they bought in on tell you who will be selling to you and when, so read the cap table and the vesting schedule as carefully as you'd read a prospectus, and treat a famous backer's logo as a marketing asset rather than a guarantee.

## Doxxed versus anonymous teams

"Doxxed" means the team's real identities are public and checkable; "anonymous" or "pseudonymous" means they aren't. Crypto's founding asset was built by a pseudonym, and some excellent projects have followed suit, so anonymity is not disqualifying by itself. What matters is whether the team has *something to lose* and whether their claims can be checked.

| Signal | Why it matters | How to check |
|---|---|---|
| Real names with verifiable histories | Reputational cost to fraud; prior shipped work you can assess | LinkedIn, GitHub, conference talks, prior company filings |
| Prior crypto projects and how they ended | Serial launchers whose previous tokens went to zero after unlocks are a pattern | Search each founder's name with "token" and "unlock"; check CoinGecko for dead projects |
| Pseudonymous but with a long public track record | Reputation attaches to the handle (some DeFi builders are famous under pseudonyms) | Years of GitHub commits, forum posts, audited contracts under the same name |
| Anonymous, new handle, token sale, admin keys | The full rug-pull profile | If all four are present, the base rate of loss is very high |
| Team on advisory boards of a dozen other projects | Attention is split; "advisor" allocations are often just free tokens | Count the projects on their bio |
| Legal structure disclosed (foundation jurisdiction, operating company) | Tells you who can be sued and where | Docs, terms of service, foundation website |

Sanctions and enforcement history matter more than they used to. The SEC's 2023–24 actions against exchanges and issuers, and the 2025 pivot toward clearer rules, mean a team's regulatory posture is a business risk you can partly assess from their disclosures.

## The venture-capital layer

Most tokens launched since 2021 were preceded by private rounds. Venture firms (a16z crypto, Paradigm, Multicoin, Pantera, Polychain, Dragonfly, and many smaller ones) bought tokens or token warrants at valuations far below the eventual public price, with vesting terms that typically included a 12-month cliff and 24–36 months of linear release. Binance Research counted more than $91 billion of venture funding into crypto from 2017 to early 2024 and estimated around $155 billion of tokens scheduled to unlock from 2024 to 2030.

**Why this creates a structural headwind.** A fund that bought at a $200 million valuation and sees the token list at $5 billion FDV has a 25× paper gain. Its limited partners expect distributions. Whatever its public statements, the fund's incentive after the cliff is to sell into any liquidity. Tokens launched in early 2024 averaged an MC/FDV of about 12%, meaning almost 90% of supply, much of it held by investors and teams at low cost, was still to arrive.

**What unlock studies show.** Analyses of hundreds of unlock events (Keyrock's 2024 study is the most cited) found that the large majority of unlocks were followed by negative price pressure, that the pressure often began weeks *before* the unlock date as holders hedged or front-ran, and that team and investor unlocks were worse than ecosystem or community unlocks. The intuition: the market prices in a seller it can see coming. A scheduled unlock is not always a sale (recipients sometimes hold or stake), so check the destination wallets after the date.

## "VC coins" versus "community coins"

The 2024–25 cycle produced a loud argument between two launch models.

**VC coin**: private rounds at rising valuations, high FDV at listing, low float, large team and investor allocations, and often a points program that turns users into unpaid marketers before a partial airdrop. Pros: funded development, professional teams, exchange relationships. Cons: the public buys the top of a valuation ladder that insiders climbed at a fraction of the price, and the unlock stream lasts for years.

**Community coin** or "fair launch": no or minimal private allocation, most supply distributed to users at launch or mined over time, sometimes no team allocation at all. Bitcoin is the archetype; Hyperliquid's 2024 launch (about 31% to users at genesis, no venture round, contributors vesting) revived the model at scale and was the counter-example everyone cited. Memecoins are the degenerate form: 100% float from day one, no vesting, and no product, which "solves" dilution by having nothing else.

Neither model is inherently better. What matters is the ratio between what insiders paid and what you're paying, and how long they have to wait to sell. A VC coin with 18 months of vesting and a foundation that publishes its wallets can be fine; a "community coin" whose community allocation went to 40 sybil wallets controlled by the team is worse than any venture deal.

## How to read a cap table

Projects rarely publish a formal cap table, but you can reconstruct one from the tokenomics section of the docs, the vesting contracts on-chain, and funding announcements (Crunchbase, Messari's fundraising database, and RootData track rounds).

Build a table with these columns and fill in what you can:

| Bucket | % of max supply | Price paid (if any) | Cliff | Vesting length | Fully unlocked by | Wallets identified? |
|---|---|---|---|---|---|---|
| Seed investors | | | | | | |
| Series A / strategic | | | | | | |
| Team and advisors | | | | | | |
| Foundation / treasury | | | | | | |
| Ecosystem / grants | | | | | | |
| Airdrop / community | | | | | | |
| Public sale / liquidity | | | | | | |

Then compute three numbers:

1. **Insider share** = investors + team + advisors. Over 40% is heavy; some 2021–24 launches exceeded 50%.
2. **Implied insider multiple** = current FDV ÷ last private-round valuation. Above 10× means the insiders' incentive to sell is overwhelming.
3. **12-month supply overhang** = tokens unlocking in the next year ÷ current circulating supply. Above 50% and price must absorb a supply increase larger than most tokens' demand growth.

Worked example. A token lists at $4 billion FDV with 15% circulating. Seed investors paid an implied $80 million valuation (50×), Series A paid $400 million (10×), and the team's allocation cost nothing. Investors and team hold 45% of max supply; their cliffs expire in month 12 and vest over 24 months after that. From month 12, roughly 1.9% of max supply unlocks monthly, which is 12.5% of the *current* float every month. Unless demand grows 12.5% a month, price falls. This isn't cynicism about the founders; it's arithmetic about the incentives.

## Foundation treasuries

Most L1s and many protocols park a large allocation (often 20–40%) in a foundation, usually a Swiss, Cayman, or Panamanian entity. Questions to answer:

- **Are the wallets published?** Arkham and Nansen label many; the best foundations publish addresses and quarterly reports (the Ethereum Foundation and Optimism's Collective are reasonable benchmarks).
- **How is it spent?** Grants that fund builders are good; "ecosystem incentives" that are really liquidity mining or market-maker loans are supply hitting the market under a friendlier label.
- **Market-maker arrangements.** Foundations routinely lend tokens to market makers with call options attached. If the price rises, the market maker exercises and keeps the tokens; these loans function as hidden supply. Disclosure is rare; the 2024–25 disputes over market-maker terms made this visible.
- **Is the foundation selling?** Watch its wallets on-chain. A foundation that sells into every rally is a permanent seller.
- **Who controls it?** If the founders are also the foundation's board, "decentralized" is decorative.

## Governance capture

A token's governance is only as decentralized as its voting distribution. Common capture patterns:

- A single VC or the foundation holds enough votes to pass anything (many DAOs have effective quorums that one wallet can meet).
- Delegates who are paid by the foundation vote with the foundation.
- Proposals structured so token holders vote to send treasury funds to entities connected to the team.
- Votes held on Snapshot (off-chain, non-binding) with execution controlled by a multisig, so the vote is advisory.

Read the last dozen proposals on Tally or the governance forum and count how many distinct entities decided them. See `how-to-read-a-whitepaper-and-docs.md`.

## Exit-liquidity patterns

"Exit liquidity" is the crypto term for buyers who provide the market into which insiders sell. The recurring patterns:

1. **The listing pump.** Heavy marketing and exchange listings timed to the token generation event, when float is smallest and price is easiest to move. Insiders can't sell yet, but the high print sets the anchor for later.
2. **The pre-unlock rally.** Announcements, partnerships, and roadmap updates cluster in the weeks before large unlocks. Check the unlock calendar whenever news flow suddenly improves.
3. **The OTC bypass.** Insiders sell locked tokens at a discount through over-the-counter deals with hedging, so the on-chain unlock date understates when selling began. Perpetual futures let them hedge before the cliff, which is why price often falls into an unlock.
4. **The treasury "diversification."** A foundation announces it is converting a portion of its tokens to stablecoins "for runway." Legitimate, and also selling.
5. **The relaunch.** Failed projects reappear under a new name with a new token, and airdrop the old holders a sliver to buy goodwill.
6. **Celebrity and influencer tokens.** Almost uniformly a transfer from fans to promoters; the 2024–25 memecoin launches associated with public figures collapsed within days or weeks in nearly every case.

## How to actually do it

1. Identify every founder and core contributor. For each, find prior projects and what happened to their tokens.
2. Find every funding round (Messari, RootData, Crunchbase) with valuation and date. Compute the implied multiple to today's FDV.
3. Rebuild the cap table from the docs and verify the vesting contracts on the block explorer.
4. Compute insider share, insider multiple, and 12-month overhang.
5. Locate foundation and team wallets (Arkham/Nansen) and check whether they've been net sellers.
6. Read the last 10–12 governance votes and count decision-makers.
7. Put the next three unlock dates in your calendar and re-check wallet behavior after each.
8. Ask the one question that summarizes everything: *who sells to me, at what multiple, and when?*

## Key takeaways

- Anonymity isn't disqualifying; anonymity plus a token sale plus admin keys plus no track record is.
- Venture backing funds development and also creates a multi-year seller with a 10–50× cost advantage.
- Unlocks are usually followed by weakness, and the weakness often starts before the date because insiders hedge.
- "VC coin" versus "community coin" is less important than insider share, insider multiple, and overhang.
- Foundations are supply; find their wallets and watch them.
- Governance is captured when a handful of entities decide every vote; count them.
- Exit-liquidity patterns (listing pumps, pre-unlock news, treasury "diversification") are predictable once you know the calendar.

## Sources

- [Binance Research: Low Float & High FDV: How Did We Get Here? (May 2024)](https://public.bnbstatic.com/static/files/research/low-float-and-high-fdv-how-did-we-get-here.pdf)
- [Binance Research estimates $155B of unlocks by 2030 (Crypto Briefing)](https://cryptobriefing.com/binance-research-token-unlocks-2030/)
- [Tokenomist: unlock calendar and research](https://tokenomist.ai/research)
- [Messari: fundraising and asset research](https://messari.io/research)
- [RootData: crypto fundraising database](https://www.rootdata.com/)
- [Arkham Intelligence: entity labeling](https://www.arkhamintelligence.com/)
- [Tally: on-chain governance](https://www.tally.xyz/)
- [Why HYPE is different: inside Hyperliquid's buyback and no-VC launch (crypto.news)](https://crypto.news/why-hype-is-different-inside-hyperliquids-buyback/)
