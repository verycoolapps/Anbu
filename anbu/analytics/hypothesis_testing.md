# Hypothesis Testing

**ANBU Division 008 · Analytics**

---

## Purpose

Hypothesis testing in ANBU is the disciplined evaluation of propositions against evidence — closer to the intelligence use of the term than the strict statistical one, though statistical testing applies where quantitative data exist. This file defines how analysts state hypotheses precisely, derive testable expectations, and update confidence as evidence accumulates.

## Scope

Applied when a question admits a definite answer assessable by evidence: did X happen, will Y occur, is Z the correct explanation. Complements ACH (which discriminates between competing explanations) by focusing on single-proposition evaluation and sequential evidence updating.

## Intelligence objectives

- State hypotheses in falsifiable form before evidence review.
- Derive discriminating expectations: what would we observe if true, if false?
- Update confidence systematically rather than by impression.
- Prevent both over- and under-reaction to new evidence.

## Core concepts

- **Falsifiable hypothesis.** A proposition that evidence could prove wrong. "The actor intends aggression" is weakly falsifiable; "the actor will move forces across the border within 90 days" is strongly falsifiable.
- **Expectation.** The observable consequence a hypothesis predicts. Strong hypotheses generate multiple, specific expectations.
- **Likelihood ratio thinking.** How much more probable is the evidence under the hypothesis than under its negation? This is the Bayesian intuition made explicit.
- **Base rate.** How often the hypothesized event occurs absent special conditions. Ignoring base rates produces wild estimates.
- **Sequential updating.** Confidence changes as evidence arrives; the product should state the update rule, not just the final number.

## Analytical methodology

1. Formulate the hypothesis as a testable proposition with a time bound and scope.
2. State the null/alternative explicitly.
3. Derive 3–7 expectations: observables predicted if true, and observables predicted if false.
4. Collect evidence against each expectation.
5. Score: expectation confirmed / disconfirmed / unobservable.
6. Update confidence: how many independent expectations confirmed, weighted by diagnosticity and source quality.
7. Report with estimative language and name residual uncertainties.

## Step-by-step workflow

1. Define the proposition precisely (actor, action, timeframe, threshold).
2. Write expectations before seeking evidence for them.
3. Task collection per `../workflows/hypothesis_driven_collection.md`.
4. For each expectation, gather verified evidence; record confirmed/disconfirmed/unobservable.
5. Apply `analysis_of_competing_hypotheses.md` if rival hypotheses compete for the same evidence.
6. Update confidence using the rubric below; document the update.
7. Write the result with disconfirmers disclosed.

## Data requirements

- A bounded, falsifiable proposition.
- Observable expectations tied to public sources.
- Evidence graded per `../verification/` standards.
- Where quantitative: sufficient data for the chosen test and awareness of its assumptions.

## Approved public sources

Official statistics and time series; legislative and regulatory records; procurement and budget documents; corporate disclosures; court records; election data; public opinion series with documented methodology; satellite and geospatial data via `../geoint/`.

## Source verification standards

Expectations are tested only against verified evidence. Statistical tests additionally require scrutiny of methodology, sampling, and conflicts of interest in the publishing body per `../verification/statistical_source_review.md`.

## Analytical framework

Confidence update rubric (qualitative):

- Expectation confirmed by multiple independent high-credibility sources → strong support.
- Confirmed by one credible source → moderate support.
- Mixed results across expectations → confidence stays low; investigate which expectation failed and why.
- Key expectation unobservable → cap confidence at MODERATE and flag the gap.

Statistical tests (t-tests, chi-square, trend tests) are appropriate only when data meet their assumptions; the analyst must state the test, the null, and the result's limits.

## Evidence requirements

- Every expectation has a stated observable and its evidence status.
- Disconfirmed expectations are reported, not dropped.
- Statistical claims cite dataset, method, and caveats.
- The proposition's timeframe is explicit — expired propositions are archived, not silently carried.

## Confidence assessment

- **HIGH** — most expectations confirmed by independent quality sources; disconfirmers searched and absent.
- **MODERATE** — core expectations confirmed but key ones unobservable or partially supported.
- **LOW** — evidence mixed; proposition plausible but expectations largely untested.
- **INSUFFICIENT** — expectations cannot be observed in public sources; report gap.

## Common analytical mistakes

- Testing a vague proposition that nothing could disprove.
- Deriving expectations after seeing the evidence (post-hoc rationalization).
- Ignoring base rates — treating a rare event's occurrence as meaningful without context.
- Counting repeated reports of one underlying claim as independent confirmations.
- Updating confidence on narrative plausibility rather than expectation results.
- Applying statistical tests without checking assumptions.

## Ethical considerations

Predictions about individuals require stronger evidence than institutional predictions. Hypothesis testing must never be used to construct guilt-by-pattern or to predict private behavior from public fragments.

## Security boundaries

Testing uses public sources only. No hypothesis may justify collection beyond OSINT scope. Predictions must include uncertainty adequate for lawful decision-making.

## Expected output

A test record: proposition, expectations with status, evidence citations, confidence update, and residual disconfirmers — annexed to the product, with the verdict summarized in the main text.

## Quality checklist

- [ ] Proposition is falsifiable, bounded, and time-stamped.
- [ ] Expectations written before evidence collection.
- [ ] Each expectation has verified evidence or an explicit unobservable flag.
- [ ] Base rate considered.
- [ ] Disconfirmers disclosed.
- [ ] Statistical tests justified or absent with reason.

## Cross-reference links

- [`analysis_of_competing_hypotheses.md`](analysis_of_competing_hypotheses.md) — multi-hypothesis discrimination.
- [`causal_analysis.md`](causal_analysis.md) — distinguishes prediction from explanation.
- [`correlation_vs_causation.md`](correlation_vs_causation.md) — guards against false inference.
- [`indicators_and_signposts.md`](indicators_and_signposts.md) — observables become indicators.
- [`trend_analysis.md`](trend_analysis.md) — quantitative hypothesis context.
- [`analytical_reasoning.md`](analytical_reasoning.md) — reasoning foundation.
- [`../verification/statistical_source_review.md`](../verification/statistical_source_review.md) — data quality.
- [`../workflows/hypothesis_driven_collection.md`](../workflows/hypothesis_driven_collection.md) — collection loop.
