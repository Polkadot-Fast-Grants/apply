# 📝 OpenSky

This is how web3 will be understood, in the future.
![alt text](https://github.com/Carl-Gustaf/polkadot-apply/blob/master/WhatsApp%20Image%202025-04-19%20at%2013.58.31.jpeg?raw=true)


## 🌟 Project Overview

**Tagline:** Infrastructure - a decentralized "floating datacenter" (Distributed Resource Network) powered by user-contributed resources and Polkadot's secure infrastructure.

**Brief Description:**  
OpenSky creates a decentralized cloud infrastructure by allowing users to build on the top of the rented out unused compute, storage, and networking resources in a secure, self-organized P2P network. This "floating datacenter" provides cloud services without fixed physical infrastructure, instead leveraging distributed resources coordinated through Polkadot's blockchain technology.

**Integration with Polkadot:**  
OpenSky utilizes Polkadot's parachain architecture to create specialized chains for resource management, verification, and marketplace operations. We leverage Substrate's flexibility to implement custom resource allocation logic, while benefiting from Polkadot's shared security model and cross-chain messaging capabilities and decentralization.

**Why We're Creating This:**  
We believe the future of cloud computing shouldn't be controlled by a handful of centralized providers. By creating a truly distributed infrastructure layer secured by Polkadot's technology, we can democratize access to computing resources, create new income streams for resource providers, and build resilient systems that aren't subject to centralized points of failure.

Its not just another application, network.
Its infrastructure - on the top of which everything can run.

Moreover, currently blockchain has very limited real-world use cases, its trapped in its own world - as soon as we leave the cryptospace, it often has no value. 
OpenSky is not a project, its a revolution - its the web3, redefined.
OpenSky will finally allow ANY application to be secured by blockchain technology.






### 🔍 Project Details

**Technology Stack:**
- **Blockchain Layer:** Substrate framework for custom parachain development
- **Smart Contracts:** ink! for resource verification and payment logic
- **Client Software:** Rust-based desktop application for resource contribution
- **Web Gateway:** React frontend with Polkadot.js integration
- **Orchestration Layer:** Custom-built scheduler with libp2p integration
- **Containerization:** Docker for secure compute isolation
- **Cryptography:** zk-SNARKs for private computation verification

**Core Architecture Components:**

1. **Resource Management Parachain:**
   - Manages the registration and verification of compute, storage, and networking resources
   - Implements reputation scoring for resource providers
   - Handles resource discovery and allocation

2. **Client Software:**
   - Runs as a background process on contributor machines
   - Manages resource allocation and isolation
   - Secures user system from malicious workloads
   - Communicates with the blockchain for task allocation and rewards

3. **Web Gateway:**
   - Provides user interface for both resource providers and consumers
   - Facilitates job submission and management
   - Displays resource contribution metrics and earnings
   - Serves as the first self-hosted service on the network itself

4. **Orchestration Protocol:**
   - Matches resource requirements with available providers
   - Implements task sharding for distributed computation
   - Ensures data redundancy and availability
   - Provides verifiable proofs of task completion

**Prior Work/Research:**
- Proof-of-concept for Docker-based compute isolation with verification
- Initial implementation of the web gateway interface
- Architectural design for P2P resource discovery using DHT

**UI Mockups:**
- Consumer dashboard for job submission and monitoring
- Contributor interface for resource allocation and earnings tracking
- Marketplace view for resource pricing dynamics

**What OpenSky Will Not Provide:**
- We are not building a general-purpose blockchain, but rather leveraging Polkadot's existing infrastructure
- We will not guarantee performance equivalent to centralized cloud providers in the initial implementation
- We are not focusing on supporting legacy applications that require high I/O performance or low latency
- We do not guarantee data sovereignty (data may be stored across global nodes with encryption)

### 🧩 Ecosystem Fit

**Where OpenSky Fits in the Ecosystem:**
OpenSky serves as critical infrastructure for the Polkadot ecosystem, providing decentralized computation resources that other parachains and applications can utilize. It extends Polkadot's capabilities beyond financial transactions into the realm of distributed computing infrastructure.

**Target Audience:**
1. Individual resource providers looking to monetize spare computing capacity
2. Developers seeking censorship-resistant and decentralized computing resources
3. DApps requiring computation beyond what's feasible on-chain
4. Organizations needing resilient infrastructure not tied to a single cloud provider

**Needs Addressed:**
1. Democratizes cloud infrastructure by creating a marketplace for individuals to participate
2. Provides truly decentralized compute resources for Web3 applications
3. Creates economic incentives for resource sharing through tokenization
4. Builds resilient infrastructure free from centralized control

**Similar Projects in Polkadot Ecosystem:**
While several projects address decentralized storage (like Crust Network) or specific compute needs, none have created a comprehensive OpenSky that combines all three resource types (compute, storage, and networking) with an integrated orchestration layer. Our comprehensive approach to resource commoditization and unified marketplace creates a unique offering within the ecosystem.

## 👥 Team

- **Team Name:** OpenSky
- **Contact Name:** [Team Member 1]
- **Contact Email:** [contact@drnlabs.xyz]
- **Website:** [https://github.com/drnlabs]

### Team members

- Carl Gustaf Ydström
- Krzysztof Strzelec

#### LinkedIn Profiles

- [Gustaf](https://www.linkedin.com/in/carl-gustaf/)
- [Krzysztof](https://www.linkedin.com/in/krzysztof-strzelec-a90939292/)

### Team Code Repos

- [Gustaf](https://github.com/Carl-Gustaf)
- [Krzysztof](https://github.com/kris27x)
  
### Team's experience

Our team combines expertise in web development, distributed systems, and cloud infrastructure:

- [Krzysztof] has experience in web development.
- [Gustaf] has background in cloud infrastructure.

## 📊 Development Status

We currently have:
- Architectural design documents for the OpenSky
- Example portotype
- Initial designs for the Web Gateway interface
- Research on integration points with Polkadot's parachain technology

## 📅 Development Roadmap

### Overview

- **Estimated Duration:** 3 months
- **Full-Time Equivalent (FTE):** 3
- **Total Costs:** $10,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | MIT |
| 0b. | Documentation | We will provide both inline documentation of the code and a comprehensive technical whitepaper explaining the architecture and protocols of OpenSky, along with setup guides for both contributors and consumers. |
| 0c. | Article | We will publish an article explaining the vision behind OpenSky, its integration with Polkadot, and the potential impact on decentralized cloud infrastructure. |
| 1. | Substrate Module: Resource Registry | Implement a custom pallet that enables registration of compute, storage, and network resources with verification mechanisms for resource availability and performance metrics. |
| 2. | Client Software Alpha | Develop a basic client allowing users to contribute resources to the network, with Docker-based isolation for compute tasks and encrypted storage functionality. |
| 3. | Web Gateway MVP | Create the initial web interface for job submission, resource management, and basic analytics for both providers and consumers. |
| 4. | Basic Orchestration Logic | Implement the core resource matching algorithm that pairs consumer requests with appropriate provider resources based on requirements and availability. |
| 5. | Tokenomics Design | Design and implement the token system that incentivizes resource contribution and handles payment for resource consumption. |

### 💰 Budget Breakdown

| Milestone | Deliverables | Cost (USD) | Estimated Completion |
| --- | --- | --- | --- |
| 1 | Resource Registry + Client Software Alpha | $5,000 | 1.5 months |
| 2 | Web Gateway MVP + Orchestration Logic + Tokenomics | $5,000 | 1.5 months |
| **Total** | | **$10,000** | **3 months** |

NOTE: The purpose of tokenomics (tokens) is to allow exchange of work (shared resources) for value. 
## 🔮 Future Plans

**Short-term Development:**
- Expand the types of workloads supported by the network
- Implement advanced resource verification mechanisms
- Develop specialized job templates for common use cases
- Create resource monitoring

**Long-term Vision:**
- Build OpenSky into a complete wholesome idea and web3 paradigm shift.
- Enable distributed computing resources like computing, storage, and networking as atomic units that can be rearanged for any task.
- Atomic units: for Compute, Networking and Storgage: Potential use case: Users can share the storage, share the computing and another user can build something on-top of it.
- Orchestraction layer: The "floating, self organised resources" needs a layer that allows available resources to complete "tasks". The big vision is that this is done in a secure and extremely redundant and resilient way.
- Encryption, Emulation, Integrity: Are key aspects in order create a distributed resource network that is secure and redundant. For this blockchain becomes a key enabling technology.
- Marketplace: The self-organising network needs to reward nodes for participating and needs to adjust cost/earnings dynamically for what is needed for the network.

**Examples of long-term OpenSky's impact:**
- Cloud services like (AWS for example) will become a gateways to the OpenSky, like search engies (for example Google's browser) is a gateway to the Internet.
- Cloud services and data centres will become large contributors to the shared resources upon which OpenSky is based.
- Applications will be efficiently distributed, and "floating", secured by Polkadot's Blockchain.
- Our hardware and software will become less relevant (PCs, smartphones), as applications will run on the OpenSky, utilizing shared resources.
- Creation of specific hardware optimized for resource sharing.
- Blockchain technology powered by Polkadot becomes a global security layer.

**Additional Funding Strategy:**
- Apply for larger grants from the Polkadot Treasury
- Seek venture funding from Web3-focused investors
- Explore potential partnerships with hardware manufacturers

## ℹ️ Additional Information

Our project builds upon concepts proven in distributed computing projects like BOINC, storage networks like Filecoin, and containerization technologies like Docker. What makes OpenSky unique is the comprehensive integration of all these elements into a cohesive system backed by Polkadot's security and interoperability features.

The OpenSky concept represents a paradigm shift in how infrastructure can be provisioned and utilized in a Web3 context. By creating this system on Polkadot, we not only leverage its technical capabilities but also position ourselves to serve the growing ecosystem of parachains and applications that require off-chain compute resources.
