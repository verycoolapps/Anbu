# Third-Party Tool Assessment

**Module:** ANBU OSINT — Security & Operational Protection
**Classification handling:** Apply research data classification rules to all outputs produced under this procedure. All stored artifacts must carry an analyst-assigned classification label.

## 1. Purpose
Provide a vetting framework for any external tool, library, service, or script proposed for use in ANBU OSINT research — ensuring that tools do not compromise researcher security, data confidentiality, evidence integrity, or legal posture before they are ever executed.

## 2. Scope
Evaluation of all non-ANBU-built software considered for research use: OSINT platforms, scraping libraries, browser extensions, API services, data providers, and analyst utilities.

## 3. Intelligence objectives
- Prevent supply-chain and tool-level compromise of research.
- Ensure tools handle data per ANBU security requirements.
- Detect tools that exfiltrate data, fingerprint researchers, or violate terms/legal boundaries.
- Maintain an approved-tools inventory with review dates.

## 4. Core concepts
- Vetting before use: no tool touches ANBU data until assessed.
- Data-flow analysis: what data does the tool receive, where does it send it, what does it retain?
- Provenance check: official source, maintainer reputation, update history, known vulnerabilities.
- Sandbox evaluation: tools run in isolated environment with test data before production use.

## 5. Analytical methodology
1. Identify tool need and candidate options.
2. Collect: official repository/release, maintainer identity, license, dependencies, telemetry disclosures.
3. Analyze data flows: inputs, outputs, network destinations, local storage.
4. Check security history: CVEs, breach reports, suspicious update patterns.
5. Sandbox test with synthetic data; monitor network and filesystem.
6. Document assessment; approve, restrict, or reject with rationale.
7. Re-assess on major version changes or annual review.

## 6. Step-by-step workflow
1. Need identified → 2. Candidate inventory → 3. Provenance + security history → 4. Data-flow analysis → 5. Sandbox test → 6. Decision recorded → 7. Approved-tools register updated → 8. Periodic re-vetting.

## 7. Data requirements
Assessment record: tool name, version, source, maintainer, license, data inputs/outputs, network destinations, telemetry, dependencies, vulnerabilities found, sandbox results, decision, restrictions, review date.

## 8. Approved public sources
Tools must access public sources only and comply with platform terms. Tools requiring credentials use dedicated research accounts per account and credential safety. Tools that require disabling security features are rejected.

## 9. Source verification standards
Verification standard: claims in tool documentation are verified against observed behavior in sandbox. Discrepancies between documented and actual data flows are treated as findings, not inconveniences.

## 10. Analytical framework
Risk matrix: data sensitivity handled × tool trustworthiness × reversibility of decision. High-sensitivity data + low-trust tool = reject or isolate. Tool handling only PUBLIC data with strong provenance may be approved with monitoring.

## 11. Evidence requirements
Approved-tools register: tool, version, approval scope, restrictions, assessment date, next review — maintained centrally; unlisted tools require assessment before use.

## 12. Confidence assessment
HIGH: full assessment with sandbox evidence, periodic re-vetting. MODERATE: assessment completed, minor gaps. LOW: tool used without assessment or assessment stale. INSUFFICIENT: no tool vetting process.

## 13. Common analytical mistakes
Installing tools from unofficial mirrors; running tools with real data before sandbox testing; ignoring telemetry disclosures; assuming open-source means safe; approving tools based on popularity alone.

## 14. Ethical considerations
A compromised tool can exfiltrate every dataset, expose researcher identity, and poison evidence — the tool layer is the highest-risk supply chain in OSINT. Vetting is not optional overhead; it is the perimeter.

## 15. Security boundaries
Using unvetted tools on classified data; disabling tool security features; approving tools that exfiltrate to unverified destinations; sharing approved-tool credentials across teams.

## 16. Expected output
Completed assessment records, approved-tools register, and sandbox test logs for each approved tool.

## 17. Quality checklist
- [ ] Classification label applied to every artifact
- [ ] Sources are public-only and logged with access timestamps
- [ ] Third-party tools verified against vetting checklist
- [ ] Chain-of-custody or handling record complete
- [ ] Audit entry written for every material action
- [ ] Peer or reviewer sign-off recorded where required
- [ ] Data-flow analysis documented
- [ ] Sandbox test completed before production use
- [ ] Review date scheduled

## 18. Cross-reference links
- Mandatory policy documents in this module: privacy_by_design.md, data_minimization_protocol.md, secure_research_workflow.md, safe_public_source_handling.md, research_data_classification.md, sensitive_data_redaction.md, personal_identifier_protection.md, account_and_credential_safety.md, secure_document_storage.md, evidence_integrity_management.md, audit_log_management.md, access_control_principles.md, third_party_tool_assessment.md, malicious_content_handling.md, cyber_safety_boundaries.md, operational_security_boundaries.md, doxxing_prevention.md, surveillance_abuse_prevention.md, targeting_and_harm_prevention.md, safety_escalation_protocol.md

