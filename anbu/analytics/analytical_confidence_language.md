# Analytical Confidence Language

**ANBU Division 008 · Analytics**

---

## Purpose

Confidence language is how analysts communicate the strength of their judgments to consumers. Vague or inflated confidence undermines the entire intelligence product — consumers cannot make good decisions if they cannot calibrate how much to trust the analysis. This file defines ANBU's estimative language standards, the mapping between evidence quality and confidence terms, and the rules for honest uncertainty communication.

## Scope

Applied to all analytical products: assessments, forecasts, warnings, indicators, and any statement expressing analytical judgment. Mandatory for all reporting. Governs both the confidence level assigned and the specific language used to express it.

## Intelligence objectives

- Ensure confidence statements accurately reflect evidence quality.
- Provide consumers with calibrated language they can act on.
- Prevent both overconfidence (which misleads) and underconfidence (which paralyzes).
- Create consistency across products so consumers can compare confidence across assessments.
- Make uncertainty explicit rather than hidden in hedged prose.

## Core concepts

- **Estimative language.** Words and phrases that convey probability or confidence — "likely," "probable," "we assess," "we judge." These must be defined and used consistently.
- **Confidence vs. probability.** Confidence is the analyst's certainty in the assessment; probability is the estimated likelihood of the event. They are related but distinct.
- **Evidence-based confidence.** Confidence derives from evidence quality, source reliability, and analytical rigor — not from how certain the analyst feels.
- **Calibration.** The match between stated confidence and actual accuracy over time. Well-calibrated analysts say "likely" and are right ~70% of the time.
- **Uncertainty disclosure.** Explicitly stating what is unknown, what would change the assessment, and what evidence is missing.
- **Consumer calibration.** Different consumers need different levels of detail; the language must work for the stated audience.

## Analytical methodology

1. Assess evidence quality per `../verification/evidence_grading.md`.
2. Determine confidence level per the rubric below.
3. Select estimative language matching the confidence level.
4. Add uncertainty disclosure: key assumptions, missing evidence, disconfirmers.
5. Verify language consistency throughout the product.
6. For forecasts: state probability range, not just confidence.

## Confidence levels and estimative language

| Level | Definition | Estimative language | Probability range |
|---|---|---|---|
| HIGH | Multiple independent high-quality sources; no credible alternatives survive; robust analysis | "We assess with high confidence," "Almost certainly," "We judge it highly likely" | 80–95% |
| MODERATE | Solid evidence base; some gaps or credible alternatives partially excluded | "We assess," "Likely," "We judge" | 55–80% |
| LOW | Thin evidence; significant gaps; credible alternatives unresolved | "We assess with low confidence," "Possibly," "We cannot rule out" | 20–55% |
| INSUFFICIENT | Evidence inadequate for any defensible judgment | "We cannot assess," "Insufficient evidence," "Unknown" | N/A |

### Usage rules

- **HIGH confidence** requires: multiple independent sources, high source reliability, completed SATs, red team review, no surviving credible alternatives.
- **MODERATE** is the default for most assessments; it signals "we have a defensible view but acknowledge limits."
- **LOW** must be stated explicitly; do not bury low confidence in hedged language.
- **INSUFFICIENT** triggers `intelligence_gap_assessment.md` — the product reports the gap, not a guess.

### Probability language for forecasts

When the question is probabilistic ("will X happen?"), use probability ranges:

- "Very likely" = 80–95%
- "Likely" = 60–80%
- "Roughly even chance" = 40–60%
- "Unlikely" = 20–40%
- "Very unlikely" = 5–20%
- "Remote" = <5%

Avoid false precision: "73.4%" implies accuracy the evidence cannot support. Use ranges: "approximately 70%" or "60–80%."

## Step-by-step workflow

1. Complete the analytical work (collection, verification, SATs).
2. Determine evidence quality and confidence level.
3. Draft the assessment using appropriate estimative language.
4. Add uncertainty disclosure: key assumptions, missing evidence, what would change the assessment.
5. Review language consistency: same confidence level = same language throughout.
6. For forecasts: add probability range and timeframe.
7. Verify no language overstates or understates the evidence.

## Data requirements

- Completed evidence base with verification grades.
- Confidence level determined per rubric.
- Consumer profile: who reads this and what decisions it informs.
- Forecast context: timeframe, event definition for probability statements.

## Approved public sources

N/A — this is a communication standard applied to all sources.

## Source verification standards

Confidence language must reflect verified evidence only. Unverified sources cap confidence at LOW regardless of how compelling the claims appear.

## Analytical framework

Language calibration examples:

| Evidence state | Wrong | Right |
|---|---|---|
| Strong multi-source | "It is certain that..." | "We assess with high confidence that..." |
| Moderate evidence | "This proves that..." | "We assess that..." |
| Thin evidence | "We believe that..." | "We assess with low confidence that... possibly..." |
| No evidence | "It seems that..." | "We cannot assess; evidence is insufficient." |

## Evidence requirements

- Confidence level stated explicitly for each major judgment.
- Uncertainty disclosure included: assumptions, gaps, disconfirmers.
- Language consistent throughout product.
- Probability ranges for forecasts, not point estimates.
- Consumer can calibrate trust based on stated confidence.

## Confidence assessment

This file governs how confidence is expressed; it does not itself assess confidence. The confidence levels defined here are applied across all analytics products.

## Common analytical mistakes

- Using "we believe" or "we think" instead of "we assess" (implies opinion, not analysis).
- Hedging everything: "it could possibly maybe" — provides no calibration.
- Overconfidence: "clearly," "obviously," "undoubtedly" on moderate evidence.
- Underconfidence: burying a strong assessment in excessive hedging.
- Inconsistent language: "high confidence" in summary, "possibly" in detail.
- False precision: exact percentages without statistical basis.
- Missing uncertainty disclosure: no mention of what would change the assessment.
- Treating confidence as binary (confident/not confident) instead of graded.

## Ethical considerations

Analysts must not inflate confidence to make products seem more valuable, nor deflate it to avoid accountability. Confidence language must honestly reflect evidence so consumers can make informed decisions. Politically inconvenient confidence levels must still be stated.

## Security boundaries

Confidence language must not be manipulated to justify classified or sensitive collection. All boundaries from `../security/` apply to the underlying analysis.

## Expected output

All products include: explicit confidence level per judgment, estimative language consistent with level, uncertainty disclosure, and probability ranges for forecasts.

## Quality checklist

- [ ] Confidence level stated explicitly.
- [ ] Estimative language matches evidence quality.
- [ ] Uncertainty disclosure included.
- [ ] Language consistent throughout.
- [ ] Probability ranges for forecasts.
- [ ] No false precision.
- [ ] Consumer can calibrate trust.

## Cross-reference links

- [`analytical_reasoning.md`](analytical_reasoning.md) — reasoning foundation.
- [`cognitive_bias_mitigation.md`](cognitive_bias_mitigation.md) — overconfidence control.
- [`risk_probability_assessment.md`](risk_probability_assessment.md) — probability estimation.
- [`intelligence_gap_assessment.md`](intelligence_gap_assessment.md) — INSUFFICIENT handling.
- [`red_team_analytical_review.md`](red_team_analytical_review.md) — confidence attack.
- [`../verification/evidence_grading.md`](../verification/evidence_grading.md) — evidence quality input.
- [`../reporting/assessment_template.md`](../reporting/assessment_template.md) — language in output.
- [`../core/analytical_standards.md`](../core/analytical_standards.md) — doctrine.
