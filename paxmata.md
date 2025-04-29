# Paxmata - Polkadot Fast Grant Application

## 📝 Name of your Project

Paxmata: Blockchain-Based Real Estate Project Management Platform

## 🌟 Project Overview

**Tagline:** Simplifying Real Estate Project Management through Blockchain Technology

**Brief Description:**
Paxmata is a blockchain-based platform designed to modernise non-commercial real estate project management. By leveraging dynamic NFTs, smart contracts, and artificial intelligence, Paxmata addresses critical inefficiencies in traditional project management while enabling secure peer-to-peer funding options. The platform introduces a novel approach to milestone verification and fund management through blockchain technology, ensuring transparency and accountability in construction projects.

**Integration with Polkadot:**
Paxmata will be built on Polkadot Asset Hub, leveraging its scalable, cross-chain compatibility and smart contract functionalities to build a decentralised marketplace for project management. Polkadot Asset Hub's interoperability allows Paxmata to seamlessly integrate with other parachains in the ecosystem, improving transaction speed and reducing costs for users. Additionally, the platform leverages Polkadot's secure blockchain infrastructure to ensure transparent, immutable project records, milestone tracking, and P2P funding mechanisms.

**Team's Interest:**
Our team is passionate about solving real-world problems in the construction and property development industry through blockchain technology. Having experienced firsthand the inefficiencies, trust issues, and lack of transparency in traditional construction project management, we believe that blockchain technology, specifically on Polkadot, offers the perfect solution to these challenges. The decentralised nature of blockchain, combined with smart contracts, provides an opportunity to create a more secure, efficient, and transparent system for managing real estate projects.

## 🔍 Project Details

### Technology Stack

- **Blockchain:** Polkadot Asset Hub for smart contracts and token standards
- **Frontend:** React.js with Web3 integration for a responsive, intuitive interface
- **Backend:** Node.js, MongoDB, and WebSocket for real-time updates
- **Smart Contracts:** Solidity (compatible with Polkadot Asset Hub)
- **AI Integration:** Machine learning models for milestone generation and document analysis
- **Storage:** IPFS for decentralised storage of project documentation and media

### Core Components

1. **Smart Contract Architecture:**
   - NFT Contract: Handles project ownership and identity through secure minting process
   - Office Contract: Manages project operations with its own permission system
   - Escrow Contract: Controls financial operations independently
   - Factory Contract: Ensures standardised deployment while maintaining security

2. **Milestone Management System:**
   - Hierarchical structure for managing parent and child milestones
   - Verification system for milestone completion
   - Automated payment release based on verified milestones

3. **SCORS (Smart Contract Objective Review System):**
   - Blockchain-verified reputation scoring for service providers
   - Objective performance metrics for accountability
   - Transparent rating system based on past performance

4. **P2P Lending Implementation:**
   - Risk-stratified lending pools (Low, Medium, High Risk)
   - Token-based interest distribution
   - Insurance fund for lender protection

5. **Dynamic NFT Implementation:**
   - Project tokens that evolve with project progression
   - Immutable record of all project activities and milestones
   - Token metadata that updates as project status changes

### Data Models

1. **Project Structure:**
```
struct Project {
    uint256 id;
    address owner;
    string metadata;
    uint256 status;
    uint256 creationTime;
    uint256 lastUpdateTime;
    bytes32 dataHash;
}
```

2. **Milestone Structure:**
```
struct Milestone {
    uint256 id;
    uint256 projectId;
    uint256 parentId;
    string description;
    uint256 amount;
    uint256 deadline;
    bool isCompleted;
    bool isVerified;
    address completedBy;
    uint256 completionTime;
    bytes32 dataHash;
}
```

3. **P2P Lending Structure:**
```
struct LendingPool {
    uint8 riskTier;
    uint256 totalValueLocked;
    uint256 utilisationRate;
    uint256 baseInterestRate;
    uint256 insuranceFundBalance;
    mapping(address => uint256) lenderBalances;
}
struct Loan {
    uint256 projectId;
    uint256 amount;
    uint256 interestRate;
    uint256 startDate;
    uint256 endDate;
    address poolAddress;
    bool isActive;
}
```

### What the Project Will Not Provide

- **Direct Cryptocurrency Exchange:** The platform will not function as a cryptocurrency exchange
- **Property Listing Service:** Paxmata is not a real estate listing platform for buying or selling properties, but this might be included in the future. First we are focusing on improving a small but specialised part of project management
- **Corporate-Level Enterprise Solutions:** While Paxmata provides robust project management, it's designed for non-commercial users rather than enterprise-level organisations
- **Full Legal Documentation Generation:** The platform will assist with project documentation but is not a legal document generator
- **Direct Investment in Properties:** The platform facilitates project funding, not direct property investment

## 🧩 Ecosystem Fit

### Project Fit in the Ecosystem

Paxmata fills a significant gap in the Polkadot ecosystem by bringing real-world asset (RWA) management to the construction and real estate sectors. While there are DeFi and NFT projects in the ecosystem, few focus on practical applications for the real estate industry. By leveraging Polkadot Asset Hub, Paxmata creates a bridge between traditional construction management and blockchain technology, expanding the use cases for Polkadot's infrastructure.

### Target Audience

1. **Individual property owners:** Homeowners looking to renovate or develop their properties
2. **Small-scale real estate developers:** Small businesses or individuals developing residential properties
3. **Construction contractors and service providers:** Electricians, plumbers, builders looking for work opportunities
4. **Peer-to-peer lenders:** Individuals interested in funding construction projects for returns
5. **Charitable organisations and NGOs:** Entities looking to fund and manage construction projects transparently

### Needs Addressed

1. **Transparent Fund Management:** Ensures project funds are only released upon milestone completion
2. **Secure Documentation:** Creates immutable records of all project documentation and progress
3. **Trust Minimisation:** Reduces reliance on intermediaries and trust between parties
4. **Efficient Contractor Matching:** Connects property owners with qualified contractors
5. **Verified Project History:** Builds a verifiable history of projects that enhances accountability
6. **Alternative Financing:** Provides P2P lending options for construction projects

### Similar Projects in Polkadot Ecosystem

There are few direct competitors in the Polkadot ecosystem focusing on non-commercial real estate project management. Some projects in the broader real estate space include:

**Archisinal:** While also focusing on real estate, Archisinal targets a different market segment. Paxmata differentiates itself by focusing specifically on non-commercial users, project management through verified milestones, and integrating P2P lending tailored for construction projects.

The lack of similar projects in this space indicates a gap in the market that Paxmata can fill. Traditional real estate platforms haven't integrated blockchain technology for project management, and existing blockchain projects haven't focused on the specific needs of non-commercial construction management.

## 👥 Team

### Team Name: 
Paxmata

### Contact Name: 
Alexander Burge

### Contact Email: 
alexander@paxmata.com

### Website: 
www.paxmata.com

### Team Members:
Alexander Burge - Founder/CEO/Head Developer

### LinkedIn Profiles:
https://www.linkedin.com/in/alexander-burge-1702142b3

### Team Code Repos:
https://github.com/AdlusMjRb

### GitHub Accounts:
https://github.com/Paxmata

### Team's Experience:
Alexander Burge brings a unique combination of real estate experience and blockchain development skills to the project:
- 6 years of real estate industry experience
- 4 years of experience as a web3 full-stack developer
- Exeter University alumnus with a background in technology and business
- Winner at the 2024/2025 EasyA hackathon for building on blockchain technology
- Developed multiple smart contract systems focusing on real estate and construction applications, p2p lending and project verification.

## 📊 Development Status

Paxmata has already made significant progress in its development:

1. **Core Smart Contracts:** The initial versions of the NFT, Office, and Escrow contracts have been created and tested in a development environment. P2P lending contracts have been designed and deployed on the Polkadot Asset Hub.
2. **Architecture Design:** The entire platform architecture, including the Factory pattern for contract deployment and security measures, has been designed and documented.
3. **Technical Whitepaper:** A comprehensive technical whitepaper detailing the platform's architecture, security mechanisms, and operational workflows has been completed.
4. **UI/UX Design:** Initial designs for the platform's user interface, focusing on user-friendly project creation and milestone tracking, have been created.
5. **P2P Lending Implementation:** The design for the P2P lending system with risk-stratified pools has been completed, including detailed contract specifications.

## 📅 Development Roadmap

### Overview

- **Estimated Duration:** 2 months
- **Full-Time Equivalent (FTE):** 1
- **Total Costs:** $10,000 USD

### Milestone 1: Core Contract Migration & Testing

**Estimated Completion:** 2 weeks
**Cost:** $5,000 USD

| Number | Deliverable | Specification |
|--------|-------------|---------------|
| 1. | License | Apache 2.0 |
| 1a. | Documentation | We will provide comprehensive documentation including: smart contract architecture overview, technical documentation for developers. |
| 2. | Complete Smart Contract Migration to Asset Hub | We will migrate and optimise all existing smart contracts to Polkadot Asset Hub, including: NFT contract for project representation, Office contract for milestone management, Escrow contract for fund management, Factory contract for deployment orchestration, and Project Manager contract for system coordination. |
| 3. | Core UI Implementation | We will develop the essential user interface components: project creation workflow, milestone management dashboard, and project status tracking interface. |

**KPI Targets:**
- Deploy all core contracts to Asset Hub testnet - 5 contracts (however, due to Asset Hub's small byte sise, current contract architecture has to be modified to fit these new constraints)
- Individual contract tests will support their functionality on Asset Hub
- 3 test projects will be completed from inception through to completion and payment

**Budget Breakdown:**
- Smart Contract Development & Migration: 80 hours × $40/hr = $3,200
- Testing & Security Analysis: 30 hours × $40/hr = $1,200
- Basic UI Implementation: 15 hours × $40/hr = $600
- Total: $5,000

### Milestone 2: P2P Lending Implementation & Platform Enhancement

**Estimated Completion:** 1 month
**Cost:** $5,000 USD

| Number | Deliverable | Specification |
|--------|-------------|---------------|
| 0a. | License | Apache 2.0 |
| 0b. | Documentation | We will provide updated documentation including: P2P lending system technical overview, user guide for lenders and borrowers, integration documentation for the lending pools, and developer documentation for the entire platform. |
| 1. | P2P Lending Implementation | We will implement and optimise the P2P lending functionality including: risk-stratified lending pools, lending pool registry for coordination, insurance fund mechanism for lender protection, interest rate calculations based on risk profiles, and loan application and management workflow. |
| 2. | Advanced UI Development | We will develop comprehensive UI components including: lending pool interface for lenders, loan application interface for borrowers, repayment tracking dashboard. |
| 3. | Partnership Implementation | We will: Begin talks with at least 2 companies or independent contractors, implement incentive mechanisms for early adopters, and set up a $500 social media marketing stratigy. |

**KPI Targets:**
- Onboard at least 25 users to the platform, though strategic marketing push on social media.
- Process at least 5 test loans through the P2P lending system
- Complete at least 3 full project cycles with milestone verification

**Budget Breakdown:**
- P2P Lending Implementation: 60 hours × $40/hr = $2,400
- Advanced UI Development: 40 hours × $40/hr = $1,600
- Partnership Development & Marketing: 25 hours × $40/hr = $1,000
- Total: $5,000

## 💰 Budget Breakdown

| Milestone | Deliverables | Cost (USD) | Estimated Completion |
|-----------|--------------|------------|----------------------|
| 1 | Core Contract Development & Testing | $5,000 | 2 weeks |
| 2 | P2P Lending Implementation & Platform Enhancement | $5,000 | 1 month |
| **Total** | | **$10,000** | **1.5 months** |

## 🔮 Future Plans

### Continued Development

Following the Fast-Grant, we plan to continue development of Paxmata with the following focus areas:

1. **Regulatory Compliance Framework:** Develop robust compliance mechanisms for different jurisdictions to ensure the platform can operate globally.
2. **Mainnet Deployment:** Move from testnet to mainnet deployment with proper legal and regulatory compliance.
3. **Mobile Application:** Create dedicated mobile applications for on-site project updates and milestone verification.
4. **Cross-Chain Integration:** Expand to other parachains within the Polkadot ecosystem to enable broader interoperability and user base.
5. **Enhanced AI Features:** Develop more sophisticated AI capabilities for automated milestone suggestion and verification.


### Additional Funding Plans
1. **Grant Programs:** Apply for additional grants from blockchain foundations and real estate innovation funds to support specific feature development and mainnet deployment.
2. **Venture Capital Funding:** After demonstrating traction with the initial platform, we plan to approach VC firms specialising in PropTech and blockchain technology for Series A funding.
3. **Strategic Partnerships:** Establish partnerships with existing real estate platforms and construction companies to create integration opportunities and potential investment.

### Vision for Growth and Impact

Our vision for Paxmata is to become the leading decentralised platform for real estate project management globally. We aim to:

1. **Transform Construction Industry Standards:** Establish new standards for transparency and accountability in construction management.
2. **Expand Access to Financing:** Enable more projects to secure funding through alternative financing methods, particularly in underserved markets.
3. **Build Global Marketplace:** Create a worldwide marketplace connecting property owners with qualified contractors and service providers.
4. **Drive Polkadot Adoption:** Showcase the practical applications of Polkadot technology in solving real-world problems, bringing new users to the ecosystem.
5. **Create Economic Opportunities:** Enable contractors and service providers to find work more efficiently while building verifiable reputations on the blockchain.

## ℹ️ Additional Information

### Work Already Completed

1. **Smart Contract Architecture:** We have already designed and implemented the core smart contract architecture, including NFT, Office, and Escrow contracts.
2. **Technical Whitepaper:** We have completed a comprehensive technical whitepaper detailing the platform's architecture and security mechanisms.
3. **Hackathon Success:** Paxmata won recognition at the 2024/2025 EasyA hackathon for its innovative approach to blockchain-based project management.
4. **UI/UX Design:** Initial designs for the user interface have been created, focusing on user-friendly project creation and milestone tracking.

### Charity Partnerships

We are in discussions with local charities including "Past, Present & Future" and "Rotary" to deploy charity construction projects on the platform. These charities have recently gained national media attention for their projects, which could provide significant visibility for Paxmata and the Polkadot ecosystem.

### Marketing Plans

With the funding, we plan to participate in PropTech conventions and industry events to showcase Paxmata to potential users. This includes creating demonstrations that allow users to create sample projects, highlighting the ease of use and benefits of our blockchain-based approach.
