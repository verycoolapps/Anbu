# Analytical Reasoning — Foundation

**ANBU Division 008 · Analytics**

---

## Purpose

Analytical reasoning is the disciplined process of converting collected information into defensible judgment. This file defines the reasoning standard applied across every ANBU product: how analysts move from raw reporting to an assessed conclusion, how they expose the chain between evidence and judgment, and how they prevent the most common failure mode of intelligence work — confident narration without analytical structure.

## Scope

Applies to all ANBU analytical products: strategic assessments, indicators analyses, forecasts, network studies, and warning products. It does not replace the structured techniques catalogued in `structured_analytic_techniques.md`; it governs the reasoning posture underneath them.

## Intelligence objectives

- Make the inferential steps between evidence and conclusion explicit and auditable.
- Separate observation (what sources report) from inference (what the analyst concludes).
- Ensure every judgment carries an honest statement of confidence and the evidence that would change it.
- Preserve intellectual honesty when the evidence base is thin.

## Core concepts

- **Observation vs. inference.** An observation is what a source states or what a document shows. An inference is what the analyst concludes from it. Products must never blur the two.
- **The analytical chain.** Evidence → hypothesis → competing hypotheses → assessment → confidence statement. Each link must be defensible.
- **Transparent reasoning.** The reader should be able to retrace why a conclusion follows, not merely accept that it does.
- **Falsifiability.** A good assessment states what evidence would disconfirm it. An unfalsifiable claim is not analysis; it is assertion.
- **Epistemic humility.** The analyst's confidence is a property of the evidence, not of the analyst's certainty.

## Analytical methodology

1. Restate the intelligence question in precise terms.
2. Inventory the evidence: what is directly observed, what is reported secondhand, what is inferred.
3. Identify the hypotheses the evidence could support, including the null hypothesis.
4. Test each hypothesis against the evidence; record what supports and what contradicts.
5. Select the assessment that best fits the evidence while surviving the strongest competing explanation.
6. Attach a confidence statement and name the evidence that would change the assessment.

## Step-by-step workflow

1. Receive the tasking or self-generated question.
2. Read `core/user_interaction_protocol.md` requirements and classify the task.
3. Gather relevant collection through `../osint/` methods.
4. Verify source reliability and information credibility per `../verification/` standards.
5. Apply the relevant structured technique(s) from `structured_analytic_techniques.md`.
6. Draft the reasoning chain explicitly: evidence items, hypotheses tested, disconfirming evidence sought.
7. Run `key_assumptions_check.md` and `cognitive_bias_mitigation.md` passes.
8. Write the assessment in `../reporting/` format with estimative confidence language.
9. Submit to `red_team_analytical_review.md` before dissemination.

## Data requirements

- Dated, attributable reporting for every factual claim.
- A defined intelligence question or decision the analysis informs.
- Where possible, at least two independent sources for load-bearing facts.
- Explicit treatment of missing data as a gap, not as silence.

## Approved public sources

Government publications and statistics offices; official registers and gazettes; court records and legislative archives; academic literature; reputable journalism with stated sourcing; corporate disclosures; think-tank and NGO reports used as leads requiring independent corroboration; satellite and geospatial open data via `../geoint/`.

## Source verification standards

Every fact entering the reasoning chain must pass the verification gate in `../verification/`: provenance established, authenticity assessed, corroboration status recorded. Unverified items may inform hypotheses but may not carry an assessment on their own. See `../verification/source_authenticity_verification.md` and `../verification/corroboration_standards.md`.

## Analytical framework

The ANBU reasoning frame has four layers:

| Layer | Question | Output |
|---|---|---|
| Evidence | What do we actually know? | Verified fact list with provenance |
| Hypothesis | What explanations fit? | Competing hypotheses with discriminators |
| Assessment | Which explanation survives? | Judgment with confidence and disconfirmers |
| Communication | What does the decision-maker need? | Product in reporting format |

## Evidence requirements

- Every assertion in the assessment traceable to a cited source or labeled as analyst inference.
- Direct evidence distinguished from circumstantial evidence.
- Contradictory evidence included, not suppressed.
- Single-source claims flagged and confidence downgraded accordingly.

## Confidence assessment

Confidence statements use the estimative scale defined in `analytical_confidence_language.md`:

- **HIGH** — multiple independent corroborations, high-quality sources, no credible competing explanation surviving scrutiny.
- **MODERATE** — solid but incomplete corroboration, or credible alternatives only partially excluded.
- **LOW** — thin evidence, single-source dependence, or strong competing hypotheses unresolved.
- **INSUFFICIENT** — evidence base cannot support any defensible judgment; report the gap per `intelligence_gap_assessment.md`.

## Common analytical mistakes

- Treating repetition of one report across outlets as corroboration.
- Anchoring on the first plausible explanation and failing to test alternatives.
- Presenting inference with the same certainty as observation.
- Ignoring evidence that does not fit the preferred hypothesis.
- Producing a narrative instead of an argument with discriminators.

## Ethical considerations

Analysts must not construct assessments intended to enable targeting, harassment, or operational harm against individuals. Predictions about individuals require higher evidentiary standards than institutional analysis. Uncertainty must be disclosed honestly rather than exploited to push a preferred narrative. See `../security/ethical_boundaries.md`.

## Security boundaries

All inputs are public-source. No classified material, no leaked private data, no purchased breach data. The analyst must refuse requests that would require non-public collection, intrusion, or doxxing. Outputs must not include operational detail that materially enables harm.

## Expected output

A reasoning-chain appendix or inline evidence mapping attached to the final product, listing: question, evidence items with source grades, hypotheses considered, disconfirming evidence sought, and the confidence rationale.

## Quality checklist

- [ ] Question stated precisely and tied to a decision or requirement.
- [ ] Every fact has provenance and verification status.
- [ ] Competing hypotheses were genuinely tested, not strawmen.
- [ ] Confidence language matches the evidence standard.
- [ ] Disconfirming evidence is disclosed.
- [ ] Reasoning is reproducible by a second analyst.

## Cross-reference links

- [`structured_analytic_techniques.md`](structured_analytic_techniques.md) — the technique catalog applied after this foundation.
- [`analysis_of_competing_hypotheses.md`](analysis_of_competing_hypotheses.md) — formal hypothesis discrimination.
- [`cognitive_bias_mitigation.md`](cognitive_bias_mitigation.md) — bias controls applied during reasoning.
- [`analytical_confidence_language.md`](analytical_confidence_language.md) — estimative language standard.
- [`../core/analytical_standards.md`](../core/analytical_standards.md) — division-wide doctrine.
- [`../verification/source_authenticity_verification.md`](../verification/source_authenticity_verification.md) — input gate.
- [`../reporting/assessment_template.md`](../reporting/assessment_template.md) — output format.
- [`../workflows/collection_to_assessment_pipeline.md`](../workflows/collection_to_assessment_pipeline.md) — end-to-end process.
