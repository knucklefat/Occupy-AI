# How Blockchains Work

**In one sentence:** A blockchain is a shared ledger that thousands of strangers keep identical copies of, where new entries are added in batches ("blocks") that are chained together with cryptographic fingerprints, and where the right to add the next batch is decided by a costly competition (proof of work) or a staked-deposit lottery (proof of stake) rather than by a bank or company.

## Start with the ledger

Every financial system is a ledger: a list of who owns what. Your bank keeps one. Visa keeps one. The DTCC keeps one for U.S. stocks. In each case, a single trusted institution holds the master copy and you trust it not to lose it, alter it, or freeze you out.

A blockchain is a ledger with no master copy. Thousands of computers ("nodes") around the world each hold a full copy, and they use a set of rules (the "protocol") to agree on what gets added. The point of the whole design is to answer one question: how do strangers who do not trust each other agree on a single version of history without a referee?

## Blocks, hashes, and the chain

Transactions are not written to the ledger one at a time. They are gathered into batches called **blocks**. Bitcoin produces a block roughly every 10 minutes; Ethereum every 12 seconds; Solana every 400 milliseconds.

Each block includes a **hash** of the previous block. A hash is a cryptographic fingerprint: you feed any data into a hash function (Bitcoin uses SHA-256) and it produces a fixed-length string of characters. Change one character of the input and the output changes completely. Because each block contains the fingerprint of the one before it, altering an old transaction would change that block's hash, which would break the fingerprint stored in the next block, and so on all the way to the present. Rewriting history means redoing every block after it, which is what makes the chain "immutable" in practice.

## Keys, addresses, and signatures

There are no accounts with usernames and passwords. Ownership is controlled by **public-key cryptography**:

- A **private key** is a very large random number that only you know. Whoever holds it can spend the coins it controls. There is no password reset.
- A **public key** is derived mathematically from the private key. Deriving it is easy; going backwards is computationally impossible.
- An **address** is a shortened, encoded version of the public key. It is what you give someone so they can pay you.

When you send coins, your wallet software uses the private key to produce a **digital signature** over the transaction. Anyone can verify with your public key that the signature is genuine, but nobody can forge it. This is why "not your keys, not your coins" is a literal statement: whoever holds the key owns the asset.

## Consensus: proof of work vs. proof of stake

The hard problem is deciding who gets to add the next block. If anyone could do it freely, an attacker could add fraudulent blocks or spend the same coin twice (the "double-spend" problem that stumped digital-cash projects for decades before Bitcoin).

**Proof of work (PoW)** — used by Bitcoin. Computers called **miners** race to find a number that, combined with the block's contents, produces a hash below a target value. The only way to find it is brute-force guessing, trillions of times per second. The winner broadcasts the block and collects a reward (newly minted coins plus transaction fees). The network automatically adjusts the difficulty every 2,016 blocks so that blocks keep arriving about every 10 minutes no matter how much computing power joins. To rewrite history, an attacker would need more computing power than the rest of the network combined (a "51% attack"), which for Bitcoin would cost billions of dollars in hardware and electricity. Security is bought with energy.

**Proof of stake (PoS)** — used by Ethereum since September 2022, plus Solana, Cardano, and most newer chains. Instead of burning electricity, participants called **validators** lock up ("stake") the chain's own coins as a deposit (32 ETH for a solo Ethereum validator). The protocol picks validators to propose and attest to blocks, roughly in proportion to their stake. Honest work earns rewards (Ethereum validators currently earn roughly 2.6–3.3% a year, as of mid-2026). Dishonest behavior, such as signing two conflicting blocks, gets the deposit destroyed ("slashing"). Security is bought with capital at risk rather than energy.

| | Proof of work | Proof of stake |
|---|---|---|
| Who adds blocks | Miners with specialized hardware | Validators with locked coins |
| Cost of attack | Buy/run more hash power than the network | Acquire and risk a majority of staked coins |
| Energy use | Very high (Bitcoin ~0.5% of world electricity, estimates vary) | Negligible (~99.9% less than PoW) |
| Reward source | New coins + fees | New coins + fees, paid to stakers |
| Main critique | Energy, hardware centralization in big farms | "Rich get richer," staking pools and exchanges concentrate control |
| Examples | Bitcoin, Litecoin, Dogecoin | Ethereum, Solana, Cardano, Avalanche |

## Nodes, miners, validators: who does what

- **Full nodes** store the whole ledger and independently check every transaction and block against the rules. They do not need to mine or stake. Anyone can run one on a home computer (Bitcoin's full history is roughly 700 GB as of 2026). Nodes are the network's enforcement layer: a block that breaks the rules is rejected no matter how much work or stake backs it.
- **Miners / validators** produce blocks and are paid for it.
- **Developers** propose rule changes, but they cannot force them. Nodes have to voluntarily upgrade.

## Why "decentralized" matters, and what it costs

The benefit of having no single operator is **censorship resistance** and **credible neutrality**: no company can freeze your balance, reverse your payment, change the money supply, or shut the network down. Bitcoin has run continuously since January 2009 with no CEO and no headquarters.

The costs are real and are the basis of most serious critiques:

1. **Throughput.** Every node processes every transaction, so the network is only as fast as a modest computer. Bitcoin handles roughly 7 transactions per second; Ethereum's base layer around 15–20. Visa averages thousands. Scaling is pushed to "Layer 2" networks built on top.
2. **No customer service.** Lost keys are lost forever. Sending to the wrong address cannot be undone. Chainalysis has estimated that roughly 20% of all bitcoin may be permanently lost.
3. **Expense.** Proof-of-work security consumes as much electricity as a mid-sized country. Proof-of-stake avoids this but pays validators with new coins, which dilutes holders.
4. **Decentralization is a spectrum, not a switch.** In practice a handful of mining pools produce most Bitcoin blocks, Lido and a few exchanges control a large share of staked ETH, and Solana runs on about 800 validators (as of early 2026). Skeptics argue many "decentralized" networks are functionally run by a small group.

## Finality: when is a transaction really done?

In proof-of-work chains, a transaction is never *mathematically* final; it just becomes exponentially harder to reverse as more blocks pile on top. The convention is to wait for six Bitcoin confirmations (about an hour) for large sums. Ethereum's proof of stake adds explicit **finality**: once two-thirds of validators have attested to a block through two "epochs" (about 13 minutes), reverting it would require destroying at least one-third of all staked ETH. Solana and some newer chains claim finality in seconds, with tradeoffs in validator requirements.

For an investor this matters when moving money between exchanges: a deposit is not yours to trade until the receiving platform considers it final.

## Forks: when the rules change

A **fork** is a change to the protocol rules.

- A **soft fork** tightens the rules; old software still accepts new blocks. Bitcoin's SegWit (2017) and Taproot (2021) upgrades were soft forks.
- A **hard fork** loosens or changes the rules so that old software rejects new blocks. If not everyone upgrades, the chain permanently splits into two coins. Bitcoin Cash split from Bitcoin in August 2017 over block size. Ethereum Classic is the original Ethereum chain that refused to reverse the 2016 DAO hack.

Forks are how blockchains are governed, and they are messy. There is no board vote; there is a negotiation among developers, miners or validators, exchanges, and users, and if it fails you get two competing assets. Holders of the original coin typically receive both.

## Key takeaways

- A blockchain is a shared ledger where blocks of transactions are linked by cryptographic hashes, making past entries practically impossible to alter.
- Ownership is a private key. Whoever controls the key controls the asset; there is no recovery process.
- Proof of work buys security with electricity and hardware; proof of stake buys it with locked capital that can be destroyed for misbehavior.
- Full nodes, not miners, enforce the rules. Mining and validating are paid jobs; running a node is a voluntary check.
- Decentralization delivers censorship resistance at the cost of speed, energy or dilution, and zero customer service. It is a spectrum, and many chains are less decentralized than advertised.
- "Finality" is probabilistic on Bitcoin and explicit on Ethereum; wait for confirmations before treating a transfer as done.
- Forks are how rule changes happen; contested ones split the coin in two.

## Sources

- [Bitcoin: A Peer-to-Peer Electronic Cash System (Nakamoto, 2008)](https://bitcoin.org/bitcoin.pdf)
- [Bitcoin.org: How does Bitcoin work?](https://bitcoin.org/en/how-it-works)
- [Ethereum.org: Proof-of-stake (PoS)](https://ethereum.org/en/developers/docs/consensus-mechanisms/pos/)
- [Ethereum.org: Proof-of-work (PoW)](https://ethereum.org/en/developers/docs/consensus-mechanisms/pow/)
- [Ethereum.org: Nodes and clients](https://ethereum.org/en/developers/docs/nodes-and-clients/)
- [Investopedia: Blockchain Facts](https://www.investopedia.com/terms/b/blockchain.asp)
- [Cambridge Bitcoin Electricity Consumption Index](https://ccaf.io/cbnsi/cbeci)
- [Datawallet: Ethereum Staking Statistics (2026)](https://www.datawallet.com/crypto/ethereum-staking-statistics-and-trends)
- [CoinLaw: Solana vs Ethereum Statistics 2026](https://coinlaw.io/solana-vs-ethereum-statistics/)
