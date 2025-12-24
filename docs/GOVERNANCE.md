# ATAL Governance Framework  
Public Review Draft v0.9

---

## 1. Purpose of This Document

This document defines the **governance model for the ATAL Standard** during its lifecycle:

- internal development  
- public review  
- versioned releases  
- long-term stewardship  
- transition to a multi-stakeholder governance body  

It establishes how ATAL evolves, who is responsible for its direction, and how changes are accepted, validated, and published.

This document governs the ATAL specification and its lifecycle. It does not define an AI governance or risk framework for organisations; it defines only the stewardship, change-control, and process obligations required to evolve and audit the ATAL Standard and ATAL-conformant implementations.


This file forms part of the **non-normative documentation** that supports ATAL’s credibility, neutrality, and long-term stability.

---

## 2. Principles of Governance

ATAL governance is guided by the following foundational principles:

### 2.1 Neutrality  
ATAL is a **vendor-neutral**, **model-neutral**, and **platform-agnostic** standard.

It must not depend on:

- a specific commercial implementation  
- a specific model provider  
- a specific cloud provider  
- proprietary tooling or infrastructure

### 2.2 Transparency  
Every change to the standard must be:

- documented  
- traceable  
- justified  
- approved through a structured review process  
- published with a versioned changelog  

### 2.3 Stability  
ATAL must maintain:

- backward compatibility where possible  
- predictable release cycles  
- clearly documented transitions  
- explicit deprecation models  

### 2.4 Independence  
ATAL must remain independent of:

- regulatory capture  
- private influence  
- commercial steering  

It must stand as a **public good**, designed to support global AI governance.

### 2.5 Public Accountability  
All future changes must be open to:

- peer review  
- expert critique  
- regulator feedback  
- global public comment  

---

## 3. Governance Structure

The ATAL governance model consists of three phases:

---

### **Phase 1: Foundational Stewardship (Current Phase)**

During the early lifecycle (v0.9 → v1.0):

- **Elytra Security** serves as the **Founding Steward**  
- All documents are authored, curated, and refined under this stewardship  
- Public review occurs via GitHub Issues  
- No external changes are merged directly into the repo  
- The Steward validates all feedback and incorporates changes into official releases  

Responsibilities of the Founding Steward:

- maintain canonical ATAL documentation  
- ensure accuracy and completeness  
- ensure alignment with global regulatory expectations  
- preserve neutrality  
- coordinate version releases  
- maintain the website (atal.elytrasecurity.com)  
- initiate the transition to multi-stakeholder governance at maturity  

---

### **Phase 2: Public Review & Multilateral Engagement**

Once ATAL v1.0 is released:

- the Steward invites participation from:  
  - regulators  
  - academia  
  - standards bodies  
  - cybersecurity organizations  
  - AI safety institutions  
  - industry practitioners  

Public engagement is limited to:

- GitHub Issues  
- structured feedback  
- formal review cycles  

No direct commits are accepted from external contributors.

Role of the Steward in this phase:

- manage comment intake  
- publish planned changes  
- release minor and patch updates  
- maintain the issue tracker  
- prepare for long-term governance transition  

---

### **Phase 3: Multi-Stakeholder Governance Body (Future Phase)**

Once ATAL matures (target: v2.0+):

A **formal Working Group** is established to assume long-term governance.

Composition:

- representatives from international standards bodies  
- regulators and public-sector experts  
- independent AI safety researchers  
- academic cryptography and ML experts  
- civil society and human rights observers  
- enterprise and industry practitioners  

Responsibilities:

- maintain and evolve ATAL  
- approve new releases  
- ratify structural changes  
- oversee mappings to external regulatory frameworks  
- preserve interoperability  
- maintain public trust and neutrality  

Elytra Security transitions from **Founding Steward → Permanent Member** with equal standing to other stakeholders.

---

## 4. Governance of the Specification (Part I–IX)

The ATAL Specification is divided into nine Parts.  
Governance applies uniformly across all of them.

### 4.1 No Partial Updates  
Changes must be applied:

- holistically  
- across all relevant Parts  
- with cross-document consistency  
- through full-file rewrites  

### 4.2 Nine-Part Stability  
Any modification affecting one Part must be checked against:

1. Human-Initiated AI Governance  
2. Autonomous AI Governance  
3. Decision Trails  
4. Self-Modification Ledger  
5. Emergent Intent Tracking  
6. Composite Accountability Graph  
7. Human-Initiated Risk (HIR) Tiers  
8. Autonomy Risk Tiers (ART)  
9. Safety Kernel & Oversight Protocols  

### 4.3 Safety-Critical Changes  
Any change that affects safety mechanisms (kill-switch, freeze protocol, oversight envelope) requires:

- extended review cycle  
- formal justification  
- approval by Working Group (once Phase 3 begins)  

---

## 5. Governance of Version Releases

### 5.1 Versioning Rules  
- Specifications use version numbers:  
  `ATAL_Specification_vX.Y.md`  
- Supporting documents are versionless  
- All changes require a matching changelog entry  
- Deprecated elements require at least one full release before removal  

### 5.2 Release Cycle  
- v0.9 → public review  
- v1.0 → stable release  
- v1.x → minor clarifications  
- v2.0 → structural evolution  

### 5.3 30-Day Public Review Requirement  
All major changes must undergo:

- **30 days of public review**  
- issue-based commentary  
- review summary  
- versioned release notes  

---

## 6. Contributor Model

### 6.1 External Contributors  
External parties may:

- review  
- comment  
- critique  
- propose ideas  

External parties may **not**:

- push commits  
- open pull requests  
- modify files directly  

### 6.2 Internal Contributors  
Only the Founding Steward may:

- write the documents  
- approve changes  
- manage releases  
- maintain the canonical repo  

### 6.3 Working Group Contributors (Future)  
When Phase 3 begins:

- members gain limited edit permissions  
- decisions must follow majority or supermajority voting (to be defined)  

---

## 7. Governance of Public Repositories

### Repository Types

1. **Internal Private Repo (current one)**  
   - working drafts  
   - instructions  
   - status logs  
   - backups  
   - internal tooling  

2. **Public ATAL Standard Repo (atal-standard)**  
   - only polished documents  
   - only nine-Part specification  
   - website pages  
   - review instructions  
   - versioned changelogs  
   - no internal files  

### Strict Separation  
No internal files may ever be moved to the public repo.

---

## 8. Compliance With External Regulations

The governance model ensures ATAL remains compatible with:

- India DPDPA  
- CERT-In requirements  
- EU AI Act  
- ISO/IEC 42001  
- NIST AI RMF  
- OECD AI principles  

The Steward ensures mappings remain up to date.

---

## 9. Decision Authority Summary

| Area | Authority (Current) | Authority (Future) |
|------|----------------------|---------------------|
| Document authorship | Founding Steward | Working Group |
| Release approval | Founding Steward | Working Group |
| Issue triage | Founding Steward | Shared |
| Safety-critical changes | Founding Steward | Supermajority vote |
| Public review | Required | Required |
| Stewardship role | Elytra Security | Multi-stakeholder body |

---

## 10. Status of This Document

- Applies during v0.9–v1.0 internal and public review  
- Will be updated once the Working Group structure is finalised  
- Non-normative but binding for process integrity  

---

End of document.
