# 📝 CHAIN-TIX

## 🌟 Project Overview

Please provide the following:

Tagline - Turning real-world event memories into on-chain collectibles and scalable loyalty programs.

**Brief Description**:
Chain-Tix is a decentralized ticketing and fan loyalty platform where real-world event attendees mint Proof of Attendance NFTs using secret words shared live at events.
Fans collect these NFTs as lasting proof of loyalty and can unlock exclusive rewards like merch drops.
The system ensures fair distribution (one mint per wallet per event) and future scalability to multiple artists and concerts.

**How Chain-Tix Integrates with Polkadot**:
Chain-Tix leverages Polkadot Asset Hub for low-cost, scalable NFT minting.
We specifically utilize Elastic Scaling to handle thousands of simultaneous mints during major events without gas wars, and Agile Coretime to allow organizers to pre-purchase blockspace for viral or high-traffic concerts.
All metadata and images are stored decentralized on IPFS, aligning with Polkadot’s vision of user-owned Web3.


**Why We Are Interested in Building Chain-Tix**:
We are passionate about creating deeper, lasting connections between artists and their real fans.
Today’s concert memories are lost after a few Instagram posts — Chain-Tix turns them into permanent, verifiable on-chain assets.
We believe Polkadot's unique infrastructure finally makes scalable, affordable, decentralized loyalty programs possible — and we’re excited to be among the first to build this future.

### 🔍 Project Details

**An overview of the technology stack to be used**

- **Blockchain:** Polkadot Asset Hub
- **Smart Contracts:** Solidity (optimized for 49KB size limit)
- **Storage:** IPFS (via Pinata) for NFT metadata and images
- **Frontend:** HTML, CSS, JavaScript (Ethers.js)
- **Wallet Connection:** MetaMask + Polkadot extensions
- **Version Control:** GitHub
- **Testing/Deployment:** Remix IDE, Pinata IPFS Gateway

Future development will migrate to **Moonbase Alpha** to enable richer smart contracts without size restrictions.

---

## 🛠️ Smart Contract Architecture

### 1. SecretCodeManager.sol
- Stores **hashed secret words** securely.
- Verifies secret codes and ensures one mint per wallet.
- `addSecret()` allows infinite event expansion without redeployment.
- `verifyAndMarkUsed()` validates secret + marks usage, returning metadata URI.

### 2. SecretPOAPRouter.sol
- Frontend interacts only with Router.
- Verifies submitted secret words via Manager.
- Calls NFT contract to mint collectible if verification succeeds.

### 3. SecretPOAPNFT.sol
- Minimal ERC-721 contract.
- Minting rights initially with deployer, updated to Router via `updateMinter()`.
- All NFTs point to IPFS metadata.

---

## 🎨 Frontend Architecture

- **Mint Page (index1.html):** Connect wallet, enter secret code, mint NFT.
- **Collectibles Page (collectibles.html):** Fetch and display owned NFTs dynamically from IPFS.
- **Rewards Page (rewards.html):** Display claimable rewards based on number of collectibles.

Frontend uses Ethers.js for blockchain communication and IPFS gateways for media retrieval.

---

## 🧠 Data Models & Core Functions

| Contract | Function | Input | Output |
|:---|:---|:---|:---|
| SecretCodeManager | `addSecret(hashedSecret, uri)` | Hash, Metadata URI | Adds new event secret |
| SecretCodeManager | `verifyAndMarkUsed(hashedSecret, user)` | Hash, Wallet | Verifies + returns URI |
| SecretPOAPRouter | `mintWithSecret(secretWord)` | Secret Word (string) | Mints collectible |
| SecretPOAPNFT | `mint(to, uri)` | Wallet, Metadata URI | Issues NFT |
| SecretPOAPNFT | `updateMinter(newMinter)` | Address | Sets Router as minter |

---

## 🚀 Proof of Concept / MVP

- Smart contracts deployed and tested on Polkadot Asset Hub.
- Full working frontend including:
  - Secret code minting
  - NFT viewing
  - Rewards system based on collectibles
- Metadata stored on IPFS.
- Complete GitHub repository available.
- Loom video demo available (link).

---

## 🧩 How Chain-Tix Uses Polkadot

- **Elastic Scaling:** Handles mass NFT minting during major concerts without congestion.
- **Agile Coretime:** Organizers can pre-purchase blockspace ahead of large events.
- **Low Gas Costs:** Enables affordable minting for every fan.
- **Decentralized Metadata:** All event collectibles are stored permanently on IPFS.
- **49KB Smart Contract Optimization:** Modular design splitting Manager, Router, and NFT contracts.

---

## 🧹 Known Limitations

- Frontend currently deployed only locally (no public hosting yet).
- NFTs are non-transferable — no secondary trading yet.
- No on-chain identity integration yet (Frequency integration planned).
- Advanced organizer dashboards not built yet.
- Smart contracts currently optimized for Asset Hub size limits — richer contracts will be migrated to **Moonbase Alpha** for future releases.

### 🧩 Ecosystem Fit

Help us locate your project in the Polkadot landscape and what problems it tries to solve by answering each of these questions:

- Where and how does your project fit into the ecosystem?
- Who is your target audience?
- What need(s) does your project meet?
- Are there any other projects similar to yours in the Polkadot ecosystem?
  - If so, how is your project different?
  - If not, why might such a project not exist yet?

> **Note**: We prioritize projects building on Plaza/Polkadot Hub, games, and DeFi applications, though all types of projects wile considered.

## 👥 Team

- **Team Name:** Chain-Tix
- **Contact Name:** Pramay Jain
- **Contact Email:** pramay07@bu.edu
- **Website:** pramay07_
### Team members

Mahir Patel

#### LinkedIn Profiles (if available)

- https://www.linkedin.com/in/pramay-jain/
- https://www.linkedin.com/in/mahir-patel21/

### Team Code Repos

https://github.com/mahir-pa/poap

Please also provide the GitHub accounts of all team members:

https://github.com/pramay2007
https://github.com/mahir-pa

# 🎟️ Chain-Tix — Polkadot Fast-Grant Application

---

## 👥 Team Experience

Our team has strong experience building on blockchain ecosystems, particularly around smart contracts, NFT minting flows, decentralized storage, and wallet integrations.  
Previous experience includes:

- Solidity smart contract development (ERC-721, POAP structures).
- Deployment and testing on Polkadot Asset Hub.
- Frontend integrations using Ethers.js and decentralized storage via IPFS.
- Participation in blockchain hackathons focused on NFTs, loyalty systems, and DeFi tools.

Chain-Tix is our next step toward creating scalable, real-world blockchain applications in the live events and entertainment industry.

---

## 📊 Development Status

We have completed a working Proof of Concept (PoC) and MVP:

- Core smart contracts (SecretCodeManager, Router, NFT Minting) are deployed and tested on Polkadot Asset Hub.
- Frontend interface built with HTML/CSS/JavaScript.
- Wallet connection and secret word minting functional.
- Collectibles display and reward claiming system working.
- IPFS-based decentralized metadata hosting for NFTs.
- GitHub Repository: [https://github.com/mahir-pa/poap]

Future phases aim to expand functionality and scalability further.

---

## 📅 Development Roadmap

### Overview

- **Estimated Duration:** 3 months
- **Full-Time Equivalent (FTE):** 1 full-time developer (with part-time support)
- **Total Costs:** $2,000 USD

---

### Milestones and Deliverables

| Number | Deliverable | Specification |
| -----: | :----------- | :------------- |
| 0a. | License | Project will be released under the MIT License. |
| 0b. | Documentation | Inline documentation across all contracts + detailed tutorial on minting and claiming rewards. |
| 0c. | Testing and Testing Guide | Full unit tests for core contracts; testing guide included. |
| 0d. | Article | Publish a Medium article summarizing development, learnings, and next steps. |
| 1. | Moonbase Migration | Deploy core smart contracts on Moonbase Alpha to lift size restrictions, allowing for richer metadata handling and broader scalability. |
| 2. | Artist Dashboard MVP | Build an MVP dashboard where event organizers can see how many collectibles have been minted per event. |
| 3. | Public Frontend Deployment | Deploy full frontend dApp to Netlify/Fleek so users can interact directly without localhost setup. |

---

## 💰 Budget Breakdown

| Milestone | Deliverables | Cost (USD) | Estimated Completion |
| :--- | :--- | :---: | :--- |
| 1 | Moonbase Migration | $1,000 | 1.5 months |
| 2 | Artist Dashboard MVP | $500 | 2 months |
| 3 | Public Frontend Deployment | $500 | 2.5–3 months |
| **Total** |  | **$2,000** | **3 months** |

Funding is intended to cover:
- Developer time (est. $25/hour × 80 hours)
- Infrastructure (IPFS pinning service, hosting costs)
- Minor UI/UX improvements for public readiness

---

## 🔮 Future Plans

After completing the Fast-Grant:

- **Chain-Tix India Launch:**  
  Launch Chain-Tix pilot program in India where ticketing problems are larger and loyalty solutions are highly demanded.  
  Start with 2–3 small concerts/events as test beds, collaborating with independent artists who are highly active but underserved by traditional platforms.

- **Immediate Go-To-Market Strategy:**  
  Upon receiving the grant, we will immediately initiate **marketing and outreach efforts** to onboard independent artists in India.  
  Focus will be on educating artists about on-chain loyalty, offering free POAP collectible drops at their concerts, and gathering real user feedback.

- **Funding Expansion:**  
  Seek additional funding via Moonbeam Foundation grants, Polkadot Treasury, and/or strategic angel investors interested in the Web3 x Events space.

- **Product Growth:**  
  Expand Chain-Tix to integrate fully with Frequency for decentralized identity management.  
  Extend POAP collectibles into tradable loyalty points, interoperable across parachains.

Our long-term vision is to become the **go-to decentralized event loyalty platform for India and then scale globally**.

---

## ℹ️ Additional Information

- Current work deployed and tested live on Polkadot Asset Hub.
- Fully open-source GitHub repository available.
- Frontend and contracts modular and extensible for future feature integrations.
- We have not applied for any other funding yet — this Fast-Grant would be our first external funding to accelerate the platform.

---

# 🏆 Thank You

We are excited to continue building Chain-Tix and contributing to the Polkadot ecosystem’s real-world adoption!

