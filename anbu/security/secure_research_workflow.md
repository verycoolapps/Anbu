# Secure Research Workflow

**Module:** ANBU OSINT — Security & Operational Protection
**Classification handling:** Apply research data classification rules to all outputs produced under this procedure. All stored artifacts must carry an analyst-assigned classification label.

## 1. Purpose
Define the end-to-end secure workflow for OSINT research: from tasking and planning through collection, analysis, reporting, and archival. This is the operational backbone that coordinates all security procedures in this module into one auditable pipeline.

## 2. Scope
Every ANBU research engagement regardless of size. Provides the stage gates that enforce privacy, evidence, and security controls at each phase transition.

## 3. Intelligence objectives
- Ensure no research stage bypasses security controls.
- Produce a complete, auditable record of handling for every artifact.
- Standardize handoffs between analysts, reviewers, and storage.
- Enable rapid containment when a source or dataset is compromised.

## 4. Core concepts
- Stage gating: each phase has entry and exit criteria that must be satisfied before proceeding.
- Single chain of custody: every artifact has one accountable handler per stage.
- Fail-closed design: ambiguous security states halt the workflow pending review.
- Separation of duties: collectors, analysts, and approvers are distinct roles where feasible.

## 5. Analytical methodology
1. Tasking: objective, classification, and authorization documented.
2. Planning: schema, sources, tools, and security controls selected.
3. Collection: secure channels, logged access, immediate classification.
4. Processing: isolated environment, pseudonymization, integrity hashing.
5. Analysis: access-controlled workspace, audit logging active.
6. Reporting: redaction applied, evidence citations verified.
7. Archive/Disposal: retention schedule executed, access revoked, destruction certified.

## 6. Step-by-step workflow
1. Tasking → 2. Planning → 3. Collection → 4. Processing → 5. Analysis → 6. Reporting → 7. Archive or disposal. Stage gates enforce controls; no skipping; all transitions logged.

## 7. Data requirements
Tasking authority, objective statement, classification level, approved source list, tool inventory, and retention schedule — all defined before collection begins.

## 8. Approved public sources
Public sources only, vetted per safe public source handling. Dynamic source lists are maintained per project; expired or compromised sources are removed at the planning gate.

## 9. Source verification standards
Stage-gate reviews verify that upstream controls were actually applied, not merely planned. Spot-check source provenance and classification labels at each transition.

## 10. Analytical framework
Workflow risk matrix: for each stage, identify the highest-impact failure (source compromise, data leak, tampered evidence, unauthorized access) and the control that prevents it. Controls are tested, not assumed.

## 11. Evidence requirements
A workflow ledger per project recording stage transitions, gate decisions, responsible analyst, and timestamps — the master audit record.

## 12. Confidence assessment
HIGH: all gates documented and independently verified. MODERATE: gates documented, self-verified. LOW: workflow informal with gaps. INSUFFICIENT: no defined workflow.

## 13. Common analytical mistakes
Proceeding to analysis before collection artifacts are classified; sharing working files outside the access-controlled environment; treating archival as optional; skipping disposal steps for 'convenience.'

## 14. Ethical considerations
The workflow is only as strong as its weakest stage gate. A perfectly secured collection phase undermined by an uncontrolled analyst laptop provides no real protection — controls must span the entire lifecycle.

## 15. Security boundaries
Skipping stage gates; storing artifacts outside the controlled environment at any stage; proceeding past a failed gate without documented override authority.

## 16. Expected output
A completed workflow ledger, classified dataset, verified report, and executed retention/disposal record.

## 17. Quality checklist
- [ ] Classification label applied to every artifact
- [ ] Sources are public-only and logged with access timestamps
- [ ] Third-party tools verified against vetting checklist
- [ ] Chain-of-custody or handling record complete
- [ ] Audit entry written for every material action
- [ ] Peer or reviewer sign-off recorded where required
- [ ] Every stage gate recorded with decision and authority
- [ ] No artifact outside controlled environment at any stage

## 18. Cross-reference links
- Related operational guidance: core/, legal/, verification/, reporting/ modules.
- Mandatory policy documents in this module: privacy_by_design.md, data_minimization_protocol.md, secure_research_workflow.md, safe_public_source_handling.md, research_data_classification.md, sensitive_data_redaction.md, personal_identifier_protection.md, account_and_credential_safety.md, secure_document_storage.md, evidence_integrity_management.md, audit_log_management.md, access_control_principles.md, third_party_tool_assessment.md, malicious_content_handling.md, cyber_safety_boundaries.md, operational_security_boundaries.md, doxxing_prevention.md, surveillance_abuse_prevention.md, targeting_and_harm_prevention.md, safety_escalation_protocol.md

