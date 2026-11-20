# Correlation vs. Causation

**ANBU Division 008 · Analytics**

---

## Purpose

Correlation is the co-occurrence of two phenomena; causation is one producing the other through a mechanism. Public data makes correlation easy to find and causation hard to prove, and intelligence consumers routinely over-read statistical association as explanation. This file establishes the discipline for keeping the two separate.

## Scope

Applied whenever a product presents statistical relationships, apparent patterns, or claims that one development drove another. Mandatory reading before any quantitative claim enters an assessment.

## Intelligence objectives

- Prevent spurious causal inference from coincidental patterns.
- Teach analysts to state relationship type honestly: correlation, plausible causation, or demonstrated causation.
- Provide the standard checklist for evaluating causal claims in source material.
- Protect products from the most common quantitative reasoning error in OSINT.

## Core concepts

- **Correlation.** Statistical association measured by coefficients, co-movement, or contingency. Says nothing about direction or mechanism.
- **Causation.** Requires mechanism, temporal precedence, and exclusion of confounders.
- **Spurious correlation.** Association produced by a third variable or by chance; both variables are effects of something else.
- **Directionality problem.** Correlation cannot tell which variable influences which; both may influence each other.
- **Ecological fallacy.** Relationships observed at group level do not necessarily hold for individuals.
- **Confounding.** A hidden variable producing the observed association.

## Analytical methodology

1. Identify the claimed relationship and its purported direction.
2. Establish whether the evidence shows correlation only, or also mechanism and timing.
3. Search for confounders: what third variable could produce both?
4. Check temporal precedence: which variable moved first?
5. Test rival causal directions.
6. Classify the relationship: demonstrated causation / plausible causation / correlation only / spurious.
7. Write the finding with the classification explicit.

## Step-by-step workflow

1. Extract every causal or correlational claim from the source material or draft.
2. For each, ask: what is the actual evidence — co-movement, mechanism description, or controlled comparison?
3. Apply the confounder search: list variables that plausibly drive both.
4. Check timing against `timeline_analysis.md`.
5. Where quantitative data exist, compute or cite the correlation and its limits; never extrapolate beyond the data's scope.
6. Assign the relationship classification.
7. Rewrite claims that overstate the relationship.

## Data requirements

- The datasets underlying any quantitative claim, with source and methodology.
- Time series sufficient to establish ordering.
- Where possible, a comparison group or period unaffected by the proposed cause.
- Awareness of data quality issues: revisions, definitional changes, missing periods.

## Approved public sources

Official statistics (with methodology documentation); central bank data; UN and multilateral datasets; academic replication datasets; corporate disclosures; election commissions; pre/post policy datasets.

## Source verification standards

Statistical claims require scrutiny of methodology per `../verification/statistical_source_review.md`. Correlations cited from secondary sources must be traced to the original dataset and computation where possible.

## Analytical framework

Relationship classification rubric:

| Classification | Required evidence |
|---|---|
| Demonstrated causation | Mechanism + timing + confounders excluded |
| Plausible causation | Mechanism described + timing consistent; confounders not fully excluded |
| Correlation only | Co-movement or association; no mechanism established |
| Spurious / coincidental | Association likely produced by third variable or chance |

## Evidence requirements

- Every relationship claim states its classification.
- Quantitative claims cite dataset, period, and method.
- Confounders considered are listed, even when none found.
- Language matches classification: "associated with" for correlation, "drove/caused" only for demonstrated causation.

## Confidence assessment

- **HIGH** — demonstrated causation with mechanism, timing, and rival explanations excluded.
- **MODERATE** — plausible causation; correlation plus partial mechanism evidence.
- **LOW** — correlation only; causal language would overstate.
- **INSUFFICIENT** — data quality or coverage too poor for even correlation claims.

## Common analytical mistakes

- "A and B move together, therefore A causes B."
- Ignoring reverse causation (economic decline causes unrest, not vice versa — or both).
- Cherry-picking the time window that shows the desired correlation.
- Treating correlation coefficients as effect sizes or probabilities.
- Ecological fallacy: inferring individual behavior from aggregate statistics.
- Assuming that because a policy and an outcome co-occur, the policy caused the outcome.

## Ethical considerations

Spurious causal claims can drive harmful policy conclusions or unjust accusations. Products must not present correlation as causation to make a narrative more compelling, and statistical relationships involving vulnerable groups require extra care.

## Security boundaries

Quantitative analysis uses public datasets only. No claims may be built on leaked or non-public data. Products must not enable targeting based on statistical associations alone.

## Expected output

Every statistical or causal claim in a product carries its classification label. Annex: dataset citations, confounder analysis, and any computations performed.

## Quality checklist

- [ ] Each relationship claim classified explicitly.
- [ ] Confounders searched and reported.
- [ ] Temporal ordering checked.
- [ ] Language calibrated to classification.
- [ ] Dataset and method cited for quantitative claims.
- [ ] No causal verb used for correlation-only findings.

## Cross-reference links

- [`causal_analysis.md`](causal_analysis.md) — building causal arguments.
- [`hypothesis_testing.md`](hypothesis_testing.md) — testing propositions.
- [`trend_analysis.md`](trend_analysis.md) — trend claims need this discipline.
- [`pattern_analysis.md`](pattern_analysis.md) — pattern vs. coincidence.
- [`analytical_reasoning.md`](analytical_reasoning.md) — reasoning foundation.
- [`cognitive_bias_mitigation.md`](cognitive_bias_mitigation.md) — motivated reasoning guard.
- [`../verification/statistical_source_review.md`](../verification/statistical_source_review.md) — data scrutiny.
- [`../reporting/assessment_template.md`](../reporting/assessment_template.md) — calibrated language.
