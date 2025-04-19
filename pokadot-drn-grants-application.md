# 📝 OpenSky

![alt text](https://github.com/Carl-Gustaf/polkadot-apply/blob/master/WhatsApp%20Image%202025-04-19%20at%2013.58.31.jpeg?raw=true)


## 🌟 Project Overview

**Tagline:** OpenSky is a decentralized computing infrastructure (Distributed Resource Network)

**Brief Description:**  
OpenSky is a decentralized computing infrastructure powered by peer allocated resources (compute, storage and network) that features Polkadot's blockchain technology to provide integrity, proof of work, security and tokenized access to resources. Blockchain is a key enabling technology on multiple levels.

It allows the exchange of OpenSky resources against token value and allows users to build on the top of the rented out unused compute, storage, and networking resources in a secure, self-organized P2P network.

**Polkadot Blockchain**
OpenSky utilizes Polkadot's parachain architecture to create specialized chains for resource management, verification, and marketplace operations. We leverage Substrate's flexibility to implement custom resource allocation logic, while benefiting from Polkadot's shared security model, cross-chain messaging capabilities and decentralization.

**Why We're Creating This**  
We want to create a completely distributed infrastructure paradigm that could fundamentally change how we think about the future of computing.

OpenSky is not just another application or network.
OpenSky is a completely integrated, fully self-sufficient infrastructure - on the top of which everything can run.

**Problem**

Currently blockchain technology has very limited real-world use cases; it's trapped in its own world - outside of the cryptospace, blockchain technology often has little value.
OpenSky utilizes Polkadot blockchain technology to enable a new level of computing paradigm. It is not a project, it's a revolution - it's the web3, redefined.
OpenSky will finally allow ANY application to be secured by blockchain technology.


### 🔍 Project Details

OpenSky's mission is to provide efficient thin clients that dynamically allocate hardware resources from almost any device. Clients work as nodes in a network where contributors get paid in tokens for performing operations.

**Technology Stack:**
Network nodes (Clients) that make up OpenSky are built with the following technologies:
- Blockchain: Encryption, Emulation and Integrity. Polkadot's blockchain becomes a key enabling technology.
- libp2p: for Peer-to-peer networking that efficiently allocates resources and distributes work.
- Rust: Core language for managing allocated resources
- Docker: Docker as a secure containerized environment

**Core Architecture Components:**

1. **Resource Management Parachain:**
   - Manages the registration and verification of compute, storage, and networking resources
   - Implements reputation scoring for resource providers
   - Handles resource discovery and allocation

2. **Client Software:**

<img width="454" alt="Screenshot 2025-04-19 at 20 21 18" src="https://github.com/user-attachments/assets/23e42b89-1731-4464-aacf-1f5b7a1ad184" />

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
  
### Compute Abstraction Levels for Distributed Execution

Abstraction Level Tradeoffs
A visualization of the different abstraction levels and their implications:
**1. Instruction-Level (Lowest)**

Approach: Distribute individual CPU instructions
Pros: Maximum flexibility, can run anything
Cons: Extremely high orchestration overhead, practically impossible at scale
Example: Emulating a CPU across multiple machines

**2. Virtual Machine Level**

Approach: Distribute bytecode instructions to VMs
Pros: Language-agnostic, reasonable isolation
Cons: High coordination overhead, complex state management
Example: Distributing JVM bytecode or WebAssembly modules

**3. Container Level (Practical Sweet Spot)**

Approach: Distribute containerized workloads with clear inputs/outputs
Pros: Good isolation, established tooling, manageable orchestration
Cons: Some overhead, requires input/output coordination
Example: Docker containers with defined interfaces

**4. Function Level**

Approach: Distribute pure functions with clear inputs/outputs
Pros: Simple orchestration, easy parallelization, minimal state complexity
Cons: Limited to certain types of workloads, not suitable for all applications
Example: AWS Lambda-style functions

**5. Service Level (Highest)**

Approach: Distribute entire microservices
Pros: Simplest orchestration, familiar programming model
Cons: Large resource requirements per unit, less granular resource allocation
Example: Running entire web services

**Coherent Theory: Functional Resource Unit (FRU)**
We propose implementing a hybrid approach based on containerized functional workloads as the atomic unit:

Atomic Compute Unit: A container with well-defined inputs and outputs
Resource Boundaries: Clear CPU, memory, storage, and time limits
State Management: Explicit state input/output through attached storage volumes
Deterministic Execution: Same inputs always produce same outputs for verification

This way we can strike a balance between flexibility and orchestration complexity.


**Hybrid Multi-Level Approach**
The hybrid approach using multiple abstraction levels is potentially the most powerful solution.

**Implementation Strategy**
<img width="529" alt="Screenshot 2025-04-19 at 20 19 15" src="https://github.com/user-attachments/assets/2a2c9c47-2b57-4e30-a7c9-f1f6c05c6eea" />

**Examples of Level-Optimized Tasks:**

Matrix multiplication: VM level (high compute density, minimal I/O)
Image processing: Container level with GPU access
Database queries: Service level with optimized storage
API endpoints: Function level for maximum parallelization

**Prior Work/Research:**
- Proof-of-concept for Docker-based compute isolation with verification
- Initial implementation of the web gateway interface
- Architectural design for P2P resource discovery using DHT

**What OpenSky Will Not Provide:**
- We are not building a general-purpose blockchain, but rather leveraging Polkadot's existing blockchain technology
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
- **Contact Name:** Gustaf
- **Contact Email:** [g.ydstrom@hotmail.com](g.ydstrom@hotmail.com)
- **Contact Email2:** [krzysztof.strzelec27x@gmail.com](krzysztof.strzelec27x@gmail.com)
- **Website:** [OpenSky repo](https://github.com/Carl-Gustaf/opensky)
- 

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

- [Krzysztof] has extensive experience in web development, with a focus on building scalable applications and implementing secure user interfaces.
- [Gustaf] has a strong background in cloud infrastructure, distributed systems architecture, and blockchain integration.

We are also collaborating with additional technical advisors who will support the project implementation, accounting for the 3 FTE mentioned in our development roadmap.

## 📊 Development Status

We currently have:
- Extensive architectural design documents for the OpenSky
- Complete ecosystem thinking
- Example prototype
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
| 0b. | Extendedn documentation | We will provide both inline documentation of the code and a comprehensive technical whitepaper explaining the architecture and protocols of OpenSky, along with setup guides for both contributors and consumers. |
| 0c. | Foundational Architecture | We will publish founding thoughs and achitectural principles.|
| 1. | Versatile Client | Develop a basic client p2p client that allocates resources and computes jobs. The client will allow users to contribute resources to the network, with Docker-based isolation for compute tasks and encrypted storage functionality. |
| 2. | OpenSky Interface | Create the initial interface for job submission, resource management, and token summary. |
| 3. | Basic Orchestration Logic | Implement the core resource matching algorithm that pairs consumer requests with appropriate provider resources based on requirements and availability. |
| 4. | Tokenomics Design | Design the token system that incentivizes resource contribution and handles payment for resource consumption. |

### 💰 Budget Breakdown

| Milestone | Deliverables | Cost (USD) | Estimated Completion |
| --- | --- | --- | --- |
| 1 | Extendedn documentation + Client Software Alpha | $5,000 | 1.5 months |
| 2 | OpenSky Interface MVP + Orchestration Logic + Tokenomics | $5,000 | 1.5 months |
| **Total** | | **$10,000** | **3 months** |

NOTE: The purpose of tokens is to mediate as a storeholder of value that can be exchanged against proof of work done by the network and shared/used resources. The goal is to provide a token with a predictable and stable value, exchangeable for currencies, but should not be a subject of speculation. For example: we could use dollar-pegged tokens like USDC, with support for other stablecoins or cryptocurrencies.

## 🔮 Future Plans

**Short-term Development:**
- Lightweight P2P client that dynamically and efficiently allocates and coordinates tasks/resources
- Expand the types of workloads supported by the network
- Implement advanced resource verification mechanisms
- Develop specialized job templates for common use cases
- Create resource monitoring systems

**Long-term Vision:**
- Build OpenSky into a complete paradigm shift for web3.
- Enable distributed computing resources like computing, storage, and networking as atomic units that can be rearranged for any task.
- Atomic units for Compute, Networking and Storage: Potential use case: Users can share storage, share computing resources, and another user can build something on top of it.
- Orchestration layer: The "floating, self-organized resources" need a layer that allows available resources to complete "tasks". The big vision is that this is done in a secure, extremely redundant and resilient way.
- Encryption, Emulation, Integrity: Are key aspects in order to create a distributed resource network that is secure and redundant. For this, blockchain becomes a key enabling technology.
- Marketplace: The self-organizing network needs to reward nodes for participating and needs to adjust cost/earnings dynamically for what is needed for the network.

**Examples of long-term OpenSky's impact:**
- Cloud services (like AWS for example) will become gateways to the OpenSky, similar to how search engines (like Google) are gateways to the Internet.
- Cloud services and data centers will become large contributors to the shared resources upon which OpenSky is based.
- Applications will be efficiently distributed and "floating", secured by Polkadot's Blockchain.
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
