# Secure Document Storage

**Module:** ANBU OSINT — Security & Operational Protection
**Classification handling:** Apply research data classification rules to all outputs produced under this procedure. All stored artifacts must carry an analyst-assigned classification label.

## 1. Purpose
Define storage requirements for all ANBU research artifacts — datasets, notes, reports, evidence files, and working documents — ensuring confidentiality, integrity, availability, and classification-appropriate access control throughout the retention period.

## 2. Scope
All research artifacts from intake through disposal. Covers local storage, network shares, cloud storage used for research, removable media, and backup systems.

## 3. Intelligence objectives
- Protect artifact confidentiality per classification level.
- Guarantee artifact integrity (no silent modification) via hashing and access control.
- Ensure availability to authorized analysts while denying access to unauthorized parties.
- Support auditable disposal with certified destruction.

## 4. Core concepts
- Compartmented storage: storage location matches classification; RESTRICTED never co-locates with lower classifications in shared systems.
- Encryption at rest and in transit for SENSITIVE and above.
- Integrity anchoring: cryptographic hashes recorded at intake for evidence-bearing artifacts.
- No unmanaged copies: working copies outside the storage system require documented justification and equivalent controls.

## 5. Analytical methodology
1. On creation/intake, classify and select storage compartment.
2. Encrypt per classification requirement.
3. For evidence-bearing artifacts, compute and record hash at intake.
4. Set access list matching need-to-know; log access.
5. Periodic integrity verification against recorded hashes.
6. On disposal, execute certified destruction and log.

## 6. Step-by-step workflow
1. Create → 2. Classify → 3. Compartment select → 4. Encrypt → 5. Hash if evidence → 6. Access-list set → 7. Access logging active → 8. Integrity checks periodic → 9. Disposal per schedule.

## 7. Data requirements
Storage metadata: classification, owner, access list, encryption status, hash (if evidence), retention deadline, location. Content stored per classification rules — this document governs the container, not the content schema.

## 8. Approved public sources
Approved storage: organization-controlled encrypted storage with access logging. Personal cloud accounts, unencrypted removable media, and consumer sync folders are prohibited for SENSITIVE+ data.

## 9. Source verification standards
Integrity verification: periodic hash re-computation compared to intake record; mismatches trigger evidence integrity management incident procedure and freeze of affected artifacts.

## 10. Analytical framework
Storage decision matrix: classification → required encryption → required access logging → permitted media. Any artifact not fitting a matrix cell is stored as RESTRICTED by default.

## 11. Evidence requirements
Storage register per project: artifact inventory with classification, location, hash status, access list, and retention deadline.

## 12. Confidence assessment
HIGH: full compartmenting, encryption verified, hashes verified periodically. MODERATE: compartmenting applied, encryption present, hash checks informal. LOW: mixed-classification storage or missing encryption. INSUFFICIENT: no storage controls.

## 13. Common analytical mistakes
Storing everything on one share regardless of classification; relying on 'the folder is private'; skipping hashes for 'non-evidence' data that later becomes evidence; indefinite retention 'just in case.'

## 14. Ethical considerations
Storage security failures harm not only the organization but sources and subjects whose data is exposed. The storage decision is an ethical decision: where data lives determines who can be harmed if it leaks.

## 15. Security boundaries
Storing RESTRICTED data on personal devices or consumer cloud; disabling encryption for convenience; granting broad access 'temporarily'; retaining data past disposal date.

## 16. Expected output
Classified, compartmented, encrypted storage with integrity hashes, access logs, and executed disposal records.

## 17. Quality checklist
- [ ] Classification label applied to every artifact
- [ ] Sources are public-only and logged with access timestamps
- [ ] Third-party tools verified against vetting checklist
- [ ] Chain-of-custody or handling record complete
- [ ] Audit entry written for every material action
- [ ] Peer or reviewer sign-off recorded where required
- [ ] Every artifact in correct compartment per classification
- [ ] Encryption verified for SENSITIVE+
- [ ] Hash verification current for evidence artifacts

## 18. Cross-reference links
- Related operational guidance: core/, legal/, verification/, reporting/ modules.
- Mandatory policy documents in this module: privacy_by_design.md, data_minimization_protocol.md, secure_research_workflow.md, safe_public_source_handling.md, research_data_classification.md, sensitive_data_redaction.md, personal_identifier_protection.md, account_and_credential_safety.md, secure_document_storage.md, evidence_integrity_management.md, audit_log_management.md, access_control_principles.md, third_party_tool_assessment.md, malicious_content_handling.md, cyber_safety_boundaries.md, operational_security_boundaries.md, doxxing_prevention.md, surveillance_abuse_prevention.md, targeting_and_harm_prevention.md, safety_escalation_protocol.md

