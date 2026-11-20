# Cyber Safety Boundaries

**Module:** ANBU OSINT — Security & Operational Protection
**Classification handling:** Apply research data classification rules to all outputs produced under this procedure. All stored artifacts must carry an analyst-assigned classification label.

## 1. Purpose
Define the hard limits on cyber activities within ANBU OSINT research — clarifying what constitutes lawful public-source research versus unauthorized access, intrusion, or cyber operations that are outside ANBU's mandate and legal authority.

## 2. Scope
All research activities with a cyber dimension: infrastructure analysis, vulnerability research, threat actor tracking, technical attribution, and any activity touching systems beyond passive observation of public data.

## 3. Intelligence objectives
- Keep ANBU research strictly within lawful, passive, public-source bounds.
- Prevent mission creep from OSINT into unauthorized intrusion or exploitation.
- Protect researchers from legal liability and operational risk.
- Maintain clear escalation path when research reveals active threats requiring response beyond ANBU's mandate.

## 4. Core concepts
- Passive vs active distinction: observing publicly accessible data is research; probing, scanning, exploiting, or accessing non-public systems is not.
- No unauthorized access: ANBU never accesses systems, accounts, or data without authorization, regardless of how obtained credentials or vulnerabilities may appear.
- Vulnerability research boundary: identifying vulnerabilities in public software for defensive purposes is permitted with documentation; weaponization or exploitation is not.
- Attribution caution: technical indicators support assessment, not accusation; confidence language per verification standards.

## 5. Analytical methodology
1. Classify the activity: passive observation, active probing, or unauthorized access attempt.
2. Passive public-source analysis proceeds normally.
3. Any activity beyond passive observation requires explicit authorization review per legal and operational security boundaries.
4. Vulnerability findings are documented defensively and reported through appropriate channels.
5. Active threat discoveries (ongoing attacks, victim data exposure) trigger safety escalation protocol, not independent response.

## 6. Step-by-step workflow
1. Activity classification → 2. Passive: proceed → 3. Beyond passive: authorization gate → 4. Documentation → 5. Escalation for active threats → 6. Legal review where required.

## 7. Data requirements
Technical indicators (IPs, domains, hashes, infrastructure mappings), passive DNS/certificate transparency data, public vulnerability disclosures, and threat-actor TTP descriptions from public reporting. Excludes: scan results from unauthorized probing, exploited access, intercepted communications.

## 8. Approved public sources
Passive data sources only: certificate transparency logs, public DNS records, passive DNS databases, public vulnerability databases, threat intelligence feeds from public reporting, and platform-provided transparency data.

## 9. Source verification standards
Technical claims require corroboration from multiple independent passive sources. Single-indicator attribution is LOW confidence by default; see verification standards.

## 10. Analytical framework
Activity decision tree: is the data publicly accessible without authentication? → passive OK. Does obtaining it require probing, scanning, credential use, or exploiting a vulnerability? → stop, authorization review required. Is it another party's private data or systems? → outside ANBU mandate, escalate.

## 11. Evidence requirements
Activity log distinguishing passive research from any gated activities, with authorization references for the latter.

## 12. Confidence assessment
HIGH: all activities demonstrably passive and public-source; boundaries documented. MODERATE: minor ambiguities resolved with documented reasoning. LOW: activity beyond passive without authorization. INSUFFICIENT: no boundary awareness.

## 13. Common analytical mistakes
Port scanning 'just to see'; testing credentials found in datasets; accessing exposed databases 'to check contents'; assuming 'it's public anyway' justifies active probing; treating vulnerability discovery as license to exploit.

## 14. Ethical considerations
OSINT research observes; it does not act. The moment research becomes interaction with target systems — even 'harmless' probing — it crosses from intelligence into operations, with different legal authority, different risk, and different accountability. ANBU's mandate ends at observation.

## 15. Security boundaries
Active scanning or probing; credential testing; accessing non-public data; exploiting vulnerabilities; intercepting communications; any action affecting target systems or data.

## 16. Expected output
Passive technical assessments, public-source infrastructure mapping, vulnerability documentation for defensive reporting, and escalated notifications for active threats.

## 17. Quality checklist
- [ ] Classification label applied to every artifact
- [ ] Sources are public-only and logged with access timestamps
- [ ] Third-party tools verified against vetting checklist
- [ ] Chain-of-custody or handling record complete
- [ ] Audit entry written for every material action
- [ ] Peer or reviewer sign-off recorded where required
- [ ] All activities classified passive vs gated
- [ ] No unauthorized access of any kind
- [ ] Vulnerability findings documented defensively

## 18. Cross-reference links
- Related operational guidance: core/, legal/, verification/, reporting/ modules.
- Apply all linked procedures as a unified control set; no procedure operates in isolation.
- Mandatory policy documents in this module: privacy_by_design.md, data_minimization_protocol.md, secure_research_workflow.md, safe_public_source_handling.md, research_data_classification.md, sensitive_data_redaction.md, personal_identifier_protection.md, account_and_credential_safety.md, secure_document_storage.md, evidence_integrity_management.md, audit_log_management.md, access_control_principles.md, third_party_tool_assessment.md, malicious_content_handling.md, cyber_safety_boundaries.md, operational_security_boundaries.md, doxxing_prevention.md, surveillance_abuse_prevention.md, targeting_and_harm_prevention.md, safety_escalation_protocol.md

