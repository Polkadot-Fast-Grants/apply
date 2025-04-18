# 📝 Prosk Assist

## 🌟 Project Overview

- **Tagline**: Streamline job applications with AI-powered, role-specific form filling and cover letter generation.
- **Description**: Prosk Assist is a Chrome and Safari web extension (with a supporting website) that automates job application form filling using AI. It saves job seekers hundreds of hours by intelligently filling forms, generating tailored cover letters, and supporting multiple role-specific profiles (e.g., Software Developer, Data Scientist). Unlike basic resume parsers, it uses fine-tuned LLMs to understand and answer unique form questions accurately, improving resume shortlisting chances.
- **Polkadot Integration**: Prosk Assist could leverage Polkadot’s decentralized identity protocols (e.g., KILT Protocol) to securely store and verify user credentials and resumes on-chain, ensuring privacy and trust. Additionally, Polkadot’s parachains could enable scalable, low-cost storage of user data and fine-tuned LLM models.
- **Why We’re Interested**: Our team is passionate about solving real-world problems for job seekers. After researching the struggles of applying to 500+ jobs in today’s market, we developed Prosk Assist to save time, reduce stress, and empower users to land their dream roles with tailored, high-quality applications.
- **Pitch Video**: https://youtu.be/H4GbNl2Bc7Y

### 🔍 Project Details

- **Technology Stack**:
  - **Frontend**: HTML, JavaScript, CSS (for Chrome/Safari extension and website), React for the website dashboard.
  - **Backend**: Node.js, Express for the website API; Python for LLM integration and fine-tuning.
  - **AI/LLM**: Fine-tuned models (e.g., based on LLaMA or BERT) hosted on cloud platforms (e.g., AWS, Hugging Face).
  - **Blockchain**: Polkadot/KILT Protocol for decentralized identity and data storage (exploratory).
  - **Database**: MongoDB for user profiles and role-specific data.
- **Core Components**:
  - **Web Extension**: Injects scripts to autofill forms, supports multiple role-specific tabs (e.g., Software Developer, Data Scientist).
  - **Website**: User dashboard to manage resumes, skills, and role profiles.
  - **LLM Module**: Fine-tuned per user to answer unique form questions accurately.
  - **Cover Letter Generator**: Analyzes job descriptions and generates tailored cover letters.
  - **Resume Enhancer**: Analyzes job descriptions and suggests user to add and remove keywords, skills. Also suggests good resume template for companies.
- **PoC/MVP**: We’ve built a prototype Chrome extension that fills basic forms using predefined data (available at \[GitHub placeholder\]). Current work focuses on LLM integration and role-specific tab functionality.
- **Mockups/UI**:
  - Extension Popup: A simple interface with buttons to select role tabs (e.g., “Software Developer”, “Data Scientist”) and trigger form filling.
  - Website Dashboard: Displays user profiles, role-specific resumes, and generated cover letters.
- **Data Models/API**:
  - **User Profile**: `{ userId, email, roles: [{ roleName, resume, skills, keywords, projects, description }], coverLetterTemplates }`
  - **API Endpoints**:
    - `POST /api/generateCoverLetter`: Takes job description and role, returns tailored cover letter.
    - `GET /api/user/roles`: Retrieves user’s role-specific profiles.
    - `POST /api/llm/answer`: Sends form question to fine-tuned LLM, returns answer.
- **Limitations**:
  - Does not handle CAPTCHA or complex multi-step authentication.
  - File uploads (e.g., resumes) require manual user action due to browser security.
  - Initial LLM fine-tuning is cloud-based, not on-chain (Polkadot integration is exploratory).

### 🧩 Ecosystem Fit

- **Fit in Polkadot Ecosystem**: Prosk Assist fits into Polkadot’s vision of user-centric, decentralized applications. By integrating with KILT Protocol, it can offer verifiable, user-controlled credentials (e.g., education, work history) stored on-chain, enhancing trust in job applications. It could also leverage Polkadot’s Plaza/Polkadot Hub for community-driven job marketplaces.
- **Target Audience**: Job seekers (e.g., recent graduates, career switchers) applying to multiple roles across industries, particularly in tech (e.g., Software Developer, Data Scientist).
- **Needs Met**:
  - Saves time by automating repetitive form filling.
  - Increases resume shortlisting rates with role-specific, tailored applications.
  - Simplifies cover letter creation with AI-generated, job-specific content.
- **Similar Projects**:
  - **In Polkadot**: No known projects directly address AI-powered job application automation. KILT Protocol focuses on identity but not form filling.
  - **Outside Polkadot**: Tools like LinkedIn Easy Apply or resume parsers exist but lack role-specific customization and LLM-driven question answering.
  - **Differentiation**: Prosk Assist’s multi-role support, fine-tuned LLMs, and potential Polkadot integration (for secure data/identity) set it apart.

### 👥 Team

- **Team Name**: Prosk Assist
- **Contact Name**: Sanjaikumar Balasubramaniyan
- **Contact Email**: sanjaibala2002@gmail.com
- **Website**: https://sanjai-11.github.io/portfolio-website/

#### Team Members

- Sanjaikumar Balasubramaniyan (Lead Developer, AI Specialist)

#### LinkedIn Profiles

- https://www.linkedin.com/in/sanjai-bala-309066202/

#### Team Code Repos

- https://github.com/sanjai-11/prosk-assist/

#### Team GitHub Accounts

- https://github.com/sanjai-11

#### Team Experience

- **Sanjaikumar Balasubramaniyan**: 5+ years in AI/ML, developed NLP models for text generation, contributed to open-source LLM projects.
- No prior blockchain projects, but the team is eager to learn and integrate Polkadot/KILT for decentralized identity.

### 📊 Development Status

- **Current State**: A prototype Chrome extension exists that autofills basic forms using predefined data. We’ve researched LLM fine-tuning for question answering and mocked up the multi-role tab interface.
- **Research**: Analyzed job application pain points (500+ applications per job seeker, 100s of hours spent) and tested existing tools (e.g., LinkedIn Easy Apply, resume parsers) to identify gaps.
- **Next Steps**: Integrate LLM for dynamic question answering, implement role-specific tabs, and explore Polkadot/KILT integration.

### 📅 Development Roadmap

- **Estimated Duration**: 3 months
- **Full-Time Equivalent (FTE)**: 3 (three team members working full-time)
- **Total Costs**: $15,000 USD

| Number | Deliverable | Specification |
| --- | --- | --- |
| 0a. | License | MIT |
| 0b. | Documentation | Inline code comments in the extension and website codebase. A tutorial explaining how users can install the extension, create role-specific profiles, and autofill forms. Hosted on the project website. |
| 0c. | Testing and Testing Guide | Unit tests for core functions (form filling, cover letter generation, LLM question answering) using Jest (for JS) and PyTest (for Python). The guide will detail how to run tests locally. |
| 0d. | Article | An article published on Medium or the project website explaining Prosk Assist’s features, impact on job seekers, and potential Polkadot integration. |
| 1. | Multi-Role Support | Implement the role-specific tab feature in the Chrome/Safari extension. Users can create up to 10 role profiles (e.g., Software Developer, Data Scientist), each with a unique resume, skills, keywords, projects, and description. Verified via a demo on a sample job application form. |
| 2. | Cover Letter Generator | Develop an AI-powered cover letter generator that analyzes job descriptions and user role profiles to produce tailored cover letters. Integrated into the extension to autofill cover letter fields. Verified via generating 3 sample cover letters for different job postings. |
| 3. | LLM Integration | Integrate a fine-tuned LLM (cloud-based) to answer unique form questions not covered by standard fields. Each user gets a model fine-tuned on their resume and profile. Verified by answering 5 sample form questions with 95%+ accuracy. |

### 💰 Budget Breakdown

| Milestone | Deliverables | Cost (USD) | Estimated Completion |
| --- | --- | --- | --- |
| 1 | Multi-Role Support, Documentation, Testing | $7,000 | 1.5 months |
| 2 | Cover Letter Generator, LLM Integration, Article | $8,000 | 1.5 months |
| **Total** |  | **$15,000** | **3 months** |

### 🔮 Future Plans

- **Feature**: Make an Independent AI Agent, which will apply to relavant jobs all by itself for the applicant.
- **Post-Grant Development**: Launch Prosk Assist publicly, add support for more browsers (Firefox), and integrate Polkadot/KILT for decentralized identity storage.
- **Additional Funding**: Seek VC funding or apply for Polkadot’s larger grants to scale LLM training and blockchain integration.
- **Vision**: Become the go-to tool for job seekers globally, reducing application time by 80% and integrating with Polkadot’s ecosystem to offer secure, verifiable credentials for hiring.

### ℹ️ Additional Information

- **Work Done**: Prototype Chrome extension and initial LLM research completed.
- **Other Teams**: No other teams have contributed yet.
- **Other Funding**: No other funding applied for; this Fast-Grant is our first step.