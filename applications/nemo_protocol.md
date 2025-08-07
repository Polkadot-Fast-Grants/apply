## **Name**

Nemo: Cross-chain AI Persona Protocol

## **Tagline**

Your on-chain trading behavior. Your AI twin. Powered by personality — shaped by MBTI, styled by your trades.

## **Project Overview**

Nemo is a protocol that transforms multichain wallet behavior into a personality-powered AI chatbot. By analyzing users' activity across Polkadot parachains — including DeFi transactions, NFT interactions, governance participation, and on-chain asset management — Nemo mints a unique AI persona, anchored in a soulbound NFT on AssetHub. These AI agents serve as chain-native personal assistants that reflect the wallet’s behavioral patterns and continuously evolve over time.

## **What We Mean by 'Trading Behavior'**

We define "trading behavior" as patterns extracted from a wallet's **on-chain DeFi interactions**, including:

* Token swaps via DEXs (e.g., HydraDX, Moonbeam-based platforms)
* Participation in liquidity pools and yield farms
* NFT buys/sells and collection affinities
* Staking preferences (duration, network, volatility profile)
* Transaction frequency, size, and portfolio volatility

This **does not** rely on centralized exchange data (like Binance, Bybit, or Gate), as these are not publicly accessible. Instead, Nemo profiles a user based on decentralized and transparent data, gathered via indexers and APIs (e.g., Subquery, Subsquid)...

Nemo focuses on **investor and behavioral profiling** rather than pure speculation. We classify users along dimensions such as:

* Risk appetite (based on token types, volatility, and diversification)
* Asset preference (blue-chip vs. mid-cap vs. memecoin)
* Chain exposure (Polkadot-native vs. cross-chain explorers)
* Holding vs. flipping tendencies

This data is used to generate AI responses contextual to the user’s unique wallet identity, creating a more personalized assistant.

## **Evolving NFT Persona**

The NFT minted for each user is a **soulbound MBTI-style persona**, stored on **AssetHub**. Due to AssetHub’s current limitations (no native smart contract logic), the evolution logic is offloaded to an external dApp smart contract which:

* **Tracks and aggregates new user behavior across supported chains**
* **Recalculates MBTI tags and traits** based on recent activity
* **Pushes updated metadata** to the user’s NFT record (via external metadata pointer)
* **Triggers visual layer changes** such as mood colors, accessory traits, or AI assistant voice themes

Only metadata (not token ownership) is updated. The visual avatar and AI agent both evolve — the image updates periodically (e.g., after every 10 meaningful behavioral shifts), and the AI adjusts its tone and response style accordingly.

## **Privacy and Anonymity**

We take user privacy seriously. While Nemo constructs AI personas based on on-chain behavior, the system is intentionally designed **not to store or expose wallet addresses within the soulbound NFT metadata**. The NFT only reflects aggregated behavioral patterns — such as preferred asset types, activity levels, or risk profiles — **without referencing or linking any identifiable address**.

All profiling is processed on the client side or through secure middleware, and the final persona can be minted in a privacy-preserving manner. Third-party observers browsing persona NFTs cannot determine the underlying wallet address. In future versions, we also plan to add a “Private Mode” that allows users to mint or interact with their persona without revealing any transaction signatures or public activity.

## **Success of a Persona?**

Each persona is rated on:

* **Accuracy**: How well it reflects actual user behavior
* **Engagement**: Number of chats initiated, insights surfaced
* **Influence**: If other users follow or fork that persona (i.e., copy wallet style)

We plan to develop a **marketplace of personas**, where users can:

* Browse top-performing personas (by ROI, risk profile, engagement)
* Filter by asset type, chain activity, behavioral type
* Chat with the AI agent to understand its investment personality
* Clone/follow personas (copy notification alerts, not trades)

## **Technical Architecture**

To balance privacy and evolution, Nemo follows this data design:

* **Data Source**: Use Subquery/Subsquid to gather on-chain activity (e.g. DEX swaps, NFT mints, staking events) for connected wallets.
* **Local Analysis**: User's browser or middleware backend extracts behavioral tags like preferred sectors, top tokens, frequency, etc.
* **Data Storage**: These behavior summaries are stored on IPFS as a JSON file (e.g. `persona_v3.json`) and linked by CID.
* **NFT Metadata**: The AssetHub-hosted NFT stores only the CID (not wallet address) and high-level traits (e.g. MBTI type).
* **Privacy Measures**:

  * No wallet address stored in NFT metadata
  * No public transaction history revealed
  * Option for private mode in future

This ensures that wallet identity is separated from persona visibility. All behavior data is used strictly for trait generation and never published as-is.

## **Development Roadmap**

**Estimated Duration**: 3 months
**FTE**: 2 full-time members
**Total Cost**: \$10,000 USD

### Deliverables 0a–0d

* **0a. License**: Apache 2.0
* **0b. Documentation**: Inline code docs and user tutorial
* **0c. Testing**: Unit test coverage for NFT contracts and backend logic; test guide included
* **0d. Article**: Medium post summarizing milestones and learnings

### Milestone 1 (Month 1–1.5)

| Deliverables                                                          |
| --------------------------------------------------------------------- |
| Behavior mapping schema (MBTI logic, token categories)                |
| Parser backend service to tag wallet activity via Subquery/Subsquid   |
| NFT contract for MBTI-type soulbound NFTs                             |
| External dApp contract to manage persona evolution + metadata updates |
| Basic UI for wallet connect, persona mint preview                     |
| Unit tests and integration with AssetHub                              |

**Cost**: \$5,000 USD

### Milestone 2 (Month 1.5–3)

| Deliverables                                                                                                     |
| ---------------------------------------------------------------------------------------------------------------- |
| Implement behavior data aggregation system with privacy-preserving architecture (Subquery → IPFS → NFT metadata) |
| AI prompt builder integrated with persona traits                                                                 |
| Chat UI + personality response variation engine                                                                  |
| Shareable persona cards and leaderboard interface                                                                |
| Public persona explorer dApp (browsing, search, filter)                                                          |
| Mocked XCMP simulation for multichain activity sync                                                              |
| Blog post + tutorial + testing & feedback round                                                                  |

**Cost**: \$5,000 USD

### Budget Breakdown

| Role               | Hours | Rate (USD/hr) | Subtotal (USD) |
| ------------------ | ----- | ------------- | -------------- |
| Backend Developer  | 120   | \$30          | \$3,600        |
| Smart Contract Dev | 80    | \$35          | \$2,800        |
| Frontend Developer | 100   | \$30          | \$3,000        |
| AI/Prompt Engineer | 30    | \$35          | \$1,050        |
| Testing & Docs     | 20    | \$25          | \$500          |
| **Total**          | —     | —             | **\$10,950**   |

Requested Grant Amount: **\$10,000** (remaining buffer self-funded)

## **Future Plans**

After the fast grant:

* Expand to full production MVP
* Launch NFT persona marketplace with social and monetization layers
* Partner with Subquery/Subsquid for richer cross-chain indexing
* Integrate with DAO governance platforms to allow persona delegation

## **Additional Information**

Nemo redefines on-chain identity using behavior, psychology, and AI. We believe every wallet holds a story — and Nemo turns that into a living, evolving personality protocol.
