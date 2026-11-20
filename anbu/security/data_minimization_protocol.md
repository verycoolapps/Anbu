# Data Minimization Protocol

**Module:** ANBU OSINT — Security & Operational Protection
**Classification handling:** Apply research data classification rules to all outputs produced under this procedure. All stored artifacts must carry an analyst-assigned classification label.

## 1. Purpose
Operationalize data minimization as a repeatable protocol that forces every ANBU research task to justify each data element before collection, preventing over-collection that creates legal exposure, security risk, and ethical liability.

## 2. Scope
All ANBU research tasks that gather, store, or process data — from single-source lookups to multi-platform correlation. Applies to both personal data and sensitive operational data.

## 3. Intelligence objectives
- Reduce dataset size to the minimum analytically sufficient set.
- Lower storage, breach, and misuse risk proportionally to data volume.
- Produce faster, more defensible analytical products.
- Demonstrate compliance posture for audits and legal review.

## 4. Core concepts
- Minimum necessary: the smallest dataset that can answer the intelligence question.
- Field-level justification: each collected attribute requires a documented purpose.
- Temporal minimization: collect only the time window relevant to the objective.
- Aggregation preference: prefer aggregated or statistical forms where analytical sufficiency permits.

## 5. Analytical methodology
1. State the intelligence question in one sentence.
2. List the minimum attributes and time window needed to answer it.
3. Design collection to retrieve only those fields.
4. Delete or exclude everything collected outside the minimum at intake.
5. Verify sufficiency: if analysis stalls for missing data, request a documented scope expansion rather than silently broadening collection.

## 6. Step-by-step workflow
1. Question → 2. Minimum schema → 3. Targeted collection → 4. Intake filtering → 5. Analysis → 6. Gap-triggered documented expansion only.

## 7. Data requirements
Only fields explicitly justified in the research schema: identifiers needed for entity resolution, timestamps, source URLs, and analytical attributes. Exclude: contact details, family information, health data, and any field not traceable to the objective.

## 8. Approved public sources
Same public-source universe as secure research workflow; minimized scope often permits use of narrower, higher-quality sources instead of bulk collection.

## 9. Source verification standards
Every dataset entry must be traceable to a named public source and collection event. Fields without provenance are purged at intake.

## 10. Analytical framework
Sufficiency test: can the dataset answer the stated question? If yes, it is minimal by definition. Re-collection requires a new schema amendment, not analyst convenience.

## 11. Evidence requirements
Minimal schemas are signed off by the lead analyst before collection; deviation requires written justification logged in the audit trail.

## 12. Confidence assessment
HIGH: schema enforced by tooling and audited. MODERATE: schema documented and manually enforced. LOW: collection exceeds schema without amendment. INSUFFICIENT: no schema exists.

## 13. Common analytical mistakes
Harvesting full profiles when only employment history is needed; retaining raw dumps indefinitely; treating 'might be useful later' as justification; duplicating the same data across multiple uncoordinated stores.

## 14. Ethical considerations
Less data means less harm potential. Minimization is the primary defense against function creep — data collected for one purpose will eventually be asked to serve another, and the smaller the original collection, the safer that future request is to answer.

## 15. Security boundaries
Collection exceeding the approved schema; storage of unfiltered bulk exports; cross-project data pooling without minimization review.

## 16. Expected output
A minimal dataset meeting the intelligence objective, with intake filter log and schema compliance record.

## 17. Quality checklist
- [ ] Classification label applied to every artifact
- [ ] Sources are public-only and logged with access timestamps
- [ ] Third-party tools verified against vetting checklist
- [ ] Chain-of-custody or handling record complete
- [ ] Audit entry written for every material action
- [ ] Peer or reviewer sign-off recorded where required
- [ ] Every field has documented justification
- [ ] Unjustified fields purged at intake

## 18. Cross-reference links
- Related operational guidance: core/, legal/, verification/, reporting/ modules.
- Apply all linked procedures as a unified control set; no procedure operates in isolation.
- Deviations from this procedure require documented authority and audit-log entry.
- Mandatory policy documents in this module: privacy_by_design.md, data_minimization_protocol.md, secure_research_workflow.md, safe_public_source_handling.md, research_data_classification.md, sensitive_data_redaction.md, personal_identifier_protection.md, account_and_credential_safety.md, secure_document_storage.md, evidence_integrity_management.md, audit_log_management.md, access_control_principles.md, third_party_tool_assessment.md, malicious_content_handling.md, cyber_safety_boundaries.md, operational_security_boundaries.md, doxxing_prevention.md, surveillance_abuse_prevention.md, targeting_and_harm_prevention.md, safety_escalation_protocol.md

