# 📝 MetaVault

## 🌟 Project Overview

- Tagline: Empowering users to control and aggregate their cross-platform data with Web3-powered consent.
- Description: MetaVault is a Web3-native data aggregation tool that collects metadata from multiple platforms (e.g., social, media, productivity) and empowers users to control access to their data via wallet-based authentication and smart contract-driven consent logs.
- Polkadot Integration: The platform leverages Polkadot’s ecosystem for scalability, security, and modularity. Smart contracts are deployed on a Polkadot-compatible chain with off-chain storage (IPFS) and Polkadot wallets for user control.
- Team Motivation: We are deeply aligned with the mission of decentralization and data sovereignty. Our team is passionate about building tools that give power back to users in a privacy-preserving way.
- https://drive.google.com/file/d/1yP1dDpl1Q-HOhCgGGlpQavR3Cnr84V2f/view?usp=sharing


### 🔍 Project Details
Technology Stack:
- Frontend: React + Ethers.js + MetaMask
- Backend: Node.js, Express
- Smart Contracts: Solidity (Ink! migration planned)
- Off-Chain Storage: IPFS or Ceramic
- Wallet Integration: Polkadot.js and MetaMask (via Substrate compatibility layer)


Architecture:
- Wallet-based auth with message signing
- Smart contract for managing data consent logs (grant/revoke)
- Metadata connectors fetching and standardizing platform data
- Dashboard to visualize and manage data access

PoC: Wallet auth + consent signing UI demo completed (HTML + Ethers.js demo available)

UI Mockups: Included in repo / available upon request


API Spec:
- GET /user/data
- POST /consent/grant
- POST /consent/revoke

Not in Scope:
- We are not storing raw user content, only metadata
- We are not building a Polkadot parachain in this phase

### 🧩 Ecosystem Fit

Help us locate your project in the Polkadot landscape and what problems it tries to solve by answering each of these questions:
- Placement: A new layer of user-controlled data aggregation and sharing for Web3 apps and services
- Target Audience: Privacy-conscious users, developers building dApps, researchers looking for ethically-sourced data


Needs Met:

- Consent-driven access to data
- Aggregation across Web2 and Web3 platforms
- Interoperability with dApps and identity protocols


Similar Projects:

- None in the Polkadot ecosystem currently offering aggregation + consent as a service

- Most projects focus on identity (e.g., KILT), not granular data control



> **Note**: We prioritize projects building on Plaza/Polkadot Hub, games, and DeFi applications, though all types of projects will be considered.

## 👥 Team

- **Team Name:** MetaVault Labs
- **Contact Name:** Jason Okorie
- **Contact Email:** jason.c.okorie@gmail.com

- **Contact Name:** Innocent Nortey
- **Contact Email:** youngjr1232@gmail.com
- **Website:**  https://github.com/jasonokorie/metavault-labs

### Team members

- Jason Okorie
- Innocent Nortey

#### LinkedIn Profiles (if available)

- [https://www.linkedin.com/{person_1}](https://www.linkedin.com/in/jasonokorie)
- [https://www.linkedin.com/{person_2}](https://www.linkedin.com/in/innocent-nortey/)

### Team Code Repos
- https://github.com/jasonokorie/metavault-labs 

Please also provide the GitHub accounts of all team members:

- [https://github.com/{team_member_1}](https://github.com/jasonokorie/)
- [https://github.com/{team_member_2}](https://github.com/innocentnortey/)

### Team's experience

- Lead Lab Coordinator at Terrapin Works
- Product Engineer Intern at Apple
- Product Manager Intern at Honeywell
- Computer Information Science at the University of Maryland

- Test Automation Engineer at John Deere
- Computer Engineering at the University of Massachusetts Lowell

## 📊 Development Status

- Frontend wallet integration prototype is complete (auth + signature)
- Smart contract outline complete and being ported to Ink!
- Flowchart, architecture diagram, and use case documentation in place
  
## 📅 Development Roadmap

This section should break the development roadmap down into milestones and deliverables. Since these will be part of the agreement, please describe *the functionality we should expect in as much detail as possible*, plus how we can verify and test that functionality.

**Important notes:**
- Frontend wallet integration prototype is complete (auth + signature)
- Smart contract outline complete and being ported to Ink!
- Flowchart, architecture diagram, and use case documentation in place

### Overview

- **Estimated Duration:** 3 months
- **Full-Time Equivalent (FTE):**  2
- **Total Costs:** $10,000 USD

> Note that deliverables 0a to 0d are mandatory. Please adapt their specification to your project.

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | Apache 2.0 / GPLv3 / MIT / Unlicense |
| 0b. | Documentation | Inline comments + user guide + README tutorial |
| 0c. | Testing and Testing Guide | Unit tests and contract tests (Truffle/Hardhat) |
| 0d. | Article | Publish on Medium: "User-Controlled Data Aggregation with MetaVault" |
| 1. | Wallet-based Auth & Consent | React frontend w/ MetaMask + message signing + user dashboard |
| 2. | Consent Smart Contract | Solidity-based contract for granting and revoking data access permissions + test coverage |


### 💰 Budget Breakdown

Please provide a breakdown of your budget by milestone:

| Milestone | Deliverables | Cost (USD) | Estimated Completion |
| --- | --- | --- | --- |
| 1 | Wallet Auth + Dashboard | $5,000 | 1.5 months |
| 2 | Smart Contract + Storage Hooks | $5,000 | 1.5 months |
| **Total** | | **$10,000** | **3 months** |

## 🔮 Future Plans

Please include:
- Expand to include Substrate-native contracts and wallet support (Polkadot.js)
- Partner with ecosystem identity tools (e.g., KILT) for verified credential flow
- Apply for larger grant / VC support after MVP validation
- Launch integrations with dApps that require user-sourced data (e.g., DAO tools, research platforms)

## ℹ️ Additional Information

Here you can add any additional information that you think is relevant to this application, such as:

- Work you have already done
- If there are any other teams who have already contributed to the project
- Other funding you may have applied for

Remember that the Fast-Grants Programme is designed as a first step for promising projects. We're looking for projects that can continue to grow beyond this initial funding.

