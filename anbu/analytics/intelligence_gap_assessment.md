# Intelligence Gap Assessment

**ANBU Division 008 · Analytics**

---

## Purpose

An intelligence gap is the distance between what we need to know and what we can actually know from available sources. Gaps are not failures — they are the honest boundaries of knowledge. This file defines how ANBU identifies, categorizes, and reports intelligence gaps, and how gap assessment drives collection priorities and consumer expectations.

## Scope

Applied to all analytical products, especially those with INSUFFICIENT confidence or where conclusions depend on missing evidence. Also used proactively to identify collection requirements before analysis begins. Covers gaps in collection, verification, access, and analytical capability.

## Intelligence objectives

- Identify what is unknown and why it matters.
- Distinguish gap types: collection gap, verification gap, access gap, analytical gap.
- Prioritize gaps by impact on the assessment.
- Drive collection requirements and consumer expectations.
- Prevent false confidence produced by unacknowledged gaps.

## Core concepts

- **Intelligence gap.** Missing information that limits analytical judgment — not merely absent data, but absent data that matters.
- **Gap types:**
  - *Collection gap* — information exists but was not collected.
  - *Verification gap* — information collected but not verified to standard.
  - *Access gap* — information exists but is not publicly accessible.
  - *Analytical gap* — information exists but cannot be analyzed with current methods.
- **Load-bearing gap.** A gap whose resolution would change the assessment — vs. peripheral gaps that don't matter.
- **Gap impact.** How much the missing information affects confidence and conclusions.
- **Collection requirement.** The specific action needed to close a gap — what to collect, from where, at what priority.
- **Observability limit.** Some things cannot be known from public sources at all; the gap is permanent within OSINT boundaries.

## Analytical methodology

1. Identify what the assessment needs to know to be confident.
2. Compare against what is actually known (verified evidence base).
3. Catalog the difference as specific gaps.
4. Classify each gap by type and assess load-bearing status.
5. Prioritize gaps by impact × feasibility of closure.
6. Generate collection requirements for closable gaps.
7. Acknowledge permanent gaps (observability limits) honestly.
8. Report gaps in the product with impact on confidence.

## Step-by-step workflow

1. List the intelligence questions the assessment must answer.
2. For each question, list the evidence needed for HIGH confidence.
3. Compare with actual verified evidence.
4. Catalog gaps: what is missing, what type, why.
5. Assess each gap's impact: would resolving it change the conclusion?
6. Prioritize: load-bearing gaps first, then by feasibility.
7. Generate collection requirements for closable gaps.
8. Flag permanent gaps (access/observability limits).
9. Write gap assessment annex; adjust confidence accordingly.
10. Route collection requirements to `../workflows/collection_to_assessment_pipeline.md`.

## Data requirements

- The intelligence questions or requirements (PIRs).
- The verified evidence base with coverage map.
- Knowledge of what public sources exist for each gap.
- Collection capacity and priorities.

## Approved public sources

Gap assessment itself doesn't collect; it identifies where public sources might fill gaps. Collection planning references `../osint/` source catalog.

## Source verification standards

Gaps are defined relative to verified evidence. An unverified report does not close a gap; it creates a verification gap. See `../verification/` standards.

## Analytical framework

Gap classification matrix:

| Gap type | Description | Example | Closable? |
|---|---|---|---|
| Collection | Not collected | Didn't search archives | Yes — task collection |
| Verification | Collected, unverified | Single-source claim | Yes — corroborate |
| Access | Exists but restricted | Classified info | No — OSINT boundary |
| Analytical | Exists, can't analyze | Data without methodology | Maybe — new methods |
| Observability | Doesn't exist publicly | Secret deliberations | No — permanent gap |

## Evidence requirements

- Gap catalog with type classification.
- Impact assessment per gap.
- Collection requirements for closable gaps.
- Permanent gaps acknowledged honestly.
- Confidence adjusted for unresolved load-bearing gaps.

## Confidence assessment

Gap assessment directly determines confidence ceiling:

- **HIGH achievable** — no load-bearing gaps; minor gaps don't affect conclusions.
- **MODERATE ceiling** — some load-bearing gaps remain; conclusions hedged accordingly.
- **LOW ceiling** — multiple load-bearing gaps; conclusions tentative.
- **INSUFFICIENT** — gaps too large for any assessment; report the gap itself.

## Common analytical mistakes

- Not identifying gaps — treating absence of evidence as evidence of absence.
- Confusing "we didn't look" with "it doesn't exist."
- Not distinguishing gap types — "collection gap" vs. "access gap" need different responses.
- Failing to prioritize: treating all gaps as equally important.
- Not generating collection requirements — gaps identified but not actionable.
- Hiding gaps to make products seem more complete.
- Assuming gaps can be closed when they're permanent observability limits.

## Ethical considerations

Gap assessment must be honest about what cannot be known. Analysts must not pretend certainty where gaps exist, nor manufacture gaps to justify more collection than needed. Permanent gaps (classified info, private deliberations) must be acknowledged, not worked around through non-OSINT means.

## Security boundaries

Gap assessment operates within OSINT boundaries. It must not generate requirements for classified collection, surveillance, or non-public sources. Access gaps are acknowledged as permanent within the OSINT boundary.

## Expected output

Gap annex: gap catalog with type/impact/classification, prioritized collection requirements, permanent-gap acknowledgment, confidence impact statement. Main product notes key gaps affecting conclusions.

## Quality checklist

- [ ] All intelligence questions mapped to evidence needs.
- [ ] Gaps cataloged and classified by type.
- [ ] Load-bearing gaps identified.
- [ ] Collection requirements generated for closable gaps.
- [ ] Permanent gaps acknowledged.
- [ ] Confidence adjusted for unresolved gaps.
- [ ] Gaps reported honestly in product.

## Cross-reference links

- [`analytical_confidence_language.md`](analytical_confidence_language.md) — INSUFFICIENT handling.
- [`key_assumptions_check.md`](key_assumptions_check.md) — untested assumptions become gaps.
- [`intelligence_synthesis.md`](intelligence_synthesis.md) — synthesis acknowledges gaps.
- [`multi_source_intelligence_fusion.md`](multi_source_intelligence_fusion.md) — fusion may have gaps.
- [`risk_probability_assessment.md`](risk_probability_assessment.md) — gaps affect probability.
- [`../osint/collection_requirements.md`](../osint/collection_requirements.md) — collection planning.
- [`../workflows/collection_to_assessment_pipeline.md`](../workflows/collection_to_assessment_pipeline.md) — gap-driven collection.
- [`../reporting/gap_assessment_template.md`](../reporting/gap_assessment_template.md) — output format.
