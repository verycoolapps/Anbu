# Analysis of Competing Hypotheses (ACH)

**ANBU Division 008 · Analytics**

---

## Purpose

ACH is the primary hypothesis-discrimination technique in ANBU. It forces the analyst to treat evidence as a discriminator between explanations rather than as support for a preferred story. This file defines the procedure, the diagnostic-evidence standard, and the pitfalls specific to matrix-based analysis.

## Scope

Applied when two or more plausible explanations exist for an observed development and the available evidence can discriminate between them. Not applied to single-hypothesis questions or purely descriptive tasks.

## Intelligence objectives

- Identify which evidence actually separates rival hypotheses.
- Prevent confirmation bias by requiring evidence to be scored against every hypothesis.
- Produce an audit trail showing why each hypothesis was retained or eliminated.
- Surface "evidence that does not fit" instead of forcing it into the favored narrative.

## Core concepts

- **Hypothesis set.** A minimum of two genuinely competing explanations; a single-hypothesis matrix is not ACH.
- **Diagnostic evidence.** Evidence that is consistent with one hypothesis and inconsistent with at least one other. Only diagnostic evidence drives elimination.
- **Non-diagnostic evidence.** Evidence consistent with all hypotheses — it may be true and still useless for discrimination.
- **Inconsistency.** Evidence that contradicts a hypothesis counts against it; ACH scores both directions.
- **Elimination logic.** Hypotheses are eliminated by accumulated inconsistency, not by a single knockout — though a decisive disconfirmation can eliminate immediately.

## Analytical methodology

The matrix is evidence (rows) × hypotheses (columns). Each cell is scored: consistent (C), inconsistent (I), or not applicable/not diagnostic (N). Scoring must be justified per cell. After scoring, count inconsistencies per hypothesis; the hypothesis with the fewest inconsistencies and most diagnostic support survives.

## Step-by-step workflow

1. **Define the question and hypotheses.** Write 2–5 mutually exclusive hypotheses covering the plausible space, including a null hypothesis ("nothing unusual is happening"). Avoid strawman alternatives.
2. **Assemble evidence.** List only verified evidence items; each gets a citation. Include contradictory items.
3. **Build the matrix.** Rows = evidence items; columns = hypotheses. Score each cell with justification.
4. **Identify diagnostics.** Mark which evidence items discriminate; weight them accordingly.
5. **Evaluate.** For each hypothesis, count inconsistencies; note which diagnostics support it.
6. **Re-examine.** Re-read the matrix looking for scoring errors and for evidence that fits no hypothesis.
7. **Conclude.** State which hypothesis(ves) survive, with confidence per `analytical_confidence_language.md`.
8. **Document.** File the matrix as an annex; summarize the reasoning in the main product.

## Data requirements

- Verified evidence items with source grades.
- Hypotheses developed before scoring begins.
- A clear decision the discrimination serves.
- Enough evidence for at least a few diagnostic items; if all evidence is non-diagnostic, the answer is INSUFFICIENT.

## Approved public sources

Primary documents and official statements for key claims; statistical series for quantitative hypotheses; reporting from multiple independent outlets only after corroboration; imagery/geospatial where relevant via `../geoint/`.

## Source verification standards

Every matrix row must trace to a verified source. If an evidence item's verification grade is low, it may be included but must be marked and its weight reduced. See `../verification/corroboration_standards.md`.

## Analytical framework

Scoring conventions used across ANBU:

- **C (consistent):** the evidence supports the hypothesis as stated.
- **I (inconsistent):** the evidence contradicts the hypothesis or is what the hypothesis predicts will not occur.
- **N (neutral):** consistent with all hypotheses or irrelevant.
- **? (uncertain):** evidence quality too poor to score; flagged for collection follow-up.

Weighting: diagnostic items outweigh non-diagnostic. Recent evidence may outweigh stale evidence when the question concerns current intent. High-credibility sources outweigh low-credibility ones at equal diagnostic value.

## Evidence requirements

- Each matrix cell has a one-line justification.
- The annex lists sources for every row.
- Inconsistent evidence is scored honestly — suppressing it is a defect.
- Evidence that fits no hypothesis is reported separately as a possible indicator of a missing hypothesis.

## Confidence assessment

- **HIGH** — surviving hypothesis holds against all credible alternatives; diagnostics are strong and multi-sourced.
- **MODERATE** — survivor leads on diagnostics but a credible alternative retains support.
- **LOW** — evidence is thin or mostly non-diagnostic; matrix cannot cleanly separate hypotheses.
- **INSUFFICIENT** — no diagnostic evidence exists; report as an intelligence gap.

## Common analytical mistakes

- Building the matrix after the conclusion is already favored.
- Counting non-diagnostic evidence as support.
- Making hypotheses non-exclusive or overlapping so nothing can be eliminated.
- Treating one inconsistent cell as fatal without weighing totality.
- Failing to include the null hypothesis, producing forced discrimination.
- "Cleaning" the matrix by removing inconvenient rows.

## Ethical considerations

ACH may be used on individuals only when the question is lawful protective or accountability analysis, and even then conclusions must stay at the confidence the evidence supports. The technique must never be tuned to produce a desired elimination.

## Security boundaries

ACH operates on public-source evidence only. It does not authorize collection escalation, surveillance, or targeting. Outputs are assessments, not operational products.

## Expected output

Annex: the completed matrix with per-cell justifications and source citations. Main product: 1–3 paragraphs stating surviving hypothesis(ves), key diagnostics, eliminated alternatives with reasons, and confidence.

## Quality checklist

- [ ] At least two genuine, mutually exclusive hypotheses plus a null.
- [ ] All rows verified and cited.
- [ ] Every cell scored with justification.
- [ ] Diagnostic vs non-diagnostic distinguished.
- [ ] Misfits reported, not hidden.
- [ ] Confidence assigned after matrix review, not before.

## Cross-reference links

- [`structured_analytic_techniques.md`](structured_analytic_techniques.md) — SAT catalog and selection matrix.
- [`hypothesis_testing.md`](hypothesis_testing.md) — probabilistic complement to ACH.
- [`key_assumptions_check.md`](key_assumptions_check.md) — tests the assumptions behind hypotheses.
- [`alternative_explanations.md`](alternative_explanations.md) — ensures rivals are genuine.
- [`analytical_reasoning.md`](analytical_reasoning.md) — reasoning foundation.
- [`cognitive_bias_mitigation.md`](cognitive_bias_mitigation.md) — bias controls for matrix scoring.
- [`../verification/evidence_grading.md`](../verification/evidence_grading.md) — source grades for rows.
- [`../reporting/annex_templates.md`](../reporting/annex_templates.md) — matrix template.
- [`../workflows/hypothesis_driven_collection.md`](../workflows/hypothesis_driven_collection.md) — collection that feeds the matrix.
