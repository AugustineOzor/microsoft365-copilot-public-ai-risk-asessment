[◄ Back to README](README.md)

# 06 · Copilot Risk Register

## Risk Register

| Risk ID | Risk | Impact | Likelihood | Rating | Primary Control |
|---|---|---|---|---|---|
| R-01 | Inaccurate or fabricated output | High | Medium | High | Human review |
| R-02 | Sensitive data appears in prompts or outputs | High | Medium | High | Data classification and user training |
| R-03 | Oversharing due to broad file permissions | High | Medium | High | Permissions review |
| R-04 | Over-reliance on Copilot output | Medium | High | High | User training and review rules |
| R-05 | Incorrect meeting summaries | Medium | Medium | Medium | Meeting owner validation |
| R-06 | Public-facing content published without review | High | Medium | High | Publication approval workflow |
| R-07 | Cultural or historical misrepresentation | High | Medium | High | Curatorial review |
| R-08 | Copyright or protected material concern | Medium | Low | Medium | Content review and source checking |
| R-09 | Prompt injection or malicious content risk | High | Low to Medium | Medium | Security controls and monitoring |
| R-10 | Audit and retention gaps | Medium | Medium | Medium | Audit logging and retention policy |
| R-11 | User misunderstanding of AI limitations | Medium | Medium | Medium | Responsible AI training |
| R-12 | Inappropriate use for restricted decisions | High | Low | Medium | Prohibited-use policy |

The NIST Generative AI Profile identifies generative AI as a cross-sectoral profile and companion resource for the AI RMF. A summary of the NIST GenAI Profile by DLA Piper identifies risks that are unique to or exacerbated by generative AI, including confabulation, data privacy, harmful bias or homogenization, human-AI configuration risks such as overreliance and automation bias, information integrity, information security, prompt injection, and intellectual property.¹ ²

## Detailed Risk Analysis

> Detailed scenario analysis is provided below for all twelve risks in the register.

### R-01: Inaccurate or Fabricated Output

**Scenario:** A staff member asks Copilot to summarize a collection-related document or draft an object description. The output appears fluent but includes unsupported facts.

**Impact:** Incorrect museum records · Poor decision-making · Public misinformation if published · Reduced trust in AI-assisted workflows

**Controls:** Treat Copilot output as draft content · Require source verification · Require human approval before official use · Require curator or registrar review for collection content

**Residual Risk:** Medium

### R-02: Sensitive Data in Prompts or Outputs

**Scenario:** A user enters donor, acquisition, HR, legal, or restricted cultural information into a Copilot prompt.

**Impact:** Privacy concern · Confidentiality concern · Records governance issue · Compliance exposure

**Controls:** Data classification training · Prohibited prompt examples · Sensitive-data handling rules · Restrict high-risk use cases · Monitor incidents

Microsoft states that with enterprise data protection, prompts and responses are protected by enterprise terms and commitments used for Microsoft 365 commercial offerings, and that prompts, responses, and data accessed through Microsoft Graph are not used to train foundation models.³

**Residual Risk:** Medium

### R-03: Oversharing Due to Broad Permissions

**Scenario:** A user asks Copilot for information, and Copilot can access documents the user technically has permission to access — even if that access was broader than intended.

**Impact:** Sensitive information discovery · Unauthorized internal visibility · Records and privacy concerns

**Controls:** Review permissions before rollout · Reduce excessive access · Apply sensitivity labels where appropriate · Maintain access governance · Train users that Copilot follows existing access permissions

Microsoft states that Copilot respects the organization's identity model and permissions.³

**Residual Risk:** Medium to High until permissions are reviewed

### R-04: Over-Reliance on Copilot Output

**Scenario:** A user accepts a Copilot-generated summary, translation, or policy interpretation without verifying it.

**Impact:** Poor decisions · Incorrect records · Mistaken action items · Reduced professional judgment

**Controls:** User training · "AI output is draft" rule · Review requirements for official records · Spot checks · Manager guidance for high-impact uses

A summary of the NIST Generative AI Profile identifies human-AI configuration risks, including overreliance and automation bias.²

**Residual Risk:** Medium

### R-05: Incorrect Meeting Summaries

**Scenario:** Copilot summarizes a meeting but misstates decisions, assigns action items incorrectly, or omits important context.

**Impact:** Incorrect follow-up · Records inconsistency · Accountability confusion

**Controls:** Meeting owner review · Decision log confirmation · Action-item owner confirmation · Official minutes template · Retention classification

**Residual Risk:** Medium

### R-06: Public-Facing Content Published Without Review

**Scenario:** A staff member uses Copilot to draft website text, exhibition copy, visitor guidance, or social media content and publishes it without review.

**Impact:** Public misinformation · Reputational harm · Inconsistent institutional voice · Cultural sensitivity concerns

**Controls:** Public content approval workflow · Communications review · Curatorial review for collection content · AI disclosure where required or appropriate · Incident response process

The European Commission's transparency guidance states that Article 50 of the EU AI Act applies from 2 August 2026 and includes transparency obligations for providers and deployers of certain AI systems, including generative and interactive AI systems — people should know when they are interacting with AI or exposed to AI-generated content.⁴

**Residual Risk:** Medium

### R-07: Cultural or Historical Misrepresentation

**Scenario:** Copilot drafts or rewrites content about culturally sensitive objects, sacred materials, contested histories, or provenance context.

**Impact:** Cultural harm · Misrepresentation · Public criticism · Loss of institutional trust

**Controls:** Curatorial review · Cultural sensitivity review · Restricted use for sensitive heritage topics · Approved terminology guide · No automatic publication

**Residual Risk:** Medium to High

### R-08: Copyright or Protected Material Concern

**Scenario:** Copilot produces content that may be similar to protected material or uses a source without proper review.

**Impact:** Copyright concern · Publication delay · Legal review need

**Controls:** Source checking · Rights review for public content · Avoid using AI output as final without review · Maintain citation and attribution expectations

Microsoft states that Microsoft 365 Copilot includes protected material detection and the Customer Copyright Commitment as part of enterprise data protection.³

**Residual Risk:** Low to Medium

### R-09: Prompt Injection or Malicious Content Risk

**Scenario:** A malicious document or webpage contains instructions designed to manipulate Copilot output.

**Impact:** Unsafe or misleading output · Information integrity risk · Security concern

**Controls:** User training · Security monitoring · Avoid blindly following generated instructions · Report suspicious outputs · Apply Microsoft 365 security controls

Microsoft states that Microsoft 365 Copilot operates with protections that include blocking harmful content, detecting protected material, and blocking prompt injections.¹

**Residual Risk:** Medium

### R-10: Audit and Retention Gaps

**Scenario:** Copilot-assisted work is created across email, chat, documents, and meeting summaries, but the organization has not defined how Copilot-related interactions should be logged, retained, or reviewed for audit purposes.

**Impact:** Difficulty reconstructing how a decision or document was reached · Weakened compliance posture · Gaps in accountability if an incident needs to be investigated · Inconsistent retention across departments

**Controls:** Extend existing retention and audit-logging policies to explicitly cover Copilot interactions · Define what is logged and for how long · Assign an owner for periodic audit-log review · Align Copilot logging with existing records-management schedules

Microsoft states that Copilot supports audit of interactions and follows administrative retention settings, depending on the organization's configuration and subscription plan.³

**Residual Risk:** Medium

### R-11: User Misunderstanding of AI Limitations

**Scenario:** A staff member treats Copilot output as authoritative rather than as a drafting aid, assuming a summary or suggestion is accurate because it reads fluently and confidently.

**Impact:** Misplaced confidence in incorrect output · Reduced critical review of AI-assisted work · Inconsistent understanding of Copilot's role across departments · Repeated errors from the same misunderstanding

**Controls:** Responsible AI training at onboarding and on a recurring basis · Clear internal messaging that Copilot output is draft material requiring review · Department-specific guidance on where AI limitations matter most · Manager reinforcement during quality and performance reviews

A summary of the NIST Generative AI Profile identifies human-AI configuration risks, including overreliance and automation bias, as risks that are unique to or exacerbated by generative AI.²

**Residual Risk:** Medium

### R-12: Inappropriate Use for Restricted Decisions

**Scenario:** A user relies on Copilot output as the basis for a decision that should be restricted to designated staff — for example, treating an AI-drafted summary as sufficient grounds for an acquisition, valuation, or repatriation-related judgment.

**Impact:** Decisions made without required expertise or authority · Policy or procedural violations · Reputational and legal exposure for high-stakes judgment calls

**Controls:** Maintain an explicit prohibited-use list · Restrict Copilot to a drafting or support role for defined decision categories · Require manager or specialist sign-off for decisions in restricted categories · Periodically audit compliance with prohibited-use rules

This risk is addressed directly by the prohibited-use list in [07-Copilot-Acceptable-Use-Policy.md](07-Copilot-Acceptable-Use-Policy.md).

**Residual Risk:** Medium

---
¹ [Microsoft 365 Copilot — Data, Privacy, and Security](https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-privacy)
² [DLA Piper — NIST Releases Its Generative Artificial Intelligence Profile](https://www.dlapiper.com/insights/publications/ai-outlook/2024/nist-releases-its-generative-artificial-intelligence-profile)
³ [Microsoft 365 Copilot — Enterprise Data Protection](https://learn.microsoft.com/en-us/microsoft-365/copilot/enterprise-data-protection)
⁴ [European Commission — Guidelines on Transparency for AI-Generated Content](https://digital-strategy.ec.europa.eu/en/policies/guidelines-transparency-ai-generated-content)

**Next:** [07 · Copilot Acceptable Use Policy →](07-Copilot-Acceptable-Use-Policy.md)
