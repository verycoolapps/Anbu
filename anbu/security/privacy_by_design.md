# Privacy by Design for OSINT Research

**Module:** ANBU OSINT — Security & Operational Protection
**Classification handling:** Apply research data classification rules to all outputs produced under this procedure. All stored artifacts must carry an analyst-assigned classification label.

## 1. Purpose
Embed privacy protection into the architecture of every OSINT research engagement from the outset, rather than retrofitting safeguards after collection begins. This procedure defines how ANBU researchers structure collection, storage, analysis, and reporting so that personal data of third parties is minimized, protected, and never exploited beyond legitimate intelligence objectives.

## 2. Scope
Applies to all OSINT collection, correlation, and reporting workflows, including bulk scraping, social media monitoring, entity profiling, and any research that may incidentally capture personal data. Covers researcher self-protection (OPSEC) as well as protection of individuals appearing in research data.

## 3. Intelligence objectives
- Minimize personal data captured at collection time.
- Ensure every research artifact can justify its data retention under purpose limitation.
- Prevent privacy harms to uninvolved third parties.
- Support lawful research under applicable jurisdictional privacy regimes (GDPR-class frameworks, local equivalents).

## 4. Core concepts
- Data minimization: collect only what the intelligence objective strictly requires.
- Purpose limitation: data collected for one objective must not be repurposed without documented authorization.
- Privacy by design: embed controls (anonymization, aggregation, access restriction) before data flows, not after.
- Legitimate interest test: documented assessment of research benefit versus privacy impact.

## 5. Analytical methodology
1. Define the intelligence objective and derive a minimal data schema.
2. Identify which personal-data fields are strictly required versus merely convenient.
3. Select collection and storage methods that support anonymization at earliest feasible stage.
4. Apply aggregation or pseudonymization for analytical working copies.
5. Conduct periodic privacy impact review against the original objective.

## 6. Step-by-step workflow
1. State objective → 2. Derive required fields → 3. Select tools with privacy-preserving options → 4. Collect → 5. Classify and pseudonymize → 6. Analyze → 7. Store under access control → 8. Report with redaction → 9. Archive or destroy per retention schedule.

## 7. Data requirements
Personal data only where required: public identifiers, professional roles, public statements, and data classes authorized by research data classification. Nothing collected 'just in case.'

## 8. Approved public sources
Public sources exclusively. Government open-data portals, official registries, court records, company filings, academic publications, and press reporting. Personal social media only where the subject's own public activity is the research object.

## 9. Source verification standards
Personal data claims must be traced to the original public source. Pseudonymized internal records must retain a reversible mapping only in the secured master index — never in analytical copies.

## 10. Analytical framework
Privacy-by-design decision tree: is the data necessary? → is the person a legitimate research subject? → can it be pseudonymized? → does retention have an end date? Default to exclusion when any answer is unclear.

## 11. Evidence requirements
Every dataset must carry: objective reference, classification label, collection date, source list, minimization justification, and retention deadline.

## 12. Confidence assessment
HIGH: data minimization proven by field-level schema audit and third-party review. MODERATE: minimization claimed, spot-checked. LOW: convenience-driven collection detected. INSUFFICIENT: no documented data requirements before collection.

## 13. Common analytical mistakes
Collecting entire social feeds when three posts are relevant; retaining data 'for future use'; mixing personal data into general research repositories without classification; treating de-identified data as anonymous.

## 14. Ethical considerations
Privacy rights of subjects persist regardless of data being publicly posted. Researchers must weigh proportionality: public availability is not unlimited license to aggregate and profile. Where research could cause foreseeable harm, apply targeting and harm prevention procedures.

## 15. Security boundaries
Collection beyond minimal necessary data; storage on unencrypted or uncontrolled systems; analysis of personal data unrelated to stated objectives; disclosure of third-party personal data in reports.

## 16. Expected output
A research data sheet per project: objective, data schema, classification, minimization justification, retention date, access list, and redaction decisions.

## 17. Quality checklist
- [ ] Classification label applied to every artifact
- [ ] Sources are public-only and logged with access timestamps
- [ ] Third-party tools verified against vetting checklist
- [ ] Chain-of-custody or handling record complete
- [ ] Audit entry written for every material action
- [ ] Peer or reviewer sign-off recorded where required
- [ ] Purpose limitation documented and enforced
- [ ] Retention deadline set and recorded

## 18. Cross-reference links
- Related operational guidance: core/, legal/, verification/, reporting/ modules.
- Apply all linked procedures as a unified control set; no procedure operates in isolation.
- Deviations from this procedure require documented authority and audit-log entry.
- Mandatory policy documents in this module: privacy_by_design.md, data_minimization_protocol.md, secure_research_workflow.md, safe_public_source_handling.md, research_data_classification.md, sensitive_data_redaction.md, personal_identifier_protection.md, account_and_credential_safety.md, secure_document_storage.md, evidence_integrity_management.md, audit_log_management.md, access_control_principles.md, third_party_tool_assessment.md, malicious_content_handling.md, cyber_safety_boundaries.md, operational_security_boundaries.md, doxxing_prevention.md, surveillance_abuse_prevention.md, targeting_and_harm_prevention.md, safety_escalation_protocol.md

