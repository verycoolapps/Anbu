# Claim Verification

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Claim verification is the atomic operation of ANBU's verification division: take one assertion, decompose it, test each component against evidence, and return a graded verdict. Every other verification file exists to serve this workflow. This file defines the end-to-end procedure and the verdict vocabulary used across the system.

## 2. Scope

Covers factual claims of any form: events, figures, quotations, media content, causation, attribution, and predictions stated as fact. Excludes normative claims ("policy X is wise") and pure analysis, which are handled in `analytics/`.

## 3. Intelligence Objectives

- Return a defensible verdict for every material claim: TRUE / MOSTLY TRUE / MIXED / MOSTLY FALSE / FALSE / UNVERIFIABLE.
- Preserve claim integrity: verify what was actually said, not a paraphrase.
- Produce verdicts reproducible by another analyst from the documented evidence.
- Feed verified claim sets into analytical products without re-verification.

## 4. Core Concepts

- **Claim decomposition:** complex claims are split into atomic sub-claims; a verdict applies per sub-claim, then aggregates.
- **Verdict ≠ confidence:** the verdict is the conclusion; the confidence band (`evidence_confidence_scoring.md`) is the strength of that conclusion.
- **UNVERIFIABLE is a verdict:** failure to verify is not failure of the claim. Record what was searched and why evidence is absent.
- **Temporal scoping:** claims about the past are verifiable; claims about the future are not — they route to forecasting in `analytics/`.

## 5. Analytical Methodology

1. **Fix the claim:** capture verbatim text, author, outlet, timestamp, and context. Check `publication_date_verification.md` and `quotation_verification.md` for attribution.
2. **Decompose:** identify each testable proposition (actor, action, time, place, quantity, causation).
3. **Evidence hunt:** search primary → secondary → tertiary in that order; apply `cross_source_corroboration.md`.
4. **Score:** fill the claim card per `source_credibility_scoring.md`.
5. **Verdict:** map score band to verdict vocabulary; note dissent and unresolved sub-claims.
6. **File:** record verdict, evidence manifest, and confidence in the audit trail.

## 6. Step-by-Step Workflow

1. Receive claim (from collection, a product draft, or a tasking).
2. Create claim record: ID, verbatim text, provenance, originating context.
3. Decompose into sub-claims; assign each an evidence target.
4. For each sub-claim: locate best evidence, run corroboration, score credibility.
5. Aggregate sub-claim verdicts; handle mixed results explicitly (do not average into mush).
6. Issue verdict card; link evidence manifest; update audit trail.
7. Queue unresolved items for additional collection via `osint/`.

## 7. Data Requirements

- Verbatim claim text with full citation metadata.
- Evidence items with provenance records and labels.
- Corroboration origin map.
- Search log documenting where evidence was sought.

## 8. Approved Public Sources

All tiers per the tier files. For claim verification specifically, prioritize: official records and statements, court documents, statistical releases, established investigative reporting with primary sourcing, platform transparency reports, and authenticated media via `image_authenticity_assessment.md` / `video_authenticity_assessment.md`.

## 9. Source Verification Standards

A verdict of TRUE requires at least one authenticated primary record or multiple independent corroborations across tiers. MOSTLY TRUE allows minor inaccuracies in detail. FALSE requires affirmative contradictory evidence — not merely absence of support.

## 10. Analytical Framework

Use the **Verdict Matrix**: sub-claim verdicts × evidence strength → aggregate verdict. Document weighting decisions (e.g., a fatal sub-claim can cap the aggregate at MOSTLY FALSE). Every verdict card states which sub-claims were decisive.

## 11. Evidence Requirements

Verdict cards must include: verbatim claim, decomposition, per-sub-claim evidence IDs, corroboration level, credibility score, verdict, confidence band, dissent notes, and the search log. Verdicts without evidence manifests are void.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | Primary-record anchored or ≥2 independent corroborations, no unresolved contradiction |
| MODERATE | Strong secondary agreement or single primary with minor gaps |
| LOW | Single-source claims or corroboration with common-origin issues |
| INSUFFICIENT | Evidence absent or claim too ambiguous to test — verdict UNVERIFIABLE |

## 13. Common Analytical Mistakes

- Verifying a headline instead of the article body (or vice versa without noting which).
- Treating "could not disprove" as TRUE.
- Forcing a binary verdict on genuinely mixed claims.
- Verifying the claim as the analyst wishes it were phrased (leading paraphrase).
- Ignoring the claim's date context — events change; verify against the time stated.

## 14. Ethical Considerations

Verdicts about identifiable persons or institutions require symmetric effort: equal rigor for confirmation and refutation. Publish verdicts with evidence links so the public can audit. Reserve FALSE for documented contradiction; contested-but-unresolved claims are reported as UNVERIFIABLE, not weaponized.

## 15. Security Boundaries

Verification is desk-based. No pretexting, no deception of sources, no access to non-public systems. For claims involving ongoing security threats, coordinate with `security/` before any public verdict.

## 16. Expected Output

Verdict cards per claim with full evidence manifests; aggregate verification reports for product sections; a queue of UNVERIFIABLE items with documented search coverage for future re-check.

## 17. Quality Checklist

- [ ] Claim captured verbatim with context
- [ ] Decomposed into testable sub-claims
- [ ] Evidence sought across all applicable tiers
- [ ] Corroboration origin map completed
- [ ] Verdict + confidence issued with evidence manifest
- [ ] Dissent and unresolved sub-claims documented
- [ ] Audit trail entry filed

## 18. Cross-Reference Links

- Method inputs: `primary_source_verification.md`, `secondary_source_verification.md`, `tertiary_source_handling.md`, `cross_source_corroboration.md`, `source_credibility_scoring.md`
- Claim integrity: `quotation_verification.md`, `publication_date_verification.md`, `translation_verification.md`
- Media claims: `image_authenticity_assessment.md`, `video_authenticity_assessment.md`, `manipulated_media_assessment.md`
- Downstream: `fact_checking_methodology.md`, `evidence_confidence_scoring.md`, `source_citation_standards.md`, `reporting/`
- Divisions: `analytics/` (claim analysis), `legal/` (defamation), `osint/` (gap collection)
