# MergeFund for Polkadot

## Project Overview
- **Tagline:** MergeFund — *Uber for developers* and *GoFundMe for repos.*
- **What:** MergeFund is a GitHub-native bounty and funding platform that gives developers a side hustle and helps maintainers get their issues solved. Maintainers post issues → fund them → contributors submit PRs → payouts happen automatically.  
- **Why:** Open source is dying because contributors don’t get paid and maintainers drown in unfunded issues. MergeFund solves this by making it easy to *fund repos the same way you’d tip a creator* — with links you can post on social media, in docs, or directly in GitHub Issues.  
- **Polkadot integration:**  
  - Add DOT payouts (using Subscan 7-day EMA price for compliance).  
  - Surface Polkadot repos/bounties in Plaza and Polkadot Hub.  
  - Provide funding links repos can share with their communities.  
- **Why us:** We’ve already onboarded 1,000+ developers. MergeFund.org is live . We’re the first to combine GitHub-native workflows with community funding links that turn repos into crowdfunded projects.

---

### Project Details
- **Stack:** Next.js (frontend), Node/TypeScript, GitHub App (webhooks), PostgreSQL/Supabase, polkadot.js (payouts), Subscan API (prices), Docker.  
- **Workflow:**  
  1. Maintainer installs the MergeFund GitHub App.  
  2. Issues are labeled as “funded” with a dollar or DOT amount.  
  3. Contributors claim and submit PRs.  
  4. On merge, payout is triggered automatically in DOT.  
  5. Repo gets a funding link (shareable anywhere: docs, Twitter, Telegram, etc.), letting the community add to the bounty pool.  

- **Not in scope (v1):** Escrow contracts, bridges, advanced custody. This proposal focuses on DOT payouts + repo onboarding + Plaza/Hub discovery.

---

### Ecosystem Fit
- **Where it fits:** Maintainers on Polkadot can close outside contributions faster; contributors get paid directly in DOT.  
- **Target users:** Polkadot core repos, parachain teams, SDKs/libraries, and ecosystem tools.  
- **Needs addressed:** Maintainers attract contributors with funded issues; contributors earn side hustle income by merging PRs.  
- **Commitment to Polkadot itself:**  
  - We want Polkadot (the network and its repos) onboarded as an early adopter.  
  - We’ll provide **custom integrations and workflows** for Polkadot maintainers.  
  - We’ll promote Polkadot’s repos to our **1,000+ signed-up developers**, driving immediate contributions and bounty completions.  

---

## Team
- **Team Name:** MergeFund  
- **Contact Name:** isaac gbaba
- **Contact Email:** isaac@mergefund.org 
- **Website:** [mergefund.org](https://mergefund.org)  
- **GitHub:** https://github.com/MergeFund  

### Team members
- Isaac Gbaba — Frontend/DevTools ( ex berkeley lab)
- Damien Johnson — Backend/Infra (ex-AWS, Accenture)  
- Evelyn yaskin — Frontend (ex-Emoney)  
- Matt boekamp — Backend (Hanover Insurance)  
- Alvin he — Finance/BD (ex-Dell, CVS)  

---

## Development Status
- MergeFund.org is live.  
- GitHub App skeleton + funded issue templates + basic dashboard working.  
- Next steps: DOT payout adapter, Polkadot repo onboarding, and Plaza/Hub discovery.

---

## Development Roadmap
> Each milestone ≤ $5,000. Total ≤ $10,000. Max delivery window: **6–8 weeks**. Payments occur **after milestone acceptance**.

### Overview
- **Duration:** 6–8 weeks  
- **FTE:** ~1.5 across period  
- **Total ask:** $7,500  

| Number | Deliverable | Specification |
|--------|-------------|---------------|
| 0a. | **License** | MIT/Apache-2.0 (OSS for all funded code) |
| 0b. | **Documentation** | “Add bounties to your repo in 5 minutes” guide |
| 0c. | **Testing** | Unit tests for payout adapter + webhook flows |
| 0d. | **Article** | Medium/Dev.to: “Uber for Developers: MergeFund + Polkadot” |

---

### Milestone 1 — DOT payouts + GitHub App flow (**$4,500**, Weeks 1–3)
- DOT payout adapter (polkadot.js + Subscan 7-day EMA)  
- Maintainer UX: funded labels, templates, PR verification  
- Screencast demo: fund issue → merge PR → payout in DOT  
- Docs, tests, draft article  

**Acceptance:** repo shows DOT payout flow reproducible by reviewers; docs/tests pass.

---

### Milestone 2 — Plaza/Hub discovery + Polkadot pilot (**$3,000**, Weeks 4–6)
- Plaza/Hub feed of Polkadot repos with active bounties  
- Onboard ≥10 Polkadot repos with funded issues  
- Close ≥10 issues with merged PRs + DOT payouts  
- Public dashboard showing metrics  
- Final article published  

**Acceptance:** live instance, pilot summary (repos, issues, merges, payouts), article.

---

### Budget Breakdown
| Milestone | Deliverables | Cost (USD) | Timeline |
|-----------|--------------|------------|----------|
| 1 | DOT payouts, GitHub App flow, docs/tests | $4,500 | Weeks 1–3 |
| 2 | Plaza/Hub discovery, 10-repo pilot, metrics | $3,000 | Weeks 4–6 |
| **Total** |  | **$7,500** | 6–8 weeks |

---

## Future Plans
- Partner with **Polkadot core repos** as a flagship adopter.  
- Push Polkadot-funded bounties directly to our **1,000+ developers**, driving activity fast.  
- Scale to **Open Source Developer Grant** (≤$30k) for advanced features (multi-sig, analytics).  
- Long term: become the **default contributor onboarding + funding layer** for the Polkadot ecosystem.  

**Most importantly:** we want Polkadot itself to **pilot MergeFund by posting funded issues**. This will showcase how maintainers can attract contributions instantly, while our dev community closes issues and ships value back to the ecosystem.
