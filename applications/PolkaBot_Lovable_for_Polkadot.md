# 📝 Polka Bot

## 🌟 Project Overview

**Tagline:** Lovable for Polkadot: The fastest way for devs to ship Web3 apps, making Polkadot the default platform to build.

**Project Description:** Polkabot is an AI-powered developer assistant/agent that lets users type a simple prompt and receive a fully functioning Web3 app, built natively for the Polkadot ecosystem. Inspired by Lovable, a no-code AI app builder for Web2, Polkabot brings that same instant-building experience to Web3, enabling both technical and non-technical creators to ship apps quickly and correctly within Polkadot’s architecture.

By going beyond LLMs that just surface documentation, Polkabot applies AI directly to code generation, using prebuilt templates, project scaffolding, and Polkadot best practices to deliver working software. 

**Polkadot Integration:** Polkabot is designed to generate apps that are fully aligned with Polkadot’s architecture, including native support for Substrate, ink! smart contracts, and cross-chain interoperability features. 

Over time, it will support a growing library of project types from DeFi and gaming to DAOs and tools, making Polkadot the fastest and most accessible platform for Web3 development.

Polkabot is part of a broader vision: accelerating the creation of Polkadot-native apps by lowering the barrier to entry and helping founders focus more on building value, not just writing code.


**Motivation:** We're passionate because we believe AI software builders are the future, and want to build this to make it the easiest place to build and launch new ideas for the leading technology in the web3 ecosystem. 

### 🔍 Project Details

**Technology Stack:**

 - React, Shadcn, Vite, Typescript, Tailwind - We expect implementation details will impact our choice of technologies as we build out this project. However, we will build a working IDE and support common Polkadot Dapp types.
 - Subxt, PAPI, SmartContracts - We would like to engage the Polkadot team to find out which project types to support.

**Core Components & Architecture:**
 - Chat UI
 - Website renderer, 
 - In-browser filestorage, 
 - Runtime environment, 
 - Build/compilation tools
 - “Export project” e.g. to continue in Cursor
 - Planner prompts
 - Execution prompts
 - Evals for core LLM steps
 - Example boilerplate Polkadot projects (as ground truth to get the AI closer to)

**Proof of Concept (MVP):** PolkaBot is live and users can generate projects to get started on projects they want to bring to production.

**What PolkaBot is NOT:**
 - Capable of producing bug-free code in 100% of prompts
 - An AI software engineer that will succeed at all project types, sizes, and complexities.
 - Capable of doing anything outside of writing code (e.g. Agentic Browsing to set up AssetHub)

### 🧩 Ecosystem Fit

**Placement in the Polkadot Ecosystem:** This project can appear in Polkadot docs and enable all Polkadot developers to get started quickly with Polkadot.
**Target Audience:** All Web3 creators, especially those wanting to build on Polkadot (hopefully partly because we made it easy for them to do so).
**Similar projects in the Polkadot ecosystem?** None
**USP:** AI App generators weren’t possible 6 months ago, and enable people to try more project types to see what they can scale.

## 👥 Team

- **Team Name:** PolkaShip
- **Contact Name:** Jerome Minney
- **Contact Email:** jeromeminney@gmail.com
- **Website:** http://github.com/jerrysam

### Team members

 - Jerome Minney (lead developer)
 - Mofiyin Onanuga (partnerships and growth)
 - Tom Bizzell (advisor)

#### LinkedIn Profiles (if available)

 - https://www.linkedin.com/in/jeromeminney
 - https://www.linkedin.com/in/mofiyin-onanuga-ba4020188/
 - https://www.linkedin.com/in/tom-bizzell

### Team Code Repos

- App builder (Hackathon Progress): https://github.com/jerrysam/lovable-for-polkadot
- Freight app (started with an App builder): https://github.com/TomBizzell/freight-futures

Please also provide the GitHub accounts of all team members:

 - http://github.com/jerrysam

### Team's experience

 - Worked for DeepMind
 - Worked for Faculty AI (Europe's largest Applied AI consultancy and OpenAI's first implementation partner)
 - Worked for Unkillable (helped build 8 different growth teams for ~Series A stage startups)
 - Founded a company, raised 6 figures, built a product, sold stake as part of a technology acquisition strategy towards Visa.
 - ex VC
 - 6 figure startup Founder
 - Scaled to 100 person Team
 - Digital & Marketing Strategy lead for 7 figure tech startups across SA,UK,US + AUS
 - + more

## 📊 Development Status

 - Hackathon MVP proved the process of creating Polkadot Dapps is possible.
 - Current focus is improving reliability of all components, including IDE, LLM prompt chains, and evals.
 - Next steps include supporting more common Polkadot Dapps and integration work outlined in the Project Details section.

## 📅 Development Roadmap

**Milestone 1:** PolkaBot IDE / Frontend
 - Create (and understand) the frontend components and UI required to build dapps in the browser.
 - Grant team/User can open a live app and prompt for code, edit the code editor, prompt for bash commands, and see the rendered website (output).
 - KPI: Frontend shown to 3 Polkadot developers and feedback gathered for usability

| item | days | rate |
|------|------|------|
| Chat UI | 3 | $250 |
| Website renderer | 2 | $250 |
| In-browser filestorage | 2 | $250 |
| Runtime environment | 3 | $250 |
| Build/compilation tools | 2 | $250 |
| Integration of the above | 2 | $250 |
| Usability research and tweaks | 2 | $250 |
| **Total** | 16 | $4000 |


**Milestone 2:** Polkadot app generation supported
 - Prompts can now generate a working Polkadot app with high reliability, targeting Polkadot Hub
 - How to demo: Users can generate apps and see that the code interfaces with polkadot hub and assets can be managed on Polkadot Hub.
 - Grant team/User can enter a prompt and receive a rendered app, with the ability to refine via follow-up prompts. Works well for one app type.
 - KPI: Product used by 3 developers, and final app / code feedback gathered for usability

| item | days | rate |
|------|------|------|
| Learn to build on Polkadot, and how to teach LLMs to do it | 3 | $250 |
| Example code snippets for LLM to recreate this | 3 | $250 |
| Optimise planning LLM | 2 | $250 |
| Optimise agentic systems | 8 | $250 |
| Build eval sets (testing but for LLMs) | 2 | $250 |
| Usability research and tweaks | 2 | $250 |
| **Total** | 20 | $5,000


**Milestone 3:** Extensibility and Documentation
 - Publish a public article and share results with the Polkadot developer community.
 - Document how to expand the AI’s capabilities to support more project types.
 - Implement unit testing, refactor codebase, and enable community contribution.
 - KPI: Deliver comprehensive documentation, testing guide, and notes for future contributors.

| item | days | rate |
|------|------|------|
| Article | 1 | $250 |
| Implement Testing, refactor | 2 | $250 |
| Documentation on expanding capabilities | 1 | $250 |
| Total | 4 | $1000 |


### Overview

- **Estimated Duration:** 3mo
- **Full-Time Equivalent (FTE):**  1.5 FTE
- **Total Costs:** $10,000


| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License: MIT |
| 0b. | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can contribute to the open source project |
| 0c. | Testing and Testing Guide | Core functions will be fully covered by comprehensive unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| 0d. | Article | We will publish an **article** that explains what was done/achieved as part of the grant. |
| 1. | IDE / Frontend | Users can prompt for code, bash, and see the rendered app |
| 2. | Stable builds | Users can prompt for a Polkadot Dapp, optimised for one type of project|
| 3. | Extensibility | Documentation and refactoring to make it easy for the project to be taken beyond the current vision |

### 💰 Budget Breakdown

Please provide a breakdown of your budget by milestone:

| Milestone | Deliverables | Cost (USD) | Estimated Completion |
| --- | --- | --- | --- |
| 1 | IDE / Frontend build environment | $4,000 | 1 months |
| 2 | Stable builds Dapp build | $5,000 | 1.5 months |
| 3 | Extensibility | $1,000 | 0.5 months |
| **Total** | | **$10,000** | **3 months** |

## 🔮 Future Plans

 - Show the project to many Polkadot developers to prioritise future efforts towards making this the preferred way all Polkadot developers start new projects
 - Extend to support multiple Dapp types
 - Position Polkabot as the default starting point for anyone building on Polkadot, especially non-technical users.
 - Continuously update LLM prompts and boilerplates to reflect the latest Polkadot standards and best practices.
 - Expand support for additional app categories and advanced features through new templates and agent capabilities.
 - Seek additional grant and VC funding to scale the platform, broaden adoption, and reduce technical barriers for Web3 developers.

## ℹ️ Additional Information
 - Genuine interest in both freight logistics and AI app builders (like Lovable) predates this project. The concept for Polkabot came together during the Easy A x Polkadot London hackathon.
 - self-initiated with no external funding or third-party contributions.
 - Open to future collaborations within the Polkadot ecosystem to expand capabilities and adoption.
