# Causal Analysis

**ANBU Division 008 · Analytics**

---

## Purpose

Causal analysis asks not just what happened or what will happen, but why — and whether a proposed cause actually produces the observed effect. In OSINT, most available evidence supports correlation far more readily than causation. This file defines how ANBU analysts evaluate causal claims, construct causal arguments, and resist the pervasive temptation to narrate sequences as causes.

## Scope

Applied when a product must explain a development (why did the government fall, why did the policy change) or evaluate a causal claim embedded in reporting ("sanctions caused the currency collapse"). Prediction tasks without explanatory requirements may rely on `hypothesis_testing.md` instead.

## Intelligence objectives

- Distinguish genuine causal mechanisms from coincidental co-occurrence.
- Build causal arguments that specify mechanism, not just sequence.
- Evaluate competing causal explanations on evidence, not plausibility.
- Warn consumers when a product's causal language exceeds its evidence.

## Core concepts

- **Causal mechanism.** The process by which a cause produces an effect — the "how," not just the "that." "A caused B" is incomplete; "A changed incentives which led actors to do X producing B" is a mechanism.
- **Necessary vs. sufficient cause.** A necessary cause must be present for the effect; a sufficient cause produces it on its own. Most real-world causes are neither purely one nor the other.
- **Causal chain.** Multi-step causation where each link must hold; chains break at their weakest link.
- **Confounders.** Third variables that produce both the proposed cause and the effect, generating spurious causation.
- **Reverse causation.** Effect preceding cause — common in political and economic data.
- **Equifinality.** Multiple different causes producing the same outcome; observing the outcome does not identify the cause.

## Analytical methodology

1. State the causal claim precisely: cause, effect, proposed mechanism, timeframe.
2. Specify the mechanism step by step.
3. Identify rival causal explanations for the same effect.
4. Look for confounders and check temporal ordering (cause before effect).
5. Seek discriminating evidence: predictions that differ between causal stories.
6. Test each link of the chain; a chain is only as strong as its weakest verified link.
7. Report the causal assessment with explicit confidence and named alternatives.

## Step-by-step workflow

1. Extract causal claims from the tasking or draft.
2. For each claim, write the mechanism in one paragraph.
3. Build a rival-cause list via `alternative_explanations.md`.
4. Check temporal ordering against `timeline_analysis.md` output.
5. Evaluate confounders using domain knowledge and `political_economy_analysis.md` where relevant.
6. Score each mechanism link: verified / plausible / speculative.
7. Compose the causal section: strongest-supported explanation, credible rivals, and what evidence would discriminate.
8. Flag any causal language in the final product that outruns the evidence.

## Data requirements

- Time-ordered evidence establishing sequence.
- Evidence about the proposed mechanism (statements of intent, observed behavioral responses, institutional changes).
- Data on confounders where quantitative claims are involved.
- Ideally, a natural experiment or policy discontinuity — rare in OSINT; acknowledge when absent.

## Approved public sources

Legislative debates and voting records revealing motive; budget reallocations; official statements before and after events; academic causal studies; court findings of fact; pre/post statistics from official series; investigative journalism with documented sourcing.

## Source verification standards

Causal claims are especially vulnerable to motivated reasoning; every link in the mechanism must trace to verified evidence. Journalistic causal assertions ("X led to Y") are treated as claims to test, not evidence.

## Analytical framework

Causal argument structure:

| Element | Requirement |
|---|---|
| Cause | Verified to have occurred, correctly timed |
| Mechanism | Each step plausible and at least partly evidenced |
| Effect | Verified to have occurred after the cause |
| Alternatives | Credible rival causes enumerated and weighed |
| Discriminators | Evidence that would distinguish the causal stories |

## Evidence requirements

- Temporal precedence documented.
- Mechanism links individually cited.
- Rival causes addressed, not ignored.
- Causal confidence never exceeds the weakest chain link's evidence grade.

## Confidence assessment

- **HIGH** — mechanism fully evidenced, alternatives excluded by discriminating evidence, timing confirmed.
- **MODERATE** — mechanism plausible and partially evidenced; alternatives possible but less supported.
- **LOW** — sequence established but mechanism speculative; multiple rival causes viable.
- **INSUFFICIENT** — cannot establish even temporal ordering reliably; describe correlation only.

## Common analytical mistakes

- Post hoc ergo propter hoc — sequence mistaken for causation.
- Single-cause bias — attributing a complex outcome to one driver.
- Ignoring equifinality — assuming the observed cause is the only possible one.
- Accepting actors' stated motives as the true cause without corroboration.
- Building a plausible-sounding mechanism with no evidentiary links.
- Confusing predictive success with causal understanding.

## Ethical considerations

Causal claims about individuals or groups can carry defamatory weight; they require higher evidentiary standards and careful language. Analysts must not construct causal narratives that serve to justify harm against lawful actors.

## Security boundaries

Causal analysis is confined to public evidence. No causal claim may be used to infer private intent beyond what public statements and behavior support, and products must not enable targeting.

## Expected output

Causal annex: claim, mechanism chain with per-link evidence status, rival causes, discriminators, and confidence. Main product summarizes the best-supported causal story with honest hedging.

## Quality checklist

- [ ] Cause precedes effect in verified timeline.
- [ ] Mechanism specified step-by-step.
- [ ] Rival causes enumerated and weighed.
- [ ] Confounders considered.
- [ ] Each chain link has evidence status.
- [ ] Causal language calibrated to evidence strength.

## Cross-reference links

- [`correlation_vs_causation.md`](correlation_vs_causation.md) — the foundational distinction.
- [`timeline_analysis.md`](timeline_analysis.md) — establishes temporal precedence.
- [`alternative_explanations.md`](alternative_explanations.md) — rival causes.
- [`political_economy_analysis.md`](political_economy_analysis.md) — structural causal drivers.
- [`hypothesis_testing.md`](hypothesis_testing.md) — prediction vs. explanation.
- [`analytical_reasoning.md`](analytical_reasoning.md) — reasoning foundation.
- [`../verification/evidence_grading.md`](../verification/evidence_grading.md) — link grading.
- [`../reporting/assessment_template.md`](../reporting/assessment_template.md) — output format.
