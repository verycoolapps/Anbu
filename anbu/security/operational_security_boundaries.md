# Operational Security Boundaries

**Module:** ANBU OSINT — Security & Operational Protection
**Classification handling:** Apply research data classification rules to all outputs produced under this procedure. All stored artifacts must carry an analyst-assigned classification label.

## 1. Purpose
Define the operational security (OPSEC) perimeter for ANBU researchers — the practices that protect researcher identity, location, associations, and methods from hostile observation, whether by source operators, threat actors, or adversarial intelligence services.

## 2. Scope
All personnel conducting OSINT research, including their digital footprint, communications, equipment, travel patterns relevant to research, and associations revealed through research activity.

## 3. Intelligence objectives
- Prevent researcher attribution by hostile actors monitoring public sources.
- Prevent correlation of research activity across projects and identities.
- Protect sources who interact with researchers.
- Reduce physical and digital risk to personnel.

## 4. Core concepts
- Identity separation: research identities are distinct from personal identity; compartmented per project risk.
- Network hygiene: controlled egress, no personal accounts on research systems, predictable-but-not-identifying access patterns.
- Device and account hygiene: dedicated devices or hardened configurations for sensitive work; MFA everywhere; no personal app ecosystems on research machines.
- Association control: limit who knows which researcher works on which project; need-to-know applies to personnel too.

## 5. Analytical methodology
1. Assess project threat level: who might monitor this research and why.
2. Select identity compartment and technical controls accordingly.
3. Provision dedicated accounts/devices per compartment.
4. Conduct all source interaction through controlled channels.
5. Periodic OPSEC review: check for exposure (breach corpora, public records linking identities).
6. On suspected compromise, rotate identities and assess exposure per safety escalation protocol.

## 6. Step-by-step workflow
1. Threat assessment → 2. Compartment selection → 3. Provisioning → 4. Controlled operations → 5. Periodic exposure review → 6. Rotation on trigger → 7. Documentation of OPSEC decisions (not the identities themselves in shared docs).

## 7. Data requirements
OPSEC plan per project: threat actors considered, identity compartments used, technical controls, exposure review dates, and incident history. Never contains actual credentials or real names in shared documentation.

## 8. Approved public sources
OPSEC must not become cover for unlawful activity: identity separation serves legitimate research protection, not evasion of legal process or platform accountability. See legal cross-references.

## 9. Source verification standards
OPSEC effectiveness is tested by exposure review: searching breach corpora, public records, and platform data for links between research identities and real identity. Negative results are documented, not assumed.

## 10. Analytical framework
Threat-tier model: Tier 1 (routine research, no specific adversary) → standard compartmentation. Tier 2 (sensitive topics, possible monitoring) → dedicated devices, separate network. Tier 3 (hostile actors expected) → maximum compartmentation, possibly external secure facilities.

## 11. Evidence requirements
OPSEC register per project recording compartment assignments, control decisions, review dates, and exposure findings — without sensitive identity details.

## 12. Confidence assessment
HIGH: compartmentation verified, exposure reviews current, zero identity links found. MODERATE: controls in place, reviews informal. LOW: identity separation incomplete or reviews absent. INSUFFICIENT: no OPSEC program.

## 13. Common analytical mistakes
Using personal email for research sign-ups; working on research laptop with personal accounts logged in; discussing sensitive projects in unencrypted channels; assuming 'nobody cares about my research'; ignoring breach-corpus exposure.

## 14. Ethical considerations
OPSEC protects researchers so they can continue legitimate work without becoming targets. It also protects sources: a researcher whose identity is exposed may expose every source who trusted them. OPSEC failure is a harm multiplier.

## 15. Security boundaries
De-anonymizing under pressure; using real identity on monitored platforms; storing research identities in personal password managers; discussing compartment details outside need-to-know; disabling security controls for convenience.

## 16. Expected output
OPSEC plan, exposure review records, compartment register, and incident history per project.

## 17. Quality checklist
- [ ] Classification label applied to every artifact
- [ ] Sources are public-only and logged with access timestamps
- [ ] Third-party tools verified against vetting checklist
- [ ] Chain-of-custody or handling record complete
- [ ] Audit entry written for every material action
- [ ] Peer or reviewer sign-off recorded where required
- [ ] Research identities fully separated from personal identity
- [ ] Exposure review current
- [ ] No personal accounts on research systems

## 18. Cross-reference links
- Related operational guidance: core/, legal/, verification/, reporting/ modules.
- Mandatory policy documents in this module: privacy_by_design.md, data_minimization_protocol.md, secure_research_workflow.md, safe_public_source_handling.md, research_data_classification.md, sensitive_data_redaction.md, personal_identifier_protection.md, account_and_credential_safety.md, secure_document_storage.md, evidence_integrity_management.md, audit_log_management.md, access_control_principles.md, third_party_tool_assessment.md, malicious_content_handling.md, cyber_safety_boundaries.md, operational_security_boundaries.md, doxxing_prevention.md, surveillance_abuse_prevention.md, targeting_and_harm_prevention.md, safety_escalation_protocol.md

