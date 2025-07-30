# 📝 Pattern: An AI agent that makes blockchain scanners simple, searchable, and human-readable.

## 🌟 Project Overview

### Description

#### Brief
Pattern is an AI agent that helps both average and power users make sense of blockchain scanner data. Right now, the scanner experience is messy—data is scattered, hard to read, and built for people who already know what they’re doing (and even they struggle sometimes). Pattern changes that. You ask a question in plain language, it pulls real-time data from scanners, breaks it down, and gives you a clear, easy-to-understand answer. Dig deeper, ask follow-ups, or just explore—without friction.

#### Polkdot Integration
With this grant, we plan to integrate the Polkadot scanner, SubQuery, and other key data sources—identified and proposed by the community—for real-time querying and question answering. We believe Pattern can significantly improve user experience while streamlining the work for devs and power users. 

#### Why us?
Pattern has been working at the intersection of AI and blockchain for the past three years. We've contributed to projects like Soniva.ai, Pocket Network, Hummingbot, and RnDAO, among others. Our live MVP currently focuses on EVM chains, and we’re now excited to expand to the Polkadot ecosystem.

#### 1-min Video Pitch
[1-min video pitch](https://drive.google.com/file/d/1aAElKZm-Cc5WkT7hWo5yVXfkFMzqb69u/view?usp=sharing)

### 🔍 Project Details

#### Technology Stack
We use a multi-agent architecture, where query will be broken down into series of tasks and the LLM detects which tools correspond to each task, using the tools data is retrieved and the result is aggregated and transformed into human format. 
![Architecture](https://i.ibb.co/7JSr19Dv/Pattern-Pitch-Frame-2.jpg)

We currently have an alpha version of our MVP live at [mvp.pattern.global](https://mvp.pattern.global), and we're actively working on stabilizing and improving the user experience.

Here are a few example queries: 
- [How much gas did I use so far? (can't believe I spent 0.18ETH 😭)](https://i.ibb.co/n81FGTwH/image-5.png)
- [What was the latest activity of the following wallet? ](https://i.ibb.co/Y7NqRdqv/image-2.png)
- [What is the builder reward in this contract?](https://i.ibb.co/chsJQgsW/image-4.png)
- [How can I transfer USDC?](https://i.ibb.co/0wj9Lpw/image-3.png)

Pattern is currently focused on fetching and interpreting information, and we don't have plans to develop a transaction builder in the near future. However, if there is sufficient demand from the community, we would certainly consider adding this feature in later phases. Hence, we will not increase on-chain activity directly.

### 🧩 Ecosystem Fit

#### Fitting in the ecosystem
Pattern fits right into the Polkadot ecosystem by improving experiences for both users and developers. dApps on Polkadot can use Pattern to offer an intuitive scanning experience, breaking down pools, liquidity, functions, and contracts in a simple way. Developers can use it to check out Polkadot contracts, transactions, and other data. Analysts get deeper insights, while users can ask questions and get the help they need to make more confident decisions.

#### Audience 
- Average Users
    - Use Pattern to easily access information about transactions, contracts, and wallets.
    - Understand events and functions happened in a transaction
- New Users
    - Ask questions to better understand their transactions and the blockchain activity around them.
    - Check contract security, by asking about previous transactions
- Power Users
    - Explain why transaction has reverted to help with contract debugging
    - Track wallet across multiple chains and aggregate the information
    - Understand inter-contract transactions and architecture
    - Ask questions about ABI and extract information using ABI

#### User research Quotes 
- **Power user:**
    - Everyone sends Etherscan links around; it would be great if you could build it into an extension that pops up on Etherscan and explains why the transaction is reverting or what is happening in the contract.
    - A widget would be great, so any dApp (like Uniswap) can integrate it, and users can ask questions about pools or transactions. The widget can even be integrated with Etherscan itself.
    - The client, while necessary, will only service new users, but as a power user, Etherscan can’t be replaced; however, an extension can improve it significantly.
    - Users are not willing to pay for this, but businesses are willing to pay for it so their users can use it.
    - It would be a great tool if it were an extension. Developers usually send me transactions asking why they are reverting; some additional context can facilitate the process.
    - I sometimes struggle to understand the interaction between different contracts, and Etherscan’s UX is not intuitive. It would be great if I could ask questions about a transaction happening between two contracts.
- **Average user:**
    - This can be a great replacement for a scanner in a new chain or network. I would love to see a new approach for scanners other than Etherscan.
- **Power user:**
    - I’m using Etherscan MCP, but if there’s an out-of-the-box solution, I’d much rather use it, as with MCP I need to manually turn it on every time.
- **Power user:**
    - Etherscan’s information is good, but Solscan is even more needed as it is more of a mess.
    - Generally, other L1s that are not EVM could benefit much further from this.

#### Needs
- Better user experience
- Simplified access to blockchain data
- Expand the use of scanners
- Streamline development for other dApps who'd like to integrate LLM to use indexed data
- Developers can levrage as a dev tooling to debug contracts and reverted transactions faster

#### Polkdot Competitor
Not that we know of. The closest project we’re aware of is Polkabot, but it focuses on documents, not real-time extraction of information. A project like this doesn’t exist yet because the LLM capable of handling such tasks is still fairly new. It needs an expanded context window, function calling, and a multi-layer architecture, which is exactly what we've been working on at Pattern for the past 6 months to get the best results.


## 👥 Team

- **Team Name:** Pattern
- **Contact Name:** Seper
- **Contact Email:** sep@pattern.global
- **Website:** https://pattern.global/
- **X:** https://x.com/0xpattern/
- **GitHub:** https://github.com/pattern-tech

### Team members

- **Seper:** [Linkedin](https://www.linkedin.com/in/sepehrin/) | [X](https://x.com/seeepeeer) | [Github](https://github.com/sepehr2github)
- **Mohammad:** [Linkedin](https://www.linkedin.com/in/mkermani144/) | [Github](https://github.com/mkermani144)
- **Yasin:** [Linkedin](https://www.linkedin.com/in/yasin-fakhar/) | [Github](https://github.com/yasinfakhar)

### Team Code Repos

- https://github.com/pattern-tech/pattern-core
- https://github.com/pattern-tech/pattern-app


### Team's experience
#### Team experience
Pattern (previously Microflow) is a decentralized team contributing to many projects across the ecosystem some of which are:
- [Soniva](https://soniva.ai/)
- HummingBot expantion from EVM to eUTxO supporting Ergo and Cardano and integrating Spectrum and Splash DEX (Check our [github](https://github.com/pattern-tech))
- Pocket Network
    - [Developed platform and carried out pokt RetroPGF program](https://www.youtube.com/watch?v=UidBGNrEFhs)
    - [Pocket Metrics Dashboard](https://metrics.pokt.network/community)
    - [Pocket Governance Upgrade](https://forum.pokt.network/t/open-technical-support-and-development-of-governance-upgrade-by-microflow/4843/9) 
- RnDAO
    - [TogetherCrew](https://www.togethercrew.com/) PoC

#### Individual experience
- **Seper:** Prev Senior Engineer at [Aragon](https://aragon.org/)
- **Mohammad:** Prev Senior Engineer at [RosenBridge](https://rosen.tech/) & [Ergo chain](https://ergoplatform.org/en/) core contributor 
- **Yasin:** Prev AI Engineer at [HoopadVision](https://hoopadvision.com/en/index.html)

## 📊 Development Status
We’ve implemented an MVP that currently supports only EVM chains. This is an alpha version, and we are working on improving performance and user experience.

Here are the repositories for:
- [Core](https://github.com/pattern-tech/pattern-core)
- [Client](https://github.com/pattern-tech/pattern-app)

A live alpha version is available [here](https://mvp.pattern.global/).


## 📅 Development Roadmap

### Milestone 1
- **Duration:** 3 weeks | **Budget:** $4,500 USD
- **Description:** Integrate mentioned data sources with Pattern core
- **Deliverables:**
    - Discover Polkdot data sources (such as [Polkdot scanner](https://polkadot.subscan.io/), [SubQuery](https://subquery.network/))
    - Integrate with data sources 
    - Integrate with any additional data source suggested by the community (providing it was feasibile)
    - Extract list of APIs and create tools interfaces 
### Milestone 2
- **Duration:** 3 weeks | **Budget:** $4,500 USD
- **Description:** Write in depth instructions for LLM and optimize tools descriptions
- **Deliverables:**
    - Add all the tools to the registry
    - Optimize performance
    - Optimize tools descriptions to reflect everything that can be done with daata
    - Create a list of 25 tested use cases as example for community 
 ### Milestone 3
- **Duration:** 1 weeks | **Budget:** $1000 USD
- **Description:** User Experience
- **Deliverables:**
    - Create a whitelabel version with Polkdot branding 
    - Host a separate client for Polkdot 
    - Encorporate brand identity 

### Overview

- **Estimated Duration:** 2 months
- **Full-Time Equivalent (FTE):**  1.5 full-time employee
- **Total Costs:** $10,000 USD


| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | MIT |
| 0b. | Documentation | We will provide a list of example queries that can be answered using pattern, plus a small video tutorial for users |
| 0c. | Testing and Testing Guide | Tests will be added on a rolling bases as we encouner issues |
| 0d. | Article | We will publish an **article** that explains what was done/achieved as part of the grant. |
| 1. | Feature: Chat client | we will create a chat client from which users can explore blockchain data |
| 2. | Feature: white label | We will use polkdot branding |
| 3. | Feature: Polkdot data sources | We will integrate Polkdot specific data sources |

### 💰 Budget Breakdown

Team members will work at the rate of $25 USD per hour, each member has a commitment of 20 hours a week to the project. 
- **Milestone 1:** (3 weeks) * (20 hours a week) * (3 members) * ($25 per hour) = $4,500
- **Milestone 2:** (3 weeks) * (20 hours a week) * (3 members) * ($25 per hour) = $4,500
- **Milestone 3:** (1 week) * (20 hours a week) * (2 members) * ($25 per hour) = $1,000

**Total requested budget accumulates to $10,000**

**Total estimated timeline for the project is 7 weeks**

## 🔮 Future Plans

### Future features
- Additional data sources
- An extention that will pop-up when you go inside scanner and helps you explore the data
- A widget that dApps can easily embed Pattern

### Funding
- Planning to seek other grants to integrate dApps and other chains.
- Once adequate integration with the various data sources is achieved and a fully-fledged V1 is completed, we will consider fundraising to create a unified aggregation layer.

### Vision
- We believe the crypto user experience needs to evolve, as the current interface is not intuitive. Pattern is the first step in this direction, serving as an experiment in using generative AI for user experience. We believe Pattern can reduce the barrier to entry and significantly improve user acquisition for Polkadot.



## ℹ️ Additional Information

We are part of the PGAT cohort and have received a $25K grant from Pocket Network to help test the new version of their mainnet and integrate Pattern with it.
https://markets.businessinsider.com/news/currencies/pocket-network-announces-winter-2025-batch-empowering-the-next-generation-of-decentralized-builders-1034336272
