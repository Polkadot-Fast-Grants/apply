# 📝 Cartpool

## 🌟 Project Overview

> **Tagline:**  
> _"Shop smarter, together. Pool your carts, unlock group deals, powered by trustless contracts."_

**CartPool** is a consumer-focused cart pooling application that allows multiple users to **pool their shopping carts** to collectively unlock offers, discounts, or bulk deals that wouldn’t be available to them individually. Once pool conditions (like minimum item quantity or participant count) are met, a **smart contract** is triggered to finalize the order.

### 🔗 Built on Polygon

CartPool starts on **Polygon** for its **EVM compatibility**, **low transaction fees**, and smooth onboarding for Web2 users. As we scale, we plan to migrate to **Polkadot**, using **Astar zkEVM** for better cross-chain capabilities and even lower gas costs.



### 🎯 Why We're Building This

- Bulk discounts and group offers are often exclusive to larger buyers.
- CartPool **democratizes** access to deals by enabling **collaborative purchasing**.
- Smart contracts enforce **transparency**, **fairness**, and **immutability** in group purchases.
- We simplify Web3 adoption for everyday users through **wallet abstraction** and **invisible blockchain interactions**.



## 🔍 Project Details

### 🧱 Tech Stack

| Layer        | Technology                      |
|--------------|----------------------------------|
| Frontend     | React + Tailwind CSS             |
| Backend      | Node.js + Firebase               |
| Smart Contract | Solidity (on Polygon Mumbai testnet) |
| Wallet       | Web3Modal + Burner Wallet option |
| Events       | Firebase backend listening to contract events |
| API Layer    | RESTful mock API (for MVP testing) |


### 🧩 Core Components
#### Smart Contracts
- **`CartPool.sol`**: Core contract for pool lifecycle logic
- **Structs**: Represent each cart pool with:
  - Minimum members
  - Item count
  - Deadline
- **Pool States**: `Open`, `Filled`, `Closed`
- **Events**: `PoolCreated`, `PoolJoined`, `PoolTriggered`

#### 🔥 Firebase Backend
- Authentication & session management
- Event listeners for smart contract triggers
- Webhook handlers for mock merchant APIs

#### 🖥 React Frontend
- Create & join cart pools
- View pool progress and statuses
- Trigger checkout once pool is ready


### 🚫 What This Project Is Not

- ❌ Not a full e-commerce platform  
- ❌ No payment processing or stablecoin integration initially  
- ❌ No DeFi tokens, NFTs, or yield mechanics  
- ❌ No required user wallets (unless opted-in)  



### 🧩 Ecosystem Fit

**Focus:** Consumer retail + social shopping  
**Gap:** No comparable Polkadot-based solution exists  

### 🎯 Target Users

- Web2 online shoppers  
- Users in countries like India, SEA where group buying is popular  
- Privacy-conscious users looking for transparent pooling  


### 🎯 User Needs Met

- ✅ Trustless collaborative purchasing  
- ✅ Access to bulk discounts with low barriers  
- ✅ Smart contract enforcement of pool rules  



### 🧠 Similar Projects

- Ethereum/Shopify-based group deals exist  
- Lack decentralized governance & transparency  
- No contract-enforced pooling logic  


### 🤔 Why This Doesn't Exist Yet

- Blockchain onboarding is a hurdle for casual users  
- **CartPool** solves this with walletless access & abstracted interactions  


## 👥 Team

- **Team Name:** Rise Labs
- **Contact Name:** Neha Koottummelkkattil Joseph
- **Contact Email:** nehajosephk1@gmail.com

### Team members

- Neha Koottummelkkattil Joseph

### LinkedIn Profiles (if available)

- [LinkedIn](https://www.linkedin.com/in/neha-joseph-00b2952a4/)


### Team Code Repos

- [GITHUB TEAM CODE REPOS](https://github.com/nehajosephh/RISE-LABS)

Please also provide the GitHub accounts of all team members:

- [GITHUB TEAM MEMBER](https://github.com/nehajosephh)

### Team's experience
-Full-stack dev (React, Node.js) 
-Solidity dev
-Data Science enthusiast


## 📊 Development Status

- ✔️ Idea & Architecture Phase  
- ✔️ Solidity smart contract skeleton done

## 📅 Development Roadmap

### Overview

- **Estimated Duration:** Duration of the whole project (maximum 3 months)
- **Full-Time Equivalent (FTE):**  2
- **Total Costs:** 10000 USD
- 


| Deliverable             | Specification                                             |
|-------------------------|-----------------------------------------------------------|
| 0a. License             | MIT                                                       |
| 0b. Documentation       | Inline comments + user tutorial                           |
| 0c. Testing             | Unit tests for all smart contract logic                   |
| 0d. Article             | Medium article explaining design and UX                   |
| 1. Smart Contract MVP   | `CartPool.sol` implementation + testnet deployment        |
| 2. Frontend & Backend   | Pool UI, Firebase event listening, order simulation       |
| 3. Order Trigger Simulation | Mock merchant integration, full pool lifecycle simulation |

### 💰 Budget Breakdown

| Milestone    | Deliverables                               | Cost    | Duration     |
|--------------|--------------------------------------------|---------|--------------|
| 1            | Smart contract MVP                         | $5,000  | 1.5 months   |
| 2            | Frontend + Backend + Mock API Integration  | $5,000  | 1.5 months   |
| **Total**    |                                            | **$10,000** | **3 months** |



### 🔮 Future Plans

-  Transition to **Polkadot / Astar zkEVM** for cross-chain scalability  
-  Partner with retailers for real cart pooling offers  
-  Add **fiat onramps** via Transak/Biconomy  
-  Apply for **Gitcoin / Astar** grants  
-  Build **mobile app** with group messaging support  
-  Add **AI-driven pool suggestions** & dynamic pricing  

### Additional Information

 - **Open-source** from day one  
-  **Community collaboration** welcome  
-  **Web2 <-> Web3 bridge** without friction  
-  **Smart contract** = source of truth for pool state  
