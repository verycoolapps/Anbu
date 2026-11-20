# Evidence Chain Management

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Evidence chain management governs how ANBU packages, stores, labels, and hands off evidentiary material so that any claim in an analytical product can be traced to its supporting items and re-verified by a third party. Provenance (`source_provenance_tracking.md`) records where an item came from; this file records how items are assembled into an argument.

## 2. Scope

Applies to dossiers, claim cards, media exhibits, document sets, datasets, and any multi-item evidentiary package. Covers internal chain integrity (did we alter, lose, or mislabel anything?) and external defensibility (can the chain survive review?).

## 3. Intelligence Objectives

- Ensure every conclusion is backed by a documented, intact evidence chain.
- Make chains inspectable: a reviewer can walk from conclusion to item without analyst assistance.
- Detect chain failures early — missing items, broken links, label drift.
- Preserve chains for legal or oversight proceedings per `legal/`.

## 4. Core Concepts

- **Claim-to-evidence mapping:** each claim in a product maps to specific evidence IDs; unmapped claims are prohibited in finished products.
- **Evidence labels:** VERIFIED (authenticated primary), CORROBORATED (multi-source agreement), SINGLE-SOURCE, UNVERIFIED LEAD, DISPROVEN. Labels are mandatory.
- **Chain integrity:** hashes at acquisition + append-only logs detect tampering.
- **Separation of evidence and inference:** the chain contains only observations; analytical judgments live in the product layer, not the evidence store.

## 5. Analytical Methodology

1. **Item registration:** every evidentiary item enters the store with ID, hash, provenance link, and label.
2. **Claim mapping:** during analysis, each claim is bound to one or more evidence IDs via claim cards (`source_credibility_scoring.md`).
3. **Label discipline:** labels update as verification progresses; history of label changes is retained.
4. **Chain assembly:** product sections cite evidence IDs; the assembler validates that every cited ID exists and carries an appropriate label.
5. **Chain audit:** before release, walk each chain end-to-end; run `verification_audit_trail.md` checks.

## 6. Step-by-Step Workflow

1. Intake item → register with provenance record → assign label.
2. During analysis, create/update claim cards binding claims to evidence IDs.
3. On label upgrade (e.g., UNVERIFIED → CORROBORATED), log the change with reason and new evidence.
4. Assemble product: attach evidence manifest listing IDs, labels, and locators per section.
5. Audit: verify all cited IDs resolve, labels meet section requirements, no DISPROVEN items cited as support.
6. Archive: freeze chain state at publication; post-publication changes create a new version.

## 7. Data Requirements

- Evidence store with unique IDs, hashes, labels, and provenance links.
- Claim-card registry binding claims to evidence.
- Versioned product manifests listing cited evidence per section.
- Access log for who viewed/exported which evidence (security requirement).

## 8. Approved Public Sources

The evidence store itself is internal, but every item in it originates from lawfully acquired public sources per `source_provenance_tracking.md`. Chains may not include material whose acquisition legality is unresolved — those go to `legal/` review first.

## 9. Source Verification Standards

An evidence chain is valid only if: (a) every item has provenance, (b) every claim maps to items, (c) labels reflect the current verification state, (d) no item is cited beyond its label's permitted use (UNVERIFIED LEAD may motivate collection, never support a conclusion).

## 10. Analytical Framework

Maintain the **Chain Graph**: claim nodes → evidence nodes → provenance nodes. Validate continuously: orphaned claims (no evidence), orphaned evidence (never cited — fine, but review), label-evidence mismatches (e.g., VERIFIED label on unauthenticated media), and circular derivation (evidence whose parent is the claim it supports — a fatal flaw).

## 11. Evidence Requirements

Each chain element requires: stable ID, content hash, provenance record ID, label with justification, acquisition timestamp, and custodian. The chain manifest for a product must be reproducible: given the manifest, an auditor can retrieve every item.

## 12. Confidence Assessment

Chain confidence is the minimum confidence across its weakest required link. A conclusion resting on one LOW item is LOW even if other items are HIGH. Report per-claim confidence (`evidence_confidence_scoring.md`) and per-chain integrity status (INTACT / GAPS / BROKEN).

## 13. Common Analytical Mistakes

- Citing evidence by description ("the video showed…") instead of evidence ID.
- Upgrading labels without logging the new supporting item.
- Letting DISPROVEN items remain cited because removal would weaken a preferred narrative.
- Confusing quantity with quality — ten UNVERIFIED items do not outweigh one VERIFIED record.
- Losing custody during handoffs between analysts or divisions.

## 14. Ethical Considerations

Chains may contain sensitive personal data. Evidence manifests distributed outside the analysis team require `legal/` review. Do not construct chains designed to mislead — e.g., selective citation that omits contradictory verified evidence is a fabrication of the record and violates doctrine.

## 15. Security Boundaries

Evidence store is access-controlled with role-based permissions and full access logging. Integrity protected via hashing; exports are logged and may require dual authorization for sensitive sets. No evidence leaves the store without a manifest and custody record.

## 16. Expected Output

Per product: an evidence manifest mapping every claim to labeled evidence IDs with locators; an integrity statement (INTACT/GAPS/BROKEN); and an archived, frozen chain snapshot retained per `legal/` retention rules.

## 17. Quality Checklist

- [ ] Every claim maps to ≥1 evidence ID
- [ ] All cited IDs exist with valid labels
- [ ] No label exceeds its evidence state
- [ ] DISPROVEN items excluded from support roles
- [ ] Manifest reproducible by third party
- [ ] Integrity statement issued

## 18. Cross-Reference Links

- Records: `source_provenance_tracking.md`, `verification_audit_trail.md`, `source_citation_standards.md`
- Labels/scoring: `source_credibility_scoring.md`, `evidence_confidence_scoring.md`, `claim_verification.md`
- Divisions: `reporting/` (manifest format), `legal/` (retention/disclosure), `security/` (access control), `workflows/` (pipeline gates)
