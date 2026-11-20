# Key Assumptions Check (KAC)

**ANBU Division 008 · Analytics**

---

## Purpose

Every assessment rests on assumptions — beliefs treated as true without direct evidence. Most analytical failures trace to an unchecked assumption, not to bad data. KAC systematically surfaces, ranks, and tests the assumptions an assessment depends on, concentrating effort where failure would hurt most.

## Scope

Applied to any assessment of MODERATE confidence or higher before dissemination, and mandatorily to strategic assessments, forecasts, and warning products. Also used standalone when a consumer asks "what are you assuming?"

## Intelligence objectives

- Make hidden premises explicit so consumers can judge the assessment's true foundation.
- Identify which assumptions, if false, would collapse or invert the conclusion.
- Direct limited collection effort toward testing fragile load-bearing assumptions.
- Reduce overconfidence produced by unexamined premises.

## Core concepts

- **Load-bearing assumption.** An assumption without which the assessment fails or reverses. These are the highest-priority targets.
- **Fragility.** The likelihood the assumption is false, judged from evidence.
- **Blast radius.** The impact on the conclusion if the assumption proves false.
- **Explicit vs. implicit assumptions.** Implicit assumptions are the dangerous ones — they are rarely stated and rarely tested.
- **Assumption hierarchy.** Not all assumptions matter equally; KAC ranks by fragility × blast radius.

## Analytical methodology

1. Draft the assessment's reasoning chain.
2. Extract every premise the chain requires — stated and unstated.
3. For each, assign fragility (evidence-supported likelihood of being true) and blast radius.
4. Rank by product of fragility and blast radius.
5. Test the top-ranked assumptions: seek confirming and disconfirming evidence.
6. Revise the assessment or downgrade confidence where assumptions remain untested and fragile.

## Step-by-step workflow

1. Write the assessment draft.
2. List assumptions in a table: assumption | fragility (H/M/L) | blast radius (H/M/L) | test result.
3. For each HIGH-priority assumption, define what evidence would confirm and what would disconfirm.
4. Task collection per `../workflows/hypothesis_driven_collection.md` for the disconfirming side.
5. Update the assessment: strengthen, hedge, or downgrade per results.
6. Record unresolved fragile assumptions in the product's uncertainty section.
7. File the KAC table as an annex.

## Data requirements

- The draft assessment with its reasoning chain visible.
- Evidence relevant to each assumption's truth value.
- Collection capacity to test at least the top-priority assumptions.

## Approved public sources

Official statements and doctrine documents for actor-behavior assumptions; budget and procurement records for capability assumptions; historical precedent datasets; expert literature for contextual assumptions; primary statistics for quantitative assumptions.

## Source verification standards

Assumption tests rest on the same verification standards as the main product. An assumption confirmed only by a single unverified report remains fragile.

## Analytical framework

Priority score = fragility × blast radius. Worked example:

| Assumption | Fragility | Blast radius | Priority |
|---|---|---|---|
| Actor retains decision-making autonomy | M | H | HIGH |
| Budget figures are accurate | L | M | MEDIUM |
| Public rhetoric reflects private intent | H | H | HIGH |

## Evidence requirements

- Each assumption states its basis: evidence, analogy, or pure inference.
- Tested assumptions cite the confirming/disconfirming evidence.
- Untested fragile assumptions are disclosed as such — never silently carried.

## Confidence assessment

KAC directly modulates confidence. An assessment resting on multiple untested HIGH-priority assumptions cannot exceed MODERATE confidence regardless of surface evidence quality. If a load-bearing assumption fails testing, the assessment must be revised or withdrawn.

## Common analytical mistakes

- Listing only assumptions the analyst already believes are true.
- Treating culturally convenient assumptions ("they will act rationally") as tested facts.
- Testing easy assumptions and skipping fragile ones.
- Assuming away the most uncomfortable premise.
- Forgetting implicit assumptions — mirror-imaging, rational-actor models, static intent.

## Ethical considerations

KAC must surface assumptions even when they undermine a politically preferred conclusion. Analysts must not selectively test assumptions that protect a desired outcome.

## Security boundaries

KAC is an internal quality procedure; it produces no additional collection requirements beyond public sources. It must never be used to justify intrusive verification of private individuals.

## Expected output

Annex: ranked assumption table with test results. Main product: explicit statement of load-bearing assumptions and any that remain unverified.

## Quality checklist

- [ ] Implicit assumptions extracted, not just explicit ones.
- [ ] Assumptions ranked by fragility × blast radius.
- [ ] Top-priority assumptions tested with cited evidence.
- [ ] Failed assumptions triggered revision or downgrade.
- [ ] Unresolved fragile assumptions disclosed.

## Cross-reference links

- [`analysis_of_competing_hypotheses.md`](analysis_of_competing_hypotheses.md) — hypotheses depend on assumptions.
- [`key_assumptions_check.md`](key_assumptions_check.md) — this file's canonical procedure reference in other products.
- [`intelligence_gap_assessment.md`](intelligence_gap_assessment.md) — untested assumptions become gaps.
- [`cognitive_bias_mitigation.md`](cognitive_bias_mitigation.md) — mirror-imaging bias check.
- [`analytical_reasoning.md`](analytical_reasoning.md) — reasoning chain that exposes assumptions.
- [`../core/analytical_standards.md`](../core/analytical_standards.md) — doctrine requiring KAC.
- [`../verification/source_authenticity_verification.md`](../verification/source_authenticity_verification.md) — evidence for tests.
- [`../workflows/collection_to_assessment_pipeline.md`](../workflows/collection_to_assessment_pipeline.md) — where KAC sits.
