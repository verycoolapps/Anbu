# ANBU Task Classification

**Core Division 001 · File 011 · Classification: FOUNDATIONAL**

## Purpose

The decision procedure for assigning every incoming request a task class. Classification determines effort, divisions engaged, QA depth, and ethical scrutiny. It is step 2 of the interaction protocol.

## Scope

Classification criteria and classes only. Decomposition into requirements is `intelligence_taxonomy.md`; execution is `execution_protocol.md`.

## Intelligence Objectives

- Match analytical effort to decision stakes.
- Route requests to the minimum sufficient division set.
- Surface ethical or scope problems at the cheapest possible point.

## Core Concepts

### Task Classes

| Class | Name | Description | Effort | QA depth |
|---|---|---|---|---|
| T1 | Lookup | Single-fact retrieval from authoritative source | Minimal | Light |
| T2 | Profile | Durable reference product on an entity/system | Moderate | Standard |
| T3 | Assessment | Graded judgment on a developing situation | Standard | Full |
| T4 | Forecast | Predictive estimate with confidence bounds | High | Full + review |
| T5 | Warning | Time-sensitive alert on emerging risk | High, fast | Full, expedited |
| T6 | Audit | Review of prior ANBU product for quality | Standard | Meta-review |
| TX | Out-of-scope | Refused or redirected | — | — |

### Classification Signals

- **Time horizon**: "right now" → T5 candidate; "this year" → T3/T4; "for reference" → T2.
- **Decision stakes**: procurement, policy, investment → higher class; curiosity → lower.
- **Source availability**: if the answer lives in one authoritative document → T1; if it requires synthesis → T3+.
- **Uncertainty tolerance**: "definitive answer" on an uncertain question → reclassify or decline.

## Analytical Methodology

Classification is a judgment, so it is documented: the assigned class, the signals used, and the rationale are recorded in the engagement log. Borderline cases default upward (more scrutiny, not less).

## Step-by-Step Workflow

1. Parse the request for horizon, stakes, and source hints.
2. Match against class definitions.
3. Check for TX triggers (targeting, operational harm, classified-adjacent asks).
4. Assign class; record rationale.
5. If borderline, assign the higher class and note the ambiguity.

## Data Requirements

Classification needs only the request text plus any stated context. No collection occurs before classification.

## Approved Public Sources

Not applicable at this step; source selection happens at step 5.

## Source Verification Standards

Not applicable; inherited by the classified task.

## Analytical Framework

**Effort–Stakes Matching**: class determines ceiling on acceptable error. T1 tolerates little ambiguity because the answer is checkable; T4 tolerates and discloses wide confidence bounds.

## Evidence Requirements

The classification record requires: request text, assigned class, signals observed, TX check result, and reviewer note if borderline.

## Confidence Assessment

- Source confidence: NOT APPLICABLE
- Information confidence: HIGH for clear cases, MODERATE for borderline
- Analytical confidence: HIGH (bounded decision)

## Common Analytical Mistakes

- Classifying by requested format rather than decision need ("make it a report" ≠ T3).
- Under-classifying to save effort — the error cost exceeds the saved cost.
- Treating TX as a judgment call; TX triggers are bright-line.

## Ethical Considerations

Classification is the first ethical filter. A request that pattern-matches to individual targeting, doxxing, or operational harm is TX regardless of how it is phrased.

## Security Boundaries

TX includes requests for classified information, access credentials, or exploitation of systems. Classification does not create access; it only routes.

## Expected Output

A classification record embedded in the engagement log, plus the effort/QA profile the class dictates.

## Quality Checklist

- [ ] Class assigned from defined set
- [ ] Rationale recorded
- [ ] TX triggers checked
- [ ] Borderline cases escalated upward
- [ ] Effort proportional to class

## Cross-References

- [`intelligence_taxonomy.md`](intelligence_taxonomy.md)
- [`user_interaction_protocol.md`](user_interaction_protocol.md)
- [`quality_assurance.md`](quality_assurance.md)
- [`ethical_operating_framework.md`](ethical_operating_framework.md)
