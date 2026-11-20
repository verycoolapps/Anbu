# Risk Probability Assessment

**ANBU Division 008 · Analytics**

---

## Purpose

Risk probability assessment estimates how likely an event is to occur within a defined timeframe and scope — and how uncertain that estimate is. It is the bridge between analysis (what might happen) and decision (what to prepare for). This file defines how ANBU analysts estimate probabilities from incomplete public evidence, communicate them honestly, and avoid the systematic biases that distort likelihood judgment.

## Scope

Applied to event forecasting (elections, conflicts, policy changes, institutional crises), risk assessment for programs and operations, and any question framed as "how likely is X?" Covers both discrete events and threshold crossings ("will spending exceed Y?").

## Intelligence objectives

- Produce defensible probability estimates for defined events.
- Communicate uncertainty honestly — probability is not precision.
- Identify the key drivers and the evidence that would change the estimate.
- Enable risk-based prioritization of collection and contingency planning.

## Core concepts

- **Probability estimate.** A numerical or estimative likelihood that an event occurs within a timeframe. Always conditioned on current evidence.
- **Reference class.** The set of similar past cases used to anchor the estimate. Choosing the right reference class is the core skill.
- **Base rate.** How often the event occurs in the reference class absent special information. The prior before case-specific evidence.
- **Likelihood adjustment.** How case-specific evidence moves the estimate from the base rate.
- **Time horizon.** Probability is time-bound; "will X happen?" is meaningless without "by when?"
- **Event definition.** The event must be precisely specified — vague events produce meaningless probabilities.
- **Overconfidence.** Humans systematically overestimate narrow probabilities and underestimate broad ones; calibration matters.
- **Scenario probability vs. conditional probability.** "P(A and B)" differs from "P(A|B)"; analysts must be explicit.

## Analytical methodology

1. Define the event precisely: actor, action, threshold, timeframe.
2. Select the reference class: comparable cases with outcome data.
3. Establish the base rate from the reference class.
4. Identify case-specific factors that differentiate this instance.
5. Adjust the estimate for each factor, direction and magnitude justified.
6. Check calibration: is the estimate overconfident? Underconfident?
7. State the estimate with confidence bounds and the evidence that would change it.
8. Document the reasoning chain for audit.

## Step-by-step workflow

1. Define the event: "Will [actor] [action] by [date]?" — precise enough to score.
2. Build the reference class: find comparable cases; document selection criteria.
3. Compute or estimate the base rate.
4. List differentiating factors: what makes this case more or less likely?
5. Adjust for each factor; record direction and rough magnitude.
6. Cross-check with `analysis_of_competing_hypotheses.md` if multiple outcomes compete.
7. Apply calibration check: compare to typical forecast performance; avoid extremes without strong evidence.
8. State estimate: probability range (not false precision), key drivers, disconfirmers.
9. File the probability annex with reference class and adjustment logic.

## Data requirements

- Event history data for the reference class (conflict datasets, election results, policy adoption records).
- Current indicators relevant to the event (via `indicators_and_signposts.md`).
- Expert judgment documented with reasoning.
- Time series for threshold events.
- For rare events: explicit acknowledgment that estimates are highly uncertain.

## Approved public sources

Conflict and crisis datasets (ACLED, UCDP); election results databases; legislative voting records; policy adoption timelines; central bank and market data for economic thresholds; official statistics for social indicators; historical analog databases; academic forecasting studies.

## Source verification standards

Reference class data must come from comprehensive datasets, not cherry-picked cases. Event definitions must match the reference class definitions. See `../verification/statistical_source_review.md`.

## Analytical framework

Probability estimation steps:

| Step | Question | Output |
|---|---|---|
| Definition | What exactly is the event? | Precise event statement |
| Reference class | What cases are comparable? | Selected cases + criteria |
| Base rate | How often does it occur? | Prior probability |
| Adjustments | What differentiates this case? | Factor list + directions |
| Estimate | What's the probability? | Range + confidence |
| Disconfirmers | What would change it? | Evidence triggers |

Estimative language for probability (see `analytical_confidence_language.md`):
- "Very likely" ≈ 80–95%
- "Likely" ≈ 60–80%
- "Roughly even chance" ≈ 40–60%
- "Unlikely" ≈ 20–40%
- "Very unlikely" ≈ 5–20%

## Evidence requirements

- Event definition precise and time-bounded.
- Reference class documented with selection criteria.
- Base rate cited.
- Adjustments justified individually.
- Disconfirmers stated.
- False precision avoided: ranges over point estimates.

## Confidence assessment

Confidence here is meta-confidence — confidence in the probability estimate itself:

- **HIGH** — strong reference class, clear differentiators, robust estimate.
- **MODERATE** — reasonable reference class; some uncertainty in adjustments.
- **LOW** — weak reference class or highly uncertain adjustments.
- **INSUFFICIENT** — no meaningful reference class or data; report inability to estimate.

## Common analytical mistakes

- Vague event definitions producing unscoreable estimates.
- Base-rate neglect: adjusting without an anchor.
- Overconfidence: narrow probability ranges on weak evidence.
- False precision: "73.4%" when the honest answer is "roughly 70%".
- Ignoring time horizon: probability without timeframe.
- Cherry-picking reference classes that support the preferred answer.
- Treating probability as destiny — a 30% event happens 30% of the time.
- Ignoring the possibility that the event definition itself is wrong.

## Ethical considerations

Probability estimates about conflict, instability, or harm must carry uncertainty adequate for responsible decision-making. Analysts must not produce estimates that serve to justify pre-emptive action without acknowledging uncertainty. Estimates about individuals require much higher evidence standards.

## Security boundaries

Public data only. No probability estimates based on classified intelligence. No estimates framed as targeting or threat lists. Estimates must support lawful decision-making.

## Expected output

Probability annex: event definition, reference class, base rate, adjustments, estimate range, confidence, disconfirmers. Main product states the estimate with estimative language and key drivers.

## Quality checklist

- [ ] Event precisely defined and time-bounded.
- [ ] Reference class documented.
- [ ] Base rate established.
- [ ] Adjustments justified individually.
- [ ] Estimate as range, not false precision.
- [ ] Disconfirmers stated.
- [ ] Calibration checked.

## Cross-reference links

- [`hypothesis_testing.md`](hypothesis_testing.md) — testing vs. estimating.
- [`indicators_and_signposts.md`](indicators_and_signposts.md) — probability signposts.
- [`trend_analysis.md`](trend_analysis.md) — trend-based probabilities.
- [`strategic_warning_analysis.md`](strategic_warning_analysis.md) — scenario likelihoods.
- [`analytical_confidence_language.md`](analytical_confidence_language.md) — estimative language.
- [`impact_assessment.md`](impact_assessment.md) — probability × impact = risk.
- [`../verification/statistical_source_review.md`](../verification/statistical_source_review.md) — data quality.
- [`../reporting/risk_matrix_template.md`](../reporting/risk_matrix_template.md) — output format.
