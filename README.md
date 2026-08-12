# Microsoft 365 Copilot Public AI Risk Assessment
<img width="1536" height="1024" alt="Designer (21)" src="https://github.com/user-attachments/assets/c1b7d89a-a602-4b8e-b549-a9dbf0b7832a" />


A real-world AI governance and risk assessment for **Microsoft 365 Copilot** in a museum, records-management, and metadata environment.

## Project Documentation

Follow the information flow from **project definition → system profiling → use-case inventory → risk classification → risk assessment → governance controls → human oversight → monitoring → incident response → audit → final recommendation**.

1. [Project Charter](./01-Project-Charter.md)
2. [Copilot System Profile](./02-Copilot-System-Profile.md)
3. [Copilot Use-Case Inventory](./03-Copilot-Use-Case-Inventory.md)
4. [Risk-Tier Model](./04-Risk-Tier-Model.md)
5. [NIST AI RMF Mapping](./05-NIST-AI-RMF-Mapping.md)
6. [Copilot Risk Register](./06-Copilot-Risk-Register.md)
7. [Detailed Risk Analysis](./07-Detailed-Risk-Analysis.md)
8. [Governance Control Framework](./08-Governance-Control-Framework.md)
9. [Copilot Acceptable Use Policy](./09-Copilot-Acceptable-Use-Policy.md)
10. [Human Review Matrix](./10-Human-Review-Matrix.md)
11. [Governance Dashboard](./11-Governance-Dashboard.md)
12. [Incident Response Plan](./12-Incident-Response-Plan.md)
13. [Audit Checklist](./13-Audit-Checklist.md)
14. [Implementation Plan](./14-Implementation-Plan.md)
15. [Key Risks and Controls](./15-Key-Risks-and-Controls.md)
16. [Final Recommendation](./16-Final-Recommendation.md)

## Executive Governance Principle

> **Copilot output is draft content. Human review is required before high-impact, official, public-facing, records-related, or culturally sensitive content is approved for use.**

## Final Decision

**Approve with Controls**


## Frameworks Used
This project applies established AI governance, AI risk management, information security, and responsible AI frameworks to support the assessment and governance of Microsoft 365 Copilot.
### 1. NIST AI Risk Management Framework (AI RMF)

The **NIST AI RMF** provides the primary structure for identifying, assessing, measuring, and managing AI risks.

The project applies the four core functions:

- **Govern** — Establish AI governance, accountability, policies, and responsibilities.
- **Map** — Identify AI use cases, stakeholders, data, context, and potential risks.
- **Measure** — Assess AI risks, performance, incidents, and control effectiveness.
- **Manage** — Apply risk treatments, human oversight, monitoring, and corrective actions.

**Official Reference:**  
[NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework)

---

### 2. NIST AI RMF — Generative AI Profile

The **NIST Generative AI Profile (NIST AI 600-1)** provides additional guidance for risks associated with generative AI systems.

It supports this project in areas including:

- Generative AI risk identification
- AI output reliability
- Human oversight
- Information integrity
- Privacy
- Security
- Responsible AI governance

**Official Reference:**  
[NIST AI Risk Management Framework — Generative AI Profile](https://www.nist.gov/publications/artificial-intelligence-risk-management-framework-generative-artificial-intelligence)

---

### 3. ISO/IEC 42001:2023 — Artificial Intelligence Management System

**ISO/IEC 42001** provides requirements for establishing, implementing, maintaining, and continually improving an **Artificial Intelligence Management System (AIMS)**.

It supports the project in:

- AI governance
- AI policies
- Roles and responsibilities
- AI risk management
- Operational controls
- Monitoring
- Continual improvement
- Governance accountability

**Official Reference:**  
[ISO/IEC 42001:2023](https://www.iso.org/standard/42001.html)

---

### 4. ISO/IEC 23894:2023 — AI Risk Management

**ISO/IEC 23894** provides guidance for organizations managing risks associated with AI systems.

It supports this project in:

- AI risk identification
- Risk assessment
- Risk treatment
- Risk ownership
- Risk monitoring
- Integration of AI risk management into organizational processes

**Official Reference:**  
[ISO/IEC 23894:2023](https://www.iso.org/standard/77304.html)

---

### 5. ISO/IEC 27001:2022 — Information Security Management System

**ISO/IEC 27001** provides the broader information-security management foundation for protecting organizational information and managing security risks.

It supports the project in:

- Information security governance
- Access control
- Information protection
- Risk management
- Security monitoring
- Incident management
- Audit and continual improvement

**Official Reference:**  
[ISO/IEC 27001:2022](https://www.iso.org/standard/27001.html)

---

## Framework Alignment

| Project Area | Primary Framework | Supporting Framework |
|---|---|---|
| AI Governance | NIST AI RMF | ISO/IEC 42001 |
| AI Risk Assessment | NIST AI RMF | ISO/IEC 23894 |
| Generative AI Risks | NIST GenAI Profile | ISO/IEC 23894 |
| AI Management System | ISO/IEC 42001 | NIST AI RMF |
| Information Security | ISO/IEC 27001 | NIST AI RMF |
| Access & Data Protection | ISO/IEC 27001 | ISO/IEC 42001 |
| Human Oversight | NIST AI RMF | ISO/IEC 42001 |
| Monitoring & Measurement | NIST AI RMF | ISO/IEC 42001 |
| Incident Response | ISO/IEC 27001 | NIST AI RMF |
| Audit & Assurance | ISO/IEC 42001 | ISO/IEC 27001 |
| Continual Improvement | ISO/IEC 42001 | NIST AI RMF |

---

## How the Frameworks Work Together

```text
                AI GOVERNANCE
                      │
          ┌───────────┴───────────┐
          │                       │
     NIST AI RMF             ISO/IEC 42001
          │                       │
   Govern / Map /          AI Management System
   Measure / Manage                │
          │                       │
          └───────────┬───────────┘
                      │
              AI RISK MANAGEMENT
                      │
               ISO/IEC 23894
                      │
                      ▼
              RISK ASSESSMENT
                      │
                      ▼
             GOVERNANCE CONTROLS
                      │
          ┌───────────┴───────────┐
          │                       │
   HUMAN OVERSIGHT          INFORMATION SECURITY
          │                  ISO/IEC 27001
          │                       │
          └───────────┬───────────┘
                      │
                      ▼
              MONITORING & AUDIT
                      │
                      ▼
            CONTINUAL IMPROVEMENT
