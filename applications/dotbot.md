# 📝 DotBot AI transactions

## 🌟 Project Overview

This desktop application represents a natural language interface for Polkadot blockchain operations, enabling users to execute complex transactions through conversational AI rather than traditional technical interfaces.

### Core Functionality

The platform leverages large language model technology to bridge the gap between user intent and blockchain execution. Users can describe their desired blockchain operations in plain English, eliminating the need for technical knowledge of transaction construction, extrinsic formatting, or specific runtime calls.

### Technical Architecture

The system interprets natural language requests and automatically generates the corresponding Polkadot transactions, including proper parameter encoding, fee calculations, and runtime-specific formatting. The AI handles the complexity of translating user intentions into valid extrinsics that can be submitted to the Polkadot network or its parachains. The core LLM is using [Fetch.AI](http://fetch.ai/) agents through Agentverse to prepare these transactions handling multi-step operations and monitoring transaction status without requiring further user input.

### User Experience

Rather than navigating complex blockchain interfaces or writing code (especially in the Polkadot ecosystem), users simply communicate their objectives conversationally. For example, a user might say "I want to stake 100 DOT to validator XYZ" or "Transfer 50 tokens to this address with a memo," and the system generates the precise transaction required.

### User Journey

The following user journey - which asks for swapping some token to another one - demonstrates one of the capability of DotBot:

1. The user starts by describing the request in the chat: *“Please DotBot, swap my USDC to DOT.”*
2. DotBot asks for the desired amount to swap.
3. The user specifies the amount (e.g., *“Please swap 500 USDC.”*).
4. DotBot asks which USDC (on which chain) to swap, and the desired destination chain.
5. The user defines the chain (e.g., *“Please swap the USDC on AssetHub, and set the destination chain to AssetHub as well.”*).
6. DotBot creates the transaction and presents it in a human-readable way.
    
    Example: *“Based on your request, the initiated transaction is awaiting your approval. After signing, it will swap 500 USDC from AssetHub to 118.5 DOT on Hydration, then automatically send the DOT back to your AssetHub account. Estimated execution time: 30 seconds. Total transaction fee: $0.262.”*
    
7. DotBot sends the transaction to the wallet, prompting the wallet extension to pop up for signing.
8. The user signs the transaction in the wallet extension.
9. Once the transaction is successful, DotBot displays the result. (e.g.: *“Your transaction was successful! 500 USDC on AssetHub was swapped for 118.5 DOT, which is now in your AssetHub account. Would you like to do more with your DOT?”*
10. The user closes or continues requests with DotBot.
### 🔍 Project Details

We expect applicants to have a solid idea about the project's expected final state. Therefore, please submit (where relevant):

- An overview of the technology stack to be used
- Documentation of core components, protocols, architecture, etc. to be deployed
- Any PoC/MVP or other relevant prior work or research on the topic
- Mockups/designs of any UI components
- Data models / API specifications of the core functionality
- What your project is *not* or will *not* provide or implement
  - This is a place for you to manage expectations and clarify any limitations

### Security Model

The tool maintains a secure separation between transaction creation and execution. While the AI constructs the transaction based on user input, the user retains full control through the signing process, ensuring private keys remain secure and users can review all transaction details before authorization.

This approach democratizes access to Polkadot's sophisticated features by removing technical barriers while preserving the security and decentralization principles of blockchain technology.

## Market Research

Several blockchain ecosystems have developed natural language transaction interfaces, but each faces significant limitations that highlight the advantages of building such a tool specifically for Polkadot.

### Existing Solutions

**Griffin AI's Transaction Execution Agent (TEA)** represents the most advanced current solution, operating across multiple EVM-compatible networks including Ethereum, Base, Arbitrum, and Polygon. Users can interact conversationally to send tokens, execute swaps on Uniswap, and manage wallet operations through natural language commands.

[**Fetch.ai](http://fetch.ai/)'s uAgent EVM MCP** provides natural language access to over 30 EVM-compatible blockchains through the Model Context Protocol, while **Infura's MCP server** enables natural language queries for Ethereum on-chain data. Additionally, various platforms like SwarmZero offer NLP interfaces primarily focused on blockchain data analysis rather than transaction execution.

### Key Disadvantages

**Ecosystem Limitations** represent the most significant constraint. Current solutions are overwhelmingly EVM-centric, meaning they cannot access the sophisticated cross-chain capabilities, governance mechanisms, or parachain-specific features that define Polkadot's architecture. This creates artificial barriers between blockchain ecosystems and limits interoperability.

**Limited Cross-Chain Functionality** represents a critical gap in current offerings. While some tools operate across multiple EVM chains, they lack true cross-chain transaction capabilities that would allow seamless asset movement and complex operations spanning different blockchain architectures. This fragmentation forces users to maintain separate interfaces and workflows for different networks.

**Security and Complexity Trade-offs** present ongoing challenges. While these tools aim to simplify blockchain interactions, they often sacrifice transparency and user control for convenience. Users may struggle to understand the underlying transactions being generated, potentially exposing them to unintended risks or sub-optimal execution paths.

A Polkadot native solution would address these fundamental disadvantages by building on Polkadot’s ecosystem linking strengths and allowing users to execute technically challenging tasks just using normal worlds avoiding technical jargon.

## Ecosystem Fit

This natural language transaction tool would function as **universal infrastructure** within the Polkadot ecosystem, serving as a universal interface layer that bridges the gap between user intent and complex blockchain operations. By integrating seamlessly with Polkadot's cross-consensus messaging protocol, it would enable users to execute sophisticated cross-parachain transactions through simple conversational commands, dramatically expanding accessibility to the network's advanced features.

The tool would significantly amplify governance participation by simplifying referendum voting and treasury proposals, while simultaneously making each parachain's unique runtime features accessible to non-technical users. Whether users want to engage with Hydration’s DeFi protocols, Moonbeam's EVM compatibility, or any other specialized parachain functionality, the conversational interface would translate their intentions into proper transactions automatically.

From a strategic perspective, this tool would accelerate ecosystem-wide adoption by serving as both a **universal API layer** for developers and an educational bridge for new users. Rather than building separate transaction construction logic, dApp developers could integrate a single conversational interface, while users naturally learn about staking, governance, and cross-chain operations through interaction rather than documentation.

The broader ecosystem impact would be substantial, likely increasing transaction volumes across parachains, enhancing cross-chain liquidity flows, and improving network security through simplified staking participation. Most importantly, this tool would position itself as **foundational infrastructure** that other ecosystem participants build upon, ultimately accelerating Polkadot's vision of a truly interoperable and user-accessible Web3 ecosystem rather than functioning as merely another application layer.


## Team

- **Team Name:** Hungarian Polkadot DAO
- **Contact Name:** Peter Ott
- **Contact Email:** [polkadothungary@proton.me](mailto:polkadothungary@proton.me)
- **Website:** https://polkadothungary.net/

### Team members

- Peter Ott
- Marklar
- Vikk
- Spectra CryptoVerse
- Fanni Borbás

### LinkedIn Profiles (if available)

- [https://www.linkedin.com/in/ottpeter](https://www.linkedin.com/in/ottpeter/)/
- https://www.linkedin.com/in/spectra-cryptoverse-a5046829a/
- https://linkedin.com/in/fanni-borbas

### Team Code Repos

This is a DAO, that's main activity is not software development. We hare an active member of the Polkadot Community since 2021 and were selected for Decentralized Voices Cohort 3 and 4. 

- https://github.com/Hungarian-Polkadot-DAO/DotBot
- http://github.com/ZelmaCorp/VotingTool

### Team's experience

**Peter**

Full Stack software developer with 4 years of professional development experience and 10 years in the cryptocurrency space, specializing in TypeScript applications. Previously won a price in the DAO Track at Polkadot Championship, demonstrating expertise in decentralized governance solutions. Has hands-on experience with decentralized technologies including IPFS and Swarm, combining deep blockchain knowledge with practical development skills.

**Marklar**

Python developer with strong AI and machine-learning focus. Experienced in building natural-language processing tools and interactive Python applications, demonstrating solid skills in data handling, model integration, and end-to-end prototyping. Combines practical software engineering with a keen interest in applying modern AI techniques to real-world problems.
**Spectra CryptoVerse**

DAO Consultant | Web3 and DeFi Advocate, spent 2 years helping organizations go DAO at the [Aragon](https://aragon.org/) Network DAO, [Hungarian Blockchain Association](https://blockchainhungary.org/rolunk-2/) Board Member, Hungarian Polkadot DAO member, Decentralised Voices Cohort 3 and 4 candidate.

**Vikk**

Economist, with a passion for decentralised technologies. He worked at CoinCash, a crypto exchange based in Hungary. During his university studies he deep dived into Polkadot for the first time in 2020. Since then Vikk became a Polkadot Ambassador, and a true Web3 and DeFi advocate. He is a key player in the Hungarian blockchain scene. Has been organizing Polkadot meetups for 3 years and represented Polkadot at industry events like [Blockchain Budapest 7.0](https://blockchainbudapest.hu/#). Vikk is also the co-founder of the Budapest Blockchain Community Week, where he organized the most attended on-site event of the week, [Polkadot Day](https://lu.ma/PolkadotDayBudapest). 

**Fanni Borbás**

UX/UI Designer and Web Developer with 5+ years of experience creating digital solutions across diverse industries. Specialised in designing user-centric interfaces for AI-powered platforms, cryptocurrency tools, and mobile applications. Has successfully delivered complete brand identities, web designs, and motion graphics for tech startups and blockchain projects. Combines deep understanding of user experience principles with technical implementation skills, creating cohesive digital experiences from concept to deployment.

# Development Roadmap

**Milestone 1**: User Interface is implemented; wallet connection and some AI functionality is working. Possibly to send messages to AI, but it can’t submit transactions to the chain.

**Milestone 2**: Possible to send funds from A account to B account, on AssetHub / PolkadotHub / Hub.

### Overview

- **Total Estimated Duration:** 2 month
- **Full-Time Equivalent (FTE):** 1.2
- **Total Costs:** 9,800 USD

### Milestone 1: User Interface and Simple Transfer

- **Estimated Duration:** 1 month of work already delivered (Core implementation is done; Testing and Documentation is under progress)
    - Github Repository: https://github.com/Hungarian-Polkadot-DAO/DotBot
    - Live PoC Demo: [https://sandbox.dotbot.zelmacorp.io](https://sandbox.dotbot.zelmacorp.io/) (Only UI and basic functionalities, such as wallet connection & AI chat integration)
- **Full-Time Equivalent (FTE):** 0.6
- **Total Costs:** 4,900 USD

| Number | Deliverable | Specification |
| --- | --- | --- |
| 0a. | License | GPLv3 |
| 0b. | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can start using the tool |
| 0c. | Testing and Testing Guide | Core functions will be fully covered by comprehensive unit tests to ensure functionality and robustness. Integration tests will be also implemented, to test external services for API change or other error. In the guide, we will describe how to run these tests. |
| 0d. | Docker | We will provide a Dockerfile that can be used to test all the functionality delivered with this milestone. |
| 0e. | Article | We will publish an **article** that explains what was done as part of the grant. |
| 1. | Design User Interface | We will design the UI of the application in Figma |
| 2. | Implement User Interface | We will implement the design of the application in React |

### Milestone 2: Asset Transfer on AssetHub

- **Estimated Duration:** 1 month
- **Full-Time Equivalent (FTE):** 0.6
- **Total Costs:** 4,900 USD

| Number | Deliverable | Specification |
| --- | --- | --- |
| 0a. | License | GPLv3 |
| 0b. | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can start using the tool |
| 0c. | Testing and Testing Guide | Core functions will be fully covered by comprehensive unit tests to ensure functionality and robustness. Integration tests will be also implemented, to test external services for API change or other error. In the guide, we will describe how to run these tests. |
| 0d. | Docker | We will provide a Dockerfile that can be used to test all the functionality delivered with this milestone. |
| 0e. | Article | We will publish an **article** that explains what was done as part of the grant). |
| 1. | Implement Asset Transfer | We will integrate [Fetch.AI](http://fetch.ai/) interaction, and will create agents on Agentverse |

# Budget Breakdown

| **Category** | **Item** | **Cost** | **Amount** | Total | Description |
| --- | --- | --- | --- | --- | --- |
| Personell | Full-Stack Developer | 10,000 USD | 0.6 FTE | 6000 USD | doing majority of the development work |
| Personnell | Project Manager | 6500 USD | 0.2 FTE | 1300 USD | Project management, coordination, application testing |
| Personnel | User Journey and Application Testing Specialist | 6500 USD | 0.2 FTE | 1300 USD | User journey / application testing, documentation writing |
| Personnel | UI/UX designer | 6,000 USD | 0.2 FTE | 1200 USD | UI/UX design, graphical elements |
|  |  |  | **Total** | **9800 USD** |  |

# Future Plans

We are trying to develop the frontend in a way, that it can be bundled into a lib later, and we are also thinking about a widget, that can be embedded into other sites and application.

Also, we will add more-and-more capabilities to the tool (for example cross-chain asset swaps and governance functions) as we continue developing the tool. 

We are planning to create a mobile version in the future as well.
