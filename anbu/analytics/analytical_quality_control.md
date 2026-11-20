# Analytical Quality Control

**ANBU Division 008 · Analytics**

---

## Purpose

Analytical quality control is the systematic process of ensuring that every ANBU analytical product meets the standards this division defines — verified evidence, sound reasoning, honest confidence, appropriate language, and complete documentation. It operates at two levels: product-level QC (checking individual assessments before dissemination) and process-level QC (evaluating the analytical system's performance over time). This file defines both.

## Scope

Applied to all analytical products before dissemination and to the analytical process itself on a recurring basis. Covers pre-publication review, post-publication evaluation, calibration tracking, and process improvement. Sits above individual techniques — it evaluates whether techniques were applied correctly and whether outputs meet standards.

## Intelligence objectives

- Catch analytical errors before they reach consumers.
- Ensure consistent quality across all products and analysts.
- Track analytical performance over time for calibration and improvement.
- Identify systematic weaknesses in the analytical process.
- Maintain the credibility that makes ANBU products trustworthy.

## Core concepts

- **Product QC.** Checking an individual assessment against standards before dissemination.
- **Process QC.** Evaluating the analytical system: are techniques applied correctly? Are standards consistent? Is performance improving?
- **Quality dimensions.** Accuracy (is it right?), completeness (is everything covered?), clarity (is it understandable?), timeliness (is it fast enough?), honesty (is uncertainty disclosed?).
- **Calibration tracking.** Comparing stated confidence/probability to actual outcomes over time.
- **Peer review.** Structured review by another analyst — the primary product QC mechanism.
- **Red team.** Adversarial review for high-stakes products — see `red_team_analytical_review.md`.
- **After-action review.** Post-event evaluation of analytical accuracy and process.
- **Quality metrics.** Measurable indicators: verification rate, confidence calibration, consumer feedback, error rates.

## Analytical methodology

### Product-level QC

1. **Self-check.** Author completes the quality checklist before submission.
2. **Peer review.** Independent analyst reviews against standards.
3. **Technical review.** For complex products, specialist review (e.g., statistical, geographic).
4. **Red team.** For high-stakes products, adversarial review.
5. **Revision.** Findings addressed; re-review if major changes.
6. **Release.** Product disseminated with QC documentation.

### Process-level QC

1. **Calibration tracking.** Record all probabilistic forecasts; compare to outcomes.
2. **Error analysis.** When assessments prove wrong, analyze why — evidence, reasoning, or bias failure?
3. **Standards review.** Periodically review and update analytical standards.
4. **Training needs.** Identify skill gaps from error patterns.
5. **Consumer feedback.** Collect and analyze consumer satisfaction and accuracy reports.

## Step-by-step workflow

### Before dissemination

1. Author completes self-check against product checklist.
2. Peer reviewer checks: evidence verification, reasoning soundness, confidence calibration, language consistency, completeness.
3. For high-stakes: red team review per `red_team_analytical_review.md`.
4. Findings adjudicated; revisions made.
5. Final check: all cross-references valid, all annexes complete, confidence language consistent.
6. Release with QC documentation attached.

### After dissemination

1. Track forecasts and predictions for calibration.
2. When outcomes known, compare to predictions.
3. Document accuracy: hit/miss, magnitude of error, cause of error.
4. Feed lessons into training and process improvement.
5. Periodic process review: are standards being met? Where are systematic weaknesses?

## Data requirements

- Product checklist for each assessment type.
- Peer review capacity.
- Red team capacity for high-stakes products.
- Forecast/outcome tracking system.
- Consumer feedback mechanism.
- Error documentation system.

## Approved public sources

QC operates on the products themselves, not external sources. However, process QC may use external benchmarks (other analytical products, academic assessments) for comparison.

## Source verification standards

QC verifies that source verification was performed correctly — not just that sources exist. Check: were sources independently verified? Was corroboration real? Were contradictions disclosed?

## Analytical framework

### Product QC checklist

| Dimension | Checks |
|---|---|
| Evidence | All sources verified? Corroboration real? Contradictions disclosed? |
| Reasoning | Conclusion follows? Alternatives tested? Assumptions checked? |
| Confidence | Matches evidence? Language calibrated? Uncertainty disclosed? |
| Completeness | All questions addressed? Gaps identified? Annexes complete? |
| Clarity | Understandable? Well-structured? Consumer-appropriate? |
| Timeliness | Delivered when needed? Collection efficient? |
| Documentation | Reasoning traceable? Sources cited? QC documented? |

### Process QC metrics

| Metric | What it measures | Target |
|---|---|---|
| Verification rate | % of load-bearing claims verified | >95% |
| Calibration | Stated confidence vs. actual accuracy | Within 10% |
| Red team findings | Issues caught before release | Trending down |
| Consumer satisfaction | Consumer ratings | >80% satisfied |
| Error rate | Assessments proven wrong | Trending down |
| Timeliness | Products delivered on time | >90% on time |

## Evidence requirements

- QC documentation for each product: who reviewed, findings, revisions.
- Calibration records: forecasts vs. outcomes.
- Error analyses: why assessments failed.
- Process review documentation.
- Consumer feedback records.

## Confidence assessment

QC affects achievable confidence:

- Product passing all QC → confidence per evidence standard.
- Product with minor QC findings → confidence may be reduced or conditions noted.
- Product failing QC → not disseminated; revised or withdrawn.
- Systematic QC failures → process review triggered; standards may need revision.

## Common analytical mistakes

- QC as rubber stamp: checking boxes without genuine review.
- Peer review by friends or same-team members (shared blind spots).
- Not tracking calibration — never learning from errors.
- Treating QC as cost center rather than quality investment.
- Inconsistent standards across products or analysts.
- Not documenting QC — no audit trail.
- Ignoring consumer feedback.
- Process QC neglected — product QC alone insufficient.
- Red team for everything (wastes resources) or nothing (misses errors).

## Ethical considerations

QC must be honest: findings reported truthfully, revisions genuine, standards applied consistently. Must not be used to suppress inconvenient analyses or to delay time-sensitive warnings for perfection. QC protects consumers; it must not become a tool for control.

## Security boundaries

QC is internal process. No QC findings shared externally without authorization. QC does not authorize additional collection beyond OSINT scope.

## Expected output

Product: QC documentation attached (reviewer, findings, revisions). Process: periodic QC report with metrics, calibration results, error analysis, improvement recommendations.

## Quality checklist

- [ ] Self-check completed before submission.
- [ ] Peer review conducted for all products.
- [ ] Red team for high-stakes products.
- [ ] Findings adjudicated and addressed.
- [ ] QC documentation attached.
- [ ] Calibration tracked for forecasts.
- [ ] Error analysis conducted for failures.
- [ ] Process review periodic.
- [ ] Consumer feedback collected.
- [ ] Standards updated based on findings.

## Cross-reference links

- [`red_team_analytical_review.md`](red_team_analytical_review.md) — adversarial review.
- [`analytical_reasoning.md`](analytical_reasoning.md) — quality foundation.
- [`analytical_confidence_language.md`](analytical_confidence_language.md) — confidence standards.
- [`cognitive_bias_mitigation.md`](cognitive_bias_mitigation.md) — bias controls.
- [`intelligence_gap_assessment.md`](intelligence_gap_assessment.md) — gap handling.
- [`../core/analytical_standards.md`](../core/analytical_standards.md) — doctrine.
- [`../verification/verification_quality_metrics.md`](../verification/verification_quality_metrics.md) — verification metrics.
- [`../reporting/qc_documentation_template.md`](../reporting/qc_documentation_template.md) — output format.
