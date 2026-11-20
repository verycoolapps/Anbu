# Sensitive Data Redaction

**Module:** ANBU OSINT — Security & Operational Protection
**Classification handling:** Apply research data classification rules to all outputs produced under this procedure. All stored artifacts must carry an analyst-assigned classification label.

## 1. Purpose
Provide the procedures for identifying and removing sensitive information from research outputs before they leave the controlled environment — in reports, shared datasets, screenshots, and communications — while preserving analytical utility and evidentiary value.

## 2. Scope
All research outputs that will be shared, published, archived outside the controlled environment, or transmitted to any party not cleared for the source classification.

## 3. Intelligence objectives
- Remove personal identifiers and sensitive details not required by the consumer of the output.
- Preserve evidentiary integrity: redaction must not alter the meaning or authenticity of retained content.
- Maintain a redaction log so that authorized reviewers can verify what was removed and why.
- Prevent accidental exposure of credentials, internal identifiers, or security-sensitive operational details.

## 4. Core concepts
- Redact by default, reveal by exception: every output assumes sensitive content must be removed unless specifically required.
- Redaction types: direct identifiers (names, IDs, handles), quasi-identifiers (combinations enabling re-identification), sensitive attributes, credentials, internal metadata, geolocation detail.
- Reversible vs irreversible: irreversible redaction for external outputs; reversible only inside the controlled environment with logged authority.
- Screenshot discipline: images may contain more than intended — full-frame review before any sharing.

## 5. Analytical methodology
1. Identify output's classification and consumer's clearance.
2. Scan for sensitive categories per personal identifier protection and research data classification.
3. Apply redaction, preserving context needed for the analytical claim.
4. Log every redaction: what, why, authority.
5. Independent verification pass by second analyst.
6. Record final output classification and distribution list.

## 6. Step-by-step workflow
1. Determine clearance → 2. Sensitive-content scan → 3. Redaction → 4. Redaction log → 5. Verification → 6. Distribution with classification header → 7. Archive redaction record with source artifact.

## 7. Data requirements
Personal names/handles, national IDs, precise addresses, contact details, health/financial data, credentials and tokens, internal case identifiers, geolocation at sensitive precision, and any third-party data not required by the report's purpose.

## 8. Approved public sources
Redaction applies to all output formats: documents, spreadsheets, images, slide decks, data exports, and code/scripts that may embed identifiers.

## 9. Source verification standards
Verification standard: a second analyst must confirm (a) no unredacted sensitive content remains and (b) retained content still supports the analytical claims. Redacted items are checked against the redaction log for completeness.

## 10. Analytical framework
Re-identification test: could a determined reader combine retained quasi-identifiers with public data to identify a person? If yes, further aggregation or removal is required before release.

## 11. Evidence requirements
Each redacted output ships with a redaction manifest: items removed, category, justification, and verifier identity — stored with the artifact, not distributed.

## 12. Confidence assessment
HIGH: double-verified with documented redaction manifest. MODERATE: verified once, manifest kept. LOW: redaction unverified or manifest incomplete. INSUFFICIENT: no redaction performed or logged.

## 13. Common analytical mistakes
Redacting names but leaving unique combinations of role+location+event that re-identify; blurring screenshots incompletely; removing content that breaks evidentiary context; failing to redact file metadata.

## 14. Ethical considerations
Redaction is not deletion of inconvenient facts — it is precision removal of unnecessary personal exposure. Over-redaction that destroys evidentiary value is also a failure: the goal is minimal necessary exposure, not minimal information.

## 15. Security boundaries
Distributing unredacted or partially redacted material; redacting without logging; reversible redaction on external outputs; metadata leakage through 'anonymized' exports.

## 16. Expected output
A released output with complete redaction manifest and verification record, plus the classified master retained internally.

## 17. Quality checklist
- [ ] Classification label applied to every artifact
- [ ] Sources are public-only and logged with access timestamps
- [ ] Third-party tools verified against vetting checklist
- [ ] Chain-of-custody or handling record complete
- [ ] Audit entry written for every material action
- [ ] Peer or reviewer sign-off recorded where required
- [ ] Redaction manifest complete and stored internally
- [ ] Second-analyst verification recorded
- [ ] File metadata and image edges checked

## 18. Cross-reference links
- Related operational guidance: core/, legal/, verification/, reporting/ modules.
- Mandatory policy documents in this module: privacy_by_design.md, data_minimization_protocol.md, secure_research_workflow.md, safe_public_source_handling.md, research_data_classification.md, sensitive_data_redaction.md, personal_identifier_protection.md, account_and_credential_safety.md, secure_document_storage.md, evidence_integrity_management.md, audit_log_management.md, access_control_principles.md, third_party_tool_assessment.md, malicious_content_handling.md, cyber_safety_boundaries.md, operational_security_boundaries.md, doxxing_prevention.md, surveillance_abuse_prevention.md, targeting_and_harm_prevention.md, safety_escalation_protocol.md

