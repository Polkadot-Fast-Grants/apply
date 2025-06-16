# 📝 Quid

## 🌟 Project Overview

Please provide the following:

- one sentence summary
  - **lvlUSD meets Bunni**
- A brief description of your project
  - **We've integrated a stablecoin basket with AAVE and Morpho to amplify yield for LPs on Uniswap V4.**
- An indication of how your project relates to / integrates into Polkadot
  - **Currently there's only Wormhole-wrapped DOT on Ethereum; this token doesn't embed any staking yield for DOT. This is a problem we need to solve in order to provide Uniswap LPs a diversified offering.** 
- An indication of why your team is interested in creating this project
  - **We currently allow Uniswap LPs to trade ETH in an optimal way against a basket of dollars. It would be awesome to give them exposure to DOT as well.**

### 🔍 Project Details

- An overview of the technology stack to be used
  - **We plan to create a basket of the top 3 staked DOT tokens, and use Wormhole to bring it to a highly customised venue on Ethereum.**
- Documentation of core components, protocols, architecture, etc. to be deployed
  - **There are 3 core contracts. The Token uses an extension to the ERC6909 standard for supporting bonds; the Router (that's on top of UniV4 with protection from sandwich attacks) has it's own "side-car" auxiliary contract. There are several mechanisms (e.g. for managing price ranges, as well as 2 kinds of withdrawals and deposits).**
- Any PoC/MVP or other relevant prior work or research on the topic
  - **github.com/QuidLabs/IMO**
- Mockups/designs of any UI components
  - **[This video demonstrates](https://vimeo.com/1043834325) the old frontend that we'll be adapting to be compatible with the latest backend as part of Milestone 2.**
- Data models / API specifications of the core functionality
  - **You can find the core data structures [in this file](https://github.com/QuidLabs/IMO/blob/main/src/imports/Types.sol)**
- What your project is *not* or will *not* provide or implement
  - **We will bring DOT (the asset) in its yield-optimal form to a new audience of non-custodial crypto users. We will not be building a parachain or an ink! contract.**

### 🧩 Ecosystem Fit

- Where and how does your project fit into the ecosystem?
  - **It fits into the Polkadot ecosystem from the outside.**
- Who is your target audience?
  - **People with prior experience using AMMs; wealth managers, family offices, DeFi hobbyists, etc.**
- What need(s) does your project meet?
  - **ETH staking yield isn't very high, but with our strategy you can earn upwards of 15% on it without much risk. We want to broaden what this strategy can do, and deliver a more cohesive experience.**
- Are there any other projects similar to yours in the Polkadot ecosystem?
  - If so, how is your project different?
    - **We believe that the power of blockchains is in their cross-polination of value. The more audiences a token can reach, the better...but it has to reach them in the right way.**
  - If not, why might such a project not exist yet?
    - **The UniV4 ecosystem is still early, and the cognitive bias of chain maximalism is still slowing many people down.**

## 👥 Team

- **Team Name:** Name of your team. If you apply as a legal entity, please use its name.
  - Quid Labs
    - PO Box 144; 3119 9 Forum Lane  
      Camana Bay, George Town  
      Grand Cayman KY1-9006
- **Contact Name:** Johnny Quid
- **Contact Email:** john@quid.io
- **Website:** x.com/QuidMint

### Team members

Please list the legal name of all grant beneficiaries. **Solo developers (1-person teams)** are eligible for funding.

#### LinkedIn Profiles (if available)

- **[Richard Tiutiun](http://linkedin.com/in/rtiutiun)**

### Team Code Repos

- **https://github.com/QuidLabs/IMO**

Please also provide the GitHub accounts of all team members:

- **https://github.com/johnquid**
- **https://github.com/tobaccorico**

### Team's experience

**We are brothers; were both involved in the world's first CBDC 15 years ago. Johnny is a pseudonym for big brother (marketing guy); as part of reinstatemet, his little brother is currently enrolled in the Berkeley Advanced LLM course, after having dropped out of the Letters and Science Bachelor of Arts CS program 10 years ago. The AI capstone will be around voice.**

## 📊 Development Status

**We already started implementing this project; it's been through two previous (riskier) phases of iteration on Uniswap, both V3-based; the latest version is more risk-averse, simpler, and uses V4.**

## 📅 Development Roadmap

### Overview

- **Estimated Duration:** 3 months
- **Full-Time Equivalent (FTE):**  2
- **Total Costs:** $10,000 USD

> Note that deliverables 0a to 0d are mandatory. Please adapt their specification to your project.

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | MIT  |
| 0b. | Documentation | We provide a lot of **inline documentation**  |
| 0c. | Testing and Testing Guide | The core functionality **is already covered** by `forge test`. |
| 0d. | README | We will extend the repo README to explain what was done/achieved as part of Milestone 2 of this grant. |
| 1. | Bonds | This feature (**already done**) provides an implicit incentive for dollars to be staked into our protocol, which solves the chicken and egg problem of needing to have both dollars and ETH in order to deposit into UniV4. |
| 2. | Sandwich protection | This feature (**already done**) allows swapping without the risk of hitting a sandwich attack. It uses a batch clearing system, [discussed here](https://github.com/0xfuturistic/sandwich-mitigating-uniswap-v2/issues/1#issuecomment-2800039974), whereby buys clear all in a row, followed by sells. |
| 3. | *NEEDS WORK* | This feature will allow LP deposits of the Wormhole-transported staked DOT token in the same way that ETH is currently staked into our protocol. This is done through a queue system which allows circumventing impermanent loss. |


### 💰 Budget Breakdown

Please provide a breakdown of your budget by milestone:

| Milestone | Deliverables | Cost (USD) | Estimated Completion |
| --- | --- | --- | --- |
| 1 | Proof of concept | $5,000 | Done (retro-active) |
| 2 | Staked DOT basket | $5,000 | 3 months |
| **Total** | | **$10,000** | **3 months** |

## 🔮 Future Plans

Please include:

- How you intend to continue development after the Fast-Grant
  - **Eventually, we would like to see more types of stablecoins entering the Polkadot ecosystem. This would create an impetus for us to transfer our mechanism design from UniswapV4 to concentrated liquidity projects in the parachain space.**
- Any plans for seeking additional funding (other grants, VC funding, etc.)
  - **We plan to demo our progress in the soonami Venturethon that is starting soon.**
- Your vision for the project's growth and impact in the Polkadot ecosystem
  - **As more systematic investment funds spring up in this season of DeFi, diversification will be an important theme. More investors from other ecocsystems gaining exposure to DOT will be conducive to their experimentation with other Polkadot infrastructure and application-layer products.** 

## ℹ️ Additional Information

- Work you have already done
  - **github.com/QuidLabs**
- If there are any other teams who have already contributed to the project
  - **ManifoldFinance.com** 
- Other funding you may have applied for
  - **We've received approval from Polygon Labs on our proposal; submitted a proposal and waiting on approval from Arbitrum.**

