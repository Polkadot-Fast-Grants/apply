# 📝 Petidot

## 🌟 Project Overview


- **Tagline:** Train, evolve, and explore with your NFT pets on Polkadot.
- PetiDot is an idle blockchain game I built where players can mint unique NFT pets, train them through staking, and send them on adventures to earn rewards. Each pet evolves through age stages, with attributes like rarity, type, and customizable names—making every NFT personal and progression-driven.
- The game is built on the Polkadot Asset Hub, using its smart contract capabilities to manage NFTs and staking mechanics. Future plans include cross-parachain features like pet trading, minigames and more secure randomness.
- I'm a solo developer passionate about web3 gaming. I created PetiDot to show how fun and user-friendly blockchain experiences can be, and Polkadot’s infrastructure made it the ideal choice for scalability, low fees, and innovation.

### 🔍 Project Details

- **Tech Stack:**  
  PetiDot is built using Solidity for smart contracts, deployed on the Polkadot Asset Hub Westend Testnet. The frontend is developed in React and communicates with the chain using Ethers.js. The app is deployed on Cloudflare Pages for fast and reliable delivery.

- **Architecture & Core Components:**  
  - **Smart Contracts:** Handle NFT minting, staking (training), metadata management, and reward logic.
  - **Frontend:** A React-based UI that interfaces with the contracts via Ethers.js, with wallet connection and user-friendly interactions.
  - **Wallet Integration:** Uses MetaMask and compatible wallets for seamless interaction with the Asset Hub.

- **PoC/MVP:**  
  A functional MVP is live at [https://petidot.pages.dev](https://petidot.pages.dev). It includes:
  - NFT minting with randomized attributes
  - Pet staking mechanics (training)
  - Age progression logic
  - Rename functionality
  - UI for interacting with and displaying NFT metadata
- **Mockups/Designs:**  
  The UI is intentionally lightweight and inspired by classic idle games. While no Figma files were created, the live MVP demonstrates the intended design system.
- **Data Models / API Specifications:**  
  - **NFT Metadata Schema:**
    - `id` (uint256): Token ID
    - `name` (string): Customizable pet name
    - `type` (string): Visual/type variation
    - `rarity` (string): Trait rarity
    - `ageStage` (uint8): Evolution stage
    - `isStaked` (bool): Training status
  - All interactions are on-chain with no backend APIs; metadata is handled directly within the contract.
- **What the Project is *Not* / Will *Not* Include:**  
  - PvP, battle mechanics, or advanced competitive gameplay
  - Off-chain game logic or backend server infrastructure

### 🧩 Ecosystem Fit

- **Where and how does your project fit into the ecosystem?**  
  PetiDot brings casual, NFT-driven gaming to the Polkadot ecosystem by leveraging the Polkadot Asset Hub for smart contract execution and NFT management. It showcases the versatility of the network beyond financial applications by introducing a gamified and approachable Web3 experience. Future features will also use Polkadot’s XCM to fetch randomness cross-chain—demonstrating a real use case for cross-parachain communication in gaming.

- **Who is your target audience?**  
  I'm targeting casual gamers, NFT collectors, and newcomers to Web3 who might find traditional blockchain apps too complex or intimidating. PetiDot is designed to be fun, intuitive, and rewarding—even for those who have never played a blockchain game before.

- **What need(s) does your project meet?**  
  PetiDot makes Web3 more approachable and engaging through simple gameplay mechanics and evolving NFT pets. It introduces users to staking, randomness, and on-chain progression in a low-risk, gamified environment. I'm planning to expand the game with a token reward system: players will participate in mini-games, and if they win, they'll earn tokens—randomly weighted based on their NFT’s attributes. These tokens can then be used to open crates with cosmetic upgrades or future gameplay items.

- **Are there any other projects similar to yours in the Polkadot ecosystem?**  
  I haven’t seen other live casual games on the Polkadot Asset Hub with idle mechanics, evolving NFTs, and mini-game-based token rewards tied to cross-chain randomness.

  - **How is your project different?**  
    PetiDot blends simplicity with depth by tying gameplay rewards to NFT traits, creating a personal and progression-driven experience. Planned use of Polkadot’s XCM to pull in cross-parachain randomness for fair token distribution also makes this more than a standalone game—it’s a demonstration of Polkadot’s core tech in action.

  - **Why might such a project not exist yet?**  
    Many Polkadot projects focus on infrastructure, DeFi, or just NFT collections. Casual solo gameplay often gets overlooked, despite its potential for onboarding and ecosystem education. I built PetiDot to fill that space—easy to use, fun to play, and designed to evolve over time with the ecosystem’s capabilities.
## 👥 Team

- **Team Name:** Petidot
- **Contact Name:** Gökay Meriç Şişik
- **Contact Email:** gkydev@proton.me
- **Website:** github.com/gkydev

### Team members

Gökay Meriç Şişik

#### LinkedIn Profiles (if available)

- [https://www.linkedin.com/gkymrc](https://www.linkedin.com/in/gokaymrc)

### Team Code Repos

- https://github.com/gkydev/EasyA-Polkadot-Hackathon

Please also provide the GitHub accounts of all team members:

- https://github.com/gkydev

### Team's experience

I'm a experienced software engineer with deep expertise in blockchain technologies, having worked on numerous projects across the space, including cryptocurrency exchanges and Web3 platforms. My work includes peer-reviewed publications in the field, some of which have been used as teaching material in university-level courses.

## 📊 Development Status

The project is actively being developed, with the current version having been built during the Esaya Hackathon. A functional MVP is already live at https://petidot.pages.dev. The code is hosted on GitHub at https://github.com/gkydev/EasyA-Polkadot-Hackathon, where you can review the smart contract implementation, frontend integration, and ongoing feature additions. This MVP includes NFT minting, pet staking (training), age progression, and basic gameplay mechanics. Future updates will introduce token rewards, mini-games, and cross-parachain randomness via Polkadot's XCM.


## 📅 Development Roadmap

### Overview

- **Estimated Duration:** 2 months
- **Full-Time Equivalent (FTE):** 1
- **Total Costs:** $10,000 USD

| Number | Deliverable | Specification |
| ------ | ----------- | ------------- |
| 0a. | License | MIT |
| 0b. | Documentation | I will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can interact with the crate and mini-game systems. |
| 0c. | Testing and Testing Guide | Core functions (crate opening, token logic, reward claims) will be fully covered by tests. The guide will explain how to run and extend tests. |
| 0d. | Article | I will publish an **article** explaining the how the new tokenomics and NFT-based mini-game reward system was developed. |

---

### Milestone 1 — Core Tokenomics, Crate System & UI Overhaul

- **Estimated Time:** 2 weeks  
- **Amount Requested:** $5,000 USD  

| Number | Deliverable                            | Specification |
|--------|----------------------------------------|---------------|
| 1a.    | **Fungible Token Deployment**          | Launch a game-native token on Asset Hub. This token will be used for crate openings and gameplay interactions. |
| 1b.    | **Crate Opening Mechanism**            | Implement smart contracts to allow users to spend tokens and open crates. Each crate mints a new NFT pet with randomized traits and rarity level. |
| 1c.    | **New Character Variants with Age Design** | Introduce new PetiDot types (e.g., fox, cat, dragon) with age-based stages (baby, teen, adult). Age will evolve visually and influence future gameplay or abilities. |
| 1d.    | **UI Revamp**                          | Redesign the interface to:<br>– Show token balances<br>– Enable crate opening flow<br>– Display newly acquired NFT characters with animated reveal<br>– Reflect character age stages in card visuals |
---

### Milestone 2 — Client Mini-Game, Reward Logic & Mainnet Launch

- **Estimated Time:** 6 weeks  
- **Amount Requested:** $5,000 USD  

| Number | Deliverable                        | Specification |
|--------|------------------------------------|---------------|
| 2a.    | **Client-Only Mini-Game**          | Implement a playful, engaging browser-based mini-game where users select an NFT pet and play short animations. Game result is determined locally (for fun), but reward claims depend on token logic. |
| 2b.    | **Rarity-Weighted Reward Engine**  | Token rewards will be issued based on the rarity and age of the NFT used to play. The smart contract handles all validation, randomness seed, and reward distribution securely. |
| 2c.    | **Randomness Engine**              | Integrate Polkadot’s XCM VRF-based randomness. |
| 2d.    | **Mainnet Deployment**             | Finalize and deploy contracts for token, NFT, crate, and reward logic to mainnet. Conduct full end-to-end test on production. |

## 🔮 Future Plans

After the Fast-Grant, I plan to focus on growing a strong community around PetiDot. The first step will be to build out the project's social media presence and start engaging with early supporters. I’ll be running a token airdrop campaign to help spread awareness and onboard new users into the ecosystem.

As the community grows, I’ll continue expanding the world of PetiDot by introducing new pet types and character variants to keep the experience fresh and engaging. I also plan to add more simple and fun mini-games to increase interactivity and give users more ways to engage with their NFT pets.

To support these growth initiatives, I intend to seek additional funding specifically to scale the airdrop and community-building efforts. My long-term goal is to position PetiDot as a fun and welcoming entry point into the Polkadot ecosystem—accessible for newcomers, yet built on powerful technology that showcases the strengths of Polkadot Asset Hub.

My vision for PetiDot is to create an approachable and playful gateway into the Polkadot ecosystem—something that lowers the barrier for new users while still showcasing Polkadot's capabilities.

## ℹ️ Additional Information

I have already developed an initial version of PetiDot during the EasyA Polkadot Hackathon, which includes NFT minting, simple crate logic, and basic UI interactions. The current implementation is live and open-source on GitHub, demonstrating early technical feasibility and user experience design.

All development has been done solely by me—there are no other contributors or teams involved in the project at this stage.

I have not applied for any other funding sources for this project. This grant application represents the first step toward scaling PetiDot into a community-focused, fun, and technically robust game in the Polkadot ecosystem.
