<img src="assets/banner.svg" width="100%" alt="Microsoft 365 Copilot Public AI Risk Assessment"/>

# Microsoft 365 Copilot Public AI Risk Assessment

**Public AI Risk Assessment and Governance Control Plan for Microsoft 365 Copilot in a Museum and Records Environment**

![Decision](https://img.shields.io/badge/Decision-Approve%20with%20Controls-2a9d3f?style=flat-square)
![Governance Status](https://img.shields.io/badge/Governance%20Status-Amber-e9a723?style=flat-square)
![Residual Risk](https://img.shields.io/badge/Residual%20Risk-Medium-e9a723?style=flat-square)
![Framework](https://img.shields.io/badge/Framework-NIST%20AI%20RMF-0a1128?style=flat-square)
![Framework](https://img.shields.io/badge/Framework-ISO%2FIEC%2042001-1b263b?style=flat-square)
![Framework](https://img.shields.io/badge/Framework-ISO%2FIEC%2023894-1b263b?style=flat-square)
![Framework](https://img.shields.io/badge/Framework-ISO%2FIEC%2027001-1b263b?style=flat-square)

## Overview

This project presents a real-world AI governance risk assessment for Microsoft 365 Copilot in a museum and records-management environment.

The assessment evaluates Copilot use cases across internal productivity, meeting summaries, metadata support, public content drafting, records workflows, and cultural heritage content. It identifies key risks — inaccurate outputs, sensitive data exposure, oversharing due to permissions, over-reliance, incorrect meeting summaries, public content errors, cultural misrepresentation, copyright concerns, prompt injection, and audit gaps — and the controls needed to manage them.

This project does **not** judge whether Microsoft 365 Copilot is "good" or "bad." Instead, it asks: if an organization uses Microsoft 365 Copilot, what risks should governance teams identify, what controls should be in place, and how should use be monitored?

> **Executive governance principle:** Copilot output is draft content. Human review is required before high-impact, official, public-facing, records-related, or culturally sensitive content is approved for use.

> Built entirely from Microsoft's public documentation and recognized AI risk-management references — no internal or proprietary organizational data is used.

## Repository Structure

Follow the information flow: **project definition → system profiling → use-case inventory → risk classification → risk assessment → governance controls → human oversight → monitoring → incident response → audit → final recommendation.**

| # | File | Contents |
|---|---|---|
| 01 | [Project-Charter.md](01-Project-Charter.md) | Project overview, rationale, objective, charter details, and scope |
| 02 | [Copilot-System-Profile.md](02-Copilot-System-Profile.md) | AI system profile — what Copilot is and how it accesses data |
| 03 | [Copilot-Use-Case-Inventory.md](03-Copilot-Use-Case-Inventory.md) | Use cases by department, data used, and risk tier |
| 04 | [Risk-Tier-Model.md](04-Risk-Tier-Model.md) | Low / Medium / High / Restricted risk-tier definitions |
| 05 | [NIST-AI-RMF-Mapping.md](05-NIST-AI-RMF-Mapping.md) | Govern–Map–Measure–Manage alignment |
| 06 | [Copilot-Risk-Register.md](06-Copilot-Risk-Register.md) | 12-risk register plus detailed risk analysis |
| 07 | [Copilot-Acceptable-Use-Policy.md](07-Copilot-Acceptable-Use-Policy.md) | Governance control framework and acceptable-use rules |
| 08 | [Human-Review-Matrix.md](08-Human-Review-Matrix.md) | Required reviewer by output type |
| 09 | [Governance-Dashboard.md](09-Governance-Dashboard.md) | Executive dashboard, metrics, and risk indicators |
| 10 | [Incident-Response-Plan.md](10-Incident-Response-Plan.md) | Four-level incident response plan |
| 11 | [Audit-Checklist.md](11-Audit-Checklist.md) | Governance, data protection, oversight, training, and monitoring checklist |
| 12 | [Executive-Summary.md](12-Executive-Summary.md) | One-page summary of risks, controls, and decision |
| 13 | [Final-Recommendation.md](13-Final-Recommendation.md) | Governance decision, approval conditions, and implementation roadmap |

## References & Frameworks

This project applies five established AI governance, AI risk management, and information-security frameworks.

**Governance frameworks**
- [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework) — primary structure for identifying, assessing, measuring, and managing AI risk; its Govern–Map–Measure–Manage functions structure this assessment
- [NIST AI RMF — Generative AI Profile (NIST AI 600-1)](https://www.nist.gov/publications/artificial-intelligence-risk-management-framework-generative-artificial-intelligence) — additional guidance for risks specific to generative AI: output reliability, human oversight, information integrity, privacy, and security
- [ISO/IEC 42001:2023 — AI Management System](https://www.iso.org/standard/42001.html) — requirements for establishing, implementing, and continually improving an AI management system (AIMS); secondary control-alignment reference
- [ISO/IEC 23894:2023 — AI Risk Management](https://www.iso.org/standard/77304.html) — guidance for identifying, assessing, treating, and monitoring AI-specific risk, and integrating it into organizational risk processes
- [ISO/IEC 27001:2022 — Information Security Management System](https://www.iso.org/standard/27001.html) — broader information-security foundation covering access control, information protection, security monitoring, and incident management
- [EU AI Act — Guidelines on Transparency for AI-Generated Content](https://digital-strategy.ec.europa.eu/en/policies/guidelines-transparency-ai-generated-content) — Article 50 transparency obligations for generative and interactive AI systems

**Framework alignment**

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

**How the frameworks work together**

```
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
```

**Microsoft 365 Copilot documentation**
- [Microsoft 365 Copilot — Data, Privacy, and Security](https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-privacy)
- [Microsoft 365 Copilot — Enterprise Data Protection](https://learn.microsoft.com/en-us/microsoft-365/copilot/enterprise-data-protection)
- [Microsoft 365 Copilot — Responsible AI Overview](https://learn.microsoft.com/en-us/microsoft-365/copilot/responsible-ai/responsible-ai-overview)

**Secondary analysis**
- [DLA Piper — NIST Releases Its Generative Artificial Intelligence Profile](https://www.dlapiper.com/insights/publications/ai-outlook/2024/nist-releases-its-generative-artificial-intelligence-profile)
