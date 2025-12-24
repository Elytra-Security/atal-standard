---
name: ATAL Peer Review Submission
about: Structured technical review feedback for the ATAL public review draft v0.9
title: "[Peer Review] <Short summary>"
labels: peer-review
assignees: venkatmangudi-elytra

---

body:
  - type: markdown
    attributes:
      value: |
        Thank you for participating in the public peer review of **ATAL (AI Traceability & Accountability Ledger)**.

        This issue form is intended exclusively for **technical, architectural, or governance-focused feedback** on the ATAL v0.9 public review draft.

        Submissions that are non-technical, promotional, implementation-specific, or speculative may be closed without response.

  - type: input
    id: affiliation
    attributes:
      label: Reviewer affiliation (optional)
      description: Organization, institution, or independent reviewer
      placeholder: Independent researcher / Company / Academic / Regulator
    validations:
      required: false

  - type: textarea
    id: affected_sections
    attributes:
      label: Affected document(s) and section(s)
      description: Reference specific ATAL document(s) and section numbers
      placeholder: "ATAL_Specification_v0.9.md – Part III, Section 3.2"
    validations:
      required: true

  - type: textarea
    id: concern
    attributes:
      label: Description of concern or observation
      description: Clearly describe the technical, architectural, or governance issue
    validations:
      required: true

  - type: textarea
    id: rationale
    attributes:
      label: Rationale or supporting reference
      description: Provide reasoning, prior art references, standards comparisons, or evidence
    validations:
      required: true

  - type: textarea
    id: suggestion
    attributes:
      label: Suggested clarification or change (optional)
      description: If applicable, propose alternative wording or an approach for consideration
    validations:
      required: false

  - type: checkboxes
    id: acknowledgment
    attributes:
      label: Acknowledgment
      options:
        - label: I acknowledge that ATAL is a draft standard under public review and that submission of feedback does not imply acceptance, endorsement, or obligation by the steward.
          required: true
