# Doxxing Prevention

**Module:** ANBU OSINT — Security & Operational Protection
**Classification handling:** Apply research data classification rules to all outputs produced under this procedure. All stored artifacts must carry an analyst-assigned classification label.

## 1. Purpose
Prevent the unauthorized collection and publication of private identifying information about any person — whether a research subject, a source, a colleague, or the researcher — through research activities, analytical products, or reporting.

## 2. Scope
All research outputs, analytical working files, reports, and communications that could contain or enable assembly of private identifying information (doxxing material).

## 3. Intelligence objectives
- Prevent harm to individuals from exposure of private data.
- Prevent ANBU from becoming a doxxing vector, wittingly or not.
- Protect sources whose identities must remain confidential for safety.
- Ensure that 'research findings' never become weapons.

## 4. Core concepts
- Doxxing definition boundary: aggregating and publishing private identifiers (home address, family details, private contact info, sensitive personal data) to enable harassment or harm is prohibited categorically.
- Public-figure vs private-individual distinction: public figures may be legitimate research subjects for their public roles; private individuals appearing incidentally receive maximum protection.
- Source protection: identities of sources are protected absolutely unless the source consents to disclosure and disclosure serves the objective.
- Assembly risk: individually public data points can become doxxing material when aggregated with intent or effect of exposure.

## 5. Analytical methodology
1. Screen all outputs for private identifying information before release.
2. Apply personal identifier protection and sensitive data redaction procedures.
3. For source identities, apply source-protection rules: pseudonymize unless consent documented.
4. For private individuals incidentally captured, purge unrelated personal data at intake per data minimization.
5. Verify no output enables re-identification of protected persons (linkability test).
6. Document decisions in redaction manifest.

## 6. Step-by-step workflow
1. Output screening → 2. Identifier scan → 3. Redaction/pseudonymization → 4. Linkability check → 5. Verification → 6. Manifest → 7. Release only after clearance.

## 7. Data requirements
Doxxing-risk indicators: home addresses, private phone numbers, family member identities, private email addresses, financial data, health information, precise daily routines, and any combination enabling physical location or harassment.

## 8. Approved public sources
All outputs destined for distribution, publication, or sharing outside the immediate analysis team. Internal analytical files are covered by personal identifier protection but doxxing review is mandatory before any external release.

## 9. Source verification standards
Verification standard: before release, a reviewer specifically checks 'could this output be used to find and harm a private person?' This is a distinct check from general redaction — it asks about harm potential, not just identifier presence.

## 10. Analytical framework
Harm-potential test: (a) Does the output identify a private individual? (b) Does it reveal private information not already widely public? (c) Could it enable harassment, stalking, or physical harm? Any yes beyond justified public-interest reporting → block or redact.

## 11. Evidence requirements
Doxxing review record: output identifier, reviewer, findings, redactions applied, and clearance decision — retained with the redaction manifest.

## 12. Confidence assessment
HIGH: doxxing review completed, linkability tested, sources protected. MODERATE: review completed with minor gaps. LOW: review skipped or linkability untested. INSUFFICIENT: no doxxing prevention.

## 13. Common analytical mistakes
Publishing 'osint investigations' that assemble home addresses and family details; treating 'it's all public info' as justification for aggregation-for-exposure; exposing sources to protect a narrative; doxxing 'in the public interest' without legal review.

## 14. Ethical considerations
Doxxing is never a research method. Information that could harm a private person is excluded regardless of how it was obtained or how interesting it is. The public's right to know has limits that private individuals' right to safety does not.

## 15. Security boundaries
Publishing or distributing identifying information enabling harm; aggregating private data for exposure; revealing source identities without consent; 'exposés' targeting private individuals.

## 16. Expected output
Doxxing-reviewed outputs with manifests, source-identity protection records, and blocked-content records where applicable.

## 17. Quality checklist
- [ ] Classification label applied to every artifact
- [ ] Sources are public-only and logged with access timestamps
- [ ] Third-party tools verified against vetting checklist
- [ ] Chain-of-custody or handling record complete
- [ ] Audit entry written for every material action
- [ ] Peer or reviewer sign-off recorded where required
- [ ] Doxxing-specific review distinct from general redaction
- [ ] Source identities protected unless documented consent
- [ ] Linkability test passed

## 18. Cross-reference links
- Related operational guidance: core/, legal/, verification/, reporting/ modules.
- Mandatory policy documents in this module: privacy_by_design.md, data_minimization_protocol.md, secure_research_workflow.md, safe_public_source_handling.md, research_data_classification.md, sensitive_data_redaction.md, personal_identifier_protection.md, account_and_credential_safety.md, secure_document_storage.md, evidence_integrity_management.md, audit_log_management.md, access_control_principles.md, third_party_tool_assessment.md, malicious_content_handling.md, cyber_safety_boundaries.md, operational_security_boundaries.md, doxxing_prevention.md, surveillance_abuse_prevention.md, targeting_and_harm_prevention.md, safety_escalation_protocol.md

