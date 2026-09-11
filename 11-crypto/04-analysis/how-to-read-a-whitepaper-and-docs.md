# How to Read a Whitepaper and Project Docs

**In one sentence:** A whitepaper is a project's opening argument, not its proof, so read it the way a skeptical reviewer would: for a clearly stated problem, a mechanism that actually solves it, honest tokenomics, and a named team whose GitHub and governance history back up the claims.

## What a whitepaper is (and isn't)

A whitepaper is the founding document of a crypto project. In the best cases it is a technical paper that explains a problem, proposes a mechanism, and lets you check the reasoning. In the worst cases it is a marketing brochure with equations pasted in for credibility. The word "whitepaper" carries prestige because Bitcoin's nine-page paper launched a trillion-dollar asset. That prestige is exactly why it gets abused.

The two benchmark documents are worth reading in full before you read anything else:

- **Bitcoin (Satoshi Nakamoto, 2008):** nine pages. States a problem (double-spending without a trusted third party), proposes a mechanism (proof-of-work chain of timestamps), analyzes the attacker's odds mathematically, and stops. There is no token sale, no roadmap, no team page, no "partners" section.
- **Ethereum (Vitalik Buterin, 2013–14):** longer, and it does describe the ETH issuance for the crowdsale, but the bulk of the document is about the state machine, gas, and what applications become possible. Its predictions were falsifiable and many came true (tokens, exchanges, DAOs) while others did not (prediction markets and identity never became dominant).

Neither paper spends a paragraph on how rich early buyers will get. Use that as your baseline.

## What a serious whitepaper should contain

| Section | What good looks like | What weak looks like |
|---|---|---|
| Problem statement | A specific, verifiable pain point with evidence | "The $X trillion industry is broken" |
| Mechanism | Explains *how* it works, including trade-offs and attack surface | Describes *what* it does with buzzwords ("AI-powered, quantum-resistant, modular") |
| Why a token is needed | Token performs a function no other asset could (security bond, fee unit, governance with teeth) | Token exists so there is something to sell |
| Tokenomics | Max/initial supply, allocation by bucket with percentages, vesting cliffs and durations, emission curve, who controls minting | "Community: 40%" with no schedule; "details to follow" |
| Security and threat model | Named assumptions, what breaks if they fail, audit plan | Silence, or "our contracts are 100% secure" |
| Team | Named people with checkable histories | Anonymous or pseudonymous with no track record |
| Roadmap | Milestones tied to technical deliverables | Milestones that are all marketing ("listing on tier-1 exchange") |
| References | Cites prior work, including competitors | Cites nothing, or only its own blog |

## Red flags, roughly ordered by seriousness

1. **Vague or missing tokenomics.** If the paper doesn't tell you what fraction of supply insiders hold and when it unlocks, assume the answer is "a lot" and "soon." See `tokenomics-analysis.md`.
2. **No named team.** Anonymity is not automatically disqualifying (Bitcoin), but an anonymous team plus a token sale plus a treasury controlled by a multisig is the standard profile of a rug pull. See `evaluating-teams-vcs-and-backers.md`.
3. **Buzzword density.** Count how many of these appear per page: AI, RWA, modular, restaking, intent, quantum, zero-knowledge, sovereign, omnichain. A real ZK project will explain its proof system; a fake one will just say "ZK."
4. **Guaranteed returns or fixed APY** anywhere in the document. Yield in crypto comes from someone paying it; if the paper can't say who, it's coming from new buyers.
5. **Plagiarism.** Paste a few distinctive sentences into a search engine. Several 2017–18 ICO whitepapers were copied nearly verbatim from other projects, and it still happens.
6. **Partnership claims without links.** "Partnered with Amazon" usually means "uses AWS."
7. **Roadmap that is all listings and marketing.** Technical projects list technical milestones.
8. **Token utility that is circular.** "The token is used to pay for services in the ecosystem" is only meaningful if the services exist and people would want them without the token.

## Beyond the paper: docs, GitHub, audits, governance

The whitepaper is a snapshot from launch. What matters now lives elsewhere.

**Documentation.** Mature projects have living docs (usually on GitBook, Docusaurus, or a docs subdomain) that explain how to use the protocol, what the contracts do, and what the admin controls are. Compare the docs to the whitepaper: did the mechanism actually ship as described, or did it quietly change?

**GitHub activity.** Open the organization's repositories and look at:

- Commit frequency over the last 90 days (not lifetime, which can be gamed with early bursts).
- Number of distinct contributors. One or two active developers on a "billion-dollar" protocol is a concentration risk.
- Whether commits are substantive or cosmetic (README edits and dependency bumps count for little).
- Whether the core repo is a fork of something else with minimal changes. Many "new L1s" are forks of Geth, Cosmos SDK, or Optimism's stack; that's fine if disclosed, alarming if hidden.
- Issues and pull requests: do outsiders open issues, and does the team respond?

Tools like Artemis, Electric Capital's Developer Report, and GitHub's own insights tab make this faster.

**Audits.** Look for the audit report itself, not the badge. Note who audited (Trail of Bits, OpenZeppelin, Spearbit, Cantina, ChainSecurity, Sigma Prime, Zellic and a handful of others have strong reputations), when, and whether the audited commit matches what's deployed. An audit from 2022 of v1 says nothing about v3 deployed last month. See `smart-contract-and-protocol-risk-assessment.md`.

**Governance.** Read the governance forum (usually Discourse) and the on-chain votes on Tally, Snapshot, or the project's own portal. Questions to answer: How many addresses actually vote? Does one entity (the foundation, a VC, an exchange) control the outcome? Have proposals been passed that benefited insiders at holders' expense? A DAO with 20 active voters is not decentralized, whatever the paper claims.

## Worked example: reading two papers side by side

Take a hypothetical "decentralized AI compute" project launched in 2025 and compare it to Ethereum's paper on three questions.

| Question | Ethereum whitepaper | Hypothetical AI-compute project |
|---|---|---|
| Why does this need a token? | ETH is the unit for gas, which prices computation and prevents spam and infinite loops. Without a scarce resource the halting problem makes the network attackable. | "Providers are rewarded in $TOKEN and users pay in $TOKEN." No explanation of why USDC wouldn't work. |
| What's the mechanism? | Full description of accounts, state transitions, gas, mining (later staking). | "Our proprietary orchestration layer matches GPU supply and demand." |
| What's the supply plan? | Presale amount, 0.099x annual issuance to miners, no VC allocation. | "Team 20%, Investors 25%, Ecosystem 30%, Community 25%," no vesting stated. |

The second project isn't necessarily fraudulent, but the paper alone gives you no way to tell. Your next step should be the GitHub, the unlock schedule, and the team's history, not the price chart.

## How to actually do it

1. **Read the paper in one sitting, before looking at the price.** Price anchors judgment.
2. **Write down the problem in one sentence.** If you can't, the paper hasn't told you.
3. **Write down why the token must exist.** If your answer is "so they could raise money," that's the answer.
4. **Extract the supply table** into a spreadsheet: buckets, percentages, cliffs, vesting length. Note anything missing.
5. **Open the GitHub** and check 90-day commits, contributor count, and fork lineage.
6. **Find the audit reports** and verify the audited commit hash against the deployed contract on the block explorer.
7. **Read the last 10 governance proposals** and who voted on them.
8. **Search for the team members** on LinkedIn, X, and prior project pages. Look for people who left prior projects right after token launches.
9. **Search the paper's distinctive sentences** for plagiarism.
10. **Rank it.** Write a one-paragraph thesis and a one-paragraph "how this fails." If you can't write the second paragraph, you haven't finished.

## Key takeaways

- Bitcoin's and Ethereum's whitepapers are the benchmark: problem, mechanism, trade-offs, and nothing about getting rich.
- A token needs a reason to exist beyond fundraising; the paper should be able to state it.
- Missing or vague tokenomics is the single most predictive red flag.
- The whitepaper is a launch-day snapshot; the docs, GitHub, audits, and governance record tell you what the project became.
- Check that the audit matches the deployed code and that the mechanism in the docs matches the mechanism in the paper.
- Buzzword density is inversely correlated with explanatory content.
- Always write the "how this fails" paragraph.

## Sources

- [Bitcoin: A Peer-to-Peer Electronic Cash System (bitcoin.org)](https://bitcoin.org/bitcoin.pdf)
- [Ethereum Whitepaper (ethereum.org)](https://ethereum.org/en/whitepaper/)
- [Electric Capital Developer Report](https://www.developerreport.com/)
- [Messari Research](https://messari.io/research)
- [Tally: on-chain governance explorer](https://www.tally.xyz/)
- [Snapshot: off-chain governance voting](https://snapshot.org/)
- [Binance Research: Low Float & High FDV (May 2024)](https://public.bnbstatic.com/static/files/research/low-float-and-high-fdv-how-did-we-get-here.pdf)
