# Tremell McAlpine Jr. — Curriculum Vitae

[← Back to profile](README.md)

- **GitHub:** [github.com/tre-mac](https://github.com/tre-mac)
- **LinkedIn:** [linkedin.com/in/tremell-mcalpine](https://www.linkedin.com/in/tremell-mcalpine/)
- **Email:** [tremell2mcalpine@gmail.com](mailto:tremell2mcalpine@gmail.com)

---

## Summary

DevSecOps intern and Information Technology student with hands-on experience in CI/CD automation, Django configuration management, deployment tracking, and AWS monitoring. I help keep company software available by monitoring and troubleshooting Docker environments and owning the QA promotion gate. AWS and Azure certified, seeking an entry-level DevSecOps or cloud role.

---

## Education

### George Mason University (GMU) — Fairfax, Virginia
**Bachelor of Science, Information Technology** | Concentration: Cloud Computing | College of Engineering & Computing  
Expected May 2027

**Honors:** Dean's List — Summer 2025, Summer 2026

### Virginia Community College System (VCCS)
Transfer credit, Fall 2022 – Summer 2024 | 63 credit hours accepted by GMU

<details>
<summary>Transfer courses</summary>

| Course | Title | Credits |
|---|---|---|
| ARTH 101 | Intro to Visual Arts | 3 |
| BIOL 103 | Survey of Cellular & Molecular Biology | 3 |
| BIOL 105 | Cellular Biology Lab | 1 |
| BUS 100 | Business and Society | 3 |
| CHEM 211 | General Chemistry I | 3 |
| CHEM 213 | General Chemistry Laboratory I | 1 |
| COMM 101 | Interpersonal and Group Interaction | 3 |
| ECON 104 | Macroeconomic Principles | 3 |
| ENGH ---- | English Elective | 3 |
| ENGH 101 | Composition | 3 |
| ENGH L372 | Introduction to Film | 3 |
| HIST 101T | Foundations of Western Civilization | 3 |
| HIST 125 | Introduction to World History | 3 |
| IT ---- | IT Elective (×5) | 16 |
| IT 104 | Introduction to Computing | 3 |
| MATH 105 | Precalculus Mathematics | 5 |
| MATH 108 | Intro Calculus: Business Applications | 3 |
| UNIV 100 | Freshman Transition | 1 |

</details>

---

## GMU Coursework

### Completed

| Term | Course | Title | Grade |
|---|---|---|---|
| Fall 2024 | IT 102 | Discrete Structures | A- |
| Fall 2024 | IT 214 | Database Fundamentals | B+ |
| Fall 2024 | IT 293 | Applied IT: Junior Transition | B |
| Fall 2024 | IT 304 | IT in the Global Economy | B+ |
| Spring 2025 | IT 105 | IT Architecture Fundamentals | B+ |
| Spring 2025 | IT 213 | Multimedia and Web Design | A |
| Spring 2025 | MBUS 300 | Accounting in a Global Economy | B- |
| Summer 2025 | ENGH 202 | Rhetoric of Simulation Games | A+ |
| Summer 2025 | IT 300 | Modern Telecommunications | B+ |
| Fall 2025 | IT 206 | Object-Oriented Techniques for IT Problem Solving | B+ |
| Fall 2025 | IT 223 | Information Security Fundamentals | B+ |
| Fall 2025 | IT 341 | Data Communications and Networking Principles | B |
| Fall 2025 | STAT 250 | Introductory Statistics I | B+ |
| Spring 2026 | IT 207 | Applied IT Programming | B+ |
| Spring 2026 | IT 216 | Systems Analysis and Design | B+ |
| Spring 2026 | IT 343 | IT Project Management | B+ |
| Spring 2026 | IT 442 | Cloud Infrastructure | B |
| Summer 2026 | ENGH 302 | Advanced Composition (Multidisciplinary) | A |
| Summer 2026 | FAVS 300 | Global Horror Film | A |

### In Progress

| Term | Course | Title |
|---|---|---|
| Fall 2026 | IT 342 | Operating Systems Fundamentals |
| Fall 2026 | IT 451 | Cloud Services Management |
| Fall 2026 | IT 492 | Senior Design Project I |
| Spring 2027 | IT 352 | Security Administration of Linux Systems |
| Spring 2027 | IT 485 | Cloud Operations |
| Spring 2027 | IT 493 | Senior Design Project II |

---

## Experience

### DevSecOps Intern — SupplyBistro
Philadelphia, PA | Aug 2026 – Present | Tech stack: AWS, GitHub, GitHub Actions, ClickUp, Django, Docker

DevSecOps intern on a Django application deployed across four environments: DEV, QA, STAGING, and PROD. I work sprint stories and technical spikes covering release promotion, configuration management, database migrations, CI/CD safety, and monitoring. As of October 2026, my role is shifting toward AWS infrastructure and monitoring.

#### Release Promotion & Deployment Verification
- Promote code across DEV → QA → STAGING → PROD and track pull requests through the pipeline, letting changes flow through each environment rather than cherry-picking into environment branches, which would put them out of sync
- Own the QA promotion gate checklist
- Defining post-deployment verification (smoke checks) for STAGING and Production deployments
- Specifying how verified deployment outcomes automatically update work-item and release state in ClickUp, starting with DEV/QA deployments and then STAGING/PROD

#### Django Configuration Management
- Refactored a monolithic Django settings module into a shared base and explicit per-environment modules (DEV, QA, STAGING, PROD), verified with zero unintended configuration changes using automated before/after fingerprint comparison
- Wrote Python tooling to capture and compare redacted environment configurations, used as audit evidence in pull requests
- Developing startup checks that enforce required Django runtime configuration when the application starts (builds on the settings refactor)

#### Database Migrations & Data Parity
- Built a CI migration gate in GitHub Actions that blocks pull requests with missing, conflicting, or broken Django migrations
- Leading a spike on synchronizing the existing DEV, QA, STAGING, and PROD databases to an approved Django migration baseline
- Developing a controlled migration-authoring workflow for developers, prototyped in an isolated sandbox repository before rollout to the main application
- Leading a spike defining a production-representative data refresh for STAGING

#### CI/CD Safety
- Building an isolated, unprivileged sandbox GitHub Actions workflow for testing pipeline changes away from the production codebase
- Ran the test cases validating reliable linting in CI

#### Monitoring & Observability
- Leading a non-production proof-of-concept spike evaluating AWS CloudWatch as the company's primary monitoring and observability platform
- Monitor and troubleshoot Docker environments

---

## Projects

### AI Security Monitor
Event-driven cloud security monitoring solution that automatically analyzes AWS account activity using AWS CloudTrail logs.

- Configured CloudTrail to deliver audit logs to Amazon S3 and trigger AWS Lambda functions through S3 event notifications
- Developed a Python-based Lambda function to parse CloudTrail records, identify security-relevant events, and perform automated risk analysis using Amazon Bedrock foundation models
- Stored security findings and AI-generated assessments in Amazon DynamoDB for historical tracking and investigation
- Integrated Amazon SNS email notifications to automatically alert administrators when high-risk or critical security events were detected

*Technologies:* AWS CloudTrail, Amazon S3, AWS Lambda, Python, Amazon Bedrock, Amazon DynamoDB, Amazon SNS

---

## Certifications

- Microsoft Certified: Azure Fundamentals (AZ-900)
- AWS Certified Cloud Practitioner
- AWS Certified AI Practitioner

---

## Skills

- **Programming:** Python, Java, SQL, Bash, YAML
- **CI/CD & DevOps:** GitHub Actions, GitHub CLI, pre-commit hooks, Docker
- **Security:** Secrets handling and redaction, secret scanning, SAST (Bandit)
- **Tools & Operating Systems:** Linux, macOS
