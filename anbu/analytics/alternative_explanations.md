# Alternative Explanations

**ANBU Division 008 · Analytics**

---

## Purpose

Every observation supports multiple explanations. The analyst's first plausible explanation is almost always the most cognitively available, not the most probable. Alternative explanations discipline the analysis by forcing genuine consideration of rival accounts — including the null hypothesis — before a conclusion is reached. This file defines how ANBU generates, evaluates, and documents alternative explanations.

## Scope

Applied to all analytical products where a conclusion is drawn from ambiguous evidence. Mandatory for assessments above MODERATE confidence requirements and for all ACH applications. Also used standalone when a consumer asks "what else could explain this?"

## Intelligence objectives

- Prevent premature closure on the first plausible explanation.
- Ensure the hypothesis space covers the plausible range, including uncomfortable alternatives.
- Provide discriminators that distinguish between rival explanations.
- Document that alternatives were genuinely considered, not dismissed.

## Core concepts

- **Hypothesis space.** The set of explanations consistent with the available evidence. The analyst's job is to map this space, not just pick a point.
- **Null hypothesis.** The default explanation: nothing unusual is happening; the observation is routine, coincidental, or already explained.
- **Competing explanations.** Genuinely different accounts that fit the same evidence — not minor variations of the preferred one.
- **Discriminator.** Evidence that distinguishes between explanations — what would we see if A rather than B were true?
- **Occam's razor vs. complexity.** Simpler explanations are preferred all else equal, but not always correct — sometimes the complex explanation is true.
- **Mirror explanation.** The alternative that the actor's stated rationale is true rather than a hidden motive.
- **Adversarial alternative.** The explanation that best serves the analyst's or consumer's interests — often the most important to test.

## Analytical methodology

1. State the preferred explanation and its evidence.
2. Generate alternatives systematically:
   - Null hypothesis (nothing unusual).
   - Mirror explanation (stated rationale is true).
   - Adversarial explanation (benefits the analyst/consumer).
   - Structural explanation (incentives, constraints, not intent).
   - Coincidence explanation (unrelated events, common cause).
   - Deception explanation (evidence is planted or misleading).
3. For each alternative, specify what evidence would support it.
4. Identify discriminators: evidence that differs between explanations.
5. Evaluate each against the evidence honestly.
6. Document: which alternatives were considered, which eliminated, why.
7. If alternatives remain viable, lower confidence accordingly.

## Step-by-step workflow

1. Write the preferred explanation.
2. Run the alternative-generation checklist (null, mirror, adversarial, structural, coincidence, deception).
3. For each alternative, ask: what evidence would we expect if this were true?
4. Check whether the evidence actually discriminates.
5. Eliminate alternatives only with cited evidence — not with "implausible."
6. If multiple alternatives survive, use `analysis_of_competing_hypotheses.md`.
7. Document the alternative space in the product annex.
8. Adjust confidence based on surviving alternatives.

## Data requirements

- The evidence base supporting the preferred explanation.
- Enough evidence breadth to test alternatives fairly.
- Collection capacity to seek discriminating evidence.
- Willingness to consider uncomfortable alternatives.

## Approved public sources

Same as the main assessment — alternatives are tested against the same evidence base. Additional sources may be sought specifically to discriminate.

## Source verification standards

Alternatives must be evaluated against verified evidence, not against the absence of evidence. "We found no evidence for X" is not evidence against X unless we looked and the evidence would have been observable.

## Analytical framework

Alternative generation checklist:

| Type | Question | Example |
|---|---|---|
| Null | Is this just routine? | Policy change is normal cycle, not response to crisis |
| Mirror | Is the stated reason true? | Official rationale matches behavior |
| Adversarial | Does it serve interests? | Assessment conveniently supports preferred policy |
| Structural | Do incentives explain it? | Budget pressures, not strategic intent |
| Coincidence | Are events unrelated? | Two events happened simultaneously by chance |
| Deception | Is evidence misleading? | Statements designed to deceive observers |

## Evidence requirements

- Preferred explanation stated with evidence.
- At least 3 alternatives generated (more for high-stakes).
- Each alternative evaluated against evidence.
- Eliminations cite specific evidence.
- Surviving alternatives disclosed with their implications.
- Null hypothesis explicitly addressed.

## Confidence assessment

Confidence is directly reduced by surviving alternatives:

- **HIGH** — alternatives generated and eliminated by discriminating evidence.
- **MODERATE** — alternatives considered; most eliminated; one or two remain weakly viable.
- **LOW** — significant alternatives remain viable; evidence does not discriminate.
- **INSUFFICIENT** — cannot generate meaningful alternatives; evidence too thin.

## Common analytical mistakes

- Generating strawman alternatives that are easy to dismiss.
- Skipping the null hypothesis.
- Eliminating alternatives with "implausible" instead of evidence.
- Not generating the adversarial alternative (the one that hurts).
- Treating absence of evidence as evidence of absence.
- Generating alternatives after the conclusion is fixed (post-hoc).
- Failing to document alternatives that were considered.

## Ethical considerations

Alternative explanations must be generated honestly, including those that undermine desired conclusions. Analysts must not suppress alternatives for political convenience. The adversarial alternative — the one that challenges the consumer's interests — must be included when relevant.

## Security boundaries

Same boundaries as main assessment. Alternative explanations do not justify additional collection beyond public sources.

## Expected output

Alternatives annex: preferred explanation, alternative list with evaluation, discriminators identified, surviving alternatives, confidence impact. Main product notes alternatives were considered.

## Quality checklist

- [ ] Preferred explanation stated clearly.
- [ ] At least 3 genuine alternatives generated.
- [ ] Null hypothesis explicitly addressed.
- [ ] Adversarial alternative included.
- [ ] Eliminations cite evidence, not plausibility.
- [ ] Surviving alternatives disclosed.
- [ ] Confidence adjusted for surviving alternatives.

## Cross-reference links

- [`analysis_of_competing_hypotheses.md`](analysis_of_competing_hypotheses.md) — formal discrimination.
- [`hypothesis_testing.md`](hypothesis_testing.md) — testing rival propositions.
- [`key_assumptions_check.md`](key_assumptions_check.md) — assumptions behind explanations.
- [`cognitive_bias_mitigation.md`](cognitive_bias_mitigation.md) — bias that suppresses alternatives.
- [`red_team_analytical_review.md`](red_team_analytical_review.md) — external alternative attack.
- [`analytical_reasoning.md`](analytical_reasoning.md) — reasoning foundation.
- [`../reporting/annex_templates.md`](../reporting/annex_templates.md) — output format.
