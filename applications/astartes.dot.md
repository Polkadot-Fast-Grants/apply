# 📝 Astartes.dot – Polkadot Fast-Grant Application

## 🌟 Project Overview

**🎯 Name of your Project:** Astartes.dot  
**🗣️ Tagline:** Tamper-Evident Logging for Zero-Trust Infrastructure

### 📌 Brief Description

Astartes is a high-integrity logging and forensic audit system designed to prevent the silent alteration of security logs in cloud and on-premises environments. The architecture proactively ensures the audit trail cannot be compromised by separating the integrity proof from the source. It uses lightweight agents to compute Merkle roots on each server, a centralised verifier to perform integrity checks and a blockchain publisher to anchor immutable proofs to Polkadot. 

This provides a verifiable, cryptographically-secured source of truth for all security-relevant telemetry. It can operate independently or complement other systems like centralised detection-as-code frameworks. It’s designed for scale and becomes more cost-efficient as infrastructure grows.

### 🧩 Polkadot Integration

Astartes gains operational resilience and cost efficiency by anchoring to Polkadot Asset Hub. By anchoring here, we inherit the full economic security and censorship resistance of the Polkadot Relay Chain, ensuring the ledger's immutability. Asset Hub serves as the zero-trust vault for our verified data hashes, cementing the integrity necessary to meet the entire end-to-end chain of custody.

### 🚀 Team Interest

Our team believes that Astartes neutralizes a critical operational gap exploited through defence evasion techniques, specifically outlined in Mitre Att&ck: **T1070.001**, **T1070.002**, **T1070.003** and **T1565.001**. Confirming its position as an imperative and viable enhancement for securing mission-critical infrastructure.

---

## 🔍 Project Details

### 🧱 Technology Stack Overview

| Component | Technology | Role |
|:---|:---|:---|
| Core Agent (Server A) | Rust | High-performance, low-overhead binary for Merkle Tree generation, local log hashing and secure communication. |
| Verification Logic (Server C) | Python / AWS Lambda / EC2 | Centralized service for integrity verification, tamper detection and generating forensic reports. |
| Data Pipeline (Bridge) | Cribl Stream | Vendor-agnostic data processing engine for filtering, normalization and routing data between Server A, B and C. |
| Blockchain Anchor (Server B) | Python / AWS Lambda | Communication layer for submitting Merkle Root transactions to Polkadot Asset Hub. |
| Trust Anchor | Polkadot Asset Hub | Immutable security layer for proof anchoring. |
| SIEM Integration | Splunk Enterprise | Target destination for forwarding verification reports and generating security alerts for tamper events. |
| Security Auditing | Aikido | Code security scanning and vulnerability analysis to ensure the integrity of the Rust and Python codebase. |

### ⚙️ Core Architecture Components

1.  **Server A (Merkle Root Agent):** A Rust binary on the source asset that monitors log files, hashes new entries, builds a Merkle Tree and forwards the full payload (with the root hash) into the Cribl pipeline. Sensitive data never leaves the host; only cryptographic representations are in transit.
2.  **Server B (Blockchain Anchor):** An AWS Lambda function that receives the Merkle Root (a sub-set of the full payload) via the Cribl routing pipeline. It is solely responsible for anchoring this hash as an immutable transaction on Polkadot Asset Hub.
3.  **Server C (Centralised Verifier):** An EC2 instance running Python logic that acts as a centralized data integrity checker. It receives payloads from Server A more frequently than Server B to enable early detection of tampering. It performs multi-dimensional checks (Log count, Leaf integrity, Category drift). Upon successful verification, it sends a "Verification" payload to Splunk for security alerting.
   
**Note:** While Astartes can route payloads directly between agents A, B and C. This grant will enable us to focus on integrating tier-1 enterprise tools. The inclusion of Cribl and Splunk is intentional. Cribl acts as our single pane of glass for data routing, fundamentally enabling flexible multi-tenant architecture (commercial goal) and Splunk proves “plug-and-play” for enterprise Security Operation Centers. 

### 🛠️ Substrate Framework Integration

The project uses a minimalist, low-cost integration approach. Web3.py is used within Server B to anchor the Merkle Root hashes to Asset Hub. This simple, direct anchoring allows Astartes to focus its resources on cryptographic speed and integrity verification; offloading the security and consensus burden to the Polkadot Relay Chain.

### 🔒 Smart Contract Design

Astartes is built to be easily auditable, no opaque complexity or surprises. Our initial smart contract deployed on Westend testnet mirrors this perfectly—it is designed solely for anchoring the critical, non-repudiable cryptographic proofs. 

---

### ⚠️ Current Limitations

- **Not a SIEM:** We are a data integrity validator, not an event alerting platform (SIEM).
- **Not a One-Stop Solution:** Astartes does not replace traditional security controls, it reinforces them.
- **Not a database:** Only Merkle Root hashes are anchored on-chain. Full log content remains at source for forensic teams to reference in the event of suspected tampering.
- **Initial Grant Scope:** The initial grant will not cover Windows/Linux package distribution; the focus will initially be proving functionality in a controlled AWS/macOS environment.

---

## 🧩 Ecosystem Fit

Astartes fits into the Security and Infrastructure layer of Polkadot’s ecosystem. By leveraging Asset Hub as an external, immutable trust anchor, we create a necessary primitive for enterprises building secure data pipelines. Astartes provides real-world utility and adoption proof for Polkadot's high-security properties outside of traditional DeFi/Web3 use cases.

### 👥 Target Audience

- **Medium-Large Enterprises:** Organisations requiring the highest level of security, compliance and integrity of security logs to mitigate insider threat scenarios.
- **Parachains/Ecosystem Projects:** Teams looking for a verifiably secure method to log and audit off-chain operational data.

### 🛠️ Problem Resolution

The primary need met is tamper-evidence and insider threat mitigation in security logging. It solves the "who watches the watchers" problem by decentralizing the ultimate proof of integrity away from the compromised system's administrative domain.

### ⚔️ Competitive Landscape

There are currently **no direct competitors** offering a commercial, off-chain, tamper-evident logging system that uses Polkadot as an immutable security anchor.

---

## 🎯 Unique Differentiation

- **Polkadot Asset Hub Anchor:** Leverages Polkadot's economic security and immutability for log integrity proof.
- **Zero-Trust Architecture:** Anchors Merkle Roots, not log data, ensuring sensitive data never leaves the host.
- **Insider Threat Mitigation:** Provides a cryptographically-secured chain of custody to prevent the silent alteration of security logs.
- **SIEM Complement:** Integrates seamlessly with existing enterprise Security Information and Event Management tools like Splunk.

---

## 🔒 Enhanced Security Architecture

Astartes is engineered following Secure by Design [Principles](https://www.security.gov.uk/policy-and-guidance/secure-by-design/principles/):
| Principle | Feature |
|:---|:---|
| **1. Responsibility** | Creates an immutable ledger on Polkadot, making log integrity risk fully auditable by risk owners. |
| **2. Secure Products** | Built with Rust (memory-safe language) and assured by Aikido security auditing. |
| **3. Risk-Driven** | Directly mitigates high-risk defence evasion techniques. |
| **5. Detect & Respond** | Provides real-time tamper detection and routes reports directly to Splunk for immediate alerting/response. |
| **7. Minimise Attack Surface** | Sensitive data never leaves the host; only small cryptographic hashes are transmitted and anchored. |
| **8. Defend in Depth** | Uses 3 Layers of Defence: Agent A (Local Cryptographic Proof), C (Integrity Verification) and B (Immutable Storage of Cryptographic Proof). |
| **9. Continuous Assurance** | Continuous integrity checks and immutable anchoring provides non-repudiable cryptographic assurance. |

## 👥 Team

**🏷️ Team Name:** Astartes.dot  
**📨 Contact Name:** Ijaz Driscoll, Marco Tsang  
**📧 Email:** ijazdriscoll@gmail.com, hkmarcoot@gmail.com
**🔗 GitHub:** [Astartes-v1](https://github.com/The-Six/astartes_dot?tab=readme-ov-file), 
[Astartes-v2](https://github.com/The-Six/Astartes-v2)

### 🧑‍🤝‍🧑 Team Members

| Name | Role | Background & Skills |
|:---|:---|:---|
| Ijaz Driscoll | Security Engineer | Prior experience in Full-stack/Web3 development. |
| Marco Tsang | Full-stack Engineer | Full-stack development. |

#### LinkedIn Profiles

- [https://www.linkedin.com/ijaz-driscoll](https://www.linkedin.com/in/ijaz-driscoll-9709541b9/)
- [https://www.linkedin.com/marco-tsang](https://www.linkedin.com/in/marco-tsang112/)

#### Github Accounts

- [Ijaz](https://github.com/The-Six)
- [Marco](https://github.com/hkmarcoot)

---

## 📊 Development Status

We completed Astartes-v1 at EasyA x Polkadot London Hackathon. It established the core Merkle Tree creation and basic Polkadot anchoring routine in a limited environment. The current application represents the transition from a simple prototype to an enterprise-focused product by automating all three agents (A, B, C) and integrating enterprise tooling.

---

## 📅 Development Roadmap

| Item | Details |
|:---|:---|
| 🕒 Estimated Duration | 6 months | 
| 👥 FTE Required | The project is structured across 4 internal phases (M1-M4) of 1.5 months each. |
| 💵 Total Costs | $15,000 USD |

---

## 📌 Milestone Breakdown

| # | Deliverable | Specification |
|:---|:---|:---|
| 0a | **License** | MIT License |
| 0b | **Documentation** | Inline code comments and a basic tutorial for deploying the three core servers (A, B, C) on an AWS environment, configuring Cribl routing and connecting to a test Splunk instance. |
| 0c | **Testing & Guide** | Comprehensive unit tests (Rust/Python) for all core functions, plus documentation to simulate a tamper event to verify Server C correctly flags the discrepancy. |
| 0d | **Technical Article** | Documentation on how Astartes.Dot uses Polkadot Asset Hub as an immutable trust anchor for enterprise security logging. |
| 1 | **Core Agent (Server A) MVP** | Develop and unit-test the Rust-based Merkle Root Agent (Server A), including automated interval-based Merkle root generation and local log hashing. Develop the Lambda function (Server B). Finalise the required project management and tooling licenses. |
| 2 | **Verification Engine & Infrastructure** | Complete the core Centralised Verification Logic (Server C). Deploy all three servers (A, B, C) on the secured Cloud Hosting environment. |
| 3 | **Cribl Pipeline & Security Audit** | Fully integrate Cribl Stream as the central data router. Finalise Server C's multi-dimensional verification logic. Complete the required Aikido security scan of our codebase. |
| 4 | **SIEM Integration & Final QA** | Implement and demonstrate the final alert routing from Server C to a test Splunk instance, showing the forensic report payload generated for a simulated log tampering event. Complete High-Load QA and stress testing on Server C. |

---

## 💰 Budget Breakdown

### 📅 Milestone Timeline

| Milestone | Deliverables | Cost (USD) | Estimated Completion |
|:---|:---|:---|:---|
| 1 | Core Agent (M1) | $2,500 | 1.5 months |
| 2 | Verification Engine (M2) | $4,600 | 3 months (1.5 months for M2) |
| 3 | Cribl Pipeline (M3) | $4,850 | 4.5 months (1.5 months for M3) |
| 4 | SIEM Integration (M4) | $3,050 | 6 months (1.5 months for M4) |
| **Total** | | **$15,000** | **6 months** |

### 🧾 Budget Allocation

**Non-Labour Allocation**

| Milestone (M) | Cost Allocation | Percentage | Detailed Breakdown |
|:---|:---|:---|:---|
| M1 (1.5): MVP - Setup & Prototype Astartes Automation | $500.00 | 7.14% | Core Dev Tooling: $500. |
| M2 (1.5): Verification Engine, Testing Infra & Cloud Hosting | $2,600.00 | 37.14% | Cloud Hosting: $1,600. Testing Infra & Data Acquisition: $1000. |
| M3 (1.5): Cribl and Aikido Integration | $2,850.00 | 40.71% | Cribl Platform Fees: $2,350. Akido (Security Scanning): $500. |
| M4 (1.5): SIEM Integration and Final Validation | $1050.00 | 15% | Splunk License: 60-day FREE Trial. Stress Testing: $550. Contingency Fund: $500. |
| **TOTAL** | **$7,000.00** | **100.0%** | |

**Labour Allocation**

| Role | Hours | Rate (USD/hr) | Total (USD) |
|:---|:---|:---|:---|
| Security Engineer | ∞ | $0 | $0 |
| Full-stack Engineer | 208 | $19.23 | $4,000 |
| Contingent Labour Reserve (Sec/Web2/Web3) | 208 | $19.23 | $4,000 |
| **Total** | | | **$8,000** |

---

## 🔮 Future Plans

### 🚀 Post-Grant Development

After we deliver the full end-to-end POC, we will focus on:
- **Agent Packaging:** Creating stable, installable packages for Linux (DEB/RPM) and Windows to expand market reach.
- **Multi-Tenant SaaS Model:** Further developing our multi-tenant architecture.
- **Deploying on Polkadot Mainnet.**

### 💸 Additional Funding Strategy

Upon successful delivery of Astartes-v2, we plan to pursue seed funding to scale marketing and enterprise adoption efforts.

### 🌍 Long-Term Vision

Our vision is to become a powerful new force in security operations. Astartes aims to definitively separate the source of truth from the operational environment with Polkadot as our trust anchor.

---

## ℹ️ Additional Information

### ✅ Completed Work

- Deployed an initial prototype that established the core Merkle Tree creation and basic Polkadot anchoring routine.
- Drafted a preliminary security case for Astartes.
- Established contact with Parity for ongoing collaboration. **Nikolai Kozlov** is our main point of contact. 

### 🏆 Previous Recognition

- **3rd Place** at EasyA x Polkadot London Hackathon.

### 👻 Defence Evasion Techniques:
- [T1070.001](https://attack.mitre.org/techniques/T1070/001/)
- [T1070.002](https://attack.mitre.org/techniques/T1070/002/)
- [T1070.003](https://attack.mitre.org/techniques/T1070/003/)
- [T1565.001](https://attack.mitre.org/techniques/T1565/001/)
