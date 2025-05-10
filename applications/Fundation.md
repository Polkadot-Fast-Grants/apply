# 📝 Fundation DApp Management System

## 🌟 Project Overview

- Purpose: Simplify and accelerate DApp deployment in the Polkadot ecosystem.

- Vision: Fundation is a modular DApp Management System (DMS) designed for the multichain future, drawing inspiration from how WordPress, Drupal, and Joomla empowered developers to easily set up and manage projects in Web2. Upon completion, it has the potential to drive significant growth in the Polkadot ecosystem, much like these CMS platforms transformed traditional web development.

- Origin: The idea emerged after I struggled to build my first DApp on Polkadot and noticed a lack of accessible tooling—not just for Polkadot but across Web3. Many existing tools are Ethereum-centric and locked into closed-source SaaS models, limiting flexibility and accessibility.





### 🔍 Project Details
# Technical Stack:
- Front-End: Next.js, Tailswind CSS, and Shadcn/ui for rapid development and modern UI design.


- Blockchain Interaction: Polkadot-API for seamless integration with Polkadot parachains and relay chains.

- Data Storage: Turso DB, a serverless centralized database, for authentication and non-finality data storage. Note: Full decentralization is not the current goal, as the technology isn’t mature enough yet. This is a pragmatic choice, with plans to explore decentralized alternatives in the future as the tech evolves.


### Authentication:
-Wallet-based signup/login via Polkadot wallets.
-Social login (Google OAuth).
-Email/password authentication.
-Passkey support (e.g., WebAuthn) for passwordless login.
-Session management with JWT for secure, persistent logins.

### Asset Management:
- Dynamic asset retrieval: Users select parachains and tokens; Fundation fetches balances and metadata.
- Pre-configured asset groups for popular tokens (e.g., DOT, KSM).
- Support for custom token additions via simple configuration.
### Settings Page:
- UI to add/remove connected wallets.
-Toggle authentication methods (e.g., disable passkeys or social logins).
- Profile management: Update username and basic user info.

### Blockchain Interaction:
- Seamless connection to any Polkadot relay chain or parachain via a dropdown menu.
- Automatic handling of chain metadata and API endpoints.

### Current Status:
- A basic MVP is live at fundation.dev, though it remains under active development. This grant will fund the completion of core features.

# Core Features of the Base Module:
- Easy Setup: Streamlined access to Polkadot’s system parachains.

- Flexible Authentication: Users can sign up with a wallet and log in via alternative methods (social login, email, passkeys). This enables read-only asset access without constant private key exposure, enhancing security and usability (e.g., checking assets without a wallet nearby).

- Asset Management: Developers can define standard asset groups to load and display based on selected chains, simplifying asset handling.

- Settings Page: Users can update usernames, add/remove wallets, and manage authentication methods (e.g., disable passkeys or specific wallet addresses).

### Deliverables:
-This grant will fund the base module (authentication, asset page, settings page, and dynamic blockchain interaction), along with detailed documentation on data models and API specifications. A DeFi module is excluded from this proposal, as it’s estimated to take over three months.


### 🧩 Ecosystem Fit

#### Role in Polkadot: Fundation supports DApp developers by providing an open-source, modular foundation tailored to Polkadot’s multichain architecture.

- Target Audience: Junior and front-end developers looking to build DApps quickly.
Example 1: A Web2 front-end developer transitioning to Web3, seeking a tool to handle DApp basics.

- Example 2: A Web3 developer wanting to focus on unique features rather than repetitive groundwork.

- Example 3: A parachain team aiming to save development time by starting with Fundation’s base module.

### Needs Addressed:
- Simplifies the development process for rapid idea deployment, reducing barriers to entry.

### Competitors:
- Apillon: A Polkadot-focused Web3 platform offering UI and API integration for parachain services.

- Thirdweb: An Ethereum/EVM-focused platform with SDKs and smart contract tools, targeting games and creator platforms.

- Magic: An Ethereum-based authentication tool using passwordless logins, not a full DApp solution.

### Differentiation:
- Fundation is open-source and self-hostable, prioritizing ease of use and flexibility. Unlike Apillon or Thirdweb, it doesn’t rely on third-party services—ensuring developers retain control and can adapt it freely without waiting for external updates.



## 👥 Team
- Team Name: Fundation

- Contact: Victor Stallone Peck (Swen) | Email: swenpeck@outlook.com

- Website: funation.dev

- Team Members: Solo developer—Victor Stallone Peck

- Code Repos: github.com/swenthebuilder

### Experience:
- I’m primarily a front-end developer with two years of backend exploration, focusing on authentication and UX. My Web3 journey began with Polkadot, inspiring this project.

"As a solo developer, I’ve planned for potential delays by building in a one-week buffer per milestone. If needed, I’ll engage part-time contributors from Polkadot’s community (e.g., via the Polkadot Discord) to assist with tasks like testing or documentation."



## 📊 Development Status
I’ve been working on this project intermittently, but I’m ready to commit more time. Currently, fundation.dev features a basic landing page and a rudimentary MVP concept.


## 📅 Development Roadmap
### Milestone 1: Base Functionality
- Duration: 1 month
- Cost: $5,000
### Deliverables:
 - Authentication: Complete wallet-based signup/login, plus social login, email, and passkey options.
- Dynamic Blockchain Asset Retrieval: Simplified asset fetching—developers select chains/tokens, and Fundation handles the rest.
- UX Refinement: Streamlined chain connections/disconnections and overall design polish.

### Milestone 2: Optimization & Release
- Duration: 1 month
- Cost: $3,000
### Deliverables:
- Code Optimization: Readable code with inline comments explaining functionality.
- Documentation: Overview, in-depth technical details, and a getting-started tutorial.
- Open-Source Release: Code published on GitHub under the MIT License.



### Overview

- Total Duration: 2 months
- FTE: 1 (solo developer)
- Total Cost: $8,000 USD



| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | MIT License for all code and artifacts.|
| 0b. | Documentation | Inline code comments and a tutorial on base components.|
| 0c. | Testing and Testing Guide |Unit tests for core functions; UX testing for simplicity/intuitiveness.|
| 1. | Authentication |Wallet-based auth (existing) plus passkeys, email, and social login. |
| 2. | Blockchain Interaction|Dynamic asset retrieval for any Polkadot relay chain or parachain. |

### 💰 Budget Breakdown

Please provide a breakdown of your budget by milestone:

| Milestone | Deliverables | Cost (USD) | Estimated Completion |
| --- | --- | --- | --- |
| 1 | Authentication (wallet, social, email, passkeys) | $2,000 | 3 weeks |
| 1 | Asset retrieval & management | $1,500| 1 weeks |
| 1 | UX design & refinement | $1,000 | 1 weeks |
 2 |Code optimization & comments | $1,000 |1 week |
  2 |Documentation & tutorials| $1,5000 |1 week  |
  | 2 |Testing (unit & UX)| $1,000 | 1 week |
| **Total** |Fully functional base module DApp | **$8,000** | **2 months** |

## 🔮 Future Plans

### Next Steps:
- Post-grant, I’ll develop a DeFi module (4–6 months), followed by community features and staking.

- Funding: Considering an OpenGov proposal after completing initial modules.

- Vision: Replicate WordPress’s 43.5% web dominance in Polkadot’s DApp ecosystem, transforming how developers build in Web3.

"To ensure long-term growth, I’ll release Fundation under the MIT License and promote it via Polkadot’s developer forums, hackathons, and social media. I’ll also explore partnerships with parachain teams for custom module development."
