
# 📝 Direct

## 🌟 Project Overview

**Tagline:**
Fast, low-cost, trustless fiat off-ramping for Web3 users.

**Description:**
Direct is a simple, trustless off-ramping solution built for Web3 users who want to convert their crypto to local fiat currencies quickly and affordably. Initially built as a devnet MVP on Solana, Direct enables users to off-ramp crypto via a web-based interface. Our mission is to simplify the crypto-to-fiat experience — especially for emerging markets — by reducing fees, improving speed, and removing reliance on centralized intermediaries.

With this grant, we aim to integrate Polkadot support, enabling Direct to connect with the broader Polkadot ecosystem and extend its reach across chains using XCM. In time, we intend to support parachains and unlock cross-border off-ramping and payments.

We're building Direct because we believe current off-ramp solutions are too slow, expensive, or centralized — especially for people who rely on crypto as income, such as freelancers or small business owners. Direct is fast, simple, and designed for real-world usage.


---

## 🔍 Project Details

### Technology Stack

* **Frontend:** React + Tailwind (web-based interface)
* **Backend:** Node.js on Railway (hosting & DB infra)
* **Wallet Integration:** Solana and Polkadot.js
* **Smart Contracts:** ink! (for Polkadot); existing Solana integration
* **Future Work:** XCM integration for parachain interoperability

### Core Architecture & Plans

* Users connect their crypto wallet via a secure web interface
* Direct allows them to off-ramp funds by selling supported tokens
* Crypto assets are pooled and converted to fiat, then sent via local methods
* Future APIs and SDKs will enable integration by other apps and wallets

### MVP (Current State)

* Fully functional web-based MVP (devnet, Solana)
* Users can off-ramp tokens through a simple UI
* Core flow includes wallet connect, initiating a request, and simulating payout

<a href="https://drive.google.com/file/d/1SUQk3nQJeRephMHPw09heGk2jPXsiMzo/view?usp=sharing">Demo video</a>

### What Direct *Is Not*

* We are not building a centralized CEX-like product
* We are not a single chain solution; direct plans to become cross chain and support as many people as we can with off ramping their crypto
* We do not work with ALL cryptocurrencies on a blockchain we support: Due to the volatile nature of tokens, we would only support stablecoins.
* We don’t offer fiat on-ramping yet (though this may come later)

---

## 🧩 Ecosystem Fit

### Where and How Does Direct Fit?

Direct brings simple, non-custodial off-ramping to Polkadot. By leveraging ink! contracts and eventually XCM, we enable stablecoin and token holders to easily move value from crypto into their bank or mobile wallets — especially in underserved markets.

### Target Users

* Crypto newcomers and DeFi users
* Freelancers and gig workers in emerging markets (e.g., Africa)
* Small merchants that accept crypto
* Builders who want to integrate fiat off-ramping into their dApps

### Needs Met

* Low-fee, high-speed off-ramping
* Simple UX — no CEX KYC or long waiting times
* Cross-border value transfer (future)
* Developer tools to integrate off-ramping

### Similar Projects in Polkadot?

We’re not aware of any Polkadot-native fiat off-ramping tool that combines trustless architecture with simplicity, speed and focus on emerging markets. Projects like Ramp and Transak are custodial and not tailored to local contexts or Polkadot.

---
## 🚀 Go-to-Market Plan
To reach real users and drive adoption, we plan the following phased approach:

### Phase 1: Polkadot Ecosystem

  * Integrate with wallets like Talisman, Nova, and SubWallet.

### Phase 2: User Acquisition in Emerging Markets

  * Host Twitter Spaces and incentive campaigns (bounties for feedback, referrals and thread contests).

---

## 👥 Team

* **Team Name:** Direct
* **Contact Name:** Adole David Enencheje
* **Contact Email:** adoledavid345@gmail.com
* **Github:** <a href="https://github.com/Willy-Wonka28">Adole David Enencheje</a>

### Team Members

* Adole David Enencheje-Full stack dev/Smart contract
* Prosper Enwerem-Backend engineer
* Oyetibo Olaoluwa-Frontend developer

### LinkedIn Profiles

* <a href="https://www.linkedin.com/in/david-adole-887057304/">Enenche's LinkedIn</a>
* <a href="https://www.linkedin.com/in/prospercoded//">Prosper's LinkedIn</a>

### GitHub Repos

* <a href="https://github.com/Willy-Wonka28/Direct/">Github Repo</a>

### GitHub Accounts

* https://github.com/Willy-Wonka28
* https://github.com/ProsperCoded
* https://github.com/TechProoo

### Team Experience

Our team consists of three student developers with experience across Solana, Sei, and ink!. We've built tools spanning AI and Web3, and participated in 4+ hackathons where we consistently placed among the top teams. We’ve shipped working prototypes, pitched at finals, and built everything from smart contracts to frontend UIs.

Enenche, our product lead, is active in the blockchain ecosystem through DAOs like Rootstock, Superteam, and Base. He has written and deployed an ink! contract, and authored a technical tutorial on it. We're comfortable with the Substrate/Polkadot stack and confident in our ability to deliver production-ready tools.

We’re deeply motivated to build useful crypto infrastructure for real users — especially in emerging markets. This grant is a crucial step toward making that a reality on Polkadot.

---

## 📊 Development Status

* MVP complete on Solana (devnet, web UI)
* Wallet integration and transaction signing working
* Backend infra deployed via Railway
* Planning architecture for ink! contract integration and token management

---

## 📅 Development Roadmap

### Overview

* **Estimated Duration:** 3 months
* **FTE:** \~0.5 (3 part-time devs, \~2 hrs/day, 6 days/week)
* **Total Costs:** \$10,000 USD

| Number | Deliverable                     | Specification                                                                            |
| ------ | ------------------------------- | ---------------------------------------------------------------------------------------- |
| 0a.    | License                         | Apache 2.0                                                                               |
| 0b.    | Documentation                   | Inline code docs and a tutorial on wallet connection and transaction flow                |
| 0c.    | Testing and Testing Guide       | Full unit tests for smart contract, backend API, and wallet flows                        |
| 0d.    | Article                         | A technical write-up covering our Polkadot integration and lessons learned               |
| 1.     | Smart Contract & Wallet Support | ink! contract for holding/converting tokens; Polkadot wallet integration (connect, sign) |
| 2.     | Off-Ramp Flow                   | Enable users to off-ramp from the Polkadot main chain to fiat with simple/familiar UI    |
| 3.     | Test & Deploy                   | Test contracts, backend infra (Railway), connect to frontend and run in real-world trial |

---

### 💰 Budget Breakdown

| Milestone | Deliverables                                                  | Cost (USD)   | Estimated Completion |
| --------- | ------------------------------------------------------------- | ------------ | -------------------- |
| 1         | ink! smart contract, wallet integration, backend logic        | \$5,000      | 1.5 months           |
| 2         | Full off-ramp flow, frontend, and testing in live environment | \$5,000      | 1.5 months           |
| **Total** |                                                               | **\$10,000** | **3 months**         |

## 💸 Detailed Cost Allocation

| Item                                      | Cost (USD) |
|-------------------------------------------|------------|
| Engineering (frontend/backend/contract)   | $6,000     |
| Smart contract audit + testing            | $1,000     |
| Hosting & infrastructure (Railway, etc.)  | $750       |
| Legal incorporation and filings           | $75        |
| User research and real-world testing      | $1,000     |
| Community & growth (initial GTM push)     | $1,175     |

**Total: $10,000**

---

## 🔮 Future Plans

After the grant:

* Integrate XCM to support multiple parachains
* Expand to other African countries and eventually expand to other continents
* Build SDKs and APIs for third-party wallet/dApp integration
* Partner with DEXs, CEXs, and wallets to power embedded offramping
* Add support for local payout providers (e.g., M-Pesa, bank APIs)
* Improve on-chain treasury logic for auto-balancing stablecoins and volatile tokens

We also plan to apply for additional funding — whether through follow-up grants or VC — to scale our infra and operations.

---

## ℹ️ Additional Information

* MVP available on Solana devnet
* All three members are active developers, working part-time as students
* Legal setup is pending; part of the grant will cover that
* We’ve previously built to Web3 projects on Solana and Sei
