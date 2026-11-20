# Personal Identifier Protection

**Module:** ANBU OSINT — Security & Operational Protection
**Classification handling:** Apply research data classification rules to all outputs produced under this procedure. All stored artifacts must carry an analyst-assigned classification label.

## 1. Purpose
Define controls for personal identifiers encountered during OSINT research — names, handles, account IDs, government identifiers, addresses, and biometric-adjacent data — covering collection, storage, correlation, and reporting so that identifier handling never becomes a privacy or security liability.

## 2. Scope
All research touching data that can identify or contribute to identifying a natural person, whether the person is a research subject, an incidental appearance, or a source operator.

## 3. Intelligence objectives
- Protect subjects from re-identification and privacy harm.
- Protect researchers from being fingerprinted through identifier correlation.
- Preserve analytical ability to resolve entities without retaining raw identifiers in working copies.
- Support lawful, proportional research consistent with privacy obligations.

## 4. Core concepts
- Direct vs quasi-identifiers: names, IDs, account handles are direct; role+location+time combinations are quasi. Both require protection.
- Pseudonymization: replace identifiers with project-scoped tokens; keep the mapping in a RESTRICTED master index only.
- Linkability control: avoid retaining datasets that allow cross-source re-identification without analytical need.
- Incidental capture rule: identifiers appearing in bulk data but unrelated to the objective are purged at intake.

## 5. Analytical methodology
1. Detect identifiers during intake and tag by type.
2. Assign pseudonyms for working copies; log mapping in secured index.
2.1 Quasi-identifier review: check combinations that could re-identify.
3. Restrict identifier-bearing fields to minimum necessary roles.
4. Apply redaction before any output.
5. On project close, destroy mapping index per retention schedule unless legal hold applies.

## 6. Step-by-step workflow
1. Intake → 2. Identifier detection/tagging → 3. Pseudonymization → 4. Quasi-identifier check → 5. Restricted-field handling → 6. Redacted output → 7. Index destruction or legal hold.

## 7. Data requirements
Identifier types: legal names, usernames/handles, email addresses, phone numbers, government IDs, account IDs, precise locations, dates of birth, and unique behavioral signatures. Exclude nothing by default; classification decides handling.

## 8. Approved public sources
Sources as per safe public source handling; additional caution for sources whose primary content is personal data (people-search sites, leaked datasets — latter are excluded entirely as non-public or unlawfully obtained).

## 9. Source verification standards
Identifier-to-source binding must be verified: a handle attributed to a person requires evidence the account belongs to them, not merely a name match. See verification standards.

## 10. Analytical framework
Linkability assessment: for each dataset, estimate the effort required to re-identify individuals using public data. High linkability + low analytical necessity = purge or aggregate.

## 11. Evidence requirements
Identifier register tracking counts by type per project, pseudonymization coverage, and purge confirmations — without recording the identifiers themselves in the register.

## 12. Confidence assessment
HIGH: pseudonymization verified, linkability assessed, zero raw identifiers in working copies. MODERATE: pseudonymization applied, linkability informal. LOW: raw identifiers present in shared artifacts. INSUFFICIENT: no identifier handling procedure.

## 13. Common analytical mistakes
Assuming pseudonyms are anonymous; keeping the mapping index on the same system as working data; re-identifying for convenience during analysis; retaining identifiers 'for verification' beyond need.

## 14. Ethical considerations
Protecting identifiers is not about protecting the powerful — it applies equally to subjects, sources, and researchers. A source who trusts ANBU with their identity must be protected absolutely; breach of that trust endangers people.

## 15. Security boundaries
Storing raw identifier datasets outside RESTRICTED compartments; transmitting identifier lists over unencrypted channels; including identifiers in report drafts shared for comment.

## 16. Expected output
Pseudonymized working dataset, secured mapping index with access log, and destruction/preservation record.

## 17. Quality checklist
- [ ] Classification label applied to every artifact
- [ ] Sources are public-only and logged with access timestamps
- [ ] Third-party tools verified against vetting checklist
- [ ] Chain-of-custody or handling record complete
- [ ] Audit entry written for every material action
- [ ] Peer or reviewer sign-off recorded where required
- [ ] Mapping index access-logged and separated from working data
- [ ] Linkability assessment documented
- [ ] Quasi-identifier combinations reviewed

## 18. Cross-reference links
- Related operational guidance: core/, legal/, verification/, reporting/ modules.
- Mandatory policy documents in this module: privacy_by_design.md, data_minimization_protocol.md, secure_research_workflow.md, safe_public_source_handling.md, research_data_classification.md, sensitive_data_redaction.md, personal_identifier_protection.md, account_and_credential_safety.md, secure_document_storage.md, evidence_integrity_management.md, audit_log_management.md, access_control_principles.md, third_party_tool_assessment.md, malicious_content_handling.md, cyber_safety_boundaries.md, operational_security_boundaries.md, doxxing_prevention.md, surveillance_abuse_prevention.md, targeting_and_harm_prevention.md, safety_escalation_protocol.md

