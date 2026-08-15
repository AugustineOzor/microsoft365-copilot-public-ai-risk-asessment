[◄ Back to README](README.md)

# 12 · Executive Summary

Microsoft 365 Copilot coordinates large language models, Microsoft Graph content that users have permission to access, and Microsoft 365 applications.¹ Because Copilot can access organizational content and generate new content, this assessment's governance focus is on **accuracy, permissions, human oversight, records governance, public-content controls, data protection, and responsible use**.

## Highest Risks Identified

| # | Risk | Primary Control |
|---|---|---|
| 1 | **Inaccurate or Fabricated Output** — Copilot generates confident but incorrect information | Human verification and source review |
| 2 | **Sensitive Data Exposure** — users enter confidential information into prompts or unintentionally reveal information | Data-classification rules and permissions management |
| 3 | **Oversharing Due to Permissions** — users can surface information they technically have access to but may not expect AI to summarize | Permissions review and governance monitoring |
| 4 | **Over-Reliance on AI** — users accept Copilot outputs without verification | Training and mandatory human review |
| 5 | **Public Content Errors** — AI-generated public content is published without review | Formal publication approval workflow |
| 6 | **Cultural Misrepresentation** — collection, provenance, or heritage content is summarized incorrectly | Curatorial and cultural review |

*(The full 12-risk register with detailed scenario analysis is in [06-Copilot-Risk-Register.md](06-Copilot-Risk-Register.md).)*

## Summary

The largest governance risks were inaccurate AI outputs, sensitive-data exposure, oversharing through permissions, over-reliance on AI-generated information, records-management concerns, public-content inaccuracies, and cultural misrepresentation. To mitigate those risks, this assessment designs controls based on human oversight, data-classification rules, permissions management, content-review workflows, records-governance controls, monitoring dashboards, audit processes, and incident-response procedures. Copilot is treated as an AI assistant that supports human work, not a replacement for professional judgment.

---
¹ [Microsoft 365 Copilot — Data, Privacy, and Security](https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-privacy)

**Next:** [13 · Final Recommendation →](13-Final-Recommendation.md)
