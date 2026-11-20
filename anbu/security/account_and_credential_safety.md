# Account and Credential Safety

**Module:** ANBU OSINT — Security & Operational Protection
**Classification handling:** Apply research data classification rules to all outputs produced under this procedure. All stored artifacts must carry an analyst-assigned classification label.

## 1. Purpose
Establish strict controls for any accounts, credentials, API keys, and authentication material used or encountered in OSINT research — preventing credential compromise, account takeover, researcher attribution, and accidental exposure of secrets in artifacts.

## 2. Scope
All research requiring authenticated access to platforms (public-registration accounts), API keys for approved services, stored credentials for source access, and any credentials encountered in collected data.

## 3. Intelligence objectives
- Prevent credential theft from compromising research or researcher identity.
- Prevent collected credentials (e.g., from breached-data exposure) from being used or retained inappropriately.
- Enable secure, auditable credential lifecycle: creation, use, rotation, revocation, destruction.
- Ensure credentials never appear in reports, logs, or shared artifacts.

## 4. Core concepts
- Dedicated research accounts: never use personal accounts for OSINT collection.
- Credential segregation: research credentials stored only in approved secret stores, never in notes, code, or documents.
- No credential testing: encountering credentials in data does not authorize validation attempts against live systems.
- Rotation discipline: credentials rotated on schedule and immediately on suspected exposure.

## 5. Analytical methodology
1. Provision dedicated research accounts per platform policy.
2. Store credentials in approved secret manager; reference by alias only.
3. Use per-project API keys with minimal scope and quotas.
4. Scan all outputs for accidental credential leakage before distribution.
5. Rotate on schedule; revoke immediately on exposure suspicion.
6. Log credential lifecycle events (creation, use context, rotation, revocation) — never the credential values.

## 6. Step-by-step workflow
1. Provision → 2. Secret-store registration → 3. Scoped use → 4. Output leakage scan → 5. Rotation/revocation → 6. Lifecycle log. Encountered third-party credentials: document provenance, do not use, escalate per safety escalation protocol if exposure risk exists.

## 7. Data requirements
Account identifiers, platform terms status, secret-store references (not values), API scopes, rotation dates, and usage context. Third-party credentials encountered in data are recorded by provenance only — never validated, never used.

## 8. Approved public sources
Only platforms permitting registered research access within their terms. API services with published, legitimate access programs. No credential sharing, no account rental, no access via compromised credentials.

## 9. Source verification standards
Credential exposure events are treated as security incidents: immediate rotation, impact assessment (what was accessed with the credential), and audit log entry.

## 10. Analytical framework
Exposure triage: was the credential value ever written to an artifact, log, or message? → if yes, assume compromise → rotate → assess access logs → document. Encounters of third-party credentials in datasets trigger doxxing/targeting review before any handling.

## 11. Evidence requirements
Credential inventory: alias, platform, scope, creation date, last rotation, custodian, and status — maintained in secret store metadata, not in research documents.

## 12. Confidence assessment
HIGH: zero credential values in any artifact; rotation current; inventory complete. MODERATE: minor gaps in rotation logs. LOW: credentials stored outside secret store or stale rotations. INSUFFICIENT: no credential management.

## 13. Common analytical mistakes
Reusing personal credentials for research; pasting API keys into scripts committed to shared repos; 'testing' found credentials; assuming a private repo makes embedded secrets safe.

## 14. Ethical considerations
Credentials are both a security asset and an attribution risk. Using a personal account for collection can expose the researcher and endanger sources who interacted with that account. Dedicated, compartmented identities are an ethical obligation, not just OPSEC.

## 15. Security boundaries
Credential use outside approved scope; storing secrets in documents, tickets, or chat; validating third-party credentials against live systems; sharing accounts between analysts without access logging.

## 16. Expected output
Credential inventory with zero exposed values, rotation log, and incident record for any exposure event.

## 17. Quality checklist
- [ ] Classification label applied to every artifact
- [ ] Sources are public-only and logged with access timestamps
- [ ] Third-party tools verified against vetting checklist
- [ ] Chain-of-custody or handling record complete
- [ ] Audit entry written for every material action
- [ ] Peer or reviewer sign-off recorded where required
- [ ] Automated scan confirms no credential values in artifacts
- [ ] All rotations current
- [ ] Third-party credentials encountered: documented, unused, escalated as required

## 18. Cross-reference links
- Related operational guidance: core/, legal/, verification/, reporting/ modules.
- Mandatory policy documents in this module: privacy_by_design.md, data_minimization_protocol.md, secure_research_workflow.md, safe_public_source_handling.md, research_data_classification.md, sensitive_data_redaction.md, personal_identifier_protection.md, account_and_credential_safety.md, secure_document_storage.md, evidence_integrity_management.md, audit_log_management.md, access_control_principles.md, third_party_tool_assessment.md, malicious_content_handling.md, cyber_safety_boundaries.md, operational_security_boundaries.md, doxxing_prevention.md, surveillance_abuse_prevention.md, targeting_and_harm_prevention.md, safety_escalation_protocol.md

