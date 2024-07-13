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



## Week 1: Intro to L1 "Primitives" 

Lecture By Rahul Saxena : https://youtu.be/cUYeTqiKLtg?si=RmW1Cq1SW_fPufU1
- General intro to Blockchain
  - Decentralised Systems
- Blockchain Timeline
- Layer1 Theory
- Blockchain Components
- Chains Overview
  - How do Ethereum & Solana work at the consensus and execution layer?
  - Trade-offs // "Trade spaces" Design decisions made by protocols to prioritize different things. Ethereum vs Solana etc.
  - Modular vs Monolithic Execution 
  - Alt VMs 
  
Additional Content (only for those interested):

- [Bitcoin White Paper Exercises](https://github.com/cooganb/bitcoin-whitepaper-exercises) These are a series of exercises, built by [Kyle Simpson,](https://github.com/getify){target=_blank} for understanding some of the concepts outlined in the Bitcoin white paper. These are not easy, but if you really would like to understand these fundamentals as they apply to blockchains, this is a great place to start.
 - [CryptoHack](https://cryptohack.org/)"A fun free platform for learning modern cryptography"
 - [CryptoPals](https://cryptopals.com/) This is *very* advanced and intense, but real to-the-metal applied cryptography! I am putting this link in here and it scares me.


## Week 2: Protocol Development Deep-Dive

This week acts as a starter to Rust for everyone and to make everyone code in Rust at a basic level. 

- Development on Ethereum(probably in Rust/GO 😉).
  - Protocol-level Development (P2P, Transaction Processing, "Node / Client Development") 
  - [[ Perhaps you'd want to check out this section from [this course](https://github.com/ConsenSys-Academy/Blockchain-Developer-Bootcamp/tree/1c47761d403026d55f54b36f62e33b1127e8da61/docs/S01-fundamentals) Built by Consensys]]

Rust resources:
- General Recommendation: Learn Rust from Day 0.
- (https://doc.rust-lang.org/stable/book/) - The Rust Book
- (https://rust-book.cs.brown.edu/) - Rust book with more detailed explanations and quizzes
- (https://youtu.be/OX9HJsJUDxA?si=1xtatEZ4VTrEzKu5) - Let's Get Rusty Playlist
- (https://doc.rust-lang.org/rust-by-example/index.html) - Rust by Example
- (https://github.com/rust-lang/rustlings) - Rustlings

Go resources:
- Basic: https://www.w3schools.com/go/go_syntax.php
- Go Channel Structure: https://blog.logrocket.com/how-use-go-channels/#:~:text=How%20to%20use%20Go%20channels%201%20Creating%20a,channel%20...%205%20Channels%20as%20function%20parameters%20
- Context: https://www.golinuxcloud.com/golang-context/
- Official docs: https://go.dev/doc/tutorial/


## Week 3: Scalability

This week gives an overview of most of the essential concepts in web3.

- Scalability Introduction: Ethereum / Bitcoin / etc as L1 (Lectures #2 and #3 in zkSync zkEVM Bootcamp)
  - Scalability Introduction
  - Approaches to Scalability
  - Layer 1 Solutions
  - Off-chain Scaling
  - Bridges / Sidechains versus Layer 2
- Typical Rollup Architecture
  - L2 Mental Model
  - Sequencers
  - Mix and Match for OP Rollups, ZK Rollups, Validiums, "L3s" or "Hyperchains"
- Rollups in more detail
- Introduction to zkEVM solutions

Resources:
- rollups - https://vitalik.eth.limo/general/2021/01/05/rollup.html
- Scaling Ethereum - https://youtu.be/zADuI0a1c9A?si=VfJ3wIiglXxX70Zc
- slides - https://docs.google.com/presentation/d/15lxDiJm_Rz5BeFzPxfFwfbys-OWgvtMXXkrBJSA2_Yk/edit#slide=id.g2b8fcc687c3_0_9
- eip4844 - https://github.com/ethereum/EIPs/blob/master/EIPS/eip-4844.md 

Things might seem confusing and tough to understand, but keep reading and exploring. Remember, blockchain's holy grail is creating a decentralized and secure network with a high transaction-per-second rate. Achieving this requires developing sophisticated mechanisms, such as implementing rollups with zero-knowledge proofs and fault-proof systems.

##### RESOURCES FROM DOUBT SESSION

1. Tornado Cash (a use case implementation of zero-knowledge proofs) Refer to the following Rare Skills blog. It explains it thoroughly in a good 30-45 min read: https://www.rareskills.io/post/how-does-tornado-cash-work

2. For those already done with rust, implement a few programs to get a good command of it. Some recommended stuff will be to : 

a) Implement a simple blockchain in Rust.
https://blog.logrocket.com/how-to-build-a-blockchain-in-rust/

b) You can develop random things ( CLI, torrent clients ) from scratch to test and improve rust, which will take a day's effort.
https://github.com/codecrafters-io/build-your-own-x?tab=readme-ov-file

c) ADVANCED:  You can try creating proofs for your Rust program and have them verified. Will give you a basic intuition of how zero-knowledge proofs are being implemented.

https://dev.risczero.com/api/
https://succinctlabs.github.io/sp1/

3. For those who are interested and want to get some initial readings and resources on Zero-knowledge proofs, refer to the following resources. It's recommended to through the ZK-Book with patience in detail,  while the others can used as extra resources, used randomly however you want.

https://www.rareskills.io/zk-book
https://zkiap.com/
https://zkhack.dev/whiteboard/

4. Practice GO a bit parallelly. You can use the resources shared earlier to learn GO. And for those who have some experience in GO and want to do some blockchain-relevant stuff with it, you can check out the Avalanche ecosystem.

https://docs.avax.network/
https://academy.avax.network/start

You can try implementing precompiles in the Avalanche Subnet EVM. It's a good task that will give you a good idea of many underlying blockchain concepts. It can be tough to grasp in the beginning, but if you are confident enough in your basics then it would be a fun thing to look through the weekend.


## Week 4: The Road Forward for Blockchain and/or Use Case
- Ethereum's Rollup-centric roadmap and alt narratives...
- DA Layers, Alt VMs(MoveVM, WasmVM, Solana VM)
- Data Availability / Protodanksharding
- Decentralised Identities, Bridges(ZK and non ZK bridges).

### Resources:
- Restaking and Eigen Layer: https://docs.eigenlayer.xyz/assets/files/EigenLayer_WhitePaper-88c47923ca0319870c611decd6e562ad.pdf
- DAS:  https://weufoundation.medium.com/foundations-of-data-availability-sampling-1a8033d8c9fc
- Celestia white paper:(celestia offers Data availability): https://arxiv.org/abs/1905.09274
- Awesome AVS(about eigenlayer restaking possibilities): https://github.com/Layr-Labs/awesome-avs

### Additional Resources :
- https://www.youtube.com/watch?v=RG7A0flGJNM
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
### Resources :
- Zk-book - https://www.rareskills.io/zk-book

### Advanced Resources :
https://github.com/LeastAuthority/moonmath-manual/releases/latest/download/main-moonmath.pdf
## Week 6: What are zkEVMs?

The most crucial part of the boot camp. Those who complete this can understand and write circuits and build Zk Dapps independently.

- Overview
- Universal Circuits / Circuit Compiler
- Proving Systems

### Resources for building :
https://github.com/LuozhuZhang/awesome-zkevm

### Additional :
- https://github.com/kkrt-labs/kakarot/
- https://github.com/0xPolygonHermez/
- https://github.com/scroll-tech/zkevm-circuits/
## Week 7: SNARKs

Lectur By Porter : https://youtu.be/gwP0sUxyYls?si=7oljYS6ynZdktJDz
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
- Lookups
- Sumcheck

### Resources :
1) Circle stark - https://elibensasson.blog/why-im-excited-by-circle-stark-and-stwo/
2) Plonk - https://blog.lambdaclass.com/all-you-wanted-to-know-about-plonk/
3) Sumcheck - https://blog.lambdaclass.com/have-you-checked-your-sums/
4) IPA - https://blog.lambdaclass.com/ipa-and-a-polynomial-commitment-scheme/
5) Binius - https://vitalik.eth.limo/general/2024/04/29/binius.html
6) ProofArgsAndZk book - https://people.cs.georgetown.edu/jthaler/ProofsArgsAndZK.html
7) Zk-book - https://www.rareskills.io/zk-book
8) Groth16 - https://www.rareskills.io/post/groth16

## Week 8 : STARKs

### STARK Implementation
- Reed Solomon codewords
- Computational integrity
- Stark arithmetisation
- FRI background

The math background of these topics would be better: lookups are introduced in Lesson 12, but it is not math-oriented. Recursion, proof composition and aggregation are introduced in Lesson 13.
- Lookups.
- Sumcheck.
### Resources:

1) https://vitalik.eth.limo/general/2017/11/09/starks_part_1.html
2) https://vitalik.eth.limo/general/2017/11/22/starks_part_2.html
3) https://vitalik.eth.limo/general/2018/07/21/starks_part_3.html
4) https://starkware.co/stark-101/  , hands-on for writing starks from scratch in python
5) https://github.com/lambdaclass/STARK101-rs , rust version of the above
6) https://medium.com/starkware/tagged/stark-math 
7) https://neptune.cash/learn/stark-anatomy/ this is a 6-part series on writing starks in python.
a good project to go with  https://neptune.cash/learn/brainfuck-tutorial/ - A tutorial on building a project demonstrating the computational integrity of a program written in Brainfuck.
If you come across any other good resources, feel free to share them in the group.

### Additional Resources: 
Starkware, lambdaclass, scroll, risc0 blogs. Toy Plonk & ZkVm implementations.

## Linking to more resources for ZK development
- https://trapdoortech.medium.com/
- https://github.com/ventali/awesome-zk
- https://www.youtube.com/@zeroknowledgefm
