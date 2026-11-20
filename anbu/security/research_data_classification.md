# Research Data Classification

**Module:** ANBU OSINT — Security & Operational Protection
**Classification handling:** Apply research data classification rules to all outputs produced under this procedure. All stored artifacts must carry an analyst-assigned classification label.

## 1. Purpose
Establish a consistent classification scheme for all data handled within ANBU OSINT research, ensuring that handling, storage, sharing, and disposal obligations match the sensitivity of the data. This is the labeling system that all other security procedures depend on.

## 2. Scope
All data entering the ANBU research environment: collected datasets, analyst notes, intermediate products, reports, and communications about research.

## 3. Intelligence objectives
- Assign every artifact a classification at creation or intake.
- Drive handling requirements from classification level.
- Prevent sensitive data from leaking into lower-classification outputs.
- Enable defensible disposal decisions.

## 4. Core concepts
- Four-level scheme: PUBLIC, INTERNAL, SENSITIVE, RESTRICTED.
- Classification by content, not by perceived importance: personal data, credentials, exploitation details, and pre-publication findings default upward.
- Derivative classification: reports inherit the highest classification of their inputs unless redaction justifies downgrade (documented).
- Reclassification events are logged with authority.

## 5. Analytical methodology
1. At intake or creation, assign classification per content rules.
2. When in doubt, classify upward; downgrade requires documented justification.
3. Store in the compartment matching classification.
4. At output time, verify report classification matches its content.
5. On project close, execute retention/disposal per classification schedule.

## 6. Step-by-step workflow
1. Create/intake → 2. Classify → 3. Store in compartment → 4. Handle per level rules → 5. Output review → 6. Retention/disposal per schedule. Any upward reclassification propagates to derivatives.

## 7. Data requirements
Classification criteria: contains personal identifiers (SENSITIVE minimum), contains credentials or security-sensitive operational detail (RESTRICTED), pre-publication intelligence findings (SENSITIVE+), derived from RESTRICTED sources (inherits or higher).

## 8. Approved public sources
Classification labels appear in document headers, file metadata, and storage folder structure. Search and access controls filter by classification.

## 9. Source verification standards
Automated spot-checks compare document content against assigned label; misclassified documents are corrected and the error logged. Analysts may not downgrade their own work without reviewer approval.

## 10. Analytical framework
Decision table: does the artifact contain personal data of third parties? → SENSITIVE. Does it contain credentials, exploit detail, or targeting-relevant operational information? → RESTRICTED. Is it wholly composed of already-public reporting with no added analysis? → INTERNAL at most.

## 11. Evidence requirements
Classification register per project listing every artifact, its label, classification rationale, and current location.

## 12. Confidence assessment
HIGH: automated checks + audit show consistent labeling. MODERATE: manual labeling with periodic review. LOW: inconsistent labels detected. INSUFFICIENT: no classification system in use.

## 13. Common analytical mistakes
Leaving classification to analyst discretion without criteria; failing to reclassify derivatives after source upgrade; storing RESTRICTED content in shared drives; treating classification as optional for 'internal notes.'

## 14. Ethical considerations
Classification is a safety mechanism, not bureaucracy. Under-classification is the dangerous failure mode: a RESTRICTED dataset labeled INTERNAL will be handled with insufficient controls and could cause real harm if exposed.

## 15. Security boundaries
Handling data above its labeled classification (impossible) — concretely: storing SENSITIVE data in PUBLIC-accessible locations, sharing RESTRICTED material in unencrypted channels, or downgrading without authority.

## 16. Expected output
Complete classification register, correctly labeled artifacts in correct compartments, and logged reclassification history.

## 17. Quality checklist
- [ ] Classification label applied to every artifact
- [ ] Sources are public-only and logged with access timestamps
- [ ] Third-party tools verified against vetting checklist
- [ ] Chain-of-custody or handling record complete
- [ ] Audit entry written for every material action
- [ ] Peer or reviewer sign-off recorded where required
- [ ] Classification label matches content on spot-check
- [ ] Derivatives carry correct inherited classification

## 18. Cross-reference links
- Related operational guidance: core/, legal/, verification/, reporting/ modules.
- Apply all linked procedures as a unified control set; no procedure operates in isolation.
- Deviations from this procedure require documented authority and audit-log entry.
- Mandatory policy documents in this module: privacy_by_design.md, data_minimization_protocol.md, secure_research_workflow.md, safe_public_source_handling.md, research_data_classification.md, sensitive_data_redaction.md, personal_identifier_protection.md, account_and_credential_safety.md, secure_document_storage.md, evidence_integrity_management.md, audit_log_management.md, access_control_principles.md, third_party_tool_assessment.md, malicious_content_handling.md, cyber_safety_boundaries.md, operational_security_boundaries.md, doxxing_prevention.md, surveillance_abuse_prevention.md, targeting_and_harm_prevention.md, safety_escalation_protocol.md

