# 📝 Harmonify

## 🌟 Project Overview

### One-liner
“Harmonify: Blockchain‑secured, AI‑powered soundtrack seamlessly curating the perfect playlist for every mood and moment with complete data transparency.”

### Brief description
Harmonify is a Polkadot‑based, blockchain‑transparent, decentralised AI platform that gives you full rights over your personal data pods—seamlessly integrating with existing music services and educational resources to democratize access and ownership. By deploying AI models on‑chain and leveraging decentralised knowledge graphs, it crafts dynamic, fine‑grained playlists tailored to your mood, habits, and preferences, while ensuring explainability and cross‑platform interoperability. Even at just 1% of its potential, Harmonify sparks a transformative shift in global music ecosystems, igniting cultural diversity and creative freedom for listeners and artists alike.

## Why We Chose Polkadot

- **Shared Security & Scalability**  
  Leverages the Relay Chain’s pooled security while letting our parachain scale AI workloads independently.

- **Substrate Customizability**  
  Tailor's runtime modules for decentralised AI agents, fine‑grained data‑pod permissions, and on‑chain explainability.

- **Cross‑Chain Interoperability**  
  Uses XCMP to natively integrate with other Web3 ecosystems (e.g., OriginTrail) without external bridges.

- **Fork‑less Upgrades & Governance**  
  Enables seamless protocol and model updates via on‑chain governance—no hard forks or downtime.

### Motivations behind building the project
For too long, music‑streaming platforms have treated listener data as their asset, hiding recommendation logic behind black‑box algorithms and limiting how much users can shape their own discovery. Hours of listening habits, mood signals, and personal preferences are collected, yet fans can’t see how those insights drive their playlists—or export and tweak them outside a single silo. This opaque approach undermines user trust and favours mass‑market hits over emerging or niche artists, stifling creative diversity and leaving listeners frustrated by one‑size‑fits‑all feeds.
 

# 🔍 Project Details

## Technology Stack  
- **Blockchain Layer:** Moonbeam (EVM‑compatible Polkadot parachain)  
- **Smart Contracts:** Solidity for DataPod and AI curation logic  
- **Cross‑Chain Messaging:** Polkadot XCM  
- **Off‑Chain Services:** Node.js microservices, Phala Network for private compute, IPFS for data hosting  
- **Front End & Indexing:** React/Next.js with Tailwind CSS, The Graph and Substrate RPCs initially, moving into app development in Swift and Kotlin

## Core Components & Protocols  
1. **DataPod Registry Contract**  
   Manages creation, ownership, and permissions of user data pods.  
2. **AI Curator Contract**  
   Encodes the playlist generation and feedback logic on‑chain.  
3. **XCM Relayer Module**  
   Handles secure message and data transfers between parachains.  
4. **AI‑Oracle Adapter**  
   Triggers off‑chain AI inference and returns results on‑chain.  
5. **Knowledge Graph Integration**  
   Retrieves and verifies metadata from OriginTrail’s decentralised graphs.  

## Exclusions & Limitations  
- **On‑Chain Audio Streaming & DRM:** Not supported in initial launch.  
- **Mobile Clients:** Deferred to a later phase.  
- **Advanced Governance & Tokenomics:** Postponed until core features are stable.  



### 🧩 Ecosystem Fit

Help us locate your project in the Polkadot landscape and what problems it tries to solve by answering each of these questions:

- Where and how does your project fit into the ecosystem?
Harmonify is delivered as a decentralised application (dApp) built on the Moonbeam parachain, leveraging EVM‑compatible smart contracts to manage user data pods and on‑chain AI curation logic while inheriting Polkadot’s shared security.
  
- Who is your target audience?
Harmonify’s core users are music fans and artists seeking better personalised playlists and (or) transparency within their listening data. We aim to act as a 3rd party tool tool that provides clarity of data usage on top of apps like Spotify, while using this data to provide better music recommendation suggestions.

- What need(s) does your project meet?
It addresses the demand for data sovereignty by giving users full rights over their listening histories and preferences, overcoming opaque data harvesting on mainstream platforms like Spotify and Apple Music. It also fulfils the need for explainable, fine‑grained playlist personalisation by deploying AI curation logic on‑chain, ensuring transparent decision‑making and continuous improvement via user feedback.

  
- Are there any other projects similar to yours in the Polkadot ecosystem?
To my knowledge, there are no d-apps in the Polka ecosystem focusing on AI‑driven, on‑chain music playlist curation. This gap likely exists because on‑chain handling of large multimedia data is technically difficult.

## 👥 Team

- **Team Name:** Harmonify
- **Contact Name:** Ram Vinjamuri
- **Contact Email:** av646@cam.ac.uk
- **My Information:**:
  Linkedin: https://www.linkedin.com/in/ram-vinjamuri/
  Website: https://ramstar3000.github.io/Portfolio/
  
### Team members
At the moment, this is a solo venture, although I have other developers [from Cambridge] interested in collaborating if I need support during this project.

### Team Code Repos

- https://github.com/ramstar3000/EnviroChain = Decentralised platform for smart environmental monitoring
- https://github.com/LeoS0112/SherlockGame = Sherlock Holmes inspired puzzle game, development into adding on-chain components is being completed
- https://github.com/ramstar3000/SkinDetection = CNN understanding project
- https://github.com/ramstar3000/Diss/tree/dev = Natural language parsing on Sanskrit (Request access as this is a private repository)

### Team's experience

I’m relatively new to the Polkadot ecosystem, having learned and built projects through EasyA hackathons. In my first solo event, I placed in the top 10, proof that I can tackle this ambitious project independently, drawing on experience from various codebases and leveraging EasyA’s guidance for any on‑chain challenges.  Additionally, I have lots of experience coding in non-blockchain, ML environments, currently working on a project within Natural Language understanding of Sanskrit. (Currently a private repository but code can be shared upon request)

For initial Polka specific help Anujayan Sugirtharan [https://www.linkedin.com/in/anujayan/] has agreed to help develop code as a temporary team member. He has built various on-chain defi application on both moonbeam and XRP Ledger, with his most notable project being a decentralised betting platform called XRPlay which he begun building in an EasyA Amsterdam hackathon!
 
## 📊 Development Status

Unfortunately development has not begun yet, at the moment I am iterating through different ways to implement this project, while completing my thesis for university, then I will focus on building this project.

## 📅 Development Roadmap

This section breaks the development roadmap down into milestones and deliverables. Since these will be part of the agreement, please describe *the functionality we should expect in as much detail as possible*, plus how we can verify and test that functionality.

**Important notes:**
- Each milestone is capped at **$5,000 USD**
- Milestones must be delivered within **3 months** of approval
- The maximum grant amount is **$10,000 USD** per application (up to **$15,000 USD** per project in exceptional cases)
- You will only receive payment after successful milestone delivery

### Overview

- **Estimated Duration:** Duration of the whole project (maximum 3 months)
- **Full-Time Equivalent (FTE):**  Average number of full-time employees working on the project
- **Total Costs:** Requested amount in USD for the whole project (maximum $10,000 USD)

> Note that deliverables 0a to 0d are mandatory. Please adapt their specification to your project.

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | We will release all code and docs under the **MIT License**.  |
| 0b. | Documentation | Inline comments [e.g. Docstrings] on all contracts and modules, plus a **User Tutorial** covering setup, DataPod creation, playlist generation, and cross‑chain configuration. |
| 0c. | Testing and Testing Guide | ≥90% unit‑test coverage for all logic; plus end‑to‑end integration test. In the guide, we will describe how to run these tests. |
| 0d. | Article | Publish a **grant recap article** (on LinkedIn preferred) detailing architecture, challenges, and outcomes. |
| 1.     | **AI Agents**             | **Specification:** Decentralised AI microservices that monitor user listening events, generate personalised track recommendations via on‑chain parameters  <br>**Verification:** Unit tests covering model invocation logic; simulate a listening session, front‑end displays the recommended tracks correctly. |
| 2.     | **Data Pods**             | **Specification:** Encrypted user data stores (pods) managed by a registry contract, enabling creation, permission grants/revocations, and metadata queries.  <br>**Verification:** Test scripts to create pods, grant/revoke access, and list pods; on‑chain event logs reflect each change; UI flow allows users to manage pod permissions successfully.                   |
| 3.     | **Knowledge Graph Integration**        | **Specification:** Adapter service to fetch and verify metadata from OriginTrail’s decentralised knowledge graphs via XCM.  <br>**Verification:** End‑to‑end test sending a metadata request over XCM to OriginTrail and receiving a valid, verifiable response stored on‑chain; UI correctly displays enriched track metadata.                                       |
| 4.     | **Privacy‑Preserving Compute**         | **Specification:** Off‑chain compute adapter using Phala Network for confidential AI jobs on user data pods.  <br>**Verification:** Trigger a private inference job on Phala with sample input, confirm compute completes off‑chain, and verify the result is returned and recorded on‑chain; unit tests for adapter reliability.                                    |


### 💰 Budget Breakdown

Please provide a breakdown of your budget by milestone:

### 💰 Budget Breakdown

| Milestone | Deliverables                                              | Cost (USD) | Estimated Completion |
|-----------|-----------------------------------------------------------|------------|----------------------|
| 1         | AI Agents                                                 | $4,000     | 1 month              |
| 2         | Data Pods                                                 | $3,000     | 1 month              |
| 3         | Knowledge Graph Integration & Privacy‑Preserving Compute  | $3,000     | 1 month              |
| **Total** |                                                           | **$10,000** | **3 months**         |


## 🔮 Future Plans

- **Post‑Grant Development**  
  After the Fast‑Grant period, we will:  
  - Expand the dApp to include native mobile clients and enhanced UI/UX flows.  
  - Implement on‑chain governance modules and tokenomics to align incentives for curators, listeners, and node operators.  
  - Roll out advanced analytics dashboards and community‑driven model fine‑tuning tools.  

- **Additional Funding Strategy**  
  - Apply for further Polkadot ecosystem grants (e.g., Decentralized Futures, Web3 Foundation) to fund development.  
  - Pursue strategic angel/seed VC rounds to scale team and infrastructure for user acquisition.  

- **Long‑Term Vision & Impact**  
- Position Harmonify as the go‑to decentralized media hub on Polkadot, interconnecting music, and knowledge graphs across parachains.  
- Grow a vibrant, community‑governed ecosystem where users own and monetise their data pods, AI agents become modular services, and new dApps plug in via XCM.  
- Drive cultural innovation by enabling emerging artists and educators to reach global audiences through transparent, permissionless discovery and curation.  


## ℹ️ Additional Information

- **Long‑Term Growth**  
- Fast‑Grant will deliver core modules and public demos, attracting contributors and paving the way for larger follow‑on grants.  
- Aims to become a composable media hub on Polkadot, fostering ecosystem partnerships and user‑driven innovation.

I am attending Y Combinator’s AI Start up school (AI‑SUS), I submitted Harmonify as part of my application for this—underscoring its promise and potential, and will participate in the two‑day program designed to inspire and support AI startups.
