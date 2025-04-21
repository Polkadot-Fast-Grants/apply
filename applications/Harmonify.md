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
 

### 🔍 Project Details


**Development Status**  
Development has not yet begun, as our lead is focused on dissertation writing and will defend in early May.  

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


### Team's experience

I’m relatively new to the Polkadot ecosystem, having learned and built projects through EasyA hackathons. In my first solo event, I placed in the top 10, proof that I can tackle this ambitious project independently, drawing on experience from various codebases and leveraging EasyA’s guidance for any on‑chain challenges.

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
| 0a. | License | Apache 2.0 / GPLv3 / MIT / Unlicense |
| 0b. | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can... |
| 0c. | Testing and Testing Guide | Core functions will be fully covered by comprehensive unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| 0d. | Article | We will publish an **article** that explains what was done/achieved as part of the grant. |
| 1. | Feature X | We will create a feature that will... (Please describe in detail) |
| 2. | Feature Y | The Y feature will... (Please describe in detail) |
| 3. | Feature Z | The Z feature will... (Please describe in detail) |

### 💰 Budget Breakdown

Please provide a breakdown of your budget by milestone:

| Milestone | Deliverables | Cost (USD) | Estimated Completion |
| --- | --- | --- | --- |
| 1 | Features X, Y | $5,000 | 1.5 months |
| 2 | Feature Z | $5,000 | 1.5 months |
| **Total** | | **$10,000** | **3 months** |

## 🔮 Future Plans

Please include:

- How you intend to continue development after the Fast-Grant
- Any plans for seeking additional funding (other grants, VC funding, etc.)
- Your vision for the project's growth and impact in the Polkadot ecosystem

## ℹ️ Additional Information

Here you can add any additional information that you think is relevant to this application, such as:

- Work you have already done
- If there are any other teams who have already contributed to the project
- Other funding you may have applied for

Remember that the Fast-Grants Programme is designed as a first step for promising projects. We're looking for projects that can continue to grow beyond this initial funding.
