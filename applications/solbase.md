# 📝 Solbase

## 🌟 Project Overview

**Tagline:**
The Web3 Audio-Social Super App built to Empower Collaboration, Creativity, & Financial Freedom through Music and Crypto Innovation.

**Description:**
Solbase is an audio-first, decentralized social platform enabling users to connect, create, and transact on-chain. It combines the engagement of Clubhouse, the discovery of Spotify, and the learning of Kindle, all integrated into a single, Web3-powered ecosystem.

The app prioritizes low-bandwidth accessibility, especially for users in emerging markets (Africa, South Asia, LATAM) where connectivity and power infrastructure are poor. By building on Polkadot, we leverage fast, low-cost, scalable, and interoperable infrastructure to enable audio-based social networking, on-chain tipping, tokenized audio NFTs, and community governance.

Solbase extends Polkadot’s ecosystem into the social and creator economy space. It uses Polkadot’s scalability, interoperability, and low-fee environment to power an audio-first Web3 platform where users can host live voice rooms, publish tokenized audio, and earn through on-chain tipping. Integration will leverage Substrate for smart contract logic, Polkadot.js API for wallet and identity, and on-chain governance for community moderation and voting. In doing so, Solbase becomes a human-facing entry point into the Polkadot network,  where people experience blockchain through conversation, content, and connection.

We started Solbase to make Web3 more inclusive for people, especially in regions like Africa where poor connectivity limits access to visual, data-heavy platforms. Audio is lightweight, natural, and human — making it the perfect medium for education, community, and creativity. Solbase enables live audio rooms, podcasts, and on-chain audio ownership, while allowing users to tip creators directly using Polkadot’s low-cost network. Built on Polkadot’s interoperable and community-driven infrastructure, Solbase aims to make Web3 intuitive, open, and truly accessible to everyone.

 [Demo video here](https://drive.google.com/file/d/10x-chJyciQYk2zJF7ITjl59ZMAIBOLcc/view?usp=drive_link)



## 🔍 Project Details

- **Blockchain:**  
  - Built on the Polkadot ecosystem with native DOT token integration for in-app tipping and transactions.  
  - The MVP version does not include smart contracts; blockchain interactions are handled through the Polkadot JS API and backend logic.  

- **Backend:**  
  - **Framework:** NestJS  
  - **Database:** MySQL  
  - **Infrastructure:** AWS (hosting, media storage, CDN delivery)  
  - **Blockchain Integration:** Polkadot JS API for wallet generation, tipping, and transaction execution  

- **Frontend:**  
  - **Mobile:** React Native 
  - **Web:** React.js (planned post-MVP for dashboards and analytics)  

- **Other Tools & Integrations:**  
  - REST API layer connecting frontend and backend  
  - Automatic Polkadot wallet generation upon signup  
  - Secure key management and account recovery handled by the backend  

---
### 🧩 Core Components, Protocols & Architecture

- **User Module:** Handles user registration, login, and automatic Polkadot wallet generation. Each new account is assigned a unique on-chain address.  
- **Creator Module:** Allows musicians, podcasters, and writers to create profiles and upload or link audio content.  
- **Tipping System:** Enables listeners to send DOT tips directly to creators’ wallets via an in-app tipping interface.  
- **Content Feed:** Displays featured and trending audio content through an intuitive and scrollable interface.  
- **Transaction Service:** Executes and tracks Polkadot API–based transactions on the backend.  


---

### 🚀 Proof of Concept / MVP

- Internal working version already developed demonstrating wallet generation and tipping flow.  
- Demo video and GitHub repository available for review.  
- **MVP Features:**  
  - User onboarding and authentication  
  - Creator registration and content listing  
  - DOT tipping via backend API  

---

### 🎨 Mockups / Design Overview

- **Mobile-first MVP** emphasizes a clean, engaging, and social audio experience.  
- **Key Screens:**  
  - **Home Feed:** Displays audio content and featured creators  
  - **Tip Interface:** Integrated with wallet balance and transaction confirmation flow  
  - **Creator Profiles:** Showcases creator details, uploaded content, and total tips  
- **Web Version (Planned):** Post-MVP phase will add dashboards and analytics for creators.  

---

### ⚠️ Project Limitations

The Solbase MVP will **not**:   
- Include NFT minting (planned for future releases)  
- Implement cross-chain swaps or DeFi mechanics at launch  
- Provide a public API or data indexer during the MVP phase  


### 🧩 Ecosystem Fit

- **Where it fits:**  
  Most Polkadot projects focus on infrastructure, DeFi, or developer tools. **Solbase** complements them by adding a social and content layer — connecting people to those technologies through everyday use. It can integrate with identity, DeFi, and NFT parachains to enable creator verification, tipping, and cross-chain content ownership. In essence, Solbase brings a consumer-facing dimension that helps new users experience the Polkadot ecosystem beyond finance.

- **Audience:**  
  Our audience is primarily a young and vibrant generation of creators, community builders, and educators who use audio to express, connect, and grow. This includes musicians, podcasters, Web3 community managers, and educational content creators who want to reach their audiences without heavy data costs or technical complexity.  
  We also target emerging-market users and Web3 newcomers — individuals eager to learn, share ideas, and earn through creativity but often limited by connectivity or resources. For them, Solbase offers an easy, voice-driven gateway into decentralized technology and financial empowerment.

- **Needs met:**  
  Solbase addresses three core needs:  
  - **Access:** Provides a low-bandwidth, inclusive entry into Web3 for people in regions with limited infrastructure.  
  - **Ownership:** Gives creators true control over their voice content through tokenization and on-chain royalties.  
  - **Community:** Enables users to connect, learn, and govern together through decentralized audio spaces.  
  Together, these make digital participation more open, rewarding, and human-centered.

- **Existing projects:**  
  Within the Polkadot ecosystem, **Subsocial** is the closest project to Solbase — a decentralized social network focused on content ownership and monetization of written media. Projects like **Bit.Country** (social metaverse experiences) and **MusicDAO** (music rights and royalties) explore related areas.  
  However, there are few, if any, Polkadot projects centered on **audio-based social interaction and creator monetization**. While some address content or community, none combine real-time voice rooms, tokenized audio, tipping, and governance in a single, accessible product.  
  Such projects are rare because most Web3 efforts have focused on finance, infrastructure, and tooling rather than social or cultural experiences. Solbase fills that gap — introducing an audio-first social layer that unites live voice conversations, podcasts, creator rewards, and learning hubs within one interoperable Web3 ecosystem.

- **How it differs:**  
  - **Subsocial** enables decentralized text-based content creation but lacks real-time, voice-driven engagement.  
  - **Bit.Country** focuses on immersive 3D metaverse experiences rather than lightweight, mobile-first social audio.  
  - **MusicDAO** tackles music royalties within a niche vertical, not community-led voice content.  
  **Solbase** stands apart by merging voice interaction, content tokenization, community governance, and micro-economies into one inclusive platform that thrives even in low-connectivity regions.  
  This positions Solbase as the **first audio-social bridge for Polkadot**, connecting millions of new users — especially creators and digital communities — to Web3 through the simplicity of sound.


## 👥 Team

- **Team Name:**  
  Solbase Team

- **Contact Name:**  
  Damilola Olayiwola  
  Emmanuel P. Charles

- **Contact Email:**  
  solbasehq@gmail.com  
  opeyemicharlese@gmail.com  
  olayiwoladamilola7@gmail.com

- **Website:**  
  [www.solbase.xyz](https://www.solbase.xyz)

### Team members

- Damilola Olayiwola  
- Emmanuel PCharles  
- Ayomide Oyediran  
- Ayomide Obiwale  
- Kosama Essien

#### LinkedIn Profiles (if available)

- [Damilola Olayiwola](https://www.linkedin.com/in/damilola-dammy-o-557b10113)
- [Emmanuel P. Charles](https://www.linkedin.com/in/emmanuelpcharles/)

### Team Code Repos

- [Solbase GitHub Organization](https://github.com/Soldapps)

Please also provide the GitHub accounts of all team members:

- [Damilola Olayiwola](https://github.com/Mozihla)
- [Emmanuel P. Charles](https://github.com/emmanuelpcharles)

### Team's experience

**Emmanuel P. Charles — Blockchain & Mobile Engineer**  
Emmanuel is a Mobile Engineer and former **Algorand DevRel Ambassador (2022)**, where he contributed to the **Algorand Swift** and **Go SDKs**.  
He has built and scaled multiple blockchain products, including **CRED**, a blockchain-powered analytics tool ranked **#2 on Aptos**, and several **DeFi and NFT** integrations at **Townesquare** across **Monad**, **Aptos**, and **Solana**.  
At **AlgoFame**, he developed a Web3 platform for agricultural stakeholders on **Algorand**, integrating **Folks Finance SDK** for staking and swaps.  
He has also contributed to **ETHNigeria**, **Lagos Blockchain Week**, and **London Tech Week**, promoting blockchain adoption globally.

**Damilola Olayiwola — Product Designer & Product Strategist**  
Damilola is a Product Designer with over **4 years of experience** building fintech and Web3 products.  
He co-founded the **Scrim App**, a blockchain-based value transfer solution that used **Scrim tokens** to enable borderless payments via email or Twitter handles.  
Scrim was **acquired by Chimoney (Canada)** in **2023**.  
Damilola has also consulted for startups, helping them design and launch inclusive, user-friendly blockchain products.


## 📊 Development Status

The core Solbase MVP is currently in development, featuring **audio playback**, **creator tipping**, which allows users to stream, and tip creators in a tokenized environment, serving as the foundation for the next phase of development.

**Repository:**  
[https://github.com/Soldapps/solbase](https://github.com/Soldapps/solbase)  

The repository contains the base code for the Solbase MVP, implemented using React Native, Node.js, and smart contract integrations.

So far, our efforts have focused on:  
- Building a mobile-first decentralized audio application  
- Integrating wallet-based tipping and reward logic  
- Conducting closed beta testing with over 300 early users  
- Designing UI/UX for the compliance dashboard and DID integration (in progress)  

These milestones demonstrate that the project is past the idea stage and entering an **integration and optimization phase** — positioning it for expansion into the **Polkadot ecosystem**.

---

## 📅 Development Roadmap

The development roadmap focuses on enhancing Solbase with **Polkadot network capabilities**, **decentralized identity verification**, and **improved audio infrastructure**.  
Each milestone is designed to deliver verifiable progress within the 3-month grant window.

| **Milestone** | **Deliverables** | **Cost (USD)** | **Estimated Completion** |
| -------------- | ---------------- | --------------- | ------------------------- |
| **Milestone 1 — Core Polkadot Integration & Audio Infrastructure (Month 1–1.5)** | - Integrate Solbase with **Polkadot testnet** for wallet and transaction functionality.<br />- Implement **micro-transaction tipping system** using Polkadot tokens.<br />- Upgrade **audio infrastructure** to IPFS/Crust for decentralized upload and playback.<br />- Extend audio features to support **playlists, podcasts, audiobooks, and creator uploads**.<br />- Conduct internal QA and publish testing guide. | $5,000 | 6 weeks |
| **Milestone 2 — Creator Verification, Compliance Dashboard & Public Beta (Month 1.5–3)** | - Implement **DID-based creator verification system** to authenticate creators and prevent piracy.<br />- Launch the **compliance and moderation dashboard** for internal content management.<br />- Deploy public **Solbase Beta** integrated with Polkadot wallets.<br />- Publish a technical article and complete final grant report. | $5,000 | 6 weeks |

**Total Grant Request:** **$10,000 USD**  
**Total Timeline:** **3 months**

Each milestone includes verifiable deliverables such as working smart contracts, UI integrations, testnet deployment proofs, and public documentation.

**Total Grant Request:** **$10,000 USD**  
**Total Timeline:** **3 months**

Each milestone includes verifiable deliverables such as working smart contracts, UI integrations, testnet deployment proofs, and public documentation.




### Overview


| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
|
| **0a.** | **Documentation** | We will provide detailed **inline documentation** within the codebase, along with a comprehensive **developer tutorial** covering Polkadot integration steps, smart contract deployment, and how creators can onboard using decentralized identities (DIDs). |
| **0b.** | **Testing and Testing Guide** | Core modules such as DID integration, Polkadot wallet connection, and tipping logic will be fully covered by **unit and integration tests**. A testing guide will describe environment setup, testnet simulation, and verification of smart contract interactions. |
| **0c.** | **Article** | We will publish an **article** on the Polkadot Forum and Medium highlighting the technical process of extending Solbase with Polkadot micro-transactions, identity verification, and decentralized audio features. |
| **1.** | **Polkadot Integration Layer** | Integrate Solbase with the **Polkadot network** to enable micro-transactions, staking rewards, and wallet interoperability. This includes connecting existing tipping and creator reward systems to Polkadot-based tokens. |
| **2.** | **Decentralized Identity (DID) & Creator Verification** | Implement a **DID-based verification system** to authenticate creators and prevent piracy while maintaining privacy. This layer will link verified DIDs to creator profiles and reward addresses. |
| **3.** | **Compliance & Moderation Dashboard** | Build an **internal dashboard** to handle flagged content, user verification, and on-chain compliance tracking — improving trust, transparency, and content integrity within the ecosystem. |
| **4.** | **Audio Infrastructure Optimization** | Upgrade the existing **audio upload and streaming modules** by integrating **IPFS/Crust** for decentralized storage and optimizing caching for low-bandwidth regions, ensuring better accessibility for users in emerging markets. |


### 💰 Budget Breakdown


| Category | Description | Amount (USD) |
| --- | --- | --- |
| **Development & Smart Contracts** | Audio upload/playback module, tipping logic, wallet and DID integration | $6,000 |
| **Audio Infrastructure** | IPFS/Crust storage, decentralized streaming, caching optimization | $2,000 |
| **KYC & Compliance** | Creator verification and anti-piracy backend | $1,500 |
| **Design & UX** | Interface refinements for audio and tipping flows | $1,200 |
| **Deployment & QA** | Play Store release, web hosting, internal testing | $1,800 |
| **Community & Documentation** | Beta materials, grant report, open-source repos | $2,500 |
| **Total** |  | **$15,000 USD** |

---

### 💰 Budget by Milestone

| Milestone | Deliverables | Cost (USD) | Estimated Completion |
| --- | --- | --- | --- |
| **Milestone 1 — Core Audio Platform Upgrade (Month 1–1.5)** | • Integrate podcast uploading and streaming feature into the existing Solbase app  <br />• Expand music library and optimize local caching for low-bandwidth users  <br />• Implement decentralized audio upload and playback via IPFS/Crust  <br />• Strengthen wallet integration and test on Polkadot testnet  <br />• Conduct internal QA and bug-fixing sprint across mobile and web builds | **$5,000** | **6 weeks** |
| **Milestone 2 — Creator Verification, Polkadot Integration & Public Deployment (Month 1.5–3)** | • Implement KYC and creator verification for piracy prevention and authenticity  <br />• Build creator tipping and reward smart contract powered by Polkadot micro-transactions  <br />• Integrate on-chain DID (Decentralized Identity) for verified creators  <br />• Prepare Play Store submission and web deployment for Solbase beta  <br />• Conduct open beta testing and finalize grant report/documentation | **$5,000** | **6 weeks** |
| **Total** |  | **$10,000** | **3 months** |


## 🔮 Future Plans

### **Post–Fast Grant Development**
After the Fast Grant, **Solbase** will focus on evolving into a full-scale, Polkadot-powered social audio network through the following milestones:

- **Closed Community Testing (500+ Users):**  
  Conduct structured beta testing cohorts to gather UX feedback, optimize wallet and on-chain interactions, and validate engagement loops.

- **Compliance & Moderation Dashboard:**  
  Build an internal tool for managing flagged content, disputes, and creator support, ensuring user safety and content quality.

- **Creator Tipping, Tokenization & Staking Expansion:**  
  Introduce a richer reward model leveraging Polkadot micro-transactions, creator staking, and voice-based engagement incentives.

- **Public Launch & Ecosystem Integration:**  
  Complete open beta and integrate with Polkadot’s identity, governance, and reputation modules for seamless user onboarding.

- **Scalability & Partnerships:**  
  Collaborate with other Polkadot parachains and audio-related projects for interoperability, music rights management, and NFT-based content ownership.

This roadmap ensures Solbase transitions from a functional MVP into a **community-governed, interoperable audio-social hub**, showcasing Polkadot’s human-centered Web3 potential.

---

### **Funding Strategy**
Yes — after completing the Fast Grant phase and reaching the next functional milestones, we plan to secure additional funding through:

- **Ecosystem Grants:**  
  Apply for follow-up grants from **Web3 Foundation**, **Astar**, and **Kusama Treasury** to support community onboarding and Polkadot feature integrations.

- **Strategic Partnerships & VC Funding:**  
  Continue discussions with Web3-focused venture firms and accelerators to raise a **seed round** for infrastructure, licensing (music APIs), and market expansion.

- **Sustainable Revenue Model:**  
  Our long-term funding strategy prioritizes sustainability through:
  - Polkadot-based transaction fees  
  - Creator royalties  
  - Premium audio spaces  
  - Premium features (analytics, ads)

  These will serve as recurring revenue streams, minimizing long-term dependency on external funding.

This approach ensures that Solbase remains **community-aligned**, **financially sustainable**, and positioned for scalable growth beyond the initial grant phase.

---

### **Vision & Ecosystem Impact**
Our vision is to make **Polkadot the home of the world’s first large-scale social audio network** — where creators, communities, and everyday users interact, transact, and govern using blockchain.

Over time, Solbase will expand into an **audio-social layer** within the Polkadot ecosystem, enabling:

- 🎙 **Voice-Based Governance Participation** — DAOs and parachain communities can hold town halls and votes through verified voice channels.  
- 🎧 **Cross-Chain Audio NFTs & Royalties** — creator content transferable across parachains, ensuring liquidity and interoperability.  
- 🪪 **Identity-Based Reputation Systems** — on-chain profiles and badges tied to verified creators and community members.  
- 🌐 **DePIN-Style Audio Nodes** — users can host or stream content while earning from decentralized participation.

By centering real human interaction, Solbase helps **shift Polkadot from a protocol-first to a people-first ecosystem**, proving that Web3 can be **social, inclusive, and culture-driven**.


## ℹ️ Additional Information

In 2023, **Solbase** participated in the **Solana Summer Camp Hackathon** organized by **DoraHacks**, one of the largest global Web3 developer competitions. We presented **Solbase DApp** — a social audio platform merging communication, education, and decentralized finance through voice.  

The project stood out for its **audio-first, low-bandwidth approach**, designed to help users in regions with limited connectivity access knowledge, create content, and transact using crypto efficiently.  

**Solbase earned 3rd place**, receiving a **$6,000 starter fund in SOL** and recognition for its innovation and user-centered design. The exposure led to valuable advisory relationships with members of the **Solana** and **DoraHacks** communities.  

This achievement validated Solbase’s vision and the team’s capability to design, build, and deliver meaningful decentralized applications. We are now expanding on that foundation by integrating **Polkadot’s scalable and interoperable infrastructure** to power creator tipping, wallet generation, and audio content tokenization.

The **current Polkadot version** of Solbase is being developed by the **Solbase Core Team**, led by **Emmanuel P. Charles** (Blockchain & Mobile Engineer) and **Damilola Olayiwola** (Product Designer & Strategist).  
While we have received guidance from mentors and advisors, **no external teams** have contributed directly to this phase.

To date, Solbase has only received the **$6,000 hackathon starter fund** from DoraHacks and has **not applied for any other grants or VC funding** related to this project.  
This **Fast Grant** application represents our **first formal ecosystem funding request**, aimed at advancing Solbase from MVP to a fully integrated Polkadot-powered product.

We view the Fast Grant as a **strategic first step** in evolving Solbase into a **flagship social audio protocol** within the Polkadot ecosystem — demonstrating how Web3 can empower **human connection, creativity, and community through sound.**

