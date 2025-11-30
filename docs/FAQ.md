# ATAL FAQ  
Public Review Draft v0.9

---

## 1. What is ATAL?

ATAL (AI Traceability & Accountability Ledger) is a vendor-neutral, implementation-independent standard for recording, governing, and auditing AI decisions.  
It ensures that every AI action — human-initiated or autonomous — is captured in a tamper-evident, regulator-ready evidence structure.

---

## 2. Why do we need ATAL?

AI systems make consequential decisions, but:

- logs are inconsistent  
- evidence is incomplete  
- model/tool chains are complex  
- autonomy risks are increasing  
- regulators cannot reconstruct what happened  

ATAL solves this by defining what must be recorded, how oversight must work, and how causality must be preserved across full AI workflows.

---

## 3. What is the 0th Law of AI Accountability?

Any AI system capable of initiating or escalating actions without direct human instruction MUST be governed by an external, independent accountability layer that can observe, restrict, pause, override, or terminate those actions.

This principle is foundational and applies broadly across all nine Parts of the specification.

---

## 4. Is ATAL a product?

No.  
ATAL is a **standard**.

It defines the rules and evidence structures required for AI accountability.  
Products or implementations must adhere to ATAL, but the standard itself contains no code.

---

## 5. How is the ATAL Specification structured?

The standard is structured across **nine Parts (I–IX)** covering:

- human-initiated actions  
- autonomous actions  
- evidence structures  
- lineage models  
- risk tiers  
- self-modification  
- emergent intent  
- safety kernel protocols  

See the specification for full details.

---

## 6. Does ATAL apply only to autonomous AI systems?

No.  
ATAL applies to:

- human-triggered actions (Part I)  
- autonomy-capable systems (Part II)  

Both modes must produce verifiable, complete ledger records.

---

## 7. Does ATAL dictate which models or tools to use?

No.  
ATAL is model-agnostic and vendor-agnostic.

It does not prescribe:

- specific LLMs  
- cloud providers  
- orchestration frameworks  
- model architectures  
- coding languages  

ATAL defines **outcomes**, not implementation choices.

---

## 8. How does ATAL support regulatory compliance?

ATAL aligns with:

- DPDPA (India)  
- CERT-In Directions  
- EU AI Act  
- ISO/IEC 42001  
- sectoral regulations  

It provides the forensic and governance requirements that regulators expect.

---

## 9. What is a Decision Trail?

A Decision Trail is the per-action evidence record containing:

- human intent (if any)  
- model(s) used  
- tool and data access  
- parameters  
- output  
- cryptographic signatures  

It is the atomic evidence unit in ATAL.

---

## 10. What is the Composite Accountability Graph (CAG)?

CAG is a causal graph linking:

- Decision Trails  
- Self-Modification Ledger entries  
- Emergent Intent Tracking events  
- tool actions  
- upstream/downstream dependencies  

It enables full reconstruction of “what happened and why.”

---

## 11. Can the AI modify its own code or tools?

Yes, but only if:

- every modification is captured in the **Self-Modification Ledger (SML)**  
- changes are cryptographically logged  
- risk-tier and oversight rules are applied  
- lineage is preserved  

Unaudited or hidden modification is non-compliant.

---

## 12. What happens if an AI system becomes unsafe?

The **Safety Kernel** (Part IX) provides:

- pause  
- throttle  
- restrict  
- override  
- kill-switch  

capabilities independent of the AI system.  
Every intervention is logged.

---

## 13. What are HIR and ART tiers?

**HIR Tiers** classify human-initiated actions based on sensitivity and risk.  
**ART Tiers** define autonomy levels (ART0–ART5) and their oversight requirements.

---

## 14. Who maintains the ATAL Standard?

The standard is stewarded by Elytra Security.  
Governance and stewardship rules are defined in the respective documents in this repository.

---

## 15. How can I contribute?

During public review windows:

- you may file GitHub Issues  
- suggestions, questions, and clarifications are welcome  
- pull requests are disabled  
- the Steward makes final editorial decisions  

See `PEER_REVIEW.md` for details.

---

## 16. Is ATAL free to use?

Yes.  
The standard is publicly available and governed by the license defined in `LICENSE.md`.  
Compliance or certification models may be separately defined.

---

## 17. Will ATAL introduce certification?

ATAL provides a **conformance structure** but does not require certification.  
Certification may be offered by independent bodies in the future.

---

## 18. Does ATAL store personal data?

ATAL itself does not store data.  
Implementations must follow relevant privacy laws (DPDPA, GDPR, etc.) when recording evidence.

---

## 19. What is the relationship between ATAL and the reference implementation?

The implementation (maintained separately) follows ATAL but does not define it.  
The standard remains vendor-neutral.

---

## 20. Where should I start?

- Read the Primer for the conceptual overview  
- Review the Specification for full requirements  
- Submit questions via Issues  

---

End of document.

---

_Last updated: 30 November 2025_  

© 2025 Elytra Security. All rights reserved for stewardship, versioning, and normative control of the ATAL Standard.  

Licensed under the ATAL Documentation License (see [LICENSE.md](../LICENSE.md)).
