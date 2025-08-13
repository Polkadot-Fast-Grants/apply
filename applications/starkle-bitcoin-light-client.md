# 📝 Name of your Project
Starkle – Bitcoin Light Client (Rust)

---

# 🌟 Project Overview

**Tagline:** Trustless Bitcoin state for Polkadot.

**What it is:** A minimal Bitcoin light client written in Rust that:
- syncs and validates Bitcoin block headers (SPV),
- verifies transaction inclusion via Merkle proofs,
- exposes a small API/SDK (Rust + WASM) for Substrate chains and off-chain workers,
- prepares ZK-verifiable export formats for future on-chain verification.

**How it relates to Polkadot:** Substrate pallets, oracles and bridges can consume **real BTC state** (payments, PoR, collateral, alerts) without centralized indexers.

**Why Polkadot.** Substrate pallets and app-chains can integrate real BTC signals with fewer trust assumptions. This grant delivers header sync, Merkle verification, fixtures, docs, tests, and a WASM wrapper; a zk-export format is prepared for later cross-chain verification.

**Why we’re building it:** BTC is the most secure chain but hard to integrate trustlessly. We reduce integration work to a lightweight client + API so Polkadot apps can unlock BTC payments and collateral with fewer trust assumptions.

---

# 🔍 Project Details

**Tech stack**
- Rust (`rust-bitcoin`, `bitcoin_hashes`), no_std-friendly where possible
- Substrate integration (off-chain worker, pallet glue code)
- WASM build for light browser/mobile usage
- Fixtures + test vectors (headers, txs, proofs)
- Optional ZK-export skeleton (JSON traces compatible with STARK/zkVM toolchains)

**Core components**
- `headers`: parse + validate chain of headers, check PoW targets & difficulty transitions
- `merkle`: verify inclusion proofs against header `merkle_root`
- `api`: read-only queries (get_header, get_tip, verify_tx_inclusion), event hooks
- `wasm`: minimal wrapper to call `api` in browser/runtime
- `fixtures`: reproducible tests for testnet regimens

**Prior work / MVP**
- Working CLI wallet: mnemonic gen, key derivation, native SegWit address
- Repo: https://github.com/JWLZGG/bitcoin-light-client-rust

**What this project is *not***
- Not a full node, not a custodial bridge, not a token wrapper.
- No mainnet security proofs on-chain in this grant (we prepare the export path, not the full verifier).

---

# 🧩 Ecosystem Fit

**Where it fits**
- Bridges/oracles needing Bitcoin confirmation proofs
- DeFi/PoR tools on Polkadot Hub/Plaza and parachains
- Custody-light mobile/web wallets (off-chain worker assisted)

**Target users**
- Substrate dev teams, oracle/bridge maintainers, wallet teams

**Needs met**
- Trust-minimized BTC integrations without centralized indexers
- Deterministic, testable proof verification

**Similar efforts**
- Kyoto/Nakamoto/MAP focus on bridges/L2s; Starkle focuses on a **small, auditable light client + SDK** for Polkadot apps.

---

# 👥 Team

**Team name:** Starkle  
**Contact:** Jeremy Chan — jeremy.chan31@gmail.com  
**Website/Repo:** https://github.com/JWLZGG/bitcoin-light-client-rust

**Members**
- **Jeremy Chan** (Founder) — DevRel @ Parity (ex), data analyst @ VanMoof; Rust + product.  
  LinkedIn: https://www.linkedin.com/in/jwlchan/  
  GitHub: https://github.com/JWLZGG

---

# 📊 Development Status

- CLI wallet working (mnemonic, derivation, SegWit address)
- Scaffolding for header parsing & proof verification in repo
- This grant covers SPV header sync, Merkle verification, docs, tests, and a WASM build + ZK-export skeleton.

---

# 📅 Development Roadmap

**Overview**  
- **Estimated Duration:** 10–12 weeks (≤ 3 months)  
- **FTE:** ~0.8 FTE (primarily solo dev + occasional collaborator)  
- **Total Cost:** **$9,950 USD**

### Milestone 0 — Required Deliverables (no cost)
**0a. License**  
MIT (code) and CC BY 4.0 (docs) for this grant’s deliverables unless Polkadot requires a specific OSI-approved license.

**0b. Documentation**  
Inline Rust doc comments plus a short tutorial (README section) showing how to build/run the client, sync headers, and verify a sample Merkle proof.

**0c. Testing & Testing Guide**  
Unit tests covering header parsing/validation and Merkle inclusion (≥80% line coverage of core modules). A TESTING.md explaining how to run the suite locally.

**0d. Article**  
A medium-length article (Mirror/Medium/Substack) summarizing the work done in this grant with links to repo, tests, and tutorial.

### Milestone 1 — SPV Header Sync & Docs — **$3,500** — 3–4 weeks
- **0a. License:** MIT
- **0b. Documentation:** README + usage guide (run sync, query tip/header)
- **0c. Testing & Guide:** Unit tests covering header parse, PoW target checks
- **0d. Article:** “Building an SPV header client for Polkadot”
- **1. Header module:** validate header chain, difficulty retarget, fork-choice (longest-work)
- **2. API:** `get_tip`, `get_header(hash/height)`, `subscribe_tip()`

**Verification:** CI passing, test vectors included, demo: sync to testnet height N and print tip.

**Acceptance criteria:** All tests pass on CI; example commands reproduce documented outputs; README section for this milestone updated.

### Milestone 2 — Merkle Proof Verification — **$3,000** — 3–4 weeks
- **3. Merkle module:** verify inclusion proofs against `merkle_root`
- **4. CLI & examples:** `verify-merkle <txid> <blockhash>` using fixtures
- **5. Fixtures:** reproducible test data (headers, tx, proof JSON)

**Verification:** run CLI to verify inclusion for provided fixtures; unit tests passing.

**Acceptance criteria:** All tests pass on CI; example commands reproduce documented outputs; README section for this milestone updated.

### Milestone 3 — WASM Build & ZK-Export Skeleton — **$3,450** — 3–4 weeks
- **6. WASM wrapper:** compile `api` to WASM, simple browser/off-chain example
- **7. ZK-export skeleton:** JSON trace format (headers/tx path) with schema + sample
- **8. Developer docs:** integration notes for Substrate off-chain worker/pallet

**Verification:** WASM demo page or example script; JSON schema + sample traces committed.

**Acceptance criteria:** All tests pass on CI; example commands reproduce documented outputs; README section for this milestone updated.

---

# 💰 Budget Breakdown

| Milestone | Deliverables (summary) | Hours | Rate | Cost |
|---|---|---:|---:|---:|
| M1 | SPV headers + docs + tests + article | 70 | $50 | $3,500 |
| M2 | Merkle verification + CLI + fixtures | 60 | $50 | $3,000 |
| M3 | WASM build + ZK-export skeleton + docs | 69 | $50 | $3,450 |
| **Total** |  | **199** |  | **$9,950** |

| Milestone | Deliverables (summary)                         | Hours | Rate  | Cost (USD) |
|-----------|------------------------------------------------|-------|-------|------------|
| 1         | Header sync (SPV), fixtures, docs              | 55    | $60/h | $3,300     |
| 2         | Merkle proof verification + tests + guide      | 55    | $60/h | $3,300     |
| 3         | WASM wrapper + examples + README tutorial      | 55    | $60/h | $3,300     |
| **Total** |                                                |       |       | **$9,900** |


*If an additional helper is engaged, hours will be rebalanced without changing the total.*

---

# 🔮 Future Plans

- Extend to **on-chain verification** (pallet or precompile) using submitted proof bundles.  
- Produce a **pallet crate** others can import; add alerting/PoR helpers.  
- Seek follow-on support (e.g., Web3 Foundation Open Grants) and/or co-funded integrations with parachains.

---

# ℹ️ Additional Information

- **Work done:** CLI wallet; repo public; initial header/merkle scaffolding.  
- **Other funding:** Polkadot Fast Grants (this application). Exploring small ecosystem grants for specific integrations.  
- **Open source:** MIT license; welcoming community contributions & audits.
