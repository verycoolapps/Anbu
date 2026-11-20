# Safe Public Source Handling

**Module:** ANBU OSINT — Security & Operational Protection
**Classification handling:** Apply research data classification rules to all outputs produced under this procedure. All stored artifacts must carry an analyst-assigned classification label.

## 1. Purpose
Govern how ANBU researchers interact with public sources — websites, archives, social platforms, forums, and repositories — so that access does not expose the researcher, trigger counter-surveillance, violate platform terms in ways that create legal risk, or contaminate evidence with manipulated content.

## 2. Scope
All interactions with external public sources during collection and verification, including automated and manual access, archived content, and source-of-record retrieval.

## 3. Intelligence objectives
- Protect researcher identity and location from source operators and hostile observers.
- Preserve evidence integrity by avoiding actions that alter source state.
- Detect and flag manipulated, honeypot, or poisoned sources.
- Ensure legal access consistent with platform terms and applicable law.

## 4. Core concepts
- OPSEC for source interaction: separate research identity, controlled network egress, predictable access patterns where appropriate.
- Read-only discipline: collection must never alter source content, accounts, or systems.
- Provenance capture: record exact access conditions (URL, timestamp, method) for every retrieval.
- Adversarial source awareness: public sources may be weaponized (disinformation, canary tokens, tracking).

## 5. Analytical methodology
1. Verify source legitimacy before first interaction (see third-party tool assessment analog for sources).
2. Access via controlled channel per operational security boundaries.
3. Capture provenance metadata at retrieval time.
4. Detect anomalies: unexpected redirects, tracking parameters, content requiring interaction.
5. Quarantine suspicious content per malicious content handling before analysis.
6. Log all access in audit log.

## 6. Step-by-step workflow
1. Source vetting → 2. Controlled access → 3. Retrieval with provenance → 4. Anomaly detection → 5. Quarantine if needed → 6. Classification and storage → 7. Periodic re-verification of source integrity.

## 7. Data requirements
Public source URLs, access timestamps, retrieval method, content hash, and contextual metadata (platform, account, language, region). For accounts used for access, credential references per account and credential safety — never credentials themselves.

## 8. Approved public sources
Public registries, news archives, government open data, academic sources, platform public pages, Internet Archive/Wayback Machine, public court and corporate filings. Excluded: sources requiring authentication beyond public registration, paywalled content accessed via credential sharing, or sources of unclear legality.

## 9. Source verification standards
Source trust tiers: authoritative (official records), reputable (established outlets), community (forums/social), unverified (anonymous claims). Every citation carries its tier; conclusions weight sources accordingly.

## 10. Analytical framework
Threat model for sources: who operates this source, what do they gain from our attention, can they fingerprint us, is content consistent with independent sources? Unanswered questions lower source confidence.

## 11. Evidence requirements
Every retrieved artifact carries provenance record: URL, timestamp, hash, retrieval method, access identity tier, and any anomalies observed.

## 12. Confidence assessment
HIGH: provenance complete, source tier assigned, anomalies investigated. MODERATE: provenance complete, minor gaps. LOW: provenance incomplete or anomalies unexplained. INSUFFICIENT: sources undocumented.

## 13. Common analytical mistakes
Clicking shortened URLs without expansion review; logging into third-party platforms with real identity; trusting a single archive snapshot without corroboration; ignoring redirect chains that leak referrer data.

## 14. Ethical considerations
Public does not mean safe. Source operators may be hostile, sources may be compromised, and even passive access can be fingerprinted. Ethical duty includes not harming source operators through aggressive scraping that degrades service.

## 15. Security boundaries
Authentication with real personal identity on research platforms; clicking unknown links directly; downloading executable or macro content from sources; storing source credentials in research notes.

## 16. Expected output
Source log with vetted entries, retrieval records, anomaly reports, and periodic source-integrity review.

## 17. Quality checklist
- [ ] Classification label applied to every artifact
- [ ] Sources are public-only and logged with access timestamps
- [ ] Third-party tools verified against vetting checklist
- [ ] Chain-of-custody or handling record complete
- [ ] Audit entry written for every material action
- [ ] Peer or reviewer sign-off recorded where required
- [ ] Provenance record complete for every artifact
- [ ] Source trust tier assigned

## 18. Cross-reference links
- Related operational guidance: core/, legal/, verification/, reporting/ modules.
- Apply all linked procedures as a unified control set; no procedure operates in isolation.
- Mandatory policy documents in this module: privacy_by_design.md, data_minimization_protocol.md, secure_research_workflow.md, safe_public_source_handling.md, research_data_classification.md, sensitive_data_redaction.md, personal_identifier_protection.md, account_and_credential_safety.md, secure_document_storage.md, evidence_integrity_management.md, audit_log_management.md, access_control_principles.md, third_party_tool_assessment.md, malicious_content_handling.md, cyber_safety_boundaries.md, operational_security_boundaries.md, doxxing_prevention.md, surveillance_abuse_prevention.md, targeting_and_harm_prevention.md, safety_escalation_protocol.md

