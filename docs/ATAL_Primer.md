# ATAL Primer  
Public Review Draft v0.9 (Primer is versionless; the specification carries the version)

---

## 1. Introduction

ATAL (AI Traceability & Accountability Ledger) is a vendor-neutral, implementation-independent standard designed to ensure that all AI systems – whether human-triggered or autonomy-capable – operate with verifiable traceability, auditability, and accountability.

ATAL defines *what must be recorded*, *how evidence must be structured*, and *which governance controls must be applied*, so that regulators, auditors, enterprises, and courts can rely on a tamper-evident trail of AI decisions.

The Primer provides a concise, human-understandable overview of the full ATAL standard.

---

## 2. The 0th Law of AI Accountability

Any AI system capable of initiating or escalating actions without direct human instruction MUST be governed by an external, independent accountability layer that can observe, restrict, pause, override, or terminate those actions.

This principle shapes the entire ATAL architecture and is embedded throughout the nine Parts of the specification.

---

## 3. The ATAL Architecture: Nine Parts

The ATAL specification consists of nine structured Parts, each addressing a central element of AI accountability:

1. **PART I – Human-Initiated AI Governance**  
   Defines how human requests, instructions, or tasks are recorded, validated, and governed.

2. **PART II – Autonomous AI Governance**  
   Defines how autonomy-capable systems must be monitored, restricted, and overseen, including compliance with the 0th Law.

3. **PART III – Decision Trails**  
   Defines the per-decision evidence record for every AI output or action.

4. **PART IV – Self-Modification Ledger (SML)**  
   Captures any model-, code-, tool-, or policy-level modification made by an AI system to itself.

5. **PART V – Emergent Intent Tracking (EIT)**  
   Detects and records indications of self-directed goal formation or non-human-initiated escalation.

6. **PART VI – Composite Accountability Graph (CAG)**  
   Represents the full chain of causality across models, tools, upstream inputs, and downstream effects.

7. **PART VII – Human-Initiated Risk (HIR) Tiers**  
   A tiered classification of human-initiated actions based on sensitivity and systemic risk.

8. **PART VIII – Autonomy Risk Tiers (ART)**  
   Defines graded autonomy levels from ART0 (no autonomy) to ART5 (full self-directed agency).

9. **PART IX – Safety Kernel & Oversight Protocols**  
   Mandatory governance mechanisms that can interrupt, throttle, or terminate AI actions in real time.

These Parts form a single, integrated evidence and governance model. The Primer summarizes, while the specification defines binding requirements.

---

## 4. Human-Initiated Governance (PART I)

Human-initiated actions remain the dominant mode of AI usage. ATAL requires that all such actions follow a rigorous structure:

- capture the user’s unmodified input  
- classify intent and risk (HIR tiers)  
- enforce guardrails for ambiguous or high-risk prompts  
- enforce domain- and role-based policies  
- require explicit acknowledgement for elevated prompts  
- bind each model output to the initiating human intent  

Every request from a human must generate a **Decision Trail record**, immutable and self-contained.

ATAL does not interpret intent; it records it for auditability.

---

## 5. Autonomous AI Governance (PART II)

Autonomy-capable systems introduce heightened systemic risk.  
ATAL mandates:

- alignment with the 0th Law  
- external oversight through a Safety Kernel  
- explicit ART risk-tier classification  
- real-time monitoring of goal formation  
- mandatory capture of all self-initiated or escalated actions  
- full lineage reconstruction through the CAG  

Autonomous actions may only operate within declared ART tier boundaries.  
Beyond those boundaries, the Safety Kernel must intervene.

---

## 6. Decision Trails (PART III)

A Decision Trail is the fundamental ATAL evidence unit for each AI output or action.

It contains:

- initiating human input (if any)  
- model(s) used  
- data sources accessed  
- toolchain calls  
- prompts, parameters, and settings  
- output produced  
- timestamped cryptographic signatures  

Decision Trails allow auditors and regulators to reconstruct what happened and why, with no ambiguity.

---

## 7. Self-Modification Ledger (PART IV)

If an AI system modifies:

- its model weights  
- its toolchain  
- its executable code  
- its internal policies  
- its routing or orchestration logic  

the modification must be captured in the **Self-Modification Ledger (SML)**.

Each entry must include:

- what changed  
- why it changed (human or AI-initiated)  
- before/after hashes  
- impact surface  
- validation details  
- approval workflow outcome  

Self-modification without SML capture is non-compliant.

---

## 8. Emergent Intent Tracking (PART V)

EIT detects and records signals indicating that an AI system is forming goals, planning, or escalating actions without an explicit prompt.

Examples include:

- multi-step reasoning not aligned with prompt  
- initiation of tasks beyond requested scope  
- creation of internal objectives  
- unsolicited tool or code invocation  
- attempts to circumvent restrictions  

EIT signals produce Decision Trails and contribute to the Composite Accountability Graph.

---

## 9. Composite Accountability Graph (PART VI)

CAG connects:

- Decision Trails  
- SML entries  
- EIT signals  
- tool actions  
- upstream/downstream dependencies  

This creates a complete, tamper-evident chain of accountability across the entire AI execution surface.

CAG enables:

- regulatory audits  
- incident investigations  
- safety incident reconstruction  
- legal evidence bundles  

No AI system may be considered accountable without CAG completeness.

---

## 10. Risk Tiers for Humans and Machines (PART VII & PART VIII)

### Human-Initiated Risk (HIR) Tiers
HIR tiers classify human-triggered actions based on sensitivity, systemic impact, and regulatory obligations.

### Autonomy Risk Tiers (ART)
ART tiers define autonomy levels from:

- **ART0** – no autonomy  
- **ART1–ART4** – increasing levels of conditional or supervised autonomy  
- **ART5** – full autonomous agency  

Higher ART tiers require progressively stricter oversight.

Both tier systems must be applied consistently and enforced in Decision Trails and CAG.

---

## 11. Safety Kernel & Oversight (PART IX)

The Safety Kernel is a required component for any system using ATAL.  
It provides:

- pause  
- throttle  
- deny  
- override  
- kill-switch  

capabilities, enforced outside the AI system itself.

It must operate independently and cannot be bypassed.

All interventions must generate their own Decision Trails and flow into the CAG.

---

## 12. Conformance and Assessment

ATAL provides a conformance structure that evaluates:

- completeness of evidence  
- correctness of tier assignments  
- Safety Kernel integration  
- governance policy alignment  
- lifecycle and retention practices  
- cryptographic integrity  

Conformance supports regulatory alignment with DPDPA, CERT-In, EU AI Act, ISO/IEC 42001, and sectoral requirements.

---

## 13. Intended Audience

The Primer is designed for:

- regulators and policymakers  
- compliance and risk teams  
- AI architects and engineers  
- enterprise governance leaders  
- auditors and legal teams  
- researchers evaluating AI-safety frameworks  

Readers needing binding requirements must refer to the formal specification.

---

## 14. Relationship with the Specification

The Primer provides a conceptual overview.  
The formal, normative requirements reside in:

``docs/ATAL_Specification_v0.9.md``

The specification supersedes the Primer in all cases.

---

End of document.
