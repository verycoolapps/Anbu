# Access Control Principles

**Module:** ANBU OSINT — Security & Operational Protection
**Classification handling:** Apply research data classification rules to all outputs produced under this procedure. All stored artifacts must carry an analyst-assigned classification label.

## 1. Purpose
Apply least-privilege, need-to-know, and role-based access control to all ANBU research data and systems, ensuring that access is granted only where required for a defined function and is continuously reviewed, revoked, and logged.

## 2. Scope
All research data stores, evidence repositories, analysis environments, communication channels, and administrative functions handling ANBU material.

## 3. Intelligence objectives
- Limit blast radius: compromise or misuse of one account affects only the minimum necessary data.
- Enable accountability: every access is attributable to a person and role.
- Support separation of duties where research integrity requires it (collector vs approver).
- Make revocation fast and complete when roles change or incidents occur.

## 4. Core concepts
- Least privilege: default deny; access granted per documented need.
- Need-to-know: classification plus functional role determines access; classification alone is insufficient.
- Role-based access control (RBAC): access tied to function, not individual preferences.
- Periodic recertification: access lists reviewed on schedule and on role change; stale access revoked.

## 5. Analytical methodology
1. Define roles (collector, analyst, reviewer, administrator, auditor) and their required data access.
2. Map roles to classification compartments and functions.
3. Provision access per role; log grants.
4. Enforce technical controls: authentication, authorization, encryption.
5. Recertify access quarterly and on any role change.
6. On departure or incident, revoke all access and verify.

## 6. Step-by-step workflow
1. Roles defined → 2. Access matrix built → 3. Provisioning → 4. Technical enforcement → 5. Audit logging active → 6. Recertification cycle → 7. Revocation on trigger events.

## 7. Data requirements
Access matrix: role × data class × permitted actions (read, analyze, export, administer). Plus user-to-role assignments and recertification dates — never password or credential data.

## 8. Approved public sources
Access control systems must themselves be secured per secure document storage and account and credential safety. Multi-factor authentication is mandatory for access to SENSITIVE+ compartments.

## 9. Source verification standards
Access reviews examine actual usage logs against granted privileges: granted-but-unused access is revoked; used-but-ungranted access is an incident.

## 10. Analytical framework
Need-to-know test: can the requester articulate the specific intelligence objective requiring this access? 'Might need it' fails. Access is granted against a documented task, not a job title alone.

## 11. Evidence requirements
Access register: users, roles, granted compartments, grant date, last recertification, and revocation status.

## 12. Confidence assessment
HIGH: RBAC enforced, MFA on sensitive compartments, quarterly recertification current. MODERATE: RBAC with minor gaps. LOW: ad-hoc access grants, stale permissions. INSUFFICIENT: no access control.

## 13. Common analytical mistakes
Granting access 'temporarily' that never expires; role creep accumulating permissions; shared accounts destroying attribution; treating access approval as a one-time event; former personnel retaining access.

## 14. Ethical considerations
Access control protects people as much as data: it prevents a compromised or malicious insider from reaching data that could harm sources and subjects, and it protects analysts from false accusation by ensuring their actions are scoped and logged.

## 15. Security boundaries
Access above classification without need-to-know; shared credentials; unrevoked access after role change; privilege escalation outside documented authority; accessing data 'out of curiosity.'

## 16. Expected output
Current access matrix, recertification records, MFA coverage report, and revocation log.

## 17. Quality checklist
- [ ] Classification label applied to every artifact
- [ ] Sources are public-only and logged with access timestamps
- [ ] Third-party tools verified against vetting checklist
- [ ] Chain-of-custody or handling record complete
- [ ] Audit entry written for every material action
- [ ] Peer or reviewer sign-off recorded where required
- [ ] All SENSITIVE+ access requires MFA
- [ ] Recertification current for all users
- [ ] No shared accounts in use

## 18. Cross-reference links
- Related operational guidance: core/, legal/, verification/, reporting/ modules.
- Mandatory policy documents in this module: privacy_by_design.md, data_minimization_protocol.md, secure_research_workflow.md, safe_public_source_handling.md, research_data_classification.md, sensitive_data_redaction.md, personal_identifier_protection.md, account_and_credential_safety.md, secure_document_storage.md, evidence_integrity_management.md, audit_log_management.md, access_control_principles.md, third_party_tool_assessment.md, malicious_content_handling.md, cyber_safety_boundaries.md, operational_security_boundaries.md, doxxing_prevention.md, surveillance_abuse_prevention.md, targeting_and_harm_prevention.md, safety_escalation_protocol.md

