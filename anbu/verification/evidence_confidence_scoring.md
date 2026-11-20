# Evidence Confidence Scoring

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Evidence confidence scoring is the system-level aggregator: it converts the outputs of every verification procedure into a single, consistent confidence band attached to claims, findings, and analytical judgments. Claim-level scoring lives in `source_credibility_scoring.md`; this file defines the portfolio-level scoring that reporting and analytics consume.

## 2. Scope

Covers confidence assignment for: individual claims (aggregated from claim cards), multi-claim findings, section-level judgments in products, and whole-product confidence statements. Defines how component scores roll up and how confidence is communicated.

## 3. Intelligence Objectives

- Produce consistent, comparable confidence bands across all ANBU products.
- Make confidence communicable: every band maps to a plain-language statement consumers can act on.
- Prevent confidence inflation: scores must reflect the weakest load-bearing evidence, not the strongest.
- Enable confidence auditing: bands must be traceable to documented inputs.

## 4. Core Concepts

- **The weakest-link rule:** a conclusion's confidence is capped by its weakest load-bearing evidence item — one LOW item in the critical path caps the conclusion.
- **Confidence ≠ probability:** bands are ordinal judgments about evidence sufficiency, not statistical probabilities of truth.
- **Asymmetric costs:** for some questions (threat warnings), the cost of false confidence exceeds the cost of false modesty; bands are set conservatively for high-stakes findings.
- **Confidence decay:** confidence degrades as evidence ages or context changes; scores carry review dates.

## 5. Analytical Methodology

1. **Inventory evidence:** list all evidence items supporting the conclusion with their individual statuses.
2. **Identify load-bearing items:** which items, if removed, would collapse the conclusion?
3. **Score each:** apply the relevant file's confidence criteria (reliability, corroboration, authenticity).
4. **Apply weakest-link:** conclusion confidence = lowest band among load-bearing items, adjusted upward only if redundancy exists (multiple independent items at the same claim).
5. **Assign band:** HIGH / MODERATE / LOW / INSUFFICIENT with justification.
6. **Document:** record the scoring rationale; file in audit trail.

## 6. Step-by-Step Workflow

1. Receive conclusion candidate (claim, finding, or product section).
2. Enumerate supporting evidence; link each to provenance and label.
3. Classify each item's confidence per its verification file.
4. Determine load-bearing set; apply weakest-link rule with redundancy check.
5. Assign band; write the one-sentence justification consumers will see.
6. Record in claim card/product manifest; set review trigger date.

## 7. Data Requirements

- Evidence manifest with per-item verification status.
- Claim cards for constituent claims.
- Load-bearing analysis (which items are critical).
- Staleness assessment (evidence age vs. claim volatility).

## 8. Approved Public Sources

The scoring consumes verification outputs, not new sources. Band definitions and calibration examples derive from the verification files and `analytics/` confidence models. Periodic calibration against known outcomes (resolved questions) refines band usage.

## 9. Source Verification Standards

Confidence bands are only valid when every load-bearing item has a completed verification record. Bands assigned without evidence manifests are void. INSUFFICIENT is a mandatory honest output — it is never a failure state but a correct finding when evidence is absent.

## 10. Analytical Framework

Use the **Confidence Rollup Table**: conclusion → load-bearing evidence items → per-item band → weakest-link result → redundancy adjustment → final band. This table appears in product appendices for auditability.

## 11. Evidence Requirements

Every published confidence band links to: the conclusion statement, the evidence manifest, the load-bearing analysis, per-item confidence records, and the justification sentence. Consumers must be able to audit why a band was assigned.

## 12. Confidence Assessment

| Level | Criteria |
|---|---|
| HIGH | All load-bearing items HIGH or redundant MODERATE+; primary-anchored where possible |
| MODERATE | Load-bearing items mostly MODERATE with minor gaps |
| LOW | Any load-bearing item LOW; significant unverified components |
| INSUFFICIENT | Critical evidence absent or untestable — conclusion should not be asserted |

## 13. Common Analytical Mistakes

- Averaging confidence across items instead of applying weakest-link.
- Letting strong evidence on minor points inflate confidence on the core claim.
- Treating INSUFFICIENT as a prompt to guess rather than to report honestly.
- Failing to decay confidence as evidence ages.
- Publishing numeric pseudo-probabilities ("73% likely") without calibrated models — bands only, unless `analytics/` provides a validated model.

## 14. Ethical Considerations

Confidence communication is a public trust function. Overstated confidence causes real-world harm (false warnings, missed threats); understated confidence causes paralysis. Bands must be honest, calibrated, and correctable — publish corrections when confidence proves misplaced.

## 15. Security Boundaries

Confidence records for security-sensitive findings are access-controlled per `security/`. Public-facing confidence bands are reviewed for operational-security implications before release.

## 16. Expected Output

Confidence bands on all claims, findings, and products; rollup tables in appendices; review-date triggers; calibration reports comparing predicted vs. resolved outcomes.

## 17. Quality Checklist

- [ ] Evidence manifest complete
- [ ] Load-bearing items identified
- [ ] Per-item confidence documented
- [ ] Weakest-link applied with redundancy check
- [ ] Band + justification recorded
- [ ] Review trigger set
- [ ] Audit trail entry filed

## 18. Cross-Reference Links

- Inputs: `source_credibility_scoring.md`, `source_reliability_assessment.md`, `cross_source_corroboration.md`, all verification procedure files
- Output consumers: `reporting/` (confidence presentation), `analytics/` (confidence models), `workflows/` (gates)
- Records: `verification_audit_trail.md`, `evidence_chain_management.md`, `source_citation_standards.md`
- Divisions: `core/` (confidence doctrine), `reporting/`, `legal/` (reliance risk)
