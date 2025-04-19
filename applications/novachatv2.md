# 📝 NovachatV2

## 🌟 Project Overview

- **Tagline:** Making Web3 effortless with AI-powered conversational DeFi.
- **Brief Description:**\
  NovachatV2 is an AI-driven chatbot designed for everyday users to interact with Polkadot’s EVM-compatible chains using natural language. It enables intuitive DeFi actions like checking balances, sending tokens, and trading/staking on decentralized exchanges (DEXs) by simply connecting a wallet and talking to the bot. The platform auto-executes read-only transactions and prompts MetaMask for state-changing ones, ensuring safety and ease. This grant will transform the Ethereum-based MVP into a production-ready platform with Polkadot EVM support, cloud deployment, and a polished user experience.
- **Integration with Polkadot:**\
  NovachatV2 will integrate with Polkadot’s EVM-compatible chains using Web3.js, supporting DeFi operations on two DEXs for trading and staking. It simplifies Web3 for regular users by automating tasks like adding RPC info to MetaMask.
- **Team Interest:**\
  As a serial hackathon winner and Web3 developer, I am passionate about removing barriers to DeFi adoption. NovachatV2’s conversational AI makes Polkadot’s EVM ecosystem accessible to non-technical users, empowering them to engage with Web3 effortlessly.

## 🔍 Project Details

- **Technology Stack:**

  - Frontend: React, TypeScript, Next.js 15+, Tailwind CSS
  - Backend: Node.js, Web3.js for blockchain interactions
  - AI: Llama 3.2 (natural language), Flock Web3 Agent Model (function calling)
  - Infrastructure: Cloud servers (AWS/GCP), WebSocket for real-time updates
  - Tools: RainbowKit for wallet integration
  - Testing: Manual testing as needed

- **Core Components:**

  1. **Conversational AI Interface:**
     - Dual-model AI: Llama 3.2 for natural language processing, Flock Web3 Agent Model for Web3 function calling.
     - Supports commands like “Check my balance” or “Swap tokens on a DEX.”
     - Auto-executes read-only transactions (e.g., balance checks) and prompts MetaMask for state-changing ones (e.g., token transfers).
     - Highly intuitive: users connect their wallet and can perform any typical DeFi action (trading, staking, sending tokens) by chatting, with the bot handling RPC configuration and transaction prompts.
  2. **Polkadot EVM Integration:**
     - Connectivity to Polkadot EVM chains for balance queries, token transfers, and DEX interactions.
     - Automatic RPC info injection into MetaMask for seamless network switching.
  3. **Function Playground:**
     - Educational interface for users to learn Web3 mechanics by manually calling functions (e.g., send tokens, check balances) and experimenting with parameters.
     - Supports custom transaction parsing, ABI-based contract interactions, and contract deployment.
  4. **Cloud Deployment:**
     - Production-ready setup with rate limits and public access for all users.

- **Relevant Prior Work:**

  - NovachatV2 MVP (Ethereum-based) is available at https://novachat-v2.vercel.app (AI functionality not working as it’s local). It supports Uniswap trading/staking, token transfers, and balance checks on EVM networks. Codebase: https://github.com/bonusducks777/novachat-v2/tree/main.
  - Won #1 Flock and Educhain bounties at UK AI Agent Hackathon (2025), #1 BNB Chain and #2 Avalanche tracks at ETH Oxford (2024) for NovachatV1.
  - Demo: YouTube pitch (begins halfway through).

- **UI Mockups:**\
  The interface will use the same UI as the MVP at https://novachat-v2.vercel.app, featuring:

  - A chat window for user-AI interaction with suggested prompts.
  - A function playground panel for manual function calls and parameter experimentation.
  - A network switcher and wallet connection button for MetaMask integration.

- **What NovachatV2 is NOT:**

  - Not a developer-focused tool or IDE for DApp development.
  - Not a custodial wallet or key management solution.
  - Not supporting non-EVM Polkadot chains in this grant.
  - Not developing cross-chain functionality or the Web3 intro educational section.

## 🧩 Ecosystem Fit

- **Ecosystem Position:**\
  NovachatV2 is a user-friendly DeFi interface for Polkadot’s EVM-compatible chains, enabling everyday users to engage with Web3 without technical knowledge.
- **Target Audience:**
  - Regular users new to DeFi who want to trade, stake, or send tokens effortlessly.
  - Crypto enthusiasts seeking a simple, conversational Web3 interface.
  - Users curious about Web3 mechanics who use the function playground to learn.
- **Needs Addressed:**
  - Eliminates technical barriers by automating RPC setup and transaction prompts.
  - Simplifies DeFi tasks (trading, staking, transfers) via natural language.
  - Educates users through the playground, fostering Web3 understanding.
  - Provides a safe, intuitive platform with MetaMask prompts for security.
- **Similar Projects:**\
  No similar projects were found in the Polkadot ecosystem (based on web searches and provided documents). Existing tools like PAPI Interactive Console and ink! AIDE target developers, not regular users. NovachatV2’s conversational AI and focus on daily DeFi users are unique.

## 👥 Team

- **Team Name:** NovachatV2
- **Contact Name:** Soumil Sahjpall
- **Contact Email:** soumil_sahjpall@hotmail.com
- **Website:** https://github.com/bonusducks777/novachat-v2

### Team Members

- Soumil Sahjpall (Solo developer)

### LinkedIn Profiles

- https://www.linkedin.com/in/soumil-sahjpall

### Team Code Repositories

- https://github.com/bonusducks777/novachat-v2
- https://github.com/bonusducks777/novatools

### GitHub Accounts

- https://github.com/bonusducks777

### Team’s Experience

Soumil Sahjpall is an experienced Web3 developer and serial hackathon winner with 5+ years in blockchain and AI. Key achievements include:

- Winner of Flock and Educhain bounties at UK AI Agent Hackathon (2025).
- Winner of BNB Chain track and 2nd place in Avalanche track at ETH Oxford (2024).
- Winner of the main hackathon track at EasyA x Polygon London (2022).
- 2nd place in the student track for the International TRON Grand Hackathon (2023).
- Finalist at EasyA x Stellar London (2024) and Harvard Hack Web3 (2022).
- Winner of a non-technical prize at EasyA x Polygon London (2022).
- Expertise in Web3.js, Llama, Flock Web3 Agent Model, and building user-focused DApps.

## 📊 Development Status

The NovachatV2 MVP, built from scratch, supports Ethereum-based DeFi interactions (Uniswap trading/staking, token transfers, balance checks) on EVM networks. It uses Llama 3.2 for natural language and the Flock Web3 Agent Model for function calling, with wallet integration via RainbowKit. The function playground allows manual testing of some functions, though contract deployment and custom transaction parsing are incomplete. The platform runs locally with the Flock model hosted via Replicate API, causing latency. MVP link: https://novachat-v2.vercel.app (AI functionality not working as it’s local). Demo link: YouTube pitch (begins halfway through). Codebase: https://github.com/bonusducks777/novachat-v2/tree/main.

**Current Features:**

- Conversational AI for crypto discussions and Web3 actions.
- Function playground with partial functionality (balance checks, token sends, Uniswap interactions).
- Wallet integration, network switching, and MetaMask RPC updates.
- Transaction queue and suggested prompts.

**Target Features (by July 31, 2025):**

- Full trading/staking on two Polkadot EVM DEXs for liquidity and yield.
- Polkadot EVM chain support for balances, transfers, and DEX interactions.
- Polished chatbot with low latency and robust function calling.
- Cloud deployment for public access with rate limits.
- Complete function playground supporting all chatbot capabilities, custom transaction parsing, ABI-based contract interactions, and contract deployment.

## 📅 Development Roadmap

### Overview

- **Estimated Duration:** 2 months (June 1, 2025 – July 31, 2025)
- **Full-Time Equivalent (FTE):** 1 solo developer
- **Total Costs:** $10,000 USD

| Number | Deliverable | Specification |
| --- | --- | --- |
| 0a. | License | MIT |
| 0b. | Documentation | Inline code documentation and a tutorial on using NovachatV2 for Polkadot EVM DeFi (e.g., trading on a DEX, sending tokens). |
| 0c. | Testing and Testing Guide | Manual testing as needed to ensure chatbot and playground functionality. A guide will detail testing procedures. |
| 0d. | Article | A blog post detailing NovachatV2’s Polkadot EVM integration, with a demo of key functions like trading and token transfers. |
| 1. | Playground Tools for Polkadot EVM | Function playground support for Polkadot EVM chains, including balance queries, token transfers, custom transaction parsing, ABI-based contract interactions, and contract deployment. |
| 2. | Chatbot Integration & Testing | Chatbot integration with playground tools for trading/staking on two Polkadot EVM DEXs, token transfers, and balance checks. Manual testing to ensure functionality and MetaMask prompt reliability. |
| 3. | Cloud Deployment & Chatbot Polish | Cloud deployment on AWS/GCP with rate limits and public access. Polished chatbot with optimized function calling and low latency using the Flock Web3 Agent Model. |

### 💰 Budget Breakdown

| Phase | Milestone | Deliverables | Cost (USD) | Estimated Completion |
| --- | --- | --- | --- | --- |
| 1 | Playground Tools for Polkadot EVM | Function playground tools | $3,000 | June 20, 2025 (3 weeks) |
| 2 | Chatbot Integration & Testing | Chatbot integration and testing | $3,000 | July 10, 2025 (3 weeks) |
| 3 | Cloud Deployment & Chatbot Polish | Cloud deployment and chatbot polish | $4,000 | July 31, 2025 (3 weeks) |
| **Total** |  |  | **$10,000** | **2 months** |

### Phase 1: Playground Tools for Polkadot EVM

- **Duration:** 3 weeks
- **Cost:** $3,000
- **Deliverables:**
  - Function playground support for Polkadot EVM chains: balance queries, token transfers, custom transaction parsing, ABI-based contract interactions, and contract deployment.
  - Automatic RPC info injection into MetaMask for network setup.
  - Manual testing to ensure playground functionality.

### Phase 2: Chatbot Integration & Testing

- **Duration:** 3 weeks
- **Cost:** $3,000
- **Deliverables:**
  - Chatbot integration with playground tools for trading/staking on two Polkadot EVM DEXs, token transfers, and balance checks.
  - Auto-execution of read-only transactions and MetaMask prompts for state-changing ones.
  - Manual testing to ensure reliable chatbot responses and MetaMask prompts.

### Phase 3: Cloud Deployment & Chatbot Polish

- **Duration:** 3 weeks
- **Cost:** $4,000
- **Deliverables:**
  - Cloud deployment on AWS/GCP with rate limits and public access.
  - Polished chatbot with optimized Flock Web3 Agent Model function calling, low latency, and robust error handling.
  - Manual testing to verify cloud performance and user experience.

## 🔮 Future Plans

- **Short-term (3-6 months post-grant):**

  - Add functionality to other EVM-based blockchain ecosystems using their respective grants programs.
  - Onboard a large user base to make Web3 accessible and intuitive for daily DeFi users.

- **Long-term (6-12 months):**

  - Implement cross-chain integration to enable token transfers between EVM chains.
  - Save user data, including chat history and wallet addresses, to provide a complete DeFi solution.

- **Additional Funding:**

  - Apply for ecosystem-specific grants (e.g., BNB Chain, Avalanche) to fund chain expansions.
  - Explore a freemium model with premium features while keeping the core open-source.

- **Ecosystem Impact:**\
  NovachatV2 aims to be the definitive conversational interface for Polkadot’s EVM ecosystem, driving user adoption by making DeFi intuitive and accessible. By simplifying interactions and providing a production-ready platform, it will empower everyday users to engage with Web3 confidently.

## ℹ️ Additional Information

- **Community Interest:** The NovachatV2 MVP won #1 Flock and Educhain bounties at the UK AI Agent Hackathon (2025), with users praising its ease of use for DeFi. Community feedback highlights demand for conversational Web3 tools.
- **Unique Value Proposition:** NovachatV2’s AI-driven interface, automatic RPC setup, and safe MetaMask prompts make it uniquely accessible for daily DeFi users, unmatched by any Polkadot tool.
- **Alignment with Fast-Grants Criteria:** The project supports Polkadot’s user ecosystem by simplifying EVM DeFi, with a proven MVP, clear roadmap, and potential for growth via other ecosystem grants.
