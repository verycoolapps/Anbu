# Malicious Content Handling

**Module:** ANBU OSINT — Security & Operational Protection
**Classification handling:** Apply research data classification rules to all outputs produced under this procedure. All stored artifacts must carry an analyst-assigned classification label.

## 1. Purpose
Define procedures for encountering hostile or weaponized content during OSINT research — booby-trapped documents, tracking pixels, exploit-laden files, disinformation payloads, and honeypots — ensuring researcher safety and preventing content from contaminating analysis or systems.

## 2. Scope
All collected content that may be hostile: documents, images, archives, executables, scripts, web pages, and messages from untrusted sources.

## 3. Intelligence objectives
- Protect researcher systems and identity from payloads.
- Prevent malicious content from reaching analysts or production systems.
- Preserve evidence value of hostile content when it is itself the research subject.
- Detect and document attacks for threat awareness.

## 4. Core concepts
- Assume hostile: all external content is untrusted until inspected.
- Quarantine before analysis: suspicious content goes to isolated environment, never opened on production systems.
- Content-type verification: file extensions and claimed types are verified against actual content.
- No execution: collected executables, macros, and scripts are never run on research systems.

## 5. Analytical methodology
1. Flag suspicious content at intake (unexpected types, executable attachments, archive-within-archive, known-bad indicators).
2. Quarantine in isolated environment.
3. Static inspection: file type, embedded objects, scripts, metadata, known-malware signatures.
4. If content is evidence, preserve per evidence integrity management; analysis proceeds on sanitized copies.
5. Document the threat: type, vector, indicators, and whether researcher exposure occurred.
6. Report per safety escalation protocol if active compromise suspected.

## 6. Step-by-step workflow
1. Intake flag → 2. Quarantine → 3. Static analysis → 4. Sanitized copy for analysis (if needed) → 5. Threat documentation → 6. Escalation if compromise → 7. Disposal of malicious originals per secure destruction.

## 7. Data requirements
Threat indicators: file hashes, content type mismatches, embedded scripts, known-bad domains, social-engineering lures, canary tokens. Exposure records: whether content was opened, executed, or transmitted.

## 8. Approved public sources
Malicious content is still evidence when it documents an operation — but it is handled exclusively in quarantine with sanitized derivatives for analysis. No exceptions.

## 9. Source verification standards
Verification of 'clean' status requires static analysis tools, not just antivirus scan. AV miss does not equal safe; novel or targeted content may evade signature detection.

## 10. Analytical framework
Risk classification: passive content (tracking pixels, fingerprinting scripts) vs active payloads (exploits, malware) vs social engineering (lures). Each triggers different containment: passive → block and document; active → isolate and escalate; social → warn personnel.

## 11. Evidence requirements
Threat log per incident: content description, indicators, containment actions, exposure assessment, and resolution.

## 12. Confidence assessment
HIGH: quarantine enforced, static analysis documented, zero exposure incidents. MODERATE: quarantine with minor process gaps. LOW: content opened before inspection. INSUFFICIENT: no malicious content procedure.

## 13. Common analytical mistakes
Opening attachments to 'see what they are'; previewing documents on production machines; disabling security warnings to view content; assuming archived content is safe; forwarding suspicious content to colleagues.

## 14. Ethical considerations
Malicious content may be deliberately planted to identify researchers, compromise systems, or manipulate analysis. Handling it safely is both self-protection and intelligence: the attack itself may be the finding.

## 15. Security boundaries
Opening uninspected content; executing or previewing suspicious files; disabling security features to view content; storing live malware outside quarantine; failing to report suspected compromise.

## 16. Expected output
Quarantined artifacts with analysis records, sanitized derivatives, threat documentation, and escalation records where applicable.

## 17. Quality checklist
- [ ] Classification label applied to every artifact
- [ ] Sources are public-only and logged with access timestamps
- [ ] Third-party tools verified against vetting checklist
- [ ] Chain-of-custody or handling record complete
- [ ] Audit entry written for every material action
- [ ] Peer or reviewer sign-off recorded where required
- [ ] All suspicious content quarantined before inspection
- [ ] No execution of collected binaries or macros
- [ ] Threat indicators documented

## 18. Cross-reference links
- Related operational guidance: core/, legal/, verification/, reporting/ modules.
- Mandatory policy documents in this module: privacy_by_design.md, data_minimization_protocol.md, secure_research_workflow.md, safe_public_source_handling.md, research_data_classification.md, sensitive_data_redaction.md, personal_identifier_protection.md, account_and_credential_safety.md, secure_document_storage.md, evidence_integrity_management.md, audit_log_management.md, access_control_principles.md, third_party_tool_assessment.md, malicious_content_handling.md, cyber_safety_boundaries.md, operational_security_boundaries.md, doxxing_prevention.md, surveillance_abuse_prevention.md, targeting_and_harm_prevention.md, safety_escalation_protocol.md

