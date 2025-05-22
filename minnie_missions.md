# 📝 Name of your Project  
**MinnieMissions**

---

## 🌟 Project Overview

**Tagline:**  
Offers a Web3 street team platform to help fans support artists and brands by completing missions, earning rewards, and tracking impact on-chain.

**Description:**  
MinnieMissions is a Web3 platform where fans complete real-world and digital promotional missions — like poster drops, social shares, and referrals — in exchange for Vibe Points (VP), NFTs, and DOT-based rewards. Fans can generate custom QR codes tied to their wallets and track mission completion, proof of attendance, and event referrals. Artists (like DR ADAKU) and brands (like EasyA) can create custom MinnieSquads and MinnieReps, and reward grassroots promotion.  

We are building MinnieMissions with the polkadot smart contracts** for mission submission, VP tracking, and streaks. Rewards and NFTs are issued via **Polkadot Asset Hub**, and we use **XCM** to connect the two.  

We’re applying to run a **pilot immediately**, where fans will earn VP by completing poster and referral missions to onboard users to EasyA's events etc. The goal is to prove the reward system in a live use case with real-world engagement. In the first instance, some manual aspects such as identifying and onboarding pilot users to get feedback will strengthen the value of the project long term.

**Why we're building this:**  
Fans do a lot of promo for creators and companies that they love — we believe those efforts should be rewarded on-chain as superfans are fundamental to the growth of artists and brands. We’re passionate about fan economies, 'fandom' culture, and Web3 accountability. Ultimately, we're showing gratitude for people who care, and they deserve it! Imagine if MinnieMissions helps creatives and brands build their first 1000 superfans and then we have a global ecosystem of superfans / different 'MinnieSquads'.

---

## 🔍 Project Details

### Technology Stack  
- **Smart Contracts:** Ink! deployed on contract parachain (Moonbeam)
- **Token Issuance:** Polkadot Asset Hub (VP, NFTs, badges)
- **Backend:** Node.js + Express + PostgreSQL
- **Frontend:** React + Polkadot.js wallet connector
- **Storage:** IPFS (optional) for poster proofs

### Core Features  
- Mission submission + VP tracker  
- Streak & timestamp logic  
- Payment splitting (artist, treasury, fan)  
- QR-based mission & referral tracking  
- NFT + VP reward minting via Asset Hub  
- XCM-based cross-chain reward flow  

### What we are NOT doing (yet)  
- We're not building our own parachain in this phase (MinnieChain is future roadmap)  
- No on-chain DAO voting logic (planned in later stage)

---

## 🧩 Ecosystem Fit

**Where we fit:**  
We sit at the intersection of community, marketing, vibes and culture. We're onboarding real-world users to Web3 via fan culture and missions — driving interaction with brands and artists across the Polkadot ecosystem.

**Target Audience:**  
- Music fans and superfans  
- Brands looking for authentic promotion  
- Community based platforms (e.g., EasyA)  
- Artists and creators building on Polkadot  

**What need we solve:**  
There is no scalable way to reward grassroots fan marketing on-chain. We solve that with QR code mission proof, VP, and on-chain reward logic.

**Similar projects?**  
There are loyalty programs in Web3, but none focused on culture, IRL poster tasks, QR referrals, and artist-led squads. We’re bringing the Web2 street team model on-chain — transparently and rewardably. 

---

## 👥 Team

- **Team Name:** MinnieMissions  
- **Contact Name:** Dr Adaku Agwunobi  
- **Contact Email:** minniemissions@dradaku.com 
- **Website:** www.minniemissions.com
- **GitHub:** https://github.com/dradaku/minniemissions

### Team Members  
- Dr Adaku Agwunobi

### LinkedIn  
- https://linkedin.com/in/jenniferagwunobi

### GitHub  
- https://github.com/dradaku

### Experience  
Dr Adaku Jennifer Agwunobi, is a British-Nigerian academic, entrepreneur, singer/songwriter and overall creative powerhouse. She is the President of the Oxford Blockchain Society, a Postdoctoral Researcher at Oxford University, and a self-taught software developer who has won and organised multiple hackathons globally. Adaku is ex-Uber where she worked in their London head office during a peak growth phase and headed up their student brand ambassador programme. She also established key partnerships with influencers, creatives, the university ecosystem at large and local businesses.

With expertise spanning blockchain, AI, cybersecurity, and health tech, she has been at the forefront of innovation, securing an Innovate UK grant and leading major Web3 initiatives worldwide. She has also spoken on global stages, moderating panels with top VCs and developers in New York, Denver, and beyond.

Beyond tech, she is a passionate advocate for diversity, inclusion and impact. Furthermore, she has been running several 'VIBES WITH DR ADAKU' events globally where she empowers people with education and vibes (all her events have performances/concerts).

DR ADAKU has done:
7+ headline concerts/events sets since 2021

Audiences reached (in-person): Over thousands attendees cumulatively. Notable venues include university campuses, creative hubs, and Lagos/London stages including opening for artists at OVO Wembley and Koko Camden.

International presence: UK, Nigeria, and virtual panels/events with global reach

🎶 Digital Content & Streaming
Debut album "the vibes are known" released in 2021. 16 original tracks blending Afrobeats, R&B, UK rap

100k+ Spotify streams and 100K+ plays across platforms (incl. YouTube)

Music videos and behind-the-scenes content generating millions of impressions on IG and TikTok

Social crossover content exploring tech + music + wellness

🌍 Community & Web3 Engagement
Cybersecurity meetups + wellness talks under the VIBES brand since 2022

Example: “Wellbeing for Changemakers” workshop at Oxford Saïd Business School (Skoll Centre, 2023)

Hosted, organised, won and participated in dozens of Web3 panels, workshops, or hackathons over the past few years

500+ people onboarded to Web3 tools via music, storytelling, and gamified experiences

📢 Social Media & Comms Reach
@dradaku handles growing steadily on X, IG, LinkedIn, TikTok

Instagram: ~26k followers (@dradaku)
TikTok: 55k followers (@dradaku)
X: 10k followers (@dradaku)

TikTok viral content: over 2million+ views in total on Afrobeats, community and well-being crossover content

---

## 📊 Development Status

- ✅ Smart contract MVP drafted in Ink!    
- ✅ NFC membership card UX mocked  
- ✅ QR referral mission structure scoped  
- ✅ Initial GitHub: https://github.com/dradaku/minniemissions  
- ✅ Multiple visuals, smart contract drafts, and deployment plan already created 
- ✅ Submitted to EasyA polkadot hackathon in April 2025
- ✅ Created a pitchdeck: https://www.canva.com/design/DAGlKAASWaA/WIxbWMAxVxuUXUP_V7rZVA/edit?utm_content=DAGlKAASWaA&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton

---

## 📅 Development Roadmap

### Overview

- **Estimated Duration:** 3 months  
- **FTE:** 1.0  
- **Total Cost:** $10,000 USD

| Number | Deliverable | Specification |
| ------ | ----------- | ------------- |
| 0a | License | MIT |
| 0b | Documentation | Inline contract docs + tutorial: “How to Launch a Squad” |
| 0c | Testing | Unit tests for smart contract logic & QR referral input |
| 0d | Article | Medium post: “Rewarding Street Teams On-Chain with Polkadot” |
| 1 | Mission Submission & VP Contract | Build and deploy Ink! smart contract for `submit_mission`, `split_payment`, `get_vp`, `get_streak` |
| 2 | QR + Asset Hub Integration | Backend integration with fan-based QR tracking + mint NFTs and VP via Asset Hub using XCM |

---

### 💰 Budget Breakdown

| Milestone | Deliverables | Cost (USD) | Completion |
| --------- | ------------ | ---------- | ---------- |
| 1 | Create MinnieMissions content (videos, blogs, visuals) to get users | $2,500 | 0.5 months |
| 2 | Identify and onboard initial 50 users for a pilot where they will get rewards for doing 'minnie missions' e.g. putting posterd up. Initial users can be global | $1,500 | 1 month |
| 3 | MVP development: Update polkadot smart contract with feedback from initial pilot/testers: e.g. mission + streak logic, payouts | $3,000 | 1 month |
| 4 | MVP development: Backend + QR integration + XCM/Asset Hub minting | $2,000 | 0.5 months |
| 5 | Test the platform at 'VIBES WITH DR ADAKU 2025' Vibe-Coding London event| $1,000 | 0.1 months |
| **Total** | | **$10,000** | **3 months** |

---

## 🔮 Future Plans

- Launch “MinnieChain” as a Substrate parachain with squad DAO logic  
- Roll out NFC membership cards that unlock perks and prove attendance  
- Run more artist and brand pilot campaigns (DR ADAKU, EasyA)  
- Seek additional funding (Web3 VC, protocol grants)  
- Expand to IRL activations at concerts, hackathons, and festivals  

---

## ℹ️ Additional Info

- We’ll launch a pilot campaign with EasyA immediately after funding and get initial users. We will also do a pilot with DR ADAKU's listeners to onboard from the artist side.
- We’ve already built UI mockups, smart contract logic, and reward structure  
- Our visuals and onboarding are focused on culture-first education and real-world engagement
