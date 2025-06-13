# 📝 Tracelet

## 🌟 Project Overview

**Tagline:** A lightweight analytics dashboard for Polkadot wallets — track on-chain activity at a glance.

**Project Description:** Tracelet is a wallet activity feed and analytics tool designed for the Polkadot ecosystem. It offers users a clean, visual dashboard to monitor wallet events including token transfers, staking operations, governance participation, and contract interactions. Think of it as a "Polkadot Etherscan + Notion Activity Feed" hybrid — designed for clarity and built with real users in mind.

The goal is to improve transparency and user trust in Polkadot dApps by making wallet activity easy to understand, audit, and share.

**Realtion to Polkadot:** racelet is being built natively for the Polkadot Hub and surrounding parachains. It leverages Substrate indexers (like SubQuery or Subsquid) to fetch wallet data, and will integrate directly with Polkadot.js wallets for a seamless experience.

**Why I'm Building This:** As a frontend engineer and Web3 builder, I've always found wallet activity to be scattered and unintuitive. I want to create a tool that simplifies this — both for users and developers. I believe Tracelet can become a standard utility in the Polkadot toolchain, especially as activity grows.

### 🔍 Project Details

#### 🔧 Technology Stack

- **Frontend:** React + TailwindCSS + Typescript
- **Wallet Integration:** polkadot.js extension
- **Backend/Indexing:** SubQuery (or optionally, Subsquid)
- **Data Source:** Polkadot.js API or Subscan API for wallet activity
- **Analytics:** PostgreSQL or Supabase for user metrics (non-custodial and privacy-respecting)
- **Deployment:** Vercel or Vultr
- **Storage (Optional):** Supabase or SQLite (for bookmarks and local history)

#### 📚 Architecture

- **Data Layer:** SubQuery indexing for historical and real-time wallet activity.
- **API Layer:** Lightweight Node.js/Express proxy server for backend filtering and pagination.
- **UI Layer:** Next.js frontend with dynamic components for wallet activity and timeline.

#### 📚 Core Features:

- Wallet activity timeline
- Filter by event type (transfer, staking, governance, etc.)
- Shareable public activity URLs
- Event aggregation charts and basic analytics

🧪 MVP / Prior Work
Currently in ideation. No public code yet — development will begin after grant approval.

🖼️ Mockups / UI Inspiration
Inspired by apps like [Zapper](https://zapper.xyz/) and DeBank feed, but simplified. Clean timeline UI with event icons and descriptions.

📉 Limitations
- Tracelet is not a block explorer
- It won’t index its own data at launch — will rely on existing APIs
- It won’t support every parachain at launch — priority will be given to Polkadot Hub + top parachains
- No write interactions or contract deployment features


### 🧩 Ecosystem Fit

#### Where it fits

Tracelet is more than just a tool for individual users — it's an infrastructure piece that supports transparency, user education, and ecosystem usability. Here's how it brings lasting value:

🧭 **1. Improves UX Across dApps**

Most Polkadot dApps rely on users manually checking Subscan or explorer logs to understand what’s happening with their wallet. Tracelet simplifies this into a clean, human-readable timeline that can be embedded in any Polkadot dApp or wallet.

This reduces user confusion and support tickets while improving trust and onboarding.

🔄 **2. Makes On-Chain Activity Understandable**

As governance and staking grow more complex, users need better visibility into what they’ve voted on, what rewards they’re receiving, and how active they’ve been. Tracelet serves as a personalized audit trail, especially useful for voters, nominators, and grant-funded builders.

🔌 **3. Developer-Friendly Building Block**

Tracelet is built to be modular and open-source. Future dApps can:

- Embed activity timelines
- Hook into wallet-based notifications
- Use the analytics layer to enrich user dashboards
- This makes Tracelet a reusable base for ecosystem tools, not just a standalone app.

📊 **4. Foundation for Polkadot User Analytics**

Tracelet opens the door for deeper ecosystem insights — without violating user privacy. As adoption grows, it could help surface:

- Most active parachains by wallet activity
- Governance participation patterns
- Ecosystem-wide behavioral trends

🛠 **5. Community Ownership and Contribution**

As an open-source project, Tracelet can become a shared utility that the community improves over time — especially with good docs, contributor-friendly architecture, and issue labeling.

#### Target Audience

- Individual Polkadot users
- Delegators and nominators
- Governance participants
- Devs needing a tool to help users track wallet activity across dApps

#### Needs it solves

- Makes wallet activity human-readable
- Offers simple analytics to help users see what they’ve done on-chain
- Gives transparency tools to small teams building in the ecosystem

#### Similar Projects:
There are analytics dashboards for Ethereum (like Etherscan's portfolio, DeBank, Zapper), but nothing similarly user-focused in Polkadot. Subscan exists but is geared toward power users. Tracelet will be clean, focused, and lightweight — ideal for regular users.

## 👥 Team

- Team Name: Tracelet Labs (solo project for now)
- Contact Name: Joshua Moses
- Contact Email: mosesjoshua350@gmail.com
- Website: https://github.com/J0shcodes/tracelet

### Team members

#### LinkedIn Profiles (if available)

https://www.linkedin.com/in/joshua-moses-4117a7209/

### Team Code Repos

- https://github.com/J0shcodes/tracelet

### GitHub Accounts

- https://github.com/J0shcodes

### Team's experience

I’m a frontend engineer with over 4 years of hands-on experience building scalable, user-focused web applications. My work spans real-time UIs, Web3 wallet integrations, and blockchain-based platforms. I've worked with tools like React, Next.js, TailwindCSS, and integrated Web3 functionality such as wallet authentication and on-chain data displays.

I’ve also authored technical guides for the Celo Foundation, covering smart contract deployment and governance participation — an experience that deepened my understanding of blockchain protocols and their user-layer implications.

Now, I’m excited to apply these skills to the Polkadot ecosystem by building a tool that improves transparency and UX for everyone interacting with wallets and dApps.

## 📊 Development Status

The Tracelet repository has been created and initial planning is underway. I’m currently outlining the architecture and defining the user flow and component structure. I haven’t begun development or indexing yet, but I’ve identified the tools and APIs I’ll be using — including SubQuery for indexing and Polkadot.js for wallet address handling.

Once the grant is approved, I plan to begin with the wallet activity feed MVP and deliver an open-source, fully documented first milestone within the first 3 weeks.

## 📅 Development Roadmap

### Overview

- **Estimated Duration:** 2 months
- **Full-Time Equivalent (FTE):** 1
- **Total Costs:** $10,000 USD

#### Milestone 1 – Activity Feed MVP

- Estimated Duration: 4 weeks
- FTE: 1
- Costs: $5,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | MIT |
| 0b. | Documentation | Inline documentation for core components; tutorial for connecting wallet and viewing your feed |
| 0c. | Testing and Testing Guide | Unit tests for wallet fetch logic, activity renderer, and filter components. Guide included. |
| 0d. | Article | A blog post explaining the project, what’s been built, and how it can be used |
| 1. | Wallet Integration | Users can connect their polkadot.js wallet and view their address’s activity feed |
| 2. | Activity Timeline | Event feed with icons, timestamps, and tags for transfer/staking/governance |
| 3. | Filtering & Pagination | Users can filter activity by type and scroll infinitely or page through history |

#### Milestone 2 – Shareable Feeds + Light Analytics

- Estimated Duration: 4 weeks
- FTE: 1
- Costs: $5,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | MIT |
| 0b. | Documentation | Updated to include shareable links, charts, and customization features |
| 0c. | Testing and Testing Guide | Tests for chart data aggregation, shareable URL generation |
| 0d. | Article | Article diving into how wallet analytics can help user trust and improve UX |
| 1. | Public Feed | 	Users can generate a public URL of their wallet feed to share with others |
| 2. | Basic Analytics | Users see simple charts: total transactions, staking events, most used dApps |
| 3. | Chain Support | Support for at least 3 parachains beyond Polkadot Hub using SubQuery endpoints |

### 💰 Budget Breakdown

Please provide a breakdown of your budget by milestone:

| Milestone | Category | Estimated Time (days) | Cost (USD)
| --- | --- | --- | --- |
| M1 | UI/UX Design & Prototyping| 2-3 | 750 |
|| React Component Dev | 7 | 1,750 |
|| SubQuery Setup & Mapping | 2-4 | 1,000 |
|| Docs & Tutorials | 2 | 500 |
|| Testing and Debugging | 2-3 | 750 |
|| M1 Subtotal || $4,750 |
| M2 | Charting & Analytics | 4 | 1,000 |
|| Public Feed URLs | 2 | 500 |
|| Multichain Intgration | 3-5 | 1,250 |
|| Docs & API Examples | 2 | 500 |
|| Testing & Final Polishing | 2-3 | 750 |
|| M2 Subtotal || $4,000 |
|| Total Dev Days | ~40 | $8,750 |
|| Buffer (infra, design, hosting) | - | $1,250 |

## 🔮 Future Plans

After the Fast-Grant, I plan to:

- Expand Tracelet to support more parachains and ecosystem wallets
- Add notification support (activity alerts via Telegram or email)
- Turn Tracelet into a developer tool — dApp teams can embed wallet feed components inside their apps
- Seek follow-up funding from the main Polkadot grants program or ecosystem VCs
- eventually open Tracelet to contributors and possibly create a plugin system for custom events

## ℹ️ Additional Information

- The Tracelet repository has been created, but development has not yet started. This proposal is meant to secure initial funding to begin building the MVP.
- This is a solo project, and no other teams have contributed to it.
- This is my first grant application within the Polkadot ecosystem, and I’m excited to begin contributing and learning as a builder in this community.
