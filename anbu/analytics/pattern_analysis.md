# Pattern Analysis

**ANBU Division 008 · Analytics**

---

## Purpose

Pattern analysis identifies recurring structures in events, behavior, and data — and, critically, distinguishes real patterns from the patterns humans inevitably find in noise. This file defines how ANBU analysts establish that a pattern exists, characterize it, and assess whether it carries predictive or explanatory value.

## Scope

Applied to event sequences, behavioral regularities, institutional outputs, conflict incident data, procurement cycles, rhetorical patterns, and any dataset where recurrence is claimed. Complements trend analysis (direction of change) and timeline analysis (sequence structure) by focusing on repetition and regularity.

## Intelligence objectives

- Establish whether an observed recurrence is statistically or behaviorally meaningful.
- Characterize pattern properties: frequency, periodicity, regularity, scope.
- Determine whether a pattern supports prediction, explanation, or merely description.
- Reject illusory patterns before they contaminate assessments.

## Core concepts

- **Pattern.** A regularity that repeats beyond chance expectation — in timing, form, participants, or sequence.
- **Base-rate expectation.** How often the pattern would appear by chance given the number of observations and the phenomenon's natural frequency.
- **Apophenia.** The human tendency to perceive patterns in random data; the central failure mode this file guards against.
- **Periodic vs. episodic patterns.** Cyclical regularity (budget cycles, exercises) vs. triggered recurrence (responses to specific stimuli).
- **Pattern scope.** Whether the pattern holds across actors, regions, and time, or is an artifact of one context.
- **Pattern breakdown.** Patterns end; identifying decay conditions is part of analysis.

## Analytical methodology

1. Define the candidate pattern precisely: what repeats, among whom, over what period.
2. Enumerate all instances; check for selection bias in which instances were noticed.
3. Establish the base rate: how often would this occur by chance?
4. Test regularity: timing distribution, form consistency, participant overlap.
5. Seek disconfirming instances — cases where the pattern should have appeared but did not.
6. Characterize the pattern and assess its stability.
7. Determine utility: prediction, explanation, or description only.
8. Report with explicit confidence and the pattern's known boundaries.

## Step-by-step workflow

1. Receive or extract the candidate pattern claim.
2. Build the instance list with dates, sources, and verification status.
3. Count total opportunities for the pattern to occur (denominator).
4. Compute or estimate the expected frequency under a null (random) model.
5. Compare observed vs. expected; assess significance honestly, including small-sample limits.
6. Look for the pattern's exceptions and ask what distinguishes them.
7. Cross-check against `timeline_analysis.md` for sequence context.
8. Write the pattern statement: existence confidence, characterization, boundaries, utility.

## Data requirements

- Complete instance enumeration, not a cherry-picked subset.
- Denominator data: total events in the relevant class.
- Long enough series for the pattern's claimed period.
- For quantitative patterns: dataset with methodology documentation.

## Approved public sources

Incident databases (ACLED, UCDP where applicable); official gazettes and procurement records; election results series; parliamentary voting records; corporate filing timelines; court dockets; conflict event datasets; official exercise schedules.

## Source verification standards

Pattern claims are especially exposed to selection bias; instances must come from comprehensive datasets, not news impressions. Verify each instance per `../verification/`; an unverified instance weakens the pattern claim.

## Analytical framework

Pattern validity tests:

| Test | Question |
|---|---|
| Frequency | Does it occur more than chance expectation? |
| Regularity | Is timing/form consistent? |
| Completeness | Were all instances and opportunities enumerated? |
| Scope | Does it hold across contexts or is it local? |
| Exceptions | What cases break it, and why? |
| Mechanism | Is there a reason the pattern should exist? |

## Evidence requirements

- Instance list with citations and dates.
- Denominator and base-rate reasoning documented.
- Exception analysis included.
- Small-sample caveats stated where applicable.

## Confidence assessment

- **HIGH** — pattern robust across multiple contexts, mechanism identifiable, exceptions explained.
- **MODERATE** — pattern consistent in the observed window but limited scope or unexplained exceptions.
- **LOW** — few instances, possible selection bias, or weak base-rate comparison.
- **INSUFFICIENT** — instances too few or data too incomplete to establish any pattern.

## Common analytical mistakes

- Finding patterns in small samples (with 3 events, almost anything "repeats").
- Selection bias: noticing instances that fit while missing non-instances.
- Ignoring the denominator — no idea how often the pattern could have occurred.
- Retro-fitting pattern descriptions to whatever the data show.
- Treating a pattern as a law; most patterns are contingent and decay.
- Confusing pattern with coincidence driven by a common third cause.

## Ethical considerations

Pattern claims about groups (e.g., "community X always responds violently") risk essentializing and harming lawful communities. Patterns must be stated with scope limits and never used to predict individual behavior.

## Security boundaries

Pattern analysis uses public data only. Patterns must not be constructed to profile private individuals or to support targeting of lawful actors.

## Expected output

Pattern annex: instance table, base-rate analysis, regularity measures, exceptions, confidence. Main product states the pattern's existence confidence and its predictive limits.

## Quality checklist

- [ ] All instances and opportunities enumerated.
- [ ] Base rate or null expectation addressed.
- [ ] Exceptions analyzed, not hidden.
- [ ] Scope limits stated.
- [ ] Mechanism hypothesized or acknowledged as absent.
- [ ] Confidence reflects sample size and completeness.

## Cross-reference links

- [`trend_analysis.md`](trend_analysis.md) — directional change vs. recurrence.
- [`timeline_analysis.md`](timeline_analysis.md) — sequence and periodicity.
- [`hypothesis_testing.md`](hypothesis_testing.md) — testing pattern significance.
- [`indicators_and_signposts.md`](indicators_and_signposts.md) — patterns become signposts.
- [`correlation_vs_causation.md`](correlation_vs_causation.md) — pattern ≠ cause.
- [`analytical_reasoning.md`](analytical_reasoning.md) — reasoning foundation.
- [`../verification/evidence_grading.md`](../verification/evidence_grading.md) — instance grading.
- [`../workflows/collection_to_assessment_pipeline.md`](../workflows/collection_to_assessment_pipeline.md) — data pipeline.
