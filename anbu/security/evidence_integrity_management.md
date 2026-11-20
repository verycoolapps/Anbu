# Evidence Integrity Management

**Module:** ANBU OSINT — Security & Operational Protection
**Classification handling:** Apply research data classification rules to all outputs produced under this procedure. All stored artifacts must carry an analyst-assigned classification label.

## 1. Purpose
Implement chain-of-custody and integrity controls for digital evidence collected during OSINT research — ensuring that any artifact used to support an analytical conclusion can be proven unaltered from collection to presentation, with a complete handling record.

## 2. Scope
All artifacts that may support findings: source captures, screenshots, dataset exports, archived pages, communications, and derived analytical products cited as evidence.

## 3. Intelligence objectives
- Prove authenticity: evidence presented must be demonstrably the same content retrieved from the source.
- Prove integrity: no alteration between collection and use.
- Prove provenance: the chain of handling is documented end-to-end.
- Support defensibility: evidence must withstand challenge in reporting, legal, or review contexts.

## 4. Core concepts
- Chain of custody: every transfer of an evidence artifact is recorded with date, handler, purpose, and hash verification.
- Write-once preservation: original captures are never modified; analysis works on copies.
- Hash anchoring: SHA-256 (or stronger) computed at intake, re-verified at each custody transfer and at presentation.
- Context preservation: evidence must retain enough context (URL, timestamp, surrounding content) to be meaningful standalone.

## 5. Analytical methodology
1. At collection, immediately hash the artifact and record provenance metadata.
2. Store original in evidence compartment, access-restricted.
3. For any handling or transfer, verify hash matches record before and after; log the event.
4. Analysis uses working copies; originals remain untouched.
5. At presentation, re-verify hash and attach integrity statement to output.
6. Any hash mismatch: freeze artifact, open integrity incident, notify per safety escalation protocol.

## 6. Step-by-step workflow
1. Collect → 2. Hash + provenance record → 3. Evidence-compartment storage → 4. Custody transfers (hash-verified, logged) → 5. Working copies for analysis → 6. Presentation with integrity statement → 7. Archival or disposal per retention.

## 7. Data requirements
Evidence record per artifact: source URL/identifier, collection timestamp, retrieval method, SHA-256 hash, file format/size, classification, custody log entries, and context metadata.

## 8. Approved public sources
Evidence derives from public sources per safe public source handling. No evidence may be obtained through unauthorized access, deception beyond approved methods, or credential misuse.

## 9. Source verification standards
Integrity verification is mechanical: hash comparison at every custody event. Verification of content authenticity (is this really what the source showed?) uses corroboration and archived snapshots per verification standards.

## 10. Analytical framework
Custody chain completeness test: for any evidence artifact, can you produce an unbroken record from collection to final use? Any gap breaks defensibility regardless of whether the content is actually correct.

## 11. Evidence requirements
Evidence register: artifact ID, hash, provenance, classification, custody log, current holder, and status (active, archived, disposed).

## 12. Confidence assessment
HIGH: complete custody chain, hashes verified at every transfer, integrity statement on outputs. MODERATE: chain complete with minor documentation gaps. LOW: custody gaps or unverified transfers. INSUFFICIENT: no integrity controls.

## 13. Common analytical mistakes
Analyzing originals directly (risking modification); storing 'the screenshot I took' without hash or provenance; re-saving files in formats that alter content; treating email forwards as self-authenticating; custody gaps during handoffs.

## 14. Ethical considerations
Evidence integrity is a promise to the consumer of intelligence that conclusions rest on unaltered facts. Cutting corners here doesn't just weaken a report — it can cause real-world harm if a fabricated or altered 'fact' drives a decision.

## 15. Security boundaries
Presenting evidence without integrity verification; modifying originals; custody transfers without logging; using evidence obtained outside authorized methods; destroying evidence subject to legal hold.

## 16. Expected output
Evidence register with complete custody chains, hash-verified artifacts, and integrity statements attached to all evidence-dependent outputs.

## 17. Quality checklist
- [ ] Classification label applied to every artifact
- [ ] Sources are public-only and logged with access timestamps
- [ ] Third-party tools verified against vetting checklist
- [ ] Chain-of-custody or handling record complete
- [ ] Audit entry written for every material action
- [ ] Peer or reviewer sign-off recorded where required
- [ ] SHA-256 recorded at intake and re-verified at every transfer
- [ ] Custody log unbroken for every active artifact
- [ ] Integrity statement attached to outputs

## 18. Cross-reference links
- Related operational guidance: core/, legal/, verification/, reporting/ modules.
- Mandatory policy documents in this module: privacy_by_design.md, data_minimization_protocol.md, secure_research_workflow.md, safe_public_source_handling.md, research_data_classification.md, sensitive_data_redaction.md, personal_identifier_protection.md, account_and_credential_safety.md, secure_document_storage.md, evidence_integrity_management.md, audit_log_management.md, access_control_principles.md, third_party_tool_assessment.md, malicious_content_handling.md, cyber_safety_boundaries.md, operational_security_boundaries.md, doxxing_prevention.md, surveillance_abuse_prevention.md, targeting_and_harm_prevention.md, safety_escalation_protocol.md

