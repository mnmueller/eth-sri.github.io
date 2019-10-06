---
  ref: steffen19zkay
  title: "zkay: Specifying and Enforcing Data Privacy in Smart Contracts"
  authors: Samuel Steffen, Benjamin Bichsel, Mario Gersbach, Noa Melchior, Petar Tsankov, Martin Vechev
  year: 2019
  month: 11
  venue: ACM CCS
  projects: blockchain-security
  awards:
  bibtex:
  paper: https://files.sri.inf.ethz.ch/website/papers/ccs19-zkay.pdf
  image: 
  talk:
  slides:
---

Privacy concerns of smart contracts are a major roadblock preventing their wider adoption. A promising approach to protect private data is hiding it with cryptographic primitives and then enforcing correctness of state updates by Non-Interactive Zero-Knowledge (NIZK) proofs. Unfortunately, NIZK statements are less expressive than smart contracts, forcing developers to keep some functionality in the contract. This results in scattered logic, split across contract code and NIZK statements, with unclear privacy guarantees.

To address these problems, we present the zkay language, which introduces privacy types defining owners of private values. zkay contracts are statically type checked to (i) ensure they are realizable using NIZK proofs and (ii) prevent unintended information leaks. Moreover, the logic of zkay contracts is easy to follow by just ignoring privacy types. To enforce zkay contracts, we automatically transform them into contracts equivalent in terms of privacy and functionality, yet executable on public blockchains.

We evaluated our approach on a proof-of-concept implementation generating Solidity contracts and implemented 10 interesting example contracts in zkay. Our results indicate that zkay is practical: On-chain cost for executing the transformed contracts is around 1M gas per transaction (~0.50US$) and off-chain cost is moderate.