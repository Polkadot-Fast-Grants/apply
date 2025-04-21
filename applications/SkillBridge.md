
Project Name: SkillsBridge

🌟 Project Overview

Please provide the following:

    If the name of your project is not descriptive, a tagline 
*Tagline:* Empowering freelancers through decentralized blockchain innovation on Polkadot
---
     A brief description of your project
#### *SkillBridge* is a decentralized freelance marketplace that leverages Polkadot’s blockchain infrastructure to address critical challenges in the global freelance economy. The platform targets three key issues: lack of trust between parties, payment delays and high fees, and access barriers faced by the underbanked.

#### By utilizing smart contracts for secure escrow, enabling instant cross-chain payments, and incorporating decentralized dispute resolution, SkillBridge creates a trustless environment that benefits freelancers and clients worldwide.



[![Ecosystem Challenges](https://github.com/MasteraSnackin/Skillbridge-UPDATE/blob/main/docs/Screenshot%202025-04-21%20194350.png)](https://github.com/MasteraSnackin/Skillbridge-UPDATE/blob/main/docs/Screenshot%202025-04-21%20194350.png)


---

    An indication of how your project relates to / integrates into Polkadot
#### 🔗 *SkillBridge* will be built as a parachain on Polkadot, leveraging cross-chain interoperability to enable seamless payments across multiple blockchains and currencies. The project will utilize the Substrate framework and ink! smart contracts to implement secure escrow services, milestone-based payments, and automated dispute resolution.

#### By taking advantage of Polkadot’s shared security model and cross-chain messaging (XCMP), SkillBridge can deliver secure, low-cost transactions while maintaining interoperability with a broad range of blockchain ecosystems.
---

    An indication of why your team is interested in creating this project
#### 💡 I am motivated to create this project because the $1.5 trillion global freelance economy—comprising 1.5 billion participants worldwide—continues to face fundamental challenges that blockchain technology is uniquely equipped to solve. Polkadot’s interoperable architecture offers an ideal foundation for building a truly global and accessible freelance marketplace, capable of connecting to multiple blockchain ecosystems and supporting fiat on/off ramps.

[![Flow Digram](https://github.com/MasteraSnackin/Skillbridge-UPDATE/blob/main/docs/Screenshot%202025-04-21%20194209.png)](https://github.com/MasteraSnackin/Skillbridge-UPDATE/blob/main/docs/Screenshot%202025-04-21%20194209.png)



### We believe that empowering freelancers with instant, secure payments and trustless work agreements will help distribute economic opportunity more equitably across the world.
---
    (Optional but big bonus points): 1-min video pitch

[1-Min Video Pitch](https://youtube.com/shorts/EF7F8Pyp_FM?feature=share)

---
🔍 Project Details

    We expect applicants to have a solid idea about the project's expected final state. Therefore, please submit (where relevant):

## An overview of the technology stack to be used 🛠️
    
- ⛓️ Blockchain: Polkadot, Substrate framework
- 📜 Smart Contracts:  ink! (native to Substrate) and/or EVM-compatible contracts for escrow, payments, and dispute resolution
- ⚛️ Frontend: React.js or Vue.js for web interface
- 🟢 Backend: APIs: Node.js with integration to Polkadot RPC endpoints, Express.js
- 💸 Payments: Integration with cross-chain bridges and stablecoins
- Databases: PostgreSQL for structured data, Redis for caching
- ☁️🗄️ Cloud/Infra: AWS, GCP, or decentralized storage for off-chain data
- 🧪 Testing: Jest for unit testing, Cypress for end-to-end testing
-  🐳☸️ DevOps: Docker, Kubernetes for scalable deployment
---
      Documentation of core components, protocols, architecture, etc. to be deployed

## Core Components & Architecture

### Smart Contract Escrow System  
* 🛡️📜 **Secure escrow** using ink! smart contracts on Substrate
* 🔒💰 **Client funds** locked until work completion is verifie
* 🎯📆 **Support** for milestone-based partial payments
* 🤖🔓 **Automated** release of fundQs upon completion verification

### Cross-Chain Payment System:
* 🌉🟣💬 **Integration** with Polkadot's XCMP for cross-chain payments
* 🌐💱⛓️ **Support** for multiple currencies through parachain connections
* 🏦💱🌉  **Bridges** to traditional payment systems for fiat on/off ramps
* 💰⬇️⚡✅ **Minimal** transaction fees and near-instant settlement

### Decentralized Dispute Resolution: 
* 🤝⛓️⚖️ **On-chain mediation** for conflict resolution
*  📁✅🔒**Evidence** submission and verification system
* 👁️⚖️📜 **Fair** , transparent arbitration process
* ⭐📈🎖️ **Reputation tracking** for both freelancers and clients

### Global Accessibility Layer:
* 🌉 **Bridges** to traditional banking systems
* 🌍 **Support** for regional payment methods
* 📱 **Mobile-first** design for regions with limited computer access
* 🌐 **Multi-language support**

#### **On-Chain Dispute Resolution:** Transparent, auditable process for handling disgreements
#### **Reputation System:** Blockchain-based, tamper-proof freelancer/client ratings
#### **Job Marketplace UI:** Intuitive interface for posting, bidding, and managing jobs
---
      Any PoC/MVP or other relevant prior work or research on the topic
### Drawing on what we learn from EchoPay 2
[EchoPay 2](https://github.com/YanniWu88/EchoPay-2/tree/master "EchoPay 2")

EchoPay 2 is an innovative payment platform concept enabling users to conduct secure, cross-chain transactions through voice commands. This repository contains the initial proof-of-concept implementation focusing on the frontend interface, wallet connection, and voice input simulation.

Key takeaway would be connection wallet, and write smart contract on rust

* **MVP**: will focus on core escrow, payment, and dispute features, with a simple job board and wallet integration.
* **PoC**: Demonstrate escrow and payment flows using testnet tokens and a basic UI
---
      Mockups/designs of any UI components
## User Interface Features

The platform will feature a clean, intuitive interface with the following key screens:

### 1. Registration and Profile Setup
- Simple registration form with email or social media login
- Sections to add skills and experience
- Portfolio showcase capabilities

### 2. Project Browsing and Bidding
- Searchable project listings with advanced filters
- Detailed project view showing requirements and budget
- Proposal submission interface including cover letter and bid amount

### 3. Smart Contract Agreement
- Clear display of contract terms and conditions
- Milestone tracking with progress indicators
- Payment release confirmation interface

### 4. Dispute Resolution Interface
- Tools for evidence submission
- Transparent process tracking for arbitration
- Resolution outcome display

[![Platform Interface](https://github.com/MasteraSnackin/Skillbridge-UPDATE/blob/main/docs/Screenshot%202025-04-21%20194120.png)](https://github.com/MasteraSnackin/Skillbridge-UPDATE/blob/main/docs/Screenshot%202025-04-21%20194120.png)

---
    Data models / API specifications of the core functionality

### 1. User Model:
- Basic profile information (name, contact, etc.)
- Skills and experience data
- Reputation and review history
- Payment information

| Field     | Details                                                                 |
|-----------|--------------------------------------------------------------------------|
| Job:      | {id, title, description, client, freelancer, status, escrow_contract_id} |
| User:     | {id, wallet_address, profile, reputation_score}                          |
| Escrow:   | {id, job_id, amount, currency, status, release_conditions}               |
| Dispute:  | {id, job_id, parties, evidence, resolution}                              |



### 2. Project Model:
- 📋 Project details and requirements
- 💰 Budget and timeline information
- 🎯 Milestone definitions
- 📈 Status tracking

### 3. Contract Model:
- 📄🤝 Agreement terms
- 💸🗓️ Payment schedule
- 📦✅ Deliverable specifications
- ⚖️🗣️ Dispute resolution terms

 ### 4. Payment API:
 - Integration with Polkadot parachains for cross-chain transactions
 - Support for fiat on/off ramps
 - Escrow management
 - Payment history tracking
---
        What your project is not or will not provide or implement

1. SkillBridge is not a traditional job board or recruitment platform for permanent employment
2. The platform will not offer general marketplace features beyond freelance services
3. We will not provide financial services beyond the payment mechanisms for completed work
4. The platform will not store or manage intellectual property rights beyond basic contract terms
5. SkillBridge will not act as a centralized arbiter, instead relying on decentralized governance mechanisms
6. SkillBridge will not provide fiat on/off-ramp services directly; instead, it will integrate existing bridges (e.g., Spacewalk, Stellar anchors).
7. It will not offer centralized arbitration; all dispute resolution is on-chain and community-driven.
8. No support for non-Polkadot blockchains except via approved cross-chain bridges.
---
        This is a place for you to manage expectations and clarify any limitations

        🧩 Ecosystem Fit
## SkillBridge in the Polkadot Ecosystem

SkillBridge fits into the Polkadot ecosystem as a specialized DeFi application focused on the freelance economy. It leverages Polkadot's core strengths in the following ways:

### 🌉 Cross-Chain Interoperability
-  Utilizes XCMP to enable payments across different parachains and blockchains, allowing freelancers and clients to use their preferred currencies.

### 🛡️ Shared Security
- Benefits from Polkadot's shared security model, ensuring high security standards for SkillBridge without the need to establish its own validator network.

### ⚡ Scalability
- Leverages Substrate's scalability to handle a growing user base and increasing transaction volumes.

### 🗳️ Governance
- Implements Polkadot's on-chain governance for platform improvements and dispute resolution mechanisms.


[![SkillBridge Architecture](https://github.com/MasteraSnackin/Skillbridge-UPDATE/blob/main/docs/Screenshot%202025-04-21%20194246.png)](https://github.com/MasteraSnackin/Skillbridge-UPDATE/blob/main/docs/Screenshot%202025-04-21%20194246.png)


---

      Help us locate your project in the Polkadot landscape and what problems it tries to solve by answering each of these questions:
      Where and how does your project fit into the ecosystem?
SkillBridge fits into the Polkadot ecosystem as a specialized DeFi application focused on the freelance economy. It leverages Polkadot's core strengths in these ways:
1. focused on the freelance economy. It leverages Polkadot's core strengths in these ways:
Cross-Chain Interoperability: Utilizes XCMP to enable payments across different parachains and blockchains, allowing freelancers and clients to use their preferred currencies.
2. Shared Security: Benefits from Polkadot's shared security model, ensuring that the platform maintains high security standards without the cost of establishing its own validator network.
3. Scalability: Leverages Substrate's scalability to handle a growing user base and increasing transaction volumes.
4. Governance: Implements Polkadot's on-chain governance for platform improvements and dispute resolution mechanisms.

---
      Who is your target audience?
- Freelancers (developers, designers, writers, etc.) seeking global opportunities, instant, secure payments and fair treatment, particularly those in emerging economies.Benefit from faster payments, reduced fees, and secure project agreements.
- Clients (startups, enterprises, DAOs) looking for borderless talent without payment complications or trust issues, Gain access to a transparent and efficient marketplace for sourcing talent with automated safeguards.
- Digital workers in unbanked or underbanked regions who need reliable access to global opportunities
- Small businesses seeking specialized skills for project-based work
---
      What need(s) does your project meet?
1. Eliminates trust issues through smart contract escrow (47% of freelancers fear non-payment)
2. Reduces payment delays from 5-14 days to near-instant settlements
3. Lowers transaction fees from 10-20% on traditional platforms to minimal blockchain fees
4. Provides financial inclusion for freelancers in underbanked regions
5. Enables cross-border payments without the complexity and fees of traditional banking
6. Promotes financial inclusion and access to Web3 jobs

[![Platform](https://github.com/MasteraSnackin/Skillbridge-UPDATE/blob/main/docs/Screenshot%202025-04-21%20194420.png)](https://github.com/MasteraSnackin/Skillbridge-UPDATE/blob/main/docs/Screenshot%202025-04-21%20194420.png)

 --- 
    Are there any other projects similar to yours in the Polkadot ecosystem?

- **Polka Finance** is a decentralized job marketplace built on the Polkadot ecosystem (and Aleph Zero), designed to connect freelancers and companies globally. It uses blockchain-based smart contracts for secure, transparent transactions, offers a dispute resolution system, and supports crypto payments. The platform aims to streamline hiring, ensure fair contracts, and make global talent accessible, with features like KYC for trust and OpenAI integration for smarter job matching.

[Polka Finance](https://taikai.network/en/nerdconf/hackathons/nerdathon/projects/cm04j49mo0ppowm016spayqd5/idea"Polka_Finance")

- **Imbue** is another Polkadot-powered freelancing platform. It allows project initiators to post tasks, receive bids from freelancers, and release payments through a milestone system. This ensures freelancers are paid for completed work and clients only pay when satisfied, leveraging blockchain for transparency and fairness.

[Imbue](https://www.imbue.network/"Imbue") not loading at this time

- **BlockchainDevs** is a marketplace for hiring freelance Polkadot developers. While not a decentralized protocol, it connects companies with freelance blockchain developers, including those specializing in Polkadot. Freelancers can negotiate terms directly with clients and work remotely on a contract basis.

[BlockchainDevs](https://www.blockchaindevs.net/hire/polkadot"BlockchainDevs") 

---
        If so, how is your project different?

- Focuses on instant, cross-chain payments and escrow for the global freelance market, not just Polkadot-native roles.
- Integrates on-chain, transparent dispute resolution and a blockchain-based reputation system.
- Prioritizes financial inclusion by leveraging stablecoins and fiat onramps via cross-chain bridges, expanding access to the unbanked.
- Build from client needs


1. Building a comprehensive freelance marketplace requires the integration of multiple complex systems, including payment processing, escrow, dispute resolution, and reputation management. However, blockchain development has historically focused more on pure financial applications than on addressing challenges in labor markets.
2. The technical expertise required to build both a user-friendly marketplace—particularly for users with little or no blockchain experience—and a robust blockchain infrastructure is rare. True cross-chain escrow and payments demand mature interoperability protocols and sophisticated smart contract infrastructure, which are only now becoming widely available on Polkadot.
3. In our recent hackathon win, EchoPay 2, we successfully used @polkadot/api to establish a quick and seamless connection to SubWallet, demonstrating our capability to work with Polkadot’s evolving ecosystem.
4. The timing is ideal: the convergence of remote work, DeFi, and broader Web3 adoption creates the perfect environment for SkillBridge to launch and scale.

### SkillBridge is positioned to fill this gap by creating a specialized solution for the global freelance economy on Polkadot.
 --- 
        If not, why might such a project not exist yet?
  N/A
---
    Note: We prioritize projects building on Plaza/Polkadot Hub, games, and DeFi applications, though all types of projects will be considered.

👥 Team

    Team Name: Name of your team. If you apply as a legal entity, please use its name.
 - Team Name: SkillBridge   
 - Contact Name:  Yanni Freya Wu
 - Contact Email: wuyanni777@gmail.com
 - Website: [SkillBridge](https://skillbridge1.netlify.app/)
  
Team members
* Yanni Freya Wu


      Please list the legal name of all grant beneficiaries. Solo developers (1-person teams) are eligible for funding. LinkedIn Profiles (if available)
 
 [[Yanni Wu Linkedin](https://www.linkedin.com/in/yanni-wu-a64850352)])
 
---
    Team Code Repos

[Skillbridge](https://github.com/MasteraSnackin/Skillbridge-UPDATE)

---

    Please also provide the GitHub accounts of all team members:

[Yanni_Wu_Github](https://github.com/YanniWu88)

Team's experience

## Professional Summary

With over eight years of experience in financial markets and investment analysis, I bring deep expertise in blockchain technology and cryptocurrency markets. My career includes strategic roles at Shanghai Boljie Digital Technology Group and PwC, where I led IPO audits, conducted financial analyses, and provided investment advisory services. My background in evaluating high-stakes investments is complemented by technical proficiency in blockchain, demonstrated through projects such as developing a voice payment system on Solana and an AI-powered racing accident monitoring system. I offer strong analytical skills and a deep commitment to Web3 innovation, consistently bringing financial rigor and strategic insight to every project I undertake.

---
    Please describe the team's relevant experience, including any previous blockchain projects or contributions to the ecosystem.

## Recent Achievements

- **Echo Pay-2:** 3rd Prize Winner, EasyA x Polkadot London Hackathon 2025  
  - Recognized for building innovative solutions on Polkadot’s interoperable, scalable, and secure blockchain platform.
- **Encode London Hackathon 2024:** 2nd Prize  
  - Awarded for excellence in blockchain application development in a highly competitive, multi-disciplinary event.

## Grants Awarded

- **Stellar Kickstarter:** December 2024  
- **Polkadot Guarantee Payout:** August 2024  

## Event Participation

- **Google Cloud x Formula E Hackathon 2024**
- **Startup Village - London 2024**

---

      📊 Development Status

      If you've already started implementing your project, please provide a link and a description of the code. Otherwise, please provide some documentation on the research and other work you have conducted before applying.

## Funding Request & Next Steps

I am seeking funding to support the following next steps in our project development:

- **Team Building:**  
  Assemble a dedicated team, leveraging connections made during the Easy A Hackathons and within the Polkadot community.

- **Technical Specifications:**  
  Create detailed specifications for the smart contract escrow system and payment flow.

- **User Experience Design:**  
  Develop preliminary user interface mockups and map out the complete user journey—from registration through to project completion.

- While code implementation has not yet begun, we are currently drafting a comprehensive technical architecture document that outlines our approach to building on Polkadot and integrating with the broader ecosystem.

---

    📅 Development Roadmap

## Project Overview

| Category              | Details                 |
|-----------------------|-------------------------|
| Estimated Duration    | 3 months                |
| Full-Time Equivalent  | 1 FTE                   |
| Total Costs           | $10,000 USD             |


## Milestone 1: Core Platform & Smart Contract Development

| Section                       | Description / Focus                                                                                          | Key Features / Coverage                                                                                              |
|-------------------------------|-------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| **0b. Documentation**         | Inline code docs & user tutorial                                                                            | - Comprehensive comments for smart contracts<br>- Step-by-step guide: job posting, bidding, escrow, cross-chain pay  |
| **0c. Testing & Security**    | Unit test coverage & testing guide                                                                          | - Instructions for running tests<br>- Validate escrow lock/release<br>- Payment settlement finality                  |
| **0d. Ecosystem Article**     | Content focus for public article                                                                            | - Polkadot XCM integration<br>- Decentralized escrow benefits<br>- Substrate’s advantages for marketplaces           |
| **1. Smart Contract Escrow**  | ink! implementation                                                                                         | - Multi-sig escrow wallet<br>- Milestone-based payments<br>- Dispute resolution oracle integration                   |
| **2. User Management System** | On-chain identity & credentialing                                                                           | - Polkadot.js extension integration<br>- Skill credentials via IPFS hashes                                           |
| **3. Job Marketplace UI**     | Core marketplace interface features                                                                         | - Search/filter projects<br>- Proposal submission with bid tiers<br>- Ratings preview for clients/freelancers        |
| **4. Payment Release Mech.**  | Testnet implementation of payment logic                                                                     | - Automated fund release on milestone approval<br>- Cross-chain settlement simulation (DOT <> KSM)          

---

    This section should break the development roadmap down into milestones and deliverables. Since these will be part of the agreement, please describe the functionality we should expect in as much detail as possible, plus how we can verify and test that functionality.
    
    Important notes:

    Each milestone is capped at $5,000 USD
    Milestones must be delivered within 3 months of approval
    The maximum grant amount is $10,000 USD per application (up to $15,000 USD per project in exceptional cases)
    You will only receive payment after successful milestone delivery

| Milestone | Deliverables                                                                                                 | Cost (USD) | Estimated Completion |
|-----------|-------------------------------------------------------------------------------------------------------------|------------|---------------------|
| 1         | Build a team looking for co-founders                                                                         | $2,000     | 1.5 weeks           |
| 2         | Define The Golden Path, user journey for the freelancer and Client. User flow mapping. <br>Complete user journey—from registration through to project completion. | $500       | 1 week              |
| 3         | Create the User Story Map: user interface designs                                                            | $500       | 1 week              |
| 4         | Define the POC, MVP & MMP                                                                                    | $1,000     | 1 week              |
| 5         | Create a detailed specification like C4 Diagrams (Context, Containers, Components and code Diagram)          | $1,000     | 2 weeks             |
| 6         | Create Simple Smart Contract Escrow                                                                          | $2,000     | 2 weeks             |
| 7         | User Registration, Project Posting                                                                           | $2,000     | 2 weeks             |
| 8         | Payment System, Platform Integration                                                                         | $1,000     | 2 weeks             |
| **Total** |                                                                                                              | **$10,000**| **3 months**        |

---

Overview

    Estimated Duration: Duration of the whole project (maximum 3 months)
    Full-Time Equivalent (FTE): Average number of full-time employees working on the project
    Total Costs: Requested amount in USD for the whole project (maximum $10,000 USD)

    Note that deliverables 0a to 0d are mandatory. Please adapt their specification to your project.

Number 	Deliverable 	Specification
0a. 	License 	Apache 2.0 / GPLv3 / MIT / Unlicense
0b. 	Documentation 	We will provide both inline documentation of the code and a basic tutorial that explains how a user can...
0c. 	Testing and Testing Guide 	Core functions will be fully covered by comprehensive unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests.
0d. 	Article 	We will publish an article that explains what was done/achieved as part of the grant.
1. 	Feature X 	We will create a feature that will... (Please describe in detail)
2. 	Feature Y 	The Y feature will... (Please describe in detail)
3. 	Feature Z 	The Z feature will... (Please describe in detail)
💰 Budget Breakdown

        Please provide a breakdown of your budget by milestone:
        Milestone 	Deliverables 	Cost (USD) 	Estimated Completion
        1 	Features X, Y 	$5,000 	1.5 months
        2 	Feature Z 	$5,000 	1.5 months
        Total 		$10,000 	3 months

---
    🔮 Future Plans

1. Build KYC system or integrate with existing platform
2. Build transparent dispute resolution 
3. Enhance the platform with additional features like advanced reputation systems and specialized marketplaces for different skill categories
4. Develop mobile applications for both Android and iOS to increase accessibility
5. Implement more sophisticated dispute resolution mechanisms, potentially utilizing a specialized justice parachain
6. Expand language support and regional payment integrations to reach more underserved markets
7. Establish a review and scoring mechanism for the delivery work results in specific industries

        How you intend to continue development after the Fast-Grant
1.   [Polkadot-grants-and-funding-guide](https://polkadot.com/blog/the-ultimate-2024-polkadot-grants-and-funding-guide/)

Any plans for seeking additional funding (other grants, VC funding, etc.)
We intend to apply for larger grants from the Polkadot Treasury for specific feature expansions, 

        Your vision for the project's growth and impact in the Polkadot ecosystem

1. Achieve 100,000+ active users within the first two years
2. Process over $50 million in freelance payments annually
3. Expand beyond digital services to include physical goods and local services
4. Create specialized sub-marketplaces for emerging technologies and blockchain development
5. Establish SkillBridge as a core infrastructure component of the Polkadot ecosystem, providing income opportunities for contributors across the network

---
ℹ️ Additional Information

    Here you can add any additional information that you think is relevant to this application, such as:

    Work you have already done
    If there are any other teams who have already contributed to the project
    Other funding you may have applied for

  ## Team Expansion Plans

Team Expansion Plans:
Just found out about this grant on Saturday so I am in discussions with two experienced developers— [Dave Cheng Linkedin](https://www.linkedin.com/in/davecheng82/) and ([James Walker Linkedin](https://www.linkedin.com/in/james-defi/)—either of whom may join the project, depending on their availability.

In addition, we are speaking with two more developers who have hands-on experience with Substrate development and are expected to join the team after the initial funding phase. Their expertise would significantly accelerate the development of more advanced features.

Relevant Experience:

Several members of our team, including myself, have personal experience working as freelancers and have encountered the exact challenges SkillBridge aims to solve. This gives us a unique, user-centered perspective that informs our product design and priorities.

We have also been active participants in the Polkadot ecosystem for over a year. Notably, we received a guarantee fund for our project EchoPay 2 at the EasyA London Hackathon 2024. In addition, we have attended numerous workshops, webinars, and community events to deepen our knowledge and strengthen our connections within the ecosystem.

    Other funding you may have applied for


On Thursday, 17 April 2025, I submitted my project [SKillBridge: Empowering Freelancers Through Decentralized Innovation](https://docs.google.com/document/d/1g6tVjUvINIDS3MUAqD0bIxgS1lInLzHLMLFrS-0P2ns/edit?tab=t.0) to the [Student Blockchain Event](https://moledao.io/#/event/8ac9b6be-343c-4f0a-bcb3-27068ab2e8f7). This submission is currently under review.







