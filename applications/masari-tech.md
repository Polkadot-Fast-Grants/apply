# 📝 Masari Tech

## 🌟 Project Overview

### Tagline

An AI-powered off-price fashion marketplace with on-chain verified excess stock transparency.

### Brief Description

Masari is building an AI-powered off-price marketplace that helps fashion brands move excess inventory profitably, while giving shoppers a personalized experience that saves them time and money. Fashion brands lose $2.5-5B in unsold stock annually, and new EU laws coming in 2026 will ban the destruction of inventory. At the same time, 82% of shoppers want AI to reduce research time, and 60-75% already shop resale or outlet. Masari taps into these shifts by combining AI personalization, price, and purpose. Now, we’re adding an on-chain transparency layer that lets brands verify specific product batches as excess stock. This badge-based module improves trust, supports compliance, and can be reused across the ecosystem as an open-source tool.

### Relation to Polkadot

Our transparency verification module will be deployed on Polkadot Asset Hub. It enables fashion brands to record a public, immutable proof that specific product batches are excess inventory.

### Why We're Creating This Project

We’re solving a $2.5B+ unsold stock problem in fashion, while anticipating regulatory pressure and shifting consumer expectations. We believe blockchain can offer lightweight, verifiable transparency for brands without requiring deep technical integration. This project also lays the foundation for more advanced sustainability data (like CO₂ tracking) and strengthens Masari’s vision of a more efficient and ethical fashion ecosystem.

### 🔍 Project Details

### Technology Stack

- **Frontend:** Next.js (React) with TailwindCSS, deployed on Vercel
- **Blockchain Layer:** Solidity smart contracts on a Polkadot-compatible EVM chain (e.g. Moonbeam)
- **Web3 Integration:** Ethers.js or Polkadot.js for contract interaction
- **Data Handling (optional):** Supabase for pre-chain metadata handling and admin auth (if needed)
- **Tooling:** Hardhat for smart contract development and testnet deployment

### Core Components & Architecture

- **Smart Contract**
  - Stores verified product batch records including: product IDs, brand ID, and excess stock attestation
  - Supports read/write functions with access control
- **Admin Interface (Web UI)**
  - Allows Masari or brand admins to submit batch-level verification (via form or CSV upload)
  - Connects to blockchain and pushes verification data to the contract
- **Public Viewer (Web UI)**
  - Lets shoppers or auditors view excess stock verification badge per product
  - Optional: filter by "Verified" products or view more details from on-chain data

### Prior Work or Proof of Concept

This feature is a new addition to Masari Tech’s ecosystem. While the transparency tracker is new, our broader marketplace has already shown traction: a 200+ user waitlist, competition wins, and active brand outreach. We’ve also partnered with a sustainability organization offering 10 free SKU-level Life Cycle Assessments (LCAs) once brand integration begins - which this module lays the groundwork for.

### Mockups / UI Concepts

We plan to build:

- A simple **Admin dashboard** (to submit excess stock batch attestations)
- A lightweight **public viewer** (to show verification badges and data on product pages)

Mockups will include:

- Input form for brands or Masari admins
- Badge UI on product pages (e.g. "Verified Excess Stock")
- Optional tooltip or detail view for transparency

### Data Model / API Overview

**Smart Contract Fields (per record):**

- `batchId` (string)
- `productIds` (array of strings)
- `brandId` (string or wallet address)
- `timestamp` (uint)
- `verified` (bool, always true if written to chain)

**Public Read Functions:**

- `getVerificationByProductId(productId)`
- `getBatchDetails(batchId)`

### What This Project _Will Not_ Include

- It will **not verify product origin or CO₂ impact** in the MVP, though fields will be reserved for future use.
- It will **not include wallet-based brand signatures** or cryptographic proofs in v1 - brands will attest through a trusted submission flow.
- It will **not replace Masari’s core marketplace**, but act as a modular verification layer.

### 🧩 Ecosystem Fit

### Where and how does your project fit into the ecosystem?

Masari brings a new real-world use case to Polkadot: on-chain verification of excess inventory in fashion retail. While most projects focus on DeFi, gaming, or infrastructure, we apply blockchain to transparency, compliance, and sustainability (all urgent challenges in fashion).

### Who is your target audience?

Fashion brands looking to manage and monetize excess stock in a compliant, trust-enhancing way (especially in the EU). Shoppers who want affordable, personalized, and transparent fashion. For this module, we also target developers and builders interested in transparency use cases beyond DeFi.

### What needs does your project meet?

We help brands prove that certain product batches are excess inventory to support compliance and ESG reporting. We also help shoppers trust that they’re buying from a responsible source.

### Are there any other projects similar to yours in the Polkadot ecosystem?

None that we’re aware of. Most supply chain projects focus on logistics or provenance. We focus on excess inventory verification - a gap that Polkadot is well-positioned to fill.

## 👥 Team

### Team Name

Masari Tech

### Contact Name

Rukaiah Edhah

### Contact Email

rukaiah.edhah@masaritech.com

### Website

https://masaritech.com/

### Team Members

- Samira Salifu
- Rukaiah Edhah
- Rashaad Lee Hue-Joseph

### LinkedIn Profiles

- https://www.linkedin.com/in/samirasal5/
- https://www.linkedin.com/in/rukaiah-edhah/
- https://www.linkedin.com/in/rleehue-joseph/

### Team Code Repos

We currently have three repositories:

- **Current Waitlist Website** – Our live site at https://masaritech.com, used to collect early interest  
- **New Waitlist Website** – A complete redesign in progress, which will include additional pages like our story, blog, and expanded brand messaging  
- **Masari Marketplace (E-commerce Platform)** – Our core product, currently under development

All repositories are currently private. However, for this specific project, the transparency module repo will be fully open-source.

### GitHub Accounts

- https://github.com/samirasal
- https://github.com/rukaiah-edhah
- https://github.com/shaaddev

### Team’s Experience

While this is our first blockchain project, we are a highly technical team of Computer Science majors with strong backgrounds in full-stack development, product design, and execution.

- **Samira (Founder & CEO)** has experience in AI and machine learning. She was recognized by Forbes 30 Under 30 as an emerging founder and won the Drexel Innovation Program.

- **Rukaiah (Founder & CPO/COO)** is a product-focused technologist who has built 5+ software projects, led multiple engineering teams, and scaled one to 1,000+ users in two weeks. She launched her first e-commerce business at 17 and has a deep understanding of operations and systems.

- **Shaad (CTO)** brings strong backend and frontend engineering skills and is fully focused on product development. He’s experienced in architecting scalable systems and will lead the implementation of our smart contract and web3 integrations.

We’re excited to apply our technical skills to the Polkadot ecosystem and are designing this project to start simple, open-source, and composable.

## 📊 Development Status

Development for the transparency module has not yet started. This application outlines the full scope, architecture, and roadmap for the project.

However, we have already begun development on the broader Masari platform, which includes:
- Our **waitlist and marketing website** (in progress), which will host key pages like blog, community, and about
- Our **e-commerce marketplace**, which will include AI personalization features to help shoppers find items faster

All repositories are currently private, but the transparency module developed under this grant will be fully open-source.

## 📅 Development Roadmap

This project will be delivered in three milestones over the course of two months. The goal is to launch a fully functional, open-source module that enables excess stock batch verification on-chain, along with a public viewer UI. Our roadmap follows a clear progression: first laying the blockchain foundation, then layering on the web interfaces and documentation needed to showcase and share the tool.

---

### Overview

- **Estimated Duration:** 2 Months
- **Full-Time Equivalent (FTE):** 1.5 FTE
- **Total Costs:** $10,000 USD

> Note that deliverables 0a to 0d are mandatory. Please adapt their specification to your project.

| Number | Deliverable                             | Specification                                                                                                                                                                                                                                                                   |
| -----: | --------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|    0a. | License                                 | MIT                                                                                                                                                                                                                                                                             |
|    0b. | Documentation                           | We will provide both inline documentation of the code and a basic tutorial that explains how a Masari/Brand Admin can submit batch verification data and how a shopper can view verification status.                                                                            |
|    0c. | Testing and Testing Guide               | Core smart contact functions and key UI interactions will be fully covered by comprehensive unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests                                                                            |
|    0d. | Article                                 | We publish an article that explains the implementation of a blockchain-based excess stock verification system, its benefits, and how it can be used.                                                                                                                            |
|     1. | Smart Contract Development & Deployment | We will develop and deploy a Solidity smart contract on a Polkadot-compatible EVM chain (e.g Moonbeam) that stores verified product batch records, including product IDs, brand ID, and excess stock attestation. This includes access control mechanisms for write functions.  |
|     2. | Admin Interface (Web UI)                | We will create a Next.js based admin interface that allows Masari or brand admins to submit batch-level verification data via form or CSV upload. This interface will connect to the blockchain and push verification data to the smart contract using Ethers.js or Polkadot.js |
|     3. | Public Viewer (Web UI)                  | We will develop a public-facing Next.js web UI that allows shoppers or auditors to view the excess stock verification badge per product. This UI will allow filtering by "Verified" products and display more details retrieved from on-chain data.                             |

### 📅 Development Roadmap

| Milestone | Deliverables | Cost (USD) | Estimated Completion |
|-----------|--------------|------------|----------------------|
| **1**     | - Smart contract development & deployment on Polkadot Asset Hub  
- Admin interface (Web UI) for batch submission  
- Inline code documentation and basic unit testing  
- **Launch goal**: test with up to **1 pilot brand** (or internal simulation if needed), aiming for **≥ 5 batch uploads**, **≥ 200 verified products**, and **≤ 0.05 DOT** per write transaction | $5,000 | 2 Months |
| **2**     | - Public viewer (Web UI) to display verification badges  
- Final testing coverage, setup guide, and educational article  
- Open-source release of the full module  
- **Launch goal**: public viewer live with **filterable verified products**, on-chain data displayed per product, and a walkthrough article to support testing and adoption | $5,000 | 1 Month |
| **Total** | — | **$10,000** | **3 Months** |

We are currently in early brand discovery and outreach. While our goal is to onboard a real partner, we will simulate batch attestations with test data if needed to meet technical launch goals and ensure on-chain functionality is fully demonstrated.

On-chain record visibility (e.g. full batch or wallet-level views) will be accessible via Polkadot-native block explorers like Subscan. We do not plan to build a separate explorer as part of this grant.


### 💰 Breakdown of Grant Use

This grant will support core tools, infrastructure, and strategic partnerships that enable us to build Masari Tech’s off-price platform.

| Category | Description | Cost (USD) |
|----------|-------------|------------|
| **AI Infrastructure & Tools** | API credits, vector database setup, and prompt engineering tools for personalized shopping experience | $2,500 |
| **Web3 Deployment & Infra** | Smart contract deployment tools, Polkadot integration support, block explorer/testing environments | $2,000 |
| **Sustainability Partnership** | Integration with SKU-level LCA provider for verified impact¹ | $1,000 |
| **Virtual Try-On Exploration** | Early pilot conversations and testing setup with VTO providers | $750 |
| **Developer Tools & Infra** | GitHub Copilot, Vercel hosting, Supabase, CI/CD, domains | $1,250 |
| **Content & Open-Source Launch** | Design, copywriting, and educational assets for public release | $1,000 |
| **Intern Enablement** | Onboarding workspace tools (e.g. Notion, Figma upgrades) | $500 |
| **Total** | — | **$10,000** |

¹ We are also exploring an optional brand-facing **impact dashboard**. If pursued, it would cost approximately **$6,000**, which is not included in this grant.

These estimates are based on ~100–120 hours of work at an average blended rate of ~$80/hour across development, UI, and content execution.

## 🔮 Future Plans

After the Fast-Grant, we plan to integrate this transparency module directly into our marketplace. We may expand it to support CO₂ impact tags using SKU-level LCAs as brand partnerships grow.

We plan to raise pre-seed funding to scale our tech and operations, while also exploring additional partnerships and grant opportunities. Later this year, we aim to launch a beta version of the marketplace to test with early users. However, we’re still validating the ideal timing for launch based on expert insights and market signals.

We're also actively growing the brand through marketing, community building, and ongoing industry engagement.

## ℹ️ Additional Information

Watch this 2-minute video to see a demo of our marketplace in action and get a quick look at where we are in our journey: [Watch here](https://youtu.be/895UsdWQkj8)