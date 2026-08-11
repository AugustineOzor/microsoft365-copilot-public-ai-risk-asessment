# 07 — Detailed Risk Analysis

## R-01 — Inaccurate or Fabricated Output
**Scenario:** Copilot produces fluent but unsupported facts.
**Controls:** Draft-content rule, source verification, human approval, registrar/curator review.
**Residual Risk:** Medium.

## R-02 — Sensitive Data in Prompts or Outputs
**Scenario:** Donor, acquisition, HR, legal, or restricted cultural information is entered into a prompt.
**Controls:** Classification training, prohibited examples, sensitive-data rules, restrictions, incident monitoring.
**Residual Risk:** Medium.

## R-03 — Oversharing Due to Permissions
**Scenario:** Copilot surfaces information because a user has broader permissions than intended.
**Controls:** Permission review, least privilege, sensitivity labels, access governance, training.
**Residual Risk:** Medium–High until permissions are reviewed.

## R-04 — Over-Reliance
**Scenario:** Users accept summaries, translations, or interpretations without verification.
**Controls:** Training, draft rule, review requirements, spot checks.
**Residual Risk:** Medium.

## R-05 — Incorrect Meeting Summaries
**Controls:** Meeting-owner review, decision-log confirmation, action-owner confirmation, official minutes template.
**Residual Risk:** Medium.

## R-06 — Public Content Published Without Review
**Controls:** Communications review, curatorial review, publication approval, escalation, incident response.
**Residual Risk:** Medium.

## R-07 — Cultural or Historical Misrepresentation
**Controls:** Curatorial review, cultural sensitivity review, restricted sensitive-topic use, approved terminology, no automatic publication.
**Residual Risk:** Medium–High.

## R-08 — Copyright/Protected Material
**Controls:** Source checking, rights review, human review, citation and attribution.
**Residual Risk:** Low–Medium.

## R-09 — Prompt Injection/Malicious Content
**Controls:** User awareness, security monitoring, suspicious-output reporting, security controls, incident management.
**Residual Risk:** Medium.
