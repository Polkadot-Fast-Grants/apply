
# CodeGuard-AI

![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)
![Build Status](https://img.shields.io/badge/build-in%20progress-orange.svg)
![Polkadot Ecosystem](https://img.shields.io/badge/Polkadot-Substrate%20%7C%20ink!-pink.svg)

<div align="center">
  <img src="(https://github.com/user-attachments/assets/4a269c13-340f-4dab-ad6c-848618c1d85a" alt="CodeGuard-AI Logo" width="200"/>
</div>

**CodeGuard-AI** is an AI-powered tool to secure and optimize **Substrate** and **ink!** projects in the Polkadot ecosystem. It detects vulnerabilities (e.g., XCM flaws, DeFi exploits), rewrites code for efficiency, and implements features like optimized storage pallets. Built with **Rust**, **PHP**, and **JavaScript**, it offers a secure web interface for user authentication, project uploads, and management, delivering enhanced code via zipped folders. Targeting **Plaza/Polkadot Hub** and **DeFi developers**, CodeGuard-AI is tested on the **Rococo testnet** and aims to empower millions of developers globally.

## Table of Contents
- [Project Overview](#project-overview)
- [Project Details](#project-details)
- [Ecosystem Fit](#ecosystem-fit)
- [Team](#team)
- [Development Status](#development-status)
- [Development Roadmap](#development-roadmap)
- [Budget Breakdown](#budget-breakdown)
- [Future Plans](#future-plans)
- [Additional Information](#additional-information)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

### Tagline
Securing Polkadot’s future with AI-driven code excellence.

### Description
CodeGuard-AI automates secure code audits for Polkadot developers by analyzing **Substrate pallets** and **ink! smart contracts**. It leverages **GPT-4o** to detect vulnerabilities, rewrite code, and implement Polkadot-specific features. The tool includes a **PHP-based web interface** with user authentication (login/register), a dashboard for statistics, settings for account security (2FA, OpenAI key), and a project report page for managing uploads and downloads. Hosted locally, it integrates **Rust** tools (`cargo-audit`, `clippy`) and **JavaScript** (Polkadot-JS API) for robust functionality, tested on **Rococo**.

### Relation to Polkadot
CodeGuard-AI integrates with:
- **Substrate**: Audits pallets for vulnerabilities (e.g., storage leaks) and optimizes efficiency.
- **ink!**: Secures DeFi contracts against exploits (e.g., reentrancy).
- **Plaza/Polkadot Hub**: Ensures XCM compatibility and cross-chain security.
- **Polkadot-JS API**: Fetches runtime metadata.
- **Rococo Testnet**: Validates functionality on parachain projects.

It addresses Polkadot’s need for secure, efficient code, supporting parachain and DeFi growth.

### Why We’re Interested
As a software engineer with over six years of experience in **Rust**, **PHP**, **JavaScript**, and **cybersecurity**, I’m driven to secure Polkadot’s ecosystem. My cybersecurity expertise fuels my passion for tackling XCM vulnerabilities and DeFi exploits using innovative technology. I aim to deliver CodeGuard-AI as a scalable tool for millions, contributing to Polkadot’s decentralized vision and global blockchain innovation.

## Project Details

### Technology Stack
- **Rust**: Preprocesses code with `cargo-audit`, `clippy`.
- **PHP**: Web backend for authentication, uploads, GPT-4o calls, zipping, delivery (PHPMailer).
- **JavaScript (Node.js)**: Integrates Polkadot-JS API.
- **GPT-4o API**: Detects vulnerabilities, rewrites code, generates features.
- **MongoDB**: Stores user accounts/projects.
- **Local Hosting**: Development server or free-tier cloud.
- **Rococo Testnet**: Tests functionality.

### Core Components
- **Authentication Module (PHP)**: Login/register with bcrypt, email verification, 2FA settings.
- **File Processor (PHP)**: Traverses projects, extracts `.rs` files, runs `cargo-audit`.
- **AI Analyzer (PHP + GPT-4o)**: Detects vulnerabilities (cybersecurity-informed).
- **Code Rewriter (PHP + GPT-4o)**: Reviews and Rewrites code, adds features, validated by `cargo-test`.
- **Web Interface (PHP + JavaScript)**: Login, register, upload, dashboard, settings, project report (Tailwind CSS).
- **Delivery Module (PHP)**: Zips and delivers code via email.

### Documentation
- **Inline**: Comments in Rust, PHP, JavaScript.
- **Tutorial**: README.md guide on authentication, uploads, reports, tests (`cargo-test`).
- **API Specs**:
  - `POST /register`: Creates account, sends verification email.
  - `POST /login`: Authenticates, returns session token.
  - `POST /upload`: Uploads project, returns ID (authenticated).
  - `GET /analyze/:id`: Returns vulnerability report.
  - `GET /download/:id`: Returns zipped code.
  - `PATCH /settings`: Updates password, 2FA, OpenAI key.

### PoC/MVP
- **Research**: Substrate vulnerabilities, ink! exploits, GPT-4o, OWASP blockchain security.
- **Prototype**: PHP CLI tool for traversal and GPT-4o (Milestone 1).

### Mockups
- **Login/Register**: Email/password forms.
- **Upload**: Drag-and-drop form.
- **Dashboard**: Statistics (projects, analyses, vulnerabilities).
- **Settings**: Account security, OpenAI key.
- **Project Report**: Lists projects, download/delete.
Mockups in Milestone 2 on GitHub.

### Data Models
```php
class User {
    public string $email; // Unique email
    public string $password; // Bcrypt-hashed
    public bool $isVerified; // Email verification
    public array $openAiKey; // Encrypted
    public bool $twoFactorEnabled; // 2FA
}

class Project {
    public string $path; // Project path
    public array $rustFiles; // .rs files
    public string $auditReport; // cargo-audit JSON
    public string $securityAnalysis; // GPT-4o report
    public string $rewrittenCode; // Generated code
    public int $userId; // Linked to user
}
```

### Limitations
- **Scope**: Substrate/ink! only; Solidity later.
- **AI**: GPT-4o third-party, code open-sourced.
- **Scale**: Single-project uploads; batch processing future.
- **Delivery**: Email primary; KILT experimental.

## Ecosystem Fit

### Fit
CodeGuard-AI supports **Plaza** and **DeFi**:
- **Plaza**: Secures XCM apps.
- **DeFi**: Audits ink! contracts.
- **Substrate**: Enhances pallet security.

### Target Audience
- Substrate/ink! developers.
- Plaza/DeFi teams (e.g., Acala, Moonbeam).

### Needs Met
- **Security**: Mitigates XCM/DeFi risks.
- **Efficiency**: Optimizes code.
- **Innovation**: Adds features (e.g., optimized storage).

### Similar Projects
- **Scout Audit**: Static Substrate analysis.
  - **Difference**: CodeGuard-AI uses dynamic analysis, adds features.
- **No Similar Tools**: Substrate complexity, novelty explain gap.

## Team

### Team Name
Manomite

### Contact Name
Adeyeye George David

### Contact Email
manomitehq@gmail.com

### Website
https://github.com/mitmelon

### Team Members
- Adeyeye George
- Adeyeye Abimbola

### LinkedIn
https://www.linkedin.com/in/manomite

### Code Repos
- https://github.com/mitmelon/codeguard-ai (TBC)

### GitHub
- https://github.com/mitmelon

### Experience
I’m a software engineer with 6+ years in **Rust**, **PHP**, **JavaScript**, and **cybersecurity**:
- **Rust**: Built Substrate pallets (voting system).
- **PHP**: Developed CMS for 100+ customers.
- **JavaScript**: Created Web3 apps with web3.js.
- **Cybersecurity**: Audited DeFi platforms, applied OWASP guidelines.
Delivered 3+ projects, including Solidity Token.

## Development Status
- **Research**: Substrate, ink!, GPT-4o, OWASP.
- **Prototype**: PHP CLI tool (Milestone 1).
- **Repo**: https://github.com/mitmelon/codeguard-ai (TBC).

## Development Roadmap

### Overview
- **Duration**: 2 months (8 weeks)
- **FTE**: 1
- **Total Costs**: $9,000

### Milestones
| Number | Deliverable | Specification | Weeks |
|--------|-------------|---------------|-------|
| 0a. | License | Apache 2.0 (all milestones) | 1–6 |
| 0b. | Documentation | Inline comments; README.md tutorial (finalized in Milestone 6) | 1–6 |
| 0c. | Testing | PHPUnit, Jest, `cargo-test`; guide in README (finalized in Milestone 6) | 1–6 |
| 0d. | Article | Medium post on CodeGuard-AI’s impact (Milestone 6) | 6 |
| 1. | Web Upload Interface | PHP web tool with: <ul><li>Login/register (bcrypt, email verification).</li><li>Upload form.</li><li>Dashboard (statistics).</li><li>Settings (2FA, OpenAI key).</li><li>Project report (download/manage).</li></ul> Deliverable: Web interface on GitHub, tested locally. | 1–1.33 |
| 2. | File Processing| Add: <ul><li>File traversal (`RecursiveDirectoryIterator`).</li><li>`cargo-audit, cargo-clippy, cargo-geiger` integration.</li></ul> Deliverable: CLI tool on GitHub, tested on Rococo. | 1.34–2.66 |
| 3. | Vulnerability Detection | Add: <ul><li>GPT-4o for vulnerability detection (XCM flaws).</li><li>Update dashboard report.</li></ul> Deliverable: Updated tool, tested on Rococo. | 2.67–4 |
| 4. | Code Rewriting | Add: <ul><li>GPT-4o code rewriting for security/efficiency.</li><li>`cargo-test` validation.</li></ul> Deliverable: Updated tool, tested on Rococo. | 4.01–5.33 |
| 5. | Feature Implementation | Add: <ul><li>Feature (optimized storage in pallet).</li><li>`cargo-test` validation.</li></ul> Deliverable: Updated tool, tested on Rococo. | 5.34–6.66 |
| 6. | Delivery & Documentation | Add: <ul><li>Zipped delivery (PHPMailer).</li><li>Final documentation, tests, article.</li></ul> Deliverable: Final tool on GitHub, tested on Rococo. | 6.67–8 |

### Weekly Breakdown
#### Milestone 1: Web Upload Interface ($1,500, Week 1–1.33)
- **Week 1 (42.5h)** - Frontend Design:
  - Login form (email/password, bcrypt, session management).
  - Register form (email verification via PHPMailer).
  - Dashboard (statistics: projects uploaded, analyses run, vulnerabilities detected).
  - Project upload page (file upload, git clone section [cloning files directly for processing]).
  - Settings page (password update, 2FA, encrypted OpenAI key input).
  - Project report page (list projects, download/delete).
  - MongoDB setup, local hosting, GitHub repo initialization.

#### Milestone 2: File Processing ($1,500, Week 1.34–2.66) - Backend
- **Week 2 (42.5h)**: 
  - File upload processing, 
  - File scanning for preventing malicious uploads
  - File transversal (`RecursiveDirectoryIterator`)
  - File Content chunking to avoid prompt limit 
  - `cargo-audit, cargo-clippy, cargo-geiger` integration, Rococo testing.

#### Milestone 3: Vulnerability Detection ($1,500, Week 2.67–4)
- **Week 3 (42.5h)**: GPT-4o API integration, cybersecurity-informed prompts (XCM/DeFi vulnerabilities).
- **Week 4 (42.5h)**: Update dashboard for reports, JavaScript (Polkadot-JS) for metadata, Rococo testing.

#### Milestone 4: Code Rewriting ($1,500, Week 4.01–5.33)
- **Week 5 (42.5h)**: GPT-4o code rewriting for security/efficiency, `cargo-test` validation, Rococo testing.

#### Milestone 5: Feature Implementation ($1,500, Week 5.34–6.66)
- **Week 6 (42.5h)**: GPT-4o feature implementation (optimized storage), `cargo-test` validation, Rococo testing.

#### Milestone 6: Delivery & Documentation ($1,500, Week 6.67–8)
- **Week 7 (42.5h)**: PHP zipping and delivery (PHPMailer), draft documentation.
- **Week 8 (42.5h)**: Final tests (PHPUnit, Jest), README tutorial, Medium article, Rococo testing.

### Verification
- **Milestone 1**: Test login, register, dashboard, upload, settings, report page; verify user/project management.
- **Milestone 2**: File processing, `cargo-audit, cargo-clippy, cargo-geiger` on Rococo.
- **Milestone 3**: Verify vulnerability report accuracy on Rococo.
- **Milestone 4**: Validate rewritten code with `cargo-test` on Rococo.
- **Milestone 5**: Test feature (optimized storage) on Rococo.
- **Milestone 6**: Confirm delivery, tests, article.

## Budget Breakdown

| Milestone | Deliverables | Cost (USD) | Weeks |
|-----------|--------------|------------|-------|
| 1 | Web Upload Interface, 0a | $1,500 | 1–1.33 |
| 2 | File Processing, 0a | $1,500 | 1.34–2.66 |
| 3 | Vulnerability Detection, 0a | $1,500 | 2.67–4 |
| 4 | Code Rewriting, 0a | $1,500 | 4.01–5.33 |
| 5 | Feature Implementation, 0a | $1,500 | 5.34–6.66 |
| 6 | Delivery & Documentation, 0a–0d | $1,500 | 6.67–8 |
| **Total** | | **$9,000** | **8 weeks** |

### Costs
- **Each Milestone**: 56 hours at $25/hour ($1,400) + $100 GPT-4o (~8.33 runs).
- **Total**: 340 hours at $25/hour ($8,500) + 50 GPT-4o runs at $10/run ($500) = $9,000.

## Future Plans
- **Development**: Add batch processing, Solidity support.
- **Funding**: Web3 Foundation Grants, VC for enterprise features.
- **Vision**: Serve millions, driving Polkadot adoption.

## Additional Information
- **Work Done**: Researched Substrate, ink!, GPT-4o, OWASP.
- **Contributors**: Solo project, no prior funding.
- **Scalability**: Secure authentication, modular design for enterprise use.

## Installation
*To be completed post-grant approval*
1. Clone the repository:
   ```bash
   git clone https://github.com/mitmelon/codeguard-ai.git
   ```
2. Install dependencies:
   ```bash
   composer install
   npm install
   ```
3. Set up MongoDB database:
   ```bash
   php MongoBase.php
   ```
4. Configure PHPMailer SMTP in `config.php`.
5. Run locally:
   ```bash
   php -S localhost:8000
   ```

## Usage
*To be completed post-development*
1. Register at `http://localhost:8000/register`.
2. Verify email via link sent by PHPMailer.
3. Log in at `http://localhost:8000/login`.
4. Set OpenAI API key in Settings.
5. Upload Substrate/ink! project via drag-and-drop.
6. View statistics on Dashboard (projects, vulnerabilities).
7. Download or manage projects on Project Report page.

## Contributing
Contributions are welcome! Please:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/xyz`).
3. Commit changes (`git commit -m 'Add xyz'`).
4. Push to the branch (`git push origin feature/xyz`).
5. Open a pull request.

## License
Apache 2.0 - see [LICENSE](LICENSE) for details.