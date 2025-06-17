📝 Name of your Project
**DecUniID**

---

🌟 **Project Overview**

**Tagline:** A decentralized identity protocol for university students globally.

**Description:**
DecUniID is a decentralized identity verification system built on Polkadot, focused on university students worldwide. It leverages decentralized identifiers (DIDs) and verifiable credentials to create secure, privacy-preserving, and portable identities that can be verified by third parties (e.g., employers, academic institutions) without exposing sensitive data.

**Integration with Polkadot:**
DecUniID utilizes Polkadot parachain infrastructure to register and verify student identities across chains and jurisdictions, offering a scalable identity backbone that any parachain can access.

**Why we’re building this:**
Student identity fraud is widespread, and current solutions are centralized and fragile. We're building DecUniID to empower students with control over their identities while allowing verifiers to trust the data. Polkadot's cross-chain interoperability makes it ideal for anchoring global identity logic.

---
Thanks for the clarification! The initial draft partially addressed the **long-term value** and **budget breakdown**, but we can **strengthen both sections**. Here's the improved version of those two components, which you can insert into your application:

---

### 🔮 **Long-Term Value to the Polkadot Ecosystem**

DecUniID provides a foundational layer for decentralized identity (DID) verification within and beyond the Polkadot ecosystem. As Polkadot scales to become the backbone of Web3, identity will be a critical pillar enabling trustless interactions. By focusing first on the university ecosystem—a globally distributed, high-trust domain—DecUniID establishes a reusable standard and gateway for broader decentralized identity adoption.

**How it adds long-term value:**

* **Reusable DID Infrastructure**: Institutions and apps building on Polkadot can plug into DecUniID’s verified student credentials for seamless onboarding, access control, credentialed voting, and proof-of-humanity.
* **Cross-chain Compatibility**: Through bridges and shared registries, DecUniID can serve parachains and future XCM-based DID flows, driving interoperability.
* **Ecosystem Adoption Driver**: Verifiable credentials linked to student status (discounts, DAO memberships, scholarships, etc.) can incentivize universities and student developers to build on Polkadot.
* **Foundation for DAO Reputation Systems**: As DAOs seek better governance models, verified education data can be used in voting weightings, task delegation, or grant access.

---

🔍 **Project Details**

**Tech Stack:**

* **Frontend/App:** Flutter
* **Backend & Storage:** Firebase (Firestore, Auth, Functions)
* **Blockchain Layer:** Polkadot-based DID registry (e.g., using KILT Protocol or custom smart contracts)
* **API/Endpoints:** RESTful API for verifiers

**Architecture:**

* DID creation on mobile app after verifying institutional email/domain
* Verifiable credential issuance and storage
* Firebase backend links to Polkadot for credential anchoring
* Public API for data consumers to verify student credentials

**PoC / MVP:**

* Data of 10,000 universities integrated
* DID issuance upon .edu or whitelisted domain verification

**What it’s not:**

* Not a centralized KYC database
* Not a public repository of sensitive student information

---

🧩 **Ecosystem Fit**

**How it fits:**
Polkadot currently lacks a universally adopted student identity layer. DecUniID fills this gap by acting as a universal ID layer usable across DeFi, gaming, DAO voting, etc.

**Target audience:**

* University students (onboarded via Flutter app)
* Verifiers (employers, scholarship bodies, academic partners)

**Problems it solves:**

* Identity verification without privacy loss
* Prevents student impersonation fraud
* Makes it easy for Polkadot-based dApps to integrate verified users

**Similar projects in Polkadot?**
No direct student-focused decentralized identity product yet.

**Why not already built?**
The challenge of onboarding real-world institutions and decentralized data handling is high — we’re solving this with domain-based trust and credential issuance.

---

👥 **Team**

* **Team Name:** GoddeyTech
* **Contact Name:** Ojewoye Wale Goddey
* **Contact Email:** \[Add your email here]
* **GitHub:** [https://github.com/goddeytech](https://github.com/goddeytech)
* **LinkedIn:** [https://www.linkedin.com/in/ojewoye-wale-goddey](https://www.linkedin.com/in/ojewoye-wale-goddey)

**Team Experience:**
Experienced solo developer with background in Firebase, Flutter, and decentralized systems. Previously built internal student directory platforms and mobile-first ID apps.

---

📊 **Development Status**

Initial database of global universities is ready (10k+).
Firebase and Flutter project architecture established.
DID implementation design in progress.

---

📅 **Development Roadmap**

**Overview**

* **Duration:** 3 months
* **FTE:** 1
* **Total Cost:** \$10,000 USD

**Milestones**

| Number | Deliverable                          | Specification                                                         |
| ------ | ------------------------------------ | --------------------------------------------------------------------- |
| 0a.    | License                              | MIT                                                                   |
| 0b.    | Documentation                        | Full API and Firebase setup guide, plus in-app identity flow tutorial |
| 0c.    | Testing Guide                        | Unit and integration tests for verification flow                      |
| 0d.    | Article                              | Publish Medium article on Polkadot student DID use case               |
| 1.     | DID & Credential Engine              | Build DID registration, credential issuance & Firebase integration    |
| 2.     | Verification API & University Import | API for third-party verifiers + ingest university list for onboarding |
| 3.     | Flutter App                          | Student mobile onboarding app to claim and present DID                |

**Budget Breakdown**

| Milestone | Deliverables                      | Cost (USD)   | Estimated Completion |
| --------- | --------------------------------- | ------------ | -------------------- |
| 1         | DID Engine & Firebase Integration | \$4,000      | 1.2 months           |
| 2         | API + University Import           | \$3,000      | 1 month              |
| 3         | Flutter App with Onboarding       | \$3,000      | 0.8 months           |
| **Total** |                                   | **\$10,000** | **3 months**         |

---

🔮 **Future Plans**

* Launch institutional onboarding for issuing universities
* Apply to Web3 Foundation Open Grants or KILT Grants for extended funding
* Build DID Wallet plugin for Polkadot.js
* Monetize API for large-scale verifiers like background check firms
* Explore NFT-based transcript anchoring or DAO-based student identity governance

---

ℹ️ **Additional Info**

* Firebase and Flutter repo scaffolding is ready
* No external funding received yet
* Looking to open-source all modules post-MVP delivery
