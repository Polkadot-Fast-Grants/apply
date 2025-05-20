# 📝 Crypto Trade Assistant

---

## 🌟 Project Overview

- **Brief description of the project:**  
  Crypto Trade Assistant is a Telegram-based cryptocurrency trading assistant on the Solana network. It enables users to
  copy professional traders, execute limit orders, perform token security checks (RugCheck), monitor wallets, stake
  assets, and track trading analytics.


- **How it relates to / integrates into Polkadot:**  
  Currently built for Solana; future plans include a bridge to Polkadot via XCM and Plaza integration.


- **Why your team is interested in this project:**  
  We aim to democratize advanced trading tools by integrating them into the familiar Telegram interface and leverage
  copy-trading to help users learn from successful traders.

---

### 🔍 Project Details

- **Technology stack overview:**
    - Python 3.10+
    - PostgreSQL 14+
    - Async architecture with asyncio
    - SQLAlchemy ORM with asyncpg
    - Prisma for migrations
    - Aiogram for Telegram interactions


- **Documentation of core components, protocols, architecture:**
    - **Telegram Interface Module:** handles user commands and message parsing
    - **Trading Engine:** wraps Solana JSON-RPC for buy/sell & limit orders
    - **RugCheck Service:** fetches token metadata and runs on-chain heuristics
    - **Copy-Trading Manager:** tracks master accounts
    - **Wallet Monitor:** subscribes to account changes via api


- **PoC/MVP or prior work:**
    - Initial Telegram bot with basic buy/sell, RugCheck deployed and copy trades


- **Data models / API specifications:**
    - **Users:** id, telegram_id, solana_wallet, _private_key, referral_code, total_volume, created_at, last_activity,
      last_buy_amount, referral_id
    - **Trades:** id, user_id, token_address, amount, price_usd, amount_sol, created_at, transaction_type, status,
      gas_fee, transaction_hash, extra_data
    - **APIs:** REST endpoints for analytics and account binding (helius-rpc)


- **What the project will NOT provide (limitations):**
    - Margin trading or leveraged positions
    - Legal financial advice

---

### 🧩 Ecosystem Fit

- **Where and how the project fits into the ecosystem:**  
  Focuses on DeFi/trading on Solana, with potential expansion to Polkadot Hub and Plaza via XCM.


- **Target audience:**  
  Retail crypto traders, Telegram user communities, crypto influencers.


- **What needs does it meet?**
    - Simplifies access to advanced trading strategies
    - Provides on-chain token security checks to mitigate rug pulls
    - Enables passive income through copy-trading


- **Similar projects in the Polkadot ecosystem:**
    - **If any:** Other trading bots exist on Solana, but none integrate copy-trading, referral bonuses, and Telegram UI
      in one product.
    - **If none:** The combined feature set (copy-trading + rug checks + affiliate system) is novel and hasn’t been
      packaged into a Telegram-first bot.

> _Note: We prioritize projects building on Plaza/Polkadot Hub, games, and DeFi._

---

## 👥 Team

- **Team Name:**  
  Incogo

- **Contact Name:**  
  Nursultan Zhuldizbekuly

- **Contact Email:**  
  nurikwy@gmail.com

- **GitHub / Telegram:**  
  - https://github.com/nurikwy
  - https://t.me/nurikwy

### Team members

- **Grant beneficiaries:**
    - Nursultan Zhuldizbekuly(CTO)

#### LinkedIn Profiles

- https://www.linkedin.com/in/nursultan-zhuldizbekuly/

### Team Code Repos

- https://github.com/nurikwy/CryptoTradeAssitant

**GitHub accounts:**

- https://github.com/nurikwy

### Team’s experience

Our core team brings together a unique blend of blockchain, backend, security and bot-development expertise:

- **Blockchain & Crypto**
    - Developed eDiploma — a portal issuing graduates’ diplomas as NFTs (React.js, Node.js, Python; ECP/Ethereum-like
      signing).
    - Built Python/Selenium parsers to fetch and process real-time cryptocurrency price data from trusted APIs and HTML
      sources.
    - Hands-on with token security heuristics through personal RugCheck experiments.


- **Telegram Bot Development**
    - Created a Telegram sales-funnel bot (Aiogram) with automated payment handling, lead heat-up messaging and scripted
      flows.
    - Implemented real-time WebSocket communications for user notifications and order status.


- **Backend & Async Architecture**
    - Expert in Python 3.8+, FastAPI/Django/Flask, SQLAlchemy + asyncpg, PostgreSQL/MySQL.
    - Designed and deployed universal CRM-style backends with WebSocket support for live updates.


- **Security & Auditing**
    - B.Sc. in Information Security (Cybersecurity) from Astana IT University.
    - Developed an automated pentesting framework to streamline vulnerability discovery (Nmap, Metasploit, Burp Suite).


- **API Integration & DevOps**
    - Integrated with third-party services: Yandex.Доставка, InDrive, CDEK, NCA Layer, Robocassa, Stripe.
    - Proficient in CI/CD pipelines, Nginx setup, server virtualization (VMware/Hyper-V), Linux server administration.


- **Analytics & Machine Learning**
    - Architected a health-monitoring AI (scikit-learn, pandas, NumPy) for risk prediction.
    - Built an AI-based plagiarism detector leveraging Google Scholar data and custom ML pipelines.

This blend of scalable async Python architecture,
deep blockchain security expertise, and Telegram-bot engineering
equips us to deliver Crypto Trade Assistant’s customizable copy-trading,
reliable RugCheck security checks, precise limit-order execution,
staking functionality, and real-time wallet monitoring.



---

## 📊 Development Status

- **Prototype:** Not yet available; core architecture and specs are finalized.
- **Documentation:** All design and research consolidated in a single `docs.md`:  
  https://github.com/nurikwy/CryptoTradeAssitant/blob/main/docs.md
- **Key Areas Covered:**
    - System architecture & Telegram interaction flows
    - Data models & relationships
    - Solana RPC integration & DEX patterns
    - On-chain security checks (RugCheck)
    - Copy-trading algorithm design
    - Polkadot Integration Research

---

## 📅 Development Roadmap

This section breaks the development roadmap down into milestones and deliverables. Each milestone is capped at **\$5,000
USD** and must be delivered within **3 months** of approval. The total grant requested is **\$15,000 USD** (exceptional
case).

**Important notes:**

* Each milestone is capped at **\$5,000 USD**
* Milestones must be delivered within **3 months** of approval
* Maximum grant amount is **\$10,000 USD** per application (up to **\$15,000 USD** in exceptional cases)
* Payment is made only after successful milestone delivery

### Overview

* **Estimated Duration:** 3 months
* **Full-Time Equivalent (FTE):** 1.5
* **Total Costs:** \$15,000

> Deliverables 0a–0d are mandatory.

| Number | Deliverable                         | Specification                                                                                                                                                                                                                                                                  |
|-------:|-------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|    0a. | License                             | MIT                                                                                                                                                                                                                                                                            |
|    0b. | Documentation                       | Inline code comments throughout + wallet registration, trading commands, copy-trading, RugCheck, limit orders, smart-money alerts and Polkadot integration.                                                                                                                    |
|    0c. | Testing                             | Telegram handlers, Trading Engine, RugCheck, CopyTrade, LimitOrder, WalletMonitor, XCM bridge. Basically user will test by himself                                                                                                                                             |
|    0d. | Article                             | Post-grant article detailing architecture, implementation steps, challenges faced, and results achieved.                                                                                                                                                                       |
|     1. | Telegram interface & Solana trading | • Full Aiogram inline-button interface<br>• Wallet registration flow with encrypted private-key storage<br>• Market buy/sell commands on Solana via JSON-RPC<br>**Verification:** Link wallet & execute buy/sell; inspect tx logs.                                             |
|     2. | Advanced trading features           | • Copy-trading module (follow/unfollow + adjustable risk slider)<br>• RugCheck on-chain metrics display<br>• Limit orders with slippage control<br>• Smart-money whale-transaction alerts<br>                                                                                  |
|     3. | Polkadot integration                | • XCM bridge for message & asset transfer to Polkadot Hub/Plaza<br>• Adapt Trading Engine to Substrate parachain<br>• Deploy a proxy pallet for order execution & wallet events<br>**Verification:** Execute cross-chain trades via Telegram; confirm messages on both chains. |

### 💰 Budget Breakdown

Each milestone covers approximately **240 developer-hours** at **\$20.83/hr** (1.5 FTE average).

| Milestone | Deliverables           |   Cost (USD) | Hours & Rate            | Estimated Completion |
|----------:|------------------------|-------------:|-------------------------|----------------------|
|         1 | 0a–0d + Feature 1      |      \$5,000 | \~240 h @ \$20.83/h     | Month 1              |
|         2 | Feature 2              |      \$5,000 | \~240 h @ \$20.83/h     | Month 2              |
|         3 | Feature 3 + 0d Article |      \$5,000 | \~240 h @ \$20.83/h     | Month 3              |
| **Total** |                        | **\$15,000** | **\~720 h @ \$20.83/h** | **3 months**         |

## 🔮 Future Plans

- **Post-Grant Development:** Expand to multi-chain support (Polkadot, Ethereum) via cross-chain bridges.
- **Additional Funding:** Apply for Parity grants, VC rounds targeting DeFi infrastructure.
- **Vision:** Become the go-to Telegram bot for secure, social crypto trading across major networks.
