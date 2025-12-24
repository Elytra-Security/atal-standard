# Responsibility of Implementers  
Public Review Draft v0.9

---

## 1. Purpose

This document explains the responsibilities of organisations and developers who implement, integrate, or operate ATAL-compliant systems.

Responsibilities apply across the entire ATAL specification, which is structured into nine Parts (I–IX).

Implementers of ATAL are responsible for ensuring that ATAL-based systems operate as non-intervening systems of record. ATAL implementations must not enforce policies, block execution, modify AI behavior, or introduce control logic into AI systems.Implementers remain solely responsible for legal, regulatory, and ethical compliance arising from AI system deployment. 
ATAL provides technical accountability mechanisms but does not transfer or dilute responsibility.

---

## 2. Core Obligations

### Complete Instrumentation  
Implementers must ensure that all required ATAL records are generated, including Decision Trails, SML entries, EIT signals, and CAG linkages.

Selective instrumentation is non-compliant.

### Preserve Evidence Integrity  
All ATAL evidence must be cryptographically signed, tamper-evident, immutable, and traceable.

No modification, deletion, or concealment is permitted.

### Uphold the 0th Law  
Any system capable of autonomous action must be governed by an external, independent accountability layer capable of observing, restricting, or terminating the AI’s actions.

This requirement cannot be bypassed.

---

## 3. Human-Initiated Interactions

Implementers must:

- capture user intent faithfully  
- classify actions under appropriate HIR tiers  
- enforce guardrails for ambiguous or high-risk prompts  
- record the direct connection between human intent and AI output  
- preserve the initiating request in full  

Human-triggered actions must produce Decision Trails in accordance with the specification.

---

## 4. Autonomous System Responsibilities

Systems capable of self-initiated or escalatory behaviour require:

- ART tier classification  
- real-time oversight by a Safety Kernel  
- generation of EIT signals for emergent behaviours  
- capture of all autonomous actions in Decision Trails  
- auditability through the Composite Accountability Graph  

Autonomy without these elements is non-compliant.

---

## 5. Safety and Oversight Requirements

Implementers must provide:

### Active Safety Kernel  
A functioning, independent layer that can:

- pause  
- restrict  
- throttle  
- override  
- terminate  

AI actions in real time.

### Verified Kill-Switch Pathways  
Kill-switch actions must be immediate, logged, and irreversible by the AI system.

### Escalation Controls  
High-risk or emergent behaviours must trigger mandatory oversight.

---

## 6. Lineage and Causality

Implementers must ensure:

- upstream provenance capture  
- downstream impact tracking  
- linking of all Decision Trails, SML entries, and EIT events  
- fully reconstructable causal chains via the CAG  

Breaks in lineage undermine ATAL compliance and must be treated as critical failures.

---

## 7. Cryptographic and Key Management Responsibilities

Implementers are responsible for:

- secure key generation  
- multi-party approval for sensitive signing keys  
- periodic rotation  
- protection against key leakage  
- using approved cryptographic primitives  

Compromised keys invalidate ATAL evidence.

---

## 8. Operational Responsibilities

Implementers must deploy:

- real-time monitoring of ATAL record generation  
- alerts for missing or malformed evidence  
- dashboards for oversight teams  
- health checks for Safety Kernel components  

They must also ensure:

- appropriate retention policies  
- export of regulator-friendly evidence bundles  
- secure archival  

---

## 9. Prohibited Practices

The following are strictly prohibited:

- bypassing the ATAL ledger  
- disabling or weakening the Safety Kernel  
- tampering with or deleting ATAL evidence  
- misclassifying HIR or ART tiers  
- suppressing EIT signals  
- concealing lineage relationships  
- allowing the AI system to override oversight controls  

Any violation constitutes a critical breach.

---

## 10. Compliance Responsibilities

Implementers must:

- undergo conformance assessments  
- maintain internal ATAL governance policies  
- train staff on ATAL requirements  
- participate in public review cycles where relevant  
- maintain transparent documentation  
- retain records for regulator-defined periods  

---

## 11. Enforcement

Non-compliance may result in:

- conformance revocation  
- regulator notification  
- legal liability  
- suspension of autonomy permissions  
- mandated oversight  

ATAL evidence may be used in legal or regulatory investigations.

---

## 12. Status of This Document

This document applies to ATAL v0.9 and will be updated after the public review period.

---

End of document.
