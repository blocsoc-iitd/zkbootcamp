# Syllabus outline ZkSync Summer Bootcamp:

## Goal:

By the end of the boot camp, all the boot campers should get a clear overview of Zero-knowledge and ZK math, and they should be able to write ZK Circuits & create ZK applications on their own, together with having a good overview of the Blockchain ecosystem.

## Timings: 

- Kickoff: 5th May 2024, offline.

- Number of Weeks: 8 Week(s) + 1 Week.

- Number of days a week: 
    - Content for five days, up to the boot camp.
    - 2 online sessions a week.
    - 1 online session will be on giving an overview of the week's syllabus. (think of it as video lectures in MOOC).
    - The other session could be doubt-solving or an overview session.

## Content:



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
  
Additional Content (only for those interested):

- [Bitcoin White Paper Exercises](https://github.com/cooganb/bitcoin-whitepaper-exercises) These are a series of exercises, built by [Kyle Simpson,](https://github.com/getify){target=_blank} for understanding some of the concepts outlined in the Bitcoin white paper. These are not easy, but if you really would like to understand these fundamentals as they apply to blockchains, this is a great place to start.
 - [CryptoHack](https://cryptohack.org/)"A fun free platform for learning modern cryptography"
 - [CryptoPals](https://cryptopals.com/) This is *very* advanced and intense, but real to-the-metal applied cryptography! I am putting this link in here and it scares me.


### Week 2: Protocol Development Deep-Dive

This week acts as a starter to Rust for everyone and to make everyone code in Rust at a basic level. 

- Development on Ethereum(probably in Rust/GO 😉).
  - Protocol-level Development (P2P, Transaction Processing, "Node / Client Development") 
  - [[ Perhaps you'd want to check out the "Consensus" section from [this course](https://github.com/ConsenSys-Academy/Blockchain-Developer-Bootcamp/tree/1c47761d403026d55f54b36f62e33b1127e8da61/docs/S01-fundamentals) I built at Consensys]]

Rust resources:
- General Recommendation: Learn Rust from Day 0.
- (https://doc.rust-lang.org/stable/book/) - The Rust Book
- (https://rust-book.cs.brown.edu/) - Rust book with more detailed explanation and quizzes
- (https://youtu.be/OX9HJsJUDxA?si=1xtatEZ4VTrEzKu5) - Let's Get Rusty Playlist
- (https://doc.rust-lang.org/rust-by-example/index.html) - Rust by Example
- (https://github.com/rust-lang/rustlings) - Rustlings

Go resources:
- Basic : https://www.w3schools.com/go/go_syntax.php
- Go Channel Structure: https://blog.logrocket.com/how-use-go-channels/#:~:text=How%20to%20use%20Go%20channels%201%20Creating%20a,channel%20...%205%20Channels%20as%20function%20parameters%20
- Context: https://www.golinuxcloud.com/golang-context/
- Official docs: https://go.dev/doc/tutorial/


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

Resources:
- rollups - https://vitalik.eth.limo/general/2021/01/05/rollup.html
- Scaling Ethereum - https://youtu.be/zADuI0a1c9A?si=VfJ3wIiglXxX70Zc
- slides - https://docs.google.com/presentation/d/15lxDiJm_Rz5BeFzPxfFwfbys-OWgvtMXXkrBJSA2_Yk/edit#slide=id.g2b8fcc687c3_0_9
- eip4844 - https://github.com/ethereum/EIPs/blob/master/EIPS/eip-4844.md 

Things might seem confusing and tough to understand, but keep reading and exploring. Remember, blockchain's holy grail is creating a decentralized and secure network with a high transaction-per-second rate. Achieving this requires developing sophisticated mechanisms, such as implementing rollups with zero-knowledge proofs and fault-proof systems.

##### RESOURCES FROM DOUBT SESSION

1. Tornado Cash (a use case implentation of zero knowledge proofs) refer to the followinG Rare Skills blog , it explains it throughly in a good 30-45 min read
https://www.rareskills.io/post/how-does-tornado-cash-work

2. For those already done with rust , implement few programs to get a good command on it. Some recommended stuff will be to : 

a) Implement a simple blockchain in Rust.
https://blog.logrocket.com/how-to-build-a-blockchain-in-rust/

b) You can develop random things ( CLI , torrent clients ) from scratch as well to test and improve rust , will take a days worth effort.
https://github.com/codecrafters-io/build-your-own-x?tab=readme-ov-file

c) ADVANCED :  You can try and create proofs for your Rust program and have them verified as well. Will give you a basic intution of how zero knowledge proofs are being implemented.

https://dev.risczero.com/api/
https://succinctlabs.github.io/sp1/

3. For those who are interested and want to get some initial readings and resources on Zero-knowledge proofs , refer to the following resorces. It's recommended to through the ZK-Book with patience in detail ,  while the others can used as extra resources , used randomly however you want.

https://www.rareskills.io/zk-book
https://zkiap.com/
https://zkhack.dev/whiteboard/

4. Practice GO a bit parallely. You can use the resources shared earlier to learn GO. And for those who have some experience in GO and want to do some blockchain relevant stuff with it , you can check out the Avalanche ecosystem.

https://docs.avax.network/
https://academy.avax.network/start

You can try implementing precompiles in the Avalanche Subnet EVM. It's a good task which will give you a good idea of many underlying blockchain concepts. It can be tough to grasp in the beginning , but if you are confident enough in your basics then it would be a fun thing to look through the weekend.


### Week 4: The Road Forward for Blockchain and/or Use Case
- Ethereum's Rollup-centric roadmap and alt narratives...
- DA Layers, Alt VMs(MoveVM, WasmVM, Solana VM)
- Data Availability / Protodanksharding
- Decentralised Identities, Bridges(ZK and non ZK bridges).

Resources:
- Restaking and Eigen Layer: https://docs.eigenlayer.xyz/assets/files/EigenLayer_WhitePaper-88c47923ca0319870c611decd6e562ad.pdf
- DAS:  https://weufoundation.medium.com/foundations-of-data-availability-sampling-1a8033d8c9fc
- Celestia white paper:(celestia offers Data availability): https://arxiv.org/abs/1905.09274
- Awesome AVS(about eigenlayer restaking possibilities): https://github.com/Layr-Labs/awesome-avs

## Week 5: What is ZK? && Math Primitives

Intro to ZK (high level)
* ZK as kompression
* ZK as privacy

### Math primitives

- Cryptography review
- Mathematical terminology
- Modular arithmetic
- Introduction to polynomials
- Group and Field theory
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

 It would be better to make these programmed in arkworks, snark, or circom.
 And give a complete overview of how these prooving systems work. like in [groth16 by rareskills](https://www.rareskills.io/post/groth16) or [plonk by lambdaclass](https://blog.lambdaclass.com/all-you-wanted-to-know-about-plonk/)
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

The math background of these topics would be better: lookups are introduced in Lesson 12, but it is not math-oriented. Recursion, proof composition and aggregation are introduced in Lesson 13.
- Lookups.
- Sumcheck.
  
Additional Resources: Starkware, lambdaclass, scroll, risc0 blogs. Toy Plonk & ZkVm implementations.

### Extra Week:
- Plonky2 hands-on examples.
- General purpose ZKVM's
- Nova, HyperPlonk, Spartan, Binius (afaik most research these days are happening on these), so it would be better to give an overview of these.

Linking to more resources for ZK development.

ORIGINAL DRAFT FOR REFERENCE:


## Implementation



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

### Week 8:

- ZK EVM, ZK Rollups.
- Sequencers
- ZK-DSL(s)


### Extra Week :

- More on ZK Math.
- ZK ML



Additional content(only for those interested): Docs of Alchemy / Alchemy University to build a DApp.

* [Bootcamp:Learn Blockchain, Solidity and Full Stack JavaScript Development:](https://www.freecodecamp.org/news/learn-blockchain-solidity-full-stack-javascript-development/)A 32 hour long comprehensive Blockchain Development Bootcamp by Patrick Collins
* [Course: CryptoZombies](https://cryptozombies.io/) One of the most well-known introductions to Solidity
* [Course: Ethernaut (OpenZeppelin)](https://ethernaut.openzeppelin.com/) An excellent in-browser "game" teaching Solidity from a security perspective.
* [Course: Intro to Solidity (Chainshot)](https://www.chainshot.com/learn/solidity) Chainshot uses a very cool interactive platform to teach Solidity
* [Wiki: Solidity by Example](https://www.solidity-by-example.org) A bunch of great examples of Solidity, including excellent design patterns, hacks and security tips.
* [Wiki: Use Web3](https://useweb3.xyz/) Another good collection of learning resources
* [Article: Test Driven Introduction to Solidity](https://michalzalecki.com/ethereum-test-driven-introduction-to-solidity/) From an older pragma version of Solidity, but might be interesting to check out! Repo accompanying the article [here.](https://github.com/MichalZalecki/tdd-solidity-intro)
* [Thread: What Does Ethereum Development Look Like Today?](https://twitter.com/smpalladino/status/1421901085279756300) Santiago Palladino, who wrote [Ethereum for Web Developers,](https://www.apress.com/gp/book/9781484252772) updates parts of his book for the current Ethereum ecosystem.
* [Article: Learn X in Y Minutes (Solidity)](https://learnxinyminutes.com/docs/solidity/)  A bit long and rough, but a comprehensive overview of learning Solidity
