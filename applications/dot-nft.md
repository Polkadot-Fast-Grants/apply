# 📝 dot-nft: Polkadot NFT CLI Tool

## 🌟 Project Overview

**Tagline:** A command-line interface tool for seamless NFT minting on the Polkadot ecosystem.

**Description:** dot-nft is a TypeScript-based CLI tool that enables developers and creators to mint NFTs on Polkadot parachains with ease. The tool provides an interactive command-line experience for uploading images, creating metadata, and minting NFTs, with initial support for Paseo Asset Hub.

**Polkadot Integration:** The project directly integrates with the Polkadot ecosystem by:
- Connecting to Paseo Asset Hub for NFT minting operations
- Using Polkadot.js APIs for blockchain interactions
- Supporting Polkadot wallet integration for transaction signing
- Following Polkadot NFT standards and best practices

**Team Interest:** I'm building this tool to lower the barrier of entry for NFT creation on Polkadot, providing a developer-friendly CLI that can be easily integrated into workflows and automation scripts. The Polkadot ecosystem needs better tooling for NFT operations, and I'm addressing this gap.

### 🔍 Project Details

**Technology Stack:**
- **Runtime:** Bun for development, compiled TypeScript for distribution
- **Language:** TypeScript with strict typing and ES modules
- **CLI Framework:** @clack/prompts for interactive user experience
- **Blockchain:** @polkadot/api for Polkadot ecosystem integration
- **Storage:** Filebase SDK for IPFS metadata and asset storage
- **Wallet:** @polkadot/extension-dapp for Polkadot wallet connectivity

**Core Architecture:**
- Interactive CLI flows with step-by-step prompts
- Modular TypeScript architecture for extensibility
- IPFS-first approach for decentralized metadata storage
- Async/await patterns for all blockchain operations
- Environment-based configuration for different networks

**UI/UX Design:**
- Clean, intuitive command-line interface
- Color-coded output using picocolors
- Progress indicators for long-running operations
- Comprehensive error handling with user-friendly messages

**What the project will NOT provide:**
- Web-based user interface (CLI-only)
- Support for non-Polkadot blockchains
- NFT marketplace functionality
- Advanced image editing capabilities

### 🧩 Ecosystem Fit

**Ecosystem Position:** dot-nft fills a critical gap in the Polkadot tooling ecosystem by providing the first dedicated CLI tool for NFT operations. It positions itself as essential infrastructure for developers and creators working with Polkadot NFTs.

**Target Audience:**
- Developers building NFT applications on Polkadot
- Digital artists and creators wanting to mint NFTs

**Needs Addressed:**
- Simplified NFT minting process on Polkadot parachains
- Standardized workflow for IPFS metadata storage
- Developer-friendly tooling for Polkadot NFT ecosystem

**Similar Projects Analysis:**
Currently, there are no dedicated CLI tools for NFT operations in the Polkadot ecosystem. Most NFT interactions require:
- Custom scripts using Polkadot.js directly
- Web-based interfaces
- Complex setup processes for each project

My project is different because it provides:
- Purpose-built CLI specifically for NFT operations
- Interactive prompts that guide users through the process
- Built-in IPFS integration and metadata handling
- Compilation for broad distribution without runtime dependencies

## 👥 Team

- **Team Name:** dot-nft Labs
- **Contact Name:** Preschian Febryantara
- **Contact Email:** preschian27@gmail.com
- **Website:** https://github.com/preschian

### Team members

Solo developer: Preschian Febryantara

#### LinkedIn Profiles

- [Preschian Febryantara](https://www.linkedin.com/in/preschian-febryantara/)

### Team Code Repos

- https://github.com/preschian/dothub-cli (dot-nft CLI project)

GitHub account:

- https://github.com/preschian

### Team's experience

**5+ Years Web Development Experience:** Extensive background in modern web development with comprehensive full-stack development skills, specializing in TypeScript, Node.js, and blockchain integrations.

**Current Role - Fullstack Developer at Koda.art:** Currently contributing as a fullstack developer at [Koda.art](https://koda.art), a platform within the Polkadot ecosystem. Through this role, I have gained comprehensive experience with:
- Polkadot.js API integration and substrate chain interactions
- Modern frontend frameworks in blockchain applications
- User experience design for Web3 applications
- Production deployment and maintenance of dApps
- Working with Polkadot NFT marketplace on AssetHub

This hands-on experience with production Polkadot applications provides deep insights into developer pain points and ecosystem needs, directly informing the development of essential tooling like dot-nft CLI.

## 📊 Development Status

The project is currently in active development with a functional foundation:

**Completed Work:**
- Complete CLI structure with @clack/prompts integration
- IPFS upload functionality via Filebase SDK
- Full Polkadot API integration for Asset Hub
- NFT collection creation and management
- NFT minting workflow implementation
- TypeScript compilation and build system
- Environment configuration management

**Repository:** https://github.com/preschian/dothub-cli

**Current State:** Phase 1 core functionality is complete with working NFT collection creation and minting capabilities. The CLI can successfully create collections and mint NFTs on Paseo Asset Hub.

**Alpha Version Available:** The project is currently in alpha testing phase. You can try the working CLI by running:
```bash
npx https://pkg.pr.new/preschian/dothub-cli/dot-nft@bff8e4c
```

This demonstrates that the core functionality is not theoretical but actually implemented and testable by the community.

## 📅 Development Roadmap

### Overview

- **Estimated Duration:** 1 month
- **Full-Time Equivalent (FTE):** 0.5
- **Total Costs:** $6,000 USD

### Milestone 1: Core CLI Foundation & Integrations ($3,000)

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | MIT License |
| 0b. | Documentation | I will provide comprehensive inline documentation and user tutorial explaining CLI usage |
| 0c. | Testing and Testing Guide | I will implement unit tests or integration tests for core functionality |
| 0d. | Article | I will publish a technical article explaining the project architecture and benefits for Polkadot NFT ecosystem |
| 1. | CLI Foundation | I will deliver a complete interactive CLI foundation with comprehensive prompts, validation, and user experience |
| 2. | Auto Release CI/CD | I will implement automated release pipeline with version management, testing, and distribution |
| 3. | Configuration Management | I will build robust configuration system for managing different environments and user preferences |
| 4. | Testnet SDK Integration | I will provide complete Polkadot SDK integration for seamless testnet connectivity and operations |
| 5. | Testnet Account Integration | I will implement secure account management and wallet integration for testnet operations |
| 6. | Upload IPFS Integration | I will deliver IPFS upload functionality with progress tracking and error handling |
| 7. | Create Collection and NFT Integration | I will provide complete collection creation and NFT minting workflow with comprehensive metadata support |

### Milestone 2: Mainnet Features ($3,000)

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 1. | Secure Config Management | I will build secure configuration management system with encrypted storage for sensitive data |
| 2. | Improve Faster Operations | I will optimize performance for faster blockchain operations and reduced transaction times |
| 3. | Kusama AssetHub Integration | I will implement complete integration with Kusama AssetHub for mainnet NFT operations |
| 4. | Polkadot AssetHub Integration | I will implement complete integration with Polkadot AssetHub for mainnet NFT operations |
| 5. | Refactor Project Structure | I will restructure the codebase with organized modules, clear separation of concerns, and scalable architecture |

### 💰 Budget Breakdown

| Milestone | Deliverables | Cost (USD) | Estimated Completion |
| --- | --- | --- | --- |
| 1 | Core CLI foundation, CI/CD, configuration, testnet integrations | $3,000 | 2 weeks |
| 2 | Mainnet features, secure config, performance optimization, AssetHub integrations | $3,000 | 2 weeks |
| **Total** | | **$6,000** | **1 month** |

**Budget Justification:**
- Focus on core CLI integrations, CI/CD automation, and mainnet readiness
- Testing, documentation, and AssetHub integrations included in development time
- Comprehensive deliverables spanning testnet foundation to production-ready mainnet features

## 🔮 Future Plans

**Post-Grant Development:**
- **Phase 3:** Support for additional Polkadot parachains (Moonbeam, Unique Network, Smartcontract on PolkaVM)
- **Phase 4:** Integration with NFT marketplaces and trading platforms
- **Phase 5:** Community-driven features based on user feedback

**Growth Vision:**
- Make dot-nft the standard CLI tool for Polkadot NFT operations
- Build a community of developers/creators using the tool
- Contribute to the broader Polkadot tooling ecosystem
- Support the growth of NFT adoption on Polkadot parachains

## ℹ️ Additional Information

**Existing Work:**
- Functional CLI foundation with upload capabilities
- Established development environment and build system
- Initial Polkadot API integration implemented

**Ecosystem Alignment:**
- Aligns with Polkadot's vision of accessible blockchain tooling
- Supports the growth of the Polkadot NFT ecosystem

**Technical Approach:**
- Compilation strategy ensures broad compatibility
- Bun used for development speed while maintaining Node.js compatibility
- Focus on developer experience and ease of use
