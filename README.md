# Syllabus outline ZkSync Summer Bootcamp:

## Goal:

By the end of the boot camp, all the boot campers should get a clear overview of Zero-knowledge and ZK math, and they should be able to write ZK Circuits & create ZK applications on their own, together with having a good overview of the Blockchain ecosystem.

## Timings: 

- Kickoff: 6th or 7th of May 2024, offline.

- Number of Weeks: 8 Week(s) + 1 Week.

- Number of days a week: 
    - Content for five days, up to the boot camp.
    - 2 online sessions a week.
    - 1 online session will be on giving an overview of the week's syllabus. (think of it as video lectures in MOOC).
    - The other session could be doubt-solving or an overview session.

## Content:

- General Recommendation: Learn Rust from Day 0. 
- zustlings
- Reading?

// BLOCKCHAIN OVERVIEW


### Week 1: Intro to L1 "Primitives" 
- General intro to Blockchain
  - Decentralised Systems
- Blockchain Timeline
- Layer1 Theory
- Blockchain Components
- Chains Overview
  - How do [[ Ethereum & Solana ]] work at the consensus and execution layer?
  - Trade-offs // "Trade spaces" Design decisions made by protocols to prioritize different things. Ethereum vs Solana etc.
  - Modular vs Monolithic Execution (<< Could also put this in Scalability section>>)
  - Alt VMs (touch on briefly)
  

Additional content(only for those interested): Docs of Alchemy / Alchemy University to build a DApp.

* [Bootcamp:Learn Blockchain, Solidity and Full Stack JavaScript Development:](https://www.freecodecamp.org/news/learn-blockchain-solidity-full-stack-javascript-development/){target=_blank} A 32 hour long comprehensive Blockchain Development Bootcamp by Patrick Collins
* [Course: CryptoZombies](https://cryptozombies.io/){target=_blank} One of the most well-known introductions to Solidity
* [Course: Ethernaut (OpenZeppelin)](https://ethernaut.openzeppelin.com/){target=_blank} An excellent in-browser "game" teaching Solidity from a security perspective.
* [Course: Intro to Solidity (Chainshot)](https://www.chainshot.com/learn/solidity){target=_blank} Chainshot uses a very cool interactive platform to teach Solidity
* [Wiki: Solidity by Example](https://www.solidity-by-example.org){target=_blank} A bunch of great examples of Solidity, including excellent design patterns, hacks and security tips.
* [Wiki: Use Web3](https://useweb3.xyz/){target=_blank} Another good collection of learning resources
* [Article: Test Driven Introduction to Solidity](https://michalzalecki.com/ethereum-test-driven-introduction-to-solidity/){target=_blank} From an older pragma version of Solidity, but might be interesting to check out! Repo accompanying the article [here.](https://github.com/MichalZalecki/tdd-solidity-intro){target=_blank}
* [Thread: What Does Ethereum Development Look Like Today?](https://twitter.com/smpalladino/status/1421901085279756300){target=_blank} Santiago Palladino, who wrote [Ethereum for Web Developers,](https://www.apress.com/gp/book/9781484252772){target=_blank} updates parts of his book for the current Ethereum ecosystem.
* [Article: Learn X in Y Minutes (Solidity)](https://learnxinyminutes.com/docs/solidity/){target=_blank} A bit long and rough, but a comprehensive overview of learning Solidity

### Week 2: Protocol Development Deep-Dive

This week acts as a starter to Rust for everyone and to make everyone code in Rust at a basic level. 

- Development on Ethereum(probably in Rust/GO 😉).
  - Protocol-level Development (P2P, Transaction Processing, "Node / Client Development") 
  - [[ Perhaps you'd want to check out the "Consensus" section from [this course](https://github.com/ConsenSys-Academy/Blockchain-Developer-Bootcamp/tree/1c47761d403026d55f54b36f62e33b1127e8da61/docs/S01-fundamentals) I built at Consensys]]

Additional Content (only for those interested):

- [Bitcoin White Paper Exercises](https://github.com/cooganb/bitcoin-whitepaper-exercises){target=_blank} These are a series of exercises, built by [Kyle Simpson,](https://github.com/getify){target=_blank} for understanding some of the concepts outlined in the Bitcoin white paper. These are not easy, but if you really would like to understand these fundamentals as they apply to blockchains, this is a great place to start.
 - [CryptoHack](https://cryptohack.org/){target=_blank} "A fun free platform for learning modern cryptography"
 - [CryptoPals](https://cryptopals.com/){target=_blank} This is *very* advanced and intense, but real to-the-metal applied cryptography! I am putting this link in here and it scares me.

### Week 3: Scalability

This week gives an overview of most of the essential concepts in web3.

- Scalability Introduction: Ethereum / Bitcion / etc as L1 (Lectures #2 and #3 in zkSync zkEVM Bootcamp)
  - Scalability Introduction
  - Approaches to Scalability
  - Layer 1 Solutions
  - Off-chain Scaling
  - Bridges / Sidechains versus layer 2
- Typical Rollup Architecture
  - L2 Mental Model
  - Sequencers
  - Mix and Match for: OP Rollups, ZK Rollups, Validiums, "L3s" or "Hyperchains"
  
  
- Rollups in more detail
- Introduction to zkEVM solutions

### Week 4: The Road Forward for Blockchain and/or Use Case
- Ethereum's Rollup-centric roadmap and alt narratives...
- DA Layers, Alt VMs(MoveVM, WasmVM, Solana VM)
- Data Availability / Protodanksharding
- Decentralised Identities, Bridges(ZK and non ZK bridges).


## Week 5: What is ZK? && Math Primitives

Intro to ZK (high level)
* ZK as kompression
* ZK as privacy

### Math primitives

[[ Manoj, feel free to put your preferred math topics here, this is borrowed from Lecture #4 of zkSync zkEVM Bootcamp --Coogan]]
- Cryptography review
- Mathematical terminology
- Modular arithmetic
- Group and Field theory
- Introduction to polynomials
- Complexity theory
- Introduction to Zero Knowledge
- Proofs

## Week 6: What are zkEVMs?

The most crucial part of the boot camp. Those who complete this can understand and write circuits and build Zk Dapps independently.

(Lectures 11-13 from zkEVM Bootcamp)
- Overview
- Universal Circuits / Circuit Compiler
- Proving Systems


Additional content: Build circuits using Rust

## Week 7-8: SNARKs, STARKs 
(Lecture #16, 17 in zkEVM Bootcamp)

### SNARK Implementation
- SNARK process overview
- Polynomial Checking
- Scroll example
- Fiat Shamir heuristic
- Comparison of schemes
- Verification cost

- Circom, Gnark

### STARK Implementation
- Reed Solomon codewords
- Computational integrity
- Stark arithmetisation
- FRI background


(Not sure what to do with these:)
### Libraries / Abstractions
- Circom, Gnark
- DSLs

### Advanced Topics
- Folding schemes
- Formal Verification
- 

## Extra Week:
- More on ZK Math
- zkML
- ZK-DSL(s)




####################################################################################


ORIGINAL DRAFT FOR REFERENCE:


## Implementation



// TODO: Distinguish these a bit

### Week 4: Intro to ZK

- What is ZK?





- What is a SNARK & STARK? 
- Types of SNARKs & STARKS.
- Fields & Groups.
- Circom/Gnark.

### Week 5- Week 7: Rust + ZK  --> Circuit writing in rust.

The most crucial part of the boot camp. Those who complete this can understand and write circuits and build Zk Dapps independently.



SNARKs
- Groth 16, Plonk
- Starks, AIR, Plonkish Systems
- Plonky2, Halo2, KGZ, NOVA (folding scheme / IVC), IPA, Pedersen commitments...

STARKs
- Lookups, Range checks
- DEEP FRI, Recursion
- FFT, NTT, Fiat Shamir, Lagrange Basis, Low degree extensions.

## Advanced Topics
- Libraries -> Ark works/lambda works (Winterfell, bellman)
- Folding Schemes
IVC, NOVA
- ZK ML
- "Programmable Encryption"

These are taught in theory and code.

### Week 

### Week 8:

- ZK EVM, ZK Rollups.
- Sequencers
- ZK-DSL(s)


### Extra Week :

- More on ZK Math.
- ZK ML