# 📝 PolkaFarm

## 🌟 Project Overview

PolkaFarm is a secure, user-friendly yield farming DApp built on Polkadot Asset Hub, enabling users to stake WND tokens and earn PLKF rewards through simple, efficient Solidity smart contracts.

PolkaFarm integrates directly with Polkadot's Asset Hub parachain, leveraging its EVM compatibility, native token staking capabilities, and shared security model to deliver a seamless DeFi experience. The platform demonstrates how traditional yield farming can be enhanced through Polkadot's unique cross-chain architecture and low fee structure.

Our team is passionate about expanding DeFi accessibility beyond high-gas networks like Ethereum. We believe Polkadot's parachain ecosystem offers the perfect architecture for creating interoperable financial applications that are both affordable to use and secure by design. PolkaFarm serves as an important DeFi primitive that demonstrates these capabilities while providing real value to users.
- (Optional but **huge bonus points**): [3-min video pitch](https://youtu.be/3-AhcPuJR0k)

### 🔍 Project Details

### Technology Stack
- **Smart Contracts**: Solidity 0.8.18+, Hardhat development environment, OpenZeppelin security patterns
- **Frontend**: React.js with functional components, ethers.js v6 for blockchain interaction, responsive CSS with dark/light mode
- **Blockchain**: Polkadot Asset Hub (currently deployed on Westend testnet)
- **Testing**: Hardhat testing framework with Chai assertions

### Core Components

1. **PolkaFarmToken Contract** (PLKF)
   - Minimal ERC-20 implementation for reward distribution
   - Minting capability restricted to the staking contract
   - Standard transfer and approval functions
   - Ownership pattern for administrative control

2. **PolkaFarmStaking Contract**
   - Direct staking of native WND tokens (Westend's native currency)
   - MasterChef-inspired reward distribution algorithm
   - Block-based reward calculation using accumulator pattern
   - Early withdrawal penalty to incentivize longer staking periods
   - Secure fund management with ownership controls

3. **React Frontend Application**
   - Clean, intuitive interface for staking operations
   - Real-time statistics display of APY, total staked, rewards
   - Wallet integration with MetaMask
   - Responsive design with dark/light mode toggle
   - Local storage for user preferences

### Architecture

The system follows a simple but effective architecture:
1. Users stake WND (native token) in the staking contract
2. The contract tracks stake amounts and block numbers
3. Rewards accrue proportionally to stake amounts
4. The staking contract mints PLKF tokens as rewards when users withdraw

The reward calculation uses the "reward debt" pattern, where:
1. Each time rewards are calculated, the global accumulator increases
2. User rewards are calculated as the difference between accrued rewards and reward debt
3. This method ensures correct reward distribution even with varying stake amounts over time

### Existing Work

PolkaFarm is already deployed on the Polkadot Asset Hub Westend testnet:

**PolkaFarmToken Contract:**
- Address: `0xeb3f68def0a92755f12afbc78c7c091882008481`
- [View on Asset Hub Westend Explorer](https://assethub-westend.subscan.io/account/0xeb3f68def0a92755f12afbc78c7c091882008481)

**PolkaFarmStaking Contract:**
- Address: `0x54c27ad8a9a35902b304c1ddda79711f23d1dd48`
- [View on Asset Hub Westend Explorer](https://assethub-westend.subscan.io/account/0x54c27ad8a9a35902b304c1ddda79711f23d1dd48)

### UI Mockups
The application is already implemented with a complete UI featuring:
- Landing page with key platform statistics
- Dashboard for user staking operations
- Dark and light mode support
- Responsive design for all device sizes

Screenshots are available in the README.md file of our repository.
- [Repository Here](https://github.com/cdermott7/PolkaFarm/tree/main).

### Project Limitations
PolkaFarm will NOT:
- Implement governance functions in the initial version (planned for future milestone)
- Support tokens beyond WND and PLKF in the initial implementation
- Include advanced features like autocompounding or lending in the MVP
- Launch on Polkadot mainnet until security audits are completed (post-grant)


### 🧩 Ecosystem Fit

### Position in Polkadot Ecosystem
PolkaFarm serves as a fundamental DeFi primitive on Polkadot Asset Hub, providing a simple but essential yield farming mechanism that can become a building block for more complex DeFi applications in the ecosystem. It demonstrates how traditional DeFi concepts can be enhanced through Polkadot's unique architecture.

### Target Audience
1. DeFi users looking for lower-cost alternatives to Ethereum-based yield farming
2. Polkadot token holders seeking additional yield opportunities
3. DeFi beginners who appreciate the simple, clean interface and lower barrier to entry
4. Developers looking for examples of DeFi implementations on Polkadot Asset Hub

### Needs Addressed
1. Accessible yield opportunities for Polkadot ecosystem tokens
2. Lower-cost DeFi alternative to Ethereum-based platforms
3. User-friendly entry point to DeFi for Polkadot users
4. Technical demonstration of EVM capabilities on Polkadot Asset Hub

### Similar Projects and Differentiation
While yield farming exists on many chains, there are currently few mature yield farming applications specifically built for Polkadot Asset Hub. Existing options like:
- Acala's aUSD staking
- Parallel Finance's staking pools

Differentiation points:
1. Direct native token staking (WND) without requiring wrapped tokens
2. Simplified UX designed for broader adoption
3. EVM compatibility allowing familiar tooling for Ethereum developers
4. Focus on Polkadot Asset Hub specifically rather than a separate parachain

## 👥 Team

- **Team Name:** PolkaFarm
- **Contact Name:** Cole Dermott
- **Contact Email:** dermottcole@gmail.com
- **Website:** https://github.com/cdermott7/PolkaFarm || https://coledermott.dev/ (2nd is outdated)

### Team members
- Cole Dermott - Head of Finance @ Waterloo Blockchain

#### LinkedIn Profiles (if available)

- https://www.linkedin.com/in/coledermott/

### Team Code Repos

- https://github.com/cdermott7/PolkaFarm

Please also provide the GitHub accounts of all team members:

- https://github.com/cdermott7

### Team's experience

Cole Dermott is the Head of Finance at Waterloo Blockchain, the premier blockchain club at the University of Waterloo. He has experience developing smart contracts and DeFi applications, having previously contributed to projects on Ethereum and Avalanche. 

His background combines financial expertise with technical development skills, making him well-positioned to develop DeFi applications that are both technically sound and economically viable.

With specific interest in the Polkadot ecosystem, Cole has been actively exploring how Substrate and Asset Hub can offer unique advantages for DeFi applications compared to traditional smart contract platforms.

## 📊 Development Status

PolkaFarm is already partially implemented:

1. **Completed Components**:
   - Core smart contracts (PolkaFarmToken.sol, PolkaFarmStaking.sol)
   - Initial frontend implementation with key features
   - Deployment to Polkadot Asset Hub Westend testnet
   - Basic documentation and user guides

2. **Code Repository**:
   - GitHub: https://github.com/cdermott7/PolkaFarm

3. **Deployed Contracts**:
   - PolkaFarmToken: 0xeb3f68def0a92755f12afbc78c7c091882008481
   - PolkaFarmStaking: 0x54c27ad8a9a35902b304c1ddda79711f23d1dd48

## 📅 Development Roadmap

### Overview

- **Estimated Duration**: 3 months
- **Full-Time Equivalent (FTE)**: 0.5
- **Total Costs**: $10,000 USD

### Initial Payment: Project Kickoff
**Payment Upon Grant Approval**: $3,000 USD

This initial funding will be used to:
- Purchase necessary development tools and services
- Cover immediate project setup costs
- Fund the first phase of development work
- Secure the developer time commitment for the project duration

### Milestone 1: Enhanced Frontend and Contract Optimization
**Estimated Duration**: 1.5 months
**Costs**: $3,500 USD

| Number | Deliverable | Specification |
|--------|-------------|---------------|
| 0a. | License | MIT |
| 0b. | Documentation | We will provide both inline documentation of the code and a comprehensive tutorial that explains how users can connect wallets, stake tokens, and claim rewards. |
| 0c. | Testing and Testing Guide | Core functions will be fully covered by unit tests using the Hardhat testing framework. The guide will detail how to run these tests and validate contract functionality. |
| 0d. | Article | We will publish an article explaining PolkaFarm's architecture, how it leverages Polkadot Asset Hub's unique features, and tutorial content for users. |
| 1. | Contract Optimization | Optimize the staking contract for gas efficiency, add partial withdrawal functionality, and implement emergency withdrawal capabilities for improved security. |
| 2. | Enhanced Frontend | Add detailed analytics dashboard with historical performance charts, improve mobile responsiveness, and implement notification system for staking events. |
| 3. | User Onboarding Improvements | Create interactive tutorial for first-time users, implement wallet connection guide specific to Asset Hub, and add tooltips explaining DeFi concepts throughout the interface. |

### Milestone 2: Advanced Features and Security
**Estimated Duration**: 1.5 months
**Costs**: $3,500 USD

| Number | Deliverable | Specification |
|--------|-------------|---------------|
| 0a. | License | MIT |
| 0b. | Documentation | Extended documentation including architectural diagrams, security considerations, and API specifications for frontend-contract interactions. |
| 0c. | Testing and Testing Guide | Comprehensive test suite including integration tests, stress tests for reward distribution, and security-focused test scenarios. Coverage reports will be generated. |
| 0d. | Article | We will publish a technical deep-dive article explaining PolkaFarm's reward mechanisms, security features, and future roadmap for integration with other Polkadot parachains. |
| 1. | Multiple Reward Pools | Implement support for multiple staking pools with different reward rates and token pairs, allowing for more diverse yield strategies. |
| 2. | Frontend Analytics Suite | Develop comprehensive analytics dashboard showing platform statistics, user performance, and APY history over time using data visualization libraries. |
| 3. | Security Audit Preparation | Implement additional security measures based on best practices, add extensive input validation, and prepare documentation required for a formal security audit. |

### 💰 Budget Breakdown

### Initial Payment: Project Kickoff
**Total Cost**: $3,000 USD

| Item | Description | Hours | Rate | Cost |
|------|-------------|-------|------|------|
| Project Setup | Development environment, tooling, initial research | 20 | $50/hr | $1,000 |
| Preliminary Development | Core feature planning, architecture refinement | 30 | $50/hr | $1,500 |
| Technical Documentation | Initial documentation and development roadmap | 10 | $50/hr | $500 |

### Milestone 1: Enhanced Frontend and Contract Optimization
**Total Cost**: $3,500 USD

| Item | Description | Hours | Rate | Cost |
|------|-------------|-------|------|------|
| Smart Contract Development | Gas optimization, partial withdrawals, emergency functions | 35 | $50/hr | $1,750 |
| Frontend Enhancements | Analytics dashboard, mobile improvements, notifications | 20 | $50/hr | $1,000 |
| Documentation & Testing | User guides, inline documentation, test coverage | 15 | $50/hr | $750 |

### Milestone 2: Advanced Features and Security
**Total Cost**: $3,500 USD

| Item | Description | Hours | Rate | Cost |
|------|-------------|-------|------|------|
| Multiple Reward Pools | Contract development for multiple pool support | 30 | $50/hr | $1,500 |
| Analytics Suite | Data visualization, historical tracking, API development | 20 | $50/hr | $1,000 |
| Security & Auditing | Security measures, validation, audit preparation | 20 | $50/hr | $1,000 |

**Total Project Budget**: $10,000 USD

## 🔮 Future Plans

### Short-term Plans (6-12 months)
1. **Security Audit**: Conduct a professional security audit before mainnet deployment
2. **Mainnet Launch**: Deploy PolkaFarm to Polkadot Asset Hub mainnet
3. **Cross-chain Integration**: Implement XCM functionality to support token transfers between parachains
4. **Community Building**: Establish a user community and feedback mechanism

### Medium-term Plans (1-2 years)
1. **Governance Implementation**: Add DAO-based governance for protocol parameter adjustments
2. **Advanced Yield Strategies**: Develop autocompounding and leveraged yield options
3. **Ecosystem Integration**: Partner with other Polkadot DeFi protocols for composite strategies
4. **Extended Token Support**: Add support for additional parachain tokens

### Funding Strategy
1. **Additional Grants**: Apply for Polkadot ecosystem grants for specific feature additions
2. **Community Funding**: Implement a community treasury funded by protocol fees
3. **Strategic Partnerships**: Establish partnerships with other Polkadot projects for joint development

### Vision for Growth
PolkaFarm aims to evolve from a simple yield farming platform to a comprehensive DeFi hub within the Polkadot ecosystem, leveraging cross-consensus messaging for interconnected financial primitives. We envision becoming a core infrastructure component that showcases the advantages of Polkadot's architecture while providing genuine utility to users.

## ℹ️ Additional Information
- Initial development was part of a blockchain hackathon project
- The current implementation demonstrates core functionality but requires additional work for production readiness
- We have established connections with several Polkadot ecosystem projects for potential future collaborations
- The team is committed to long-term development regardless of grant funding, though the funding would significantly accelerate development
