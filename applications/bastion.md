# 📝 Name of your Project

**Bastion Protocol**

## 🌟 Project Overview

**Tagline:** Community-powered savings and lending with embedded identity and rewards on Polkadot.

**Brief Description:**  
Bastion Protocol is a **community finance super-wallet** built on Polkadot Asset Hub with native USDC support. It allows small groups to form circles for **pooled savings, micro-lending, and dynamic rewards**, underpinned by decentralized identity and reputation. Users can save, borrow, and earn together in a frictionless mobile-first app.

**Polkadot Integration:**  
- Built natively on **Polkadot Asset Hub** with USDC.  
- Smart contracts in **ink!**, with optional cross-chain messaging (XCM) for extensions.  
- Identity verification via **KILT Protocol**.  
- Rewards as **NFTs on Asset Hub** or **Unique Network**.  

**Team Interest:**  
We’ve experienced firsthand the pain of fragmented community finance tools (informal lending circles, ROSCAs, and migrant remittances). Bastion Protocol is our attempt to bring these global use cases to Polkadot, powered by secure, interoperable, and user-friendly primitives.

### 🔍 Project Details

- **Technology Stack**:  
  - **Frontend:** Next.js + TailwindCSS (mobile-first PWA)  
  - **Wallet Integration:** SubWallet SDK / walt.id embedded wallet  
  - **Smart Contracts:** ink! v6.x on Asset Hub-compatible parachain  
  - **Database:** Supabase (for off-chain metadata & reputation tracking)  
  - **Identity:** KILT Protocol for verifiable credentials  
  - **Rewards:** NFT issuance via Asset Hub / Unique Network

- **Core Components:**  
  1. Circle creation & pooled savings contracts  
  2. Micro-lending logic (loan requests, repayments, caps)  
  3. Reputation scoring (on-chain + off-chain hybrid)  
  4. Rewards module (NFT badges + points)  

- **PoC/MVP:**  
  Initial MVP will allow:  
  - Create/join a circle  
  - Deposit USDC into shared pool  
  - Request and repay micro-loans  
  - Receive NFT reward on successful repayment

- **What Bastion Protocol is not:**  
  - Not a high-yield DeFi product (focus on community utility)  
  - Not a DAO treasury management suite  
  - Not a crypto exchange

### 🧩 Ecosystem Fit

- **Fit in Ecosystem:** Bastion Protocol bridges real-world community finance needs (savings circles, migrant remittances, student lending clubs) into Polkadot via Asset Hub.  
- **Target Audience:** Students, migrant workers, village/community co-ops, and DAOs seeking lightweight credit/savings solutions.  
- **Needs Met:** Trustworthy community savings & lending with embedded wallets and verifiable credentials.  
- **Differentiation:** Unlike existing DeFi lending markets (Parallel, Acala), Bastion Protocol focuses on **small circles + social trust + DID-based reputation**. No direct equivalent exists in Polkadot today.

## 👥 Team

- **Team Name:** Bastion Labs  
- **Contact Name:** Kunal Drall  
- **Contact Email:** kunaldrall29@gmail.com  
- **Website:** https://github.com/kunal-drall/powergrid_network

### Team members

- **Kunal Drall** – Project Lead & ink! Smart Contracts Engineer

#### LinkedIn Profiles
- https://linkedin.com/in/kunaldrall

### Team Code Repos
- https://github.com/kunal-drall/powergrid_network
- https://github.com/kunal-drall/EducateFi
- https://github.com/kunal-drall/curachain

### Team’s experience
Kunal is a proven blockchain architect and Polkadot Fast Grant recipient with strong ink!/Substrate expertise.  
- **PowerGrid Network:** Polkadot Fast Grant recipient (decentralized virtual power plant)  
- **EducateFi:** Blockchain-powered education finance prototype  
- **CuraChain:** Healthcare blockchain platform  
- **ISA Solarthon Winner (3rd Position):** Blockchain-based solar forecasting system  
- **Technical Expertise:** ink! smart contracts, Substrate, Rust, tokenomics, cross-chain design

## 📊 Development Status
- Initial research & architecture defined.  
- UI mockups for circle creation & lending prepared.  
- Test environment ready with USDC on Asset Hub.  
- Prototype flow: deposit → borrow → repay → NFT reward.
- <img width="775" height="485" alt="image" src="https://github.com/user-attachments/assets/ca72e36d-201c-4410-966d-d5b60b72efb3" />
- <img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/a8456865-c978-467e-b758-bd7e2115fcae" />



## 📅 Development Roadmap

### Overview
- **Estimated Duration:** 2 months  
- **FTE:** 1.0 (Kunal full-time)  
- **Total Costs:** $10,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | MIT License |
| 0b. | Documentation | Inline docs + tutorial for creating/joining a circle, depositing USDC, borrowing, repaying |
| 0c. | Testing and Testing Guide | Unit + integration tests for pool creation, deposits, loans, repayments |
| 0d. | Article | Publish blog post on Bastion Protocol’s approach to community finance on Polkadot |
| 1a. | Circle Creation & Pooling | ink! contract for circle creation + pooled USDC deposits; Frontend UI for joining/creating a circle and viewing balances |
| 1b. | Micro-lending Logic | Borrow/repay function with repayment limits; Circle-based lending flows integrated into UI; Loan tracking with repayment history |
| 2a. | Rewards Module | NFT issuance upon repayment + simple off-chain reputation counter integrated in dashboard; Display badges/reputation in UI |
| 2b. | Integration & Testing | End-to-end integration of wallet (SubWallet), smart contracts, and frontend flows; Full testing and deployment on testnet |

### 💰 Budget Breakdown

| Milestone | Deliverables | Cost (USD) | Estimated Completion |
| --- | --- | --- | --- |
| 1 | Circle Creation & Pooling + Micro-lending Logic | $5,000 | 1 month |
| 2 | Rewards Module + Integration & Testing | $5,000 | 1 month |
| **Total** | | **$10,000** | **2 months** |

## 🔮 Future Plans
- Expand reputation system with KILT credentials  
- Add yield integration (Bifrost liquid staking for savings)  
- Extend to DAOs for treasury micro-loans  
- Seek additional ecosystem funding + VC partnerships for scaling

## ℹ️ Additional Information
- Prior work includes PowerGrid Network (Polkadot Fast Grant winner).  
- MVP will be open-sourced.  
- Potential collaborations with KILT, Bifrost, and Unique Network.

