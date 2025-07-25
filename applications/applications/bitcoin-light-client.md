# 📝 StarkBTC Light Client

## 🌟 Project Overview

Please provide the following:

Tagline: Bringing trustless Bitcoin state to Polkadot and Substrate-based chains.

This project is a Rust-based Bitcoin light client that performs simplified payment verification (SPV), enabling any Substrate chain to access verifiable Bitcoin state without relying on custodians or oracles. It lays the foundation for integrating Bitcoin into Polkadot-native DeFi, payments and cross-chain tooling — with zk-STARK trace export as a future extension.

-Relation to Polkadot:

Built in Rust with direct compatibility for integration into Substrate-based parachains.

Enables any chain in the Polkadot ecosystem to verify Bitcoin transactions natively.

Potential to bridge Bitcoin to chains like Acala, Interlay, or Moonbeam for real-world DeFi use.

Why we're building it:
Wrapped BTC is centralised and exposes users to custodial risk. Our project aims to remove this bottleneck and offer a cryptographic alternative: trust-minimized Bitcoin validation inside Polkadot.

### 🔍 Project Details

We expect applicants to have a solid idea about the project's expected final state. Therefore, please submit (where relevant):

### Technology Stack:
### Language: Rust

### Core Library: rust-bitcoin for parsing headers and transactions

Merkle Proofs + Header Chain Verification: Custom logic

CLI Interface: Rust-based command-line interface

Optional Future Export: zk-STARK proof compatibility via Cairo (Starknet) or zkLLVM

Optional API layer: JSON-RPC or GraphQL endpoint for Polkadot integration 

- Architecture Overview:

Wallet Layer: Generates a Bitcoin keypair, tracks UTXOs, and crafts transactions

Header Sync: Verifies PoW difficulty and chains valid Bitcoin block headers

Merkle Proof Verification: Given a txid, validates inclusion in a known block

STARK Export (Milestone 2): Optional module to export transaction verification trace

Substrate Compatibility: Modularised output format for potential parachain or off-chain worker consumption

### Proof of Concept / Prior Work:

 wallet-gen-working: Keypair generation and basic CLI wallet in Rust (GitHub tagged)

 Merkle verification and header chain logic in active development

Notion teaser and pitch deck already circulated with VC interest from a16z-aligned scouts

Designed with extensibility for ZK verification and cross-chain compatibility

### UI/UX Components:
UI is TBD; however the initial version is CLI-based for simplicity. Potential API layer may support UI in later stages.

### Data Models / API Specifications of the Core Functionality
This is minimal for now since the MVP is CLI-based, but we're defining key structs and potential future API behaviour:
Internal Rust Structs (planned or implemented):

```struct Wallet {
    pubkey: bitcoin::PublicKey,
    utxos: Vec<UTXO>,
}

struct UTXO {
    txid: bitcoin::Txid,
    vout: u32,
    value: u64,
    script_pubkey: bitcoin::Script,
}

struct HeaderChain {
    headers: Vec<bitcoin::BlockHeader>,
}

struct MerkleProof {
    txid: bitcoin::Txid,
    proof: Vec<bitcoin::hashes::sha256d::Hash>,
    merkle_root: bitcoin::TxMerkleNode,
    position: u32,
}

### Optional JSON-RPC or REST API (future module):

```GET /wallet/balance
Response: { "address": "bc1...", "balance": 120000 }

POST /tx/proof
Body: { "txid": "abc123...", "block_hash": "def456..." }
Response: { "valid": true, "proof": [...], "root": "..." }

GET /headers/latest
Response: { "height": 845921, "hash": "0000..." } ```

This minimal structure supports wallet operations, block syncing and Merkle inclusion proofs. If integrated into a parachain or off-chain worker, this API can expose verifiable BTC state to Polkadot apps.

### What the project is not (for now):

 Not a full validating Bitcoin node

 Does not support full Taproot / Schnorr script execution

 No full-fledged bridge mechanism implemented (this is infra for others to build on)

 Not intended to custody or wrap BTC itself — we verify its state only

 ### Expectations / Clarified Limitations
The project does not aim to replace full Bitcoin nodes — it offers a lightweight and trust-minimised alternative for verifying key aspects of Bitcoin state.

No real BTC will be bridged or held; we are verifying proof, not facilitating transfer or custody.

zk-STARK export is exploratory and modular, not guaranteed in Milestone 1 (but will be defined clearly in Milestone 2).

The tool relies on public APIs for initial data fetching (e.g., Electrum, Blockstream). Future improvements could add P2P modules.

While designed with interoperability in mind, integrations (e.g. Acala, Interlay) will depend on demand and partnership traction.

### 🧩 Ecosystem Fit

### Where and how does your project fit into the ecosystem?
This light client allows Polkadot-based applications (e.g. parachains or off-chain workers) to verify Bitcoin state (e.g. UTXOs, tx inclusion) without needing a full Bitcoin node. It lays the groundwork for trust-minimized BTC integrations — including payment rails, oracle-free price feeds, and BTC-based DeFi on Polkadot.

### Who is your target audience?

Builders on Polkadot needing non-custodial BTC data access

DeFi protocols and parachains seeking Bitcoin collateral (e.g. Acala, Interlay)

Oracles and off-chain workers that want verifiable BTC proofs without depending on third-party infrastructure

Security-conscious dApps needing zero-trust state validation

### What need(s) does your project meet?

Enables trustless Bitcoin state access on Substrate-based chains

Reduces reliance on custodial bridges like wBTC

Opens paths for BTC-backed lending, payments, staking

Provides developer tooling for those needing SPV proofs, Merkle verification or lightweight header sync

### Are there any other projects similar to yours in the Polkadot ecosystem?
Yes — projects like Interlay offer BTC-pegged assets (iBTC), but they rely on vaults and bridging mechanisms. There are no lightweight SPV-based Bitcoin clients intended for integration with off-chain workers, zk-bridges, or runtime modules today.

### If so, how is your project different?

We focus on verifiability, not custodianship

No vaults, oracles or bridge dependencies

It's designed to be integrated modularly into parachains, zk-apps or cross-chain protocols

Enables proof export for ZK/STARK-based bridging or attestation use cases

### If not, why might such a project not exist yet?

Historically, Bitcoin’s UTXO model and proof format are harder to integrate with smart contract chains

Most BTC integrations have focused on custodial bridging, which introduces centralization

Recent advances in zk infrastructure, off-chain workers and modular clients have now made this approach viable

## 👥 Team

- **Team Name:** Starkle
- **Contact Name:** Jeremy Chan
- **Contact Email:** jeremy.chan31@gmail.com
- **Website:** Your website, GitHub org, blog, or similar

### Team members

Jeremy Chan

#### LinkedIn Profiles (if available)

- https://www.linkedin.com/in/jwlchan/
- https://www.linkedin.com/{person_2}

### Team Code Repos

- https://github.com/{your_organisation}/{project_1}
- https://github.com/{your_organisation}/{project_2}

Please also provide the GitHub accounts of all team members:

- https://github.com/jwlzgg
- https://github.com/{team_member_2}

### Team's experience

Jeremy Chan is a seasoned Rust developer and blockchain infrastructure specialist with a background in validator operations, developer tooling and zero-knowledge research. He previously worked at Parity Technologies, where he contributed to Polkadot ecosystem development and validator relations.

Beyond a past as a data analyst and DevOps engineer, Jeremy also has a track record in Web3 business development, community engagement and writing, arcing technical depth with ecosystem fluency. He is the sole author and architect of the Starkle Bitcoin light client, which is engineered in Rust for modular, SPV-based Bitcoin state verification. His current focus is on cross-chain integration, particularly enabling non-custodial BTC verification in zk and EVM environments.

## 📊 Development Status

The project is currently under active development. The initial repo is live at:

[🔗 https://github.com/jwlchan/starkle-liteclient](https://github.com/JWLZGG/bitcoin-light-client-rust)

** Key features already implemented:**

✅ Wallet Generation Module: Deterministic Bitcoin keypair and address generation, using Rust.

✅ Modular Project Structure: Clear separation of CLI logic, wallet logic, and future SPV modules.

✅ Milestone Tagging: Tagged release wallet-gen-working confirms working CLI wallet generation.

✅ Early Devlog: Continuous commits demonstrate progress and build momentum for public visibility.

**Research and design already conducted:**

Feasibility studies of ZK-verifiable Bitcoin light clients and non-custodial cross-chain BTC usage

 Early use case design for exposing verified BTC state to other ecosystems, including zk, Substrate, and EVM-based chains

 Ongoing investor and ecosystem outreach to validate demand and identify integration targets

** Upcoming development focuses on:**

 SPV Header Sync: Download and verify Bitcoin block headers, validate PoW and longest-chain consensus

 Merkle Proof Verification: Validate transaction inclusion within blocks using proof data

 CLI Interface Expansion: Enable querying and display of verified BTC state


## 📅 Development Roadmap

Overview

Estimated Duration: 2 months

Full-Time Equivalent (FTE): 1.0

Total Costs: $8,000 USD

## PROPOSAL: Start with Milestone 1 and apply for the rest based on delivery

## Milestone 1 – Wallet Key & Address Tooling (2 weeks)

| Deliverable | Specification |
|-------------|---------------|
| **0a. License** | MIT |
| **0b. Documentation** | Rustdoc + README tutorial for generating keys and addresses |
| **0c. Testing and Testing Guide** | Unit tests for key generation, address derivation |
| **0d. Article** | Medium post introducing Bitcoin key/address generation in Rust |
| **1. Key & Address CLI** | CLI to generate a secp256k1 keypair and derive a native SegWit address (bech32) |
| **2. Address Validation** | Utility to verify and decode Bitcoin addresses (bech32) |

Cost: $2,500

Estimated Completion: 2 weeks

## Milestone 2 – Header Sync & Validation Engine (3 weeks)

| Deliverable | Specification |
|-------------|---------------|
| **0a. License** | MIT |
| **0b. Documentation** | Explain chain tip detection, block header rules |
| **0c. Testing and Testing Guide** | Tests for PoW, timestamp, version rules |
| **0d. Article** | Blog post explaining minimal SPV sync in Rust |
| **3. Header Parser** | Validate header fields and link to prior header |
| **4. PoW Validator** | Verify difficulty target and proof-of-work |
| **5. Sync Tool** | CLI to sync and display current chain tip from remote source |

Cost: $4,000

Estimated Completion: 2 weeks

## Milestone 3 – Merkle Proof Verifier & Tx Watcher (4 weeks)

| Deliverable | Specification |
|-------------|---------------|
| **0a. License** | MIT |
| **0b. Documentation** | CLI usage guide for proof ingestion and tx validation |
| **0c. Testing and Testing Guide** | JSON fixture-based tests for valid/invalid proofs |
| **0d. Article** | Deep dive on verifying Bitcoin tx inclusion with SPV |
| **6. Merkle Proof Verifier** | CLI to check txid inclusion using Merkle path + header |
| **7. Transaction Watcher** | Tool to monitor txid and report confirmation status and height |

Cost: $3,000

Estimated Completion: 3 weeks


**Optional (Future Module)**
If the grant is extended, later expanded to a future grant applied for:
- Export data to zk-friendly format (e.g. Cairo for STARK proofs)
- Implement a JSON-RPC or REST API layer
- Begin integration with Polkadot-based frontends, wallets or bridges

### Overview

- **Estimated Duration:** Duration of the whole project (maximum 3 months)
- **Full-Time Equivalent (FTE):**  Average number of full-time employees working on the project
- **Total Costs:** Requested amount in USD for the whole project (maximum $10,000 USD)

> Note that deliverables 0a to 0d are mandatory. Please adapt their specification to your project.

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | Apache 2.0 / GPLv3 / MIT / Unlicense |
| 0b. | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can... |
| 0c. | Testing and Testing Guide | Core functions will be fully covered by comprehensive unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| 0d. | Article | We will publish an **article** that explains what was done/achieved as part of the grant. |
| 1. | Feature X | We will create a feature that will... (Please describe in detail) |
| 2. | Feature Y | The Y feature will... (Please describe in detail) |
| 3. | Feature Z | The Z feature will... (Please describe in detail) |

### 💰 Budget Breakdown

Please provide a breakdown of your budget by milestone:

| Milestone | Deliverables                                                                 | Hours (est.) | Cost (USD) | Estimated Completion |
|-----------|------------------------------------------------------------------------------|--------------|------------|-----------------------|
| 1         | Wallet generation (BIP32/BIP39), address derivation, UTXO tooling, unit tests | 60 hrs       | $3,000     | 3 weeks               |
| 2         | Header sync, Merkle proof validation, inclusion check logic, ZK prep hooks   | 80 hrs       | $4,000     | 3 weeks               |
| 3         | Documentation, test suite expansion, user guide, and grant article publication | 60 hrs       | $3,000     | 2 weeks               |
| **Total** |                                                                              | **200 hrs**  | **$10,000**| **8 weeks total**     |



## 🔮 Future Plans

**Continued Development**
Following the Fast-Grant, we plan to:

Complete and productionize the Bitcoin light client with full header sync, inclusion proof verification and interoperability modules (e.g., JSON-RPC, Substrate pallet bindings).

Begin implementation of STARK-verifiable proof generation for Bitcoin state, enabling zk-friendly cross-chain integrations.

Explore a browser-based or mobile-compatible light client version for front-end dApps and wallets.

**Additional Funding Plans**
We are actively preparing a pre-seed funding round (~$300K–350K) to:

Support continued development over a 12–18 month runway.

Hire 2–3 key team members (including a co-founder, protocol engineer, and product/UX designer).

Fund a professional security audit (~$35K) and cover legal incorporation costs.

This project has already drawn interest from ecosystem-aligned investors and scouts (e.g., a16z network, European web3 VCs), and we intend to pursue additional public grants from:

Web3 Foundation long-form grants,

HRF’s Bitcoin Development Fund,

ZK-focused research funds.

**Vision for Polkadot Ecosystem Impact**
We envision Starkle as a foundational Bitcoin <-> Polkadot bridging primitive that:

Enables trust-minimised Bitcoin integration into parachains and dApps without relying on custodians.

Supports new BTC-native DeFi protocols on Polkadot, using verifiable balances and proof-based state tracking.

Lays the groundwork for future zk-light clients and optimistic message passing across ecosystems.

Ultimately, Starkle expands the design space for multi-chain applications by making Bitcoin interoperable, composable and provable within Polkadot and beyond.

## ℹ️ Additional Information

Work Completed to Date

- Wallet Key Generation Module: Working implementation using Bitcoin descriptors and PSBT standards; with support for single-sig keypairs.
-  Repo Live: Codebase available - repo provided above
- Applied to the HRF grant; VC interest from a16z and Dragonfly-aligned scouts

This is expected to grow beyond the initial funding, which we have amply demonstrated above.
