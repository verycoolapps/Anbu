# Conflicting Evidence Resolution

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Conflicting evidence is normal in intelligence work — witnesses disagree, records contradict, timelines collide. This file defines how ANBU resolves (or honestly manages) conflicts: determining which evidence is stronger, when conflicts are irreducible, and how to report contested findings without false resolution.

## 2. Scope

Covers conflicts between sources, between a source and a record, between records, and between evidence and established context. Applies to factual conflicts; analytical disagreements are handled in `analytics/` structured techniques.

## 3. Intelligence Objectives

- Systematically weigh competing evidence instead of intuitively picking a side.
- Distinguish resolvable conflicts (one side is stronger) from irreducible ones (genuinely contested).
- Preserve minority evidence — the weaker side may be the true one.
- Report contested findings with explicit uncertainty rather than forced consensus.

## 4. Core Concepts

- **Conflict taxonomy:** factual contradiction (can't both be true), detail divergence (both can be true, details differ), temporal conflict (sequence disagreement), attribution conflict (who said/did what), and interpretation conflict (same facts, different meaning).
- **Evidence hierarchy:** primary authenticated records outweigh secondary accounts; contemporaneous outweighs retrospective; independent corroboration outweighs single sources — but hierarchy yields to context (a fabricated "primary" loses to a corroborated record).
- **Irreducible conflict:** when evidence is balanced, the correct output is a contested finding with both positions documented — not a coin flip.
- **Conflict as signal:** persistent conflicts between official records and observed reality are themselves analytical findings (credibility gaps, information operations, institutional dysfunction).

## 5. Analytical Methodology

1. **Document both sides completely:** each position gets its evidence set, provenance, and credibility scores — before weighing begins.
2. **Classify the conflict type** per the taxonomy.
3. **Test each side:** re-verify key evidence; check for fabrication, bias, motivation; apply `source_bias_assessment.md`.
4. **Weigh by criteria:** evidentiary quality, independence, contemporaneity, specificity, and convergence with unrelated evidence.
5. **Attempt synthesis:** sometimes conflicts dissolve — e.g., "both happened, at different times/places" or "different definitions of the same term."
6. **Decide:** RESOLVED (winner with justification), CONTESTED (irreducible, report both), or ESCALATED (needs collection/expert).

## 6. Step-by-Step Workflow

1. Identify the conflicting claims and their evidence chains.
2. Build the conflict record: positions, evidence IDs, provenance, credibility scores.
3. Classify conflict type; check for definitional or temporal reconciliation.
4. Re-verify pivotal evidence on each side; hunt for decisive new evidence.
5. Apply weighing criteria; document the reasoning explicitly.
6. Issue resolution status; if CONTESTED, specify what evidence would resolve it and queue collection.
7. File in audit trail; contested findings carry both evidence sets into `reporting/`.

## 7. Data Requirements

- Complete evidence sets for all positions.
- Provenance and credibility records per `source_provenance_tracking.md` and `source_credibility_scoring.md`.
- Conflict-type classification.
- Weighing rationale documented.
- Collection requirements list for unresolved conflicts.

## 8. Approved Public Sources

All standard tiers. For conflict resolution specifically, prioritize primary records on both sides, official statements, court records, and contemporaneous documentation. When conflicts involve technical questions, route to domain experts via `analytics/` or external specialists.

## 9. Source Verification Standards

Resolution decisions must be evidence-driven, documented, and reversible: if new evidence emerges, the resolution reopens. Never resolve a conflict by source prestige alone ("the bigger outlet is probably right") — prestige is an input, not a verdict.

## 10. Analytical Framework

Use the **Conflict Ledger**: position A evidence | position B evidence | conflict type | weighing criteria scores | resolution status | reopening triggers. Ledgers are auditable and support `conflicting_evidence_resolution` reviews by senior analysts.

## 11. Evidence Requirements

Conflict records include: both positions verbatim, all evidence with provenance, type classification, weighing analysis, resolution or contested status, dissent documentation, and reopening criteria. Contested findings published in products must present both sides proportionally to evidence strength.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | Resolution based on authenticated primary record or overwhelming independent convergence |
| MODERATE | Resolution based on clearly stronger evidence set with minor gaps |
| LOW | Contested but leaning; publish as probable with both sides noted |
| INSUFFICIENT | Irreducibly balanced — publish as CONTESTED, confidence in neither side |

## 13. Common Analytical Mistakes

- Resolving conflicts by intuition or institutional preference rather than criteria.
- Discarding the losing side's evidence instead of preserving it in the record.
- Treating "majority of sources" as resolution when all share one origin.
- Forcing binary resolution on conflicts that are actually definitional.
- Letting the preferred analytic narrative choose the winner.

## 14. Ethical Considerations

False resolution is a form of fabrication: presenting contested questions as settled misleads consumers. Publish contested status honestly. When conflicts involve individuals, ensure symmetric rigor — do not resolve against the less powerful party on thinner scrutiny.

## 15. Security Boundaries

Resolution work is analytical and desk-based. Do not contact conflicting parties for "clarification" as a verification method; do not adjudicate disputes involving ongoing security operations — route to `security/` and `legal/`.

## 16. Expected Output

Conflict ledgers per contested question; resolution memos for resolved conflicts; contested-finding sections for `reporting/`; collection taskings for evidence that would resolve open conflicts.

## 17. Quality Checklist

- [ ] Both positions documented with full evidence
- [ ] Conflict type classified
- [ ] Reconciliation possibilities tested
- [ ] Pivotal evidence re-verified
- [ ] Weighing criteria applied and documented
- [ ] Resolution or contested status issued
- [ ] Minority evidence preserved
- [ ] Reopening triggers defined

## 18. Cross-Reference Links

- Evidence base: `source_credibility_scoring.md`, `cross_source_corroboration.md`, `claim_verification.md`, `evidence_confidence_scoring.md`
- Source context: `source_bias_assessment.md`, `source_reliability_assessment.md`, `conflicting_evidence_resolution` peers
- Downstream: `reporting/` (contested findings), `analytics/` (structured techniques), `legal/`
- Records: `evidence_chain_management.md`, `verification_audit_trail.md`, `source_citation_standards.md`
