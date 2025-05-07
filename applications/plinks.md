# 📝 Name of your Project

**Plinks – 1-Click Payment Links for Polkadot Asset Hub**

## 🌟 Project Overview

**Tagline:** Simple, shareable crypto payment links for Polkadot – like Solana Blinks but for Polkadot Asset Hub.

**Description:**  
Plinks is a web app that allows users to generate and share payment links for DOT and other Asset Hub tokens. These links enable one-click payments using MetaMask on Polkadot’s EVM-compatible Asset Hub. Plinks simplifies crypto transactions for both requesters and payers by abstracting away wallet addresses and manual transfer steps.

**Polkadot Integration:**  
Plinks is natively deployed on the **Polkadot Asset Hub**, using a Solidity smart contract that tracks payment requests and completions. The app leverages the EVM compatibility of Asset Hub, allowing for seamless MetaMask interaction.

**Why we’re building this:**  
Polkadot lacks user-friendly tools for basic payment use cases. We saw an opportunity to build something as simple and viral as PayPal.me for crypto, unlocking new utility for DOT and other tokens on the Asset Hub.

**Video Pitch (1 min):**  
https://www.tella.tv/video/polkadot-payment-links-made-easy-6273

## 🔍 Project Details

**Tech Stack:**

- **Frontend:** React + TypeScript, Tailwind CSS  
- **Smart Contract:** Solidity contract deployed on Polkadot Asset Hub  
- **Web3 Integration:** Ethers.js + MetaMask  
- **Blockchain:** Polkadot Asset Hub (EVM-compatible)

**Core Components:**

- `Plinks.sol` contract to log payment requests and completion  
- React app to generate links and handle user flow  
- `contractService.ts` to interface with blockchain  
- MetaMask wallet integration for users to pay with one click

**MVP Link:**  
[Blockscout Contract](https://blockscout-asset-hub.parity-chains-scw.parity.io/address/0x1CdaB5E4Ed70c52B73080CDA83c943790f2eDB95?tab=txs)

**UI Mockups:** Live in the demo video above.

**Exclusions:**  
We do not handle custodial wallets or fiat on-ramps. Plinks focuses only on generating and interacting with payment links via MetaMask.

## 🧩 Ecosystem Fit

- **Fit:** This is a practical onboarding tool that brings new users and use cases to Polkadot by simplifying peer-to-peer payments.  
- **Target Audience:**  
  - Individuals or creators requesting payment (e.g., freelance, tips, donations)  
  - Users who need to send crypto payments without complex wallet setups  
- **Needs Met:**  
  - Simple UX for sending/receiving DOT and WND  
  - EVM-based usability with Polkadot’s speed and fees  
- **Similar Projects:** None in the Polkadot ecosystem with the same focus on MetaMask-based 1-click payments via links  
- **Why this gap exists:** Payment UX in Polkadot has mostly targeted dApps and infrastructure—not simple, user-facing tools

## 👥 Team

- **Team Name:** Plinks  
- **Contact Name:** Hitarth Khurana  
- **Contact Email:** hitarth@uwaterloo.ca
- **Website:** https://github.com/hitarthkhurana/plinks

### Team members

- Hitarth Khurana (Co-President of Waterloo Blockchain)

**LinkedIn:**

- https://www.linkedin.com/in/hitarthkhurana/  

**GitHub Repos:**

- https://github.com/hitarthkhurana/plinks  

**GitHub Handles:**

- https://github.com/hitarthkhurana  

**Team Experience:**  
Computer Science at the University of Waterloo with strong experience building in the Polkadot and Solana ecosystems. Current Co-president of Waterloo Blockchain. Prior work includes hackathon-winning projects, Web3 integrations, and smart contract development. Currently working at Axal and BitGo. Previously worked at Mach Exchange.

## 📊 Development Status

A full MVP is complete and deployed on Asset Hub. Demo available here:  
https://www.tella.tv/video/polkadot-payment-links-made-easy-6273  
Smart Contract: [Blockscout Link](https://blockscout-asset-hub.parity-chains-scw.parity.io/address/0x1CdaB5E4Ed70c52B73080CDA83c943790f2eDB95?tab=txs)

# 📅 Development Roadmap

### Overview

- **Estimated Duration:** 3 months  
- **FTE:** 1.5  
- **Total Costs:** $10,000 USD

| Number | Deliverable | Specification |
| ------ | ----------- | ------------- |
| 0a | License | MIT |
| 0b | Documentation | We will provide inline code documentation and a basic tutorial on using Plinks to send/receive DOT. |
| 0c | Testing & Guide | Unit tests for smart contracts and front-end functionality will be written and documented. |
| 0d | Article | We'll publish an article describing how we built Plinks and how it improves payment UX on Polkadot. |
| 1 | Project Kickoff + Core MVP | This milestone is considered delivered at the time of grant acceptance. It covers: (1) Project kickoff, (2) Smart contract deployment to Asset Hub, and (3) UI for link creation and MetaMask-based payments. |
| 2 | QR Codes + Transaction History | Add support for QR code generation for payment links, and display a user’s payment history fetched from the contract. |

### 💰 Budget Breakdown

| Milestone | Deliverables | Cost (USD) | Estimated Completion |
| --------- | ------------ | ---------- | --------------------- |
| 1 | Project Kickoff + MVP (upon grant acceptance) | $5,000 | Grant acceptance |
| 2 | QR Codes + History | $5,000 | End of Month 3 |
| **Total** |  | **$10,000** | **3 months** |

## 🔮 Future Plans

- Implement Solana Blinks-style “Tweet-to-Pay” functionality  
- Support more tokens beyond DOT/WND  
- Release a mobile version of the app  
- Partner with creator platforms to integrate Plinks as a payment method  
- Seek additional support from the Polkadot Ecosystem or participate in follow-on programs like Decentralized Futures

## ℹ️ Additional Information

- Project was initially built for the EasyA Harvard Hackathon  
- Fully working MVP with live contract on Asset Hub  
- We have not received any prior funding for this project  
- We believe Plinks can serve as a foundational payment layer for individuals and creators using Polkadot
