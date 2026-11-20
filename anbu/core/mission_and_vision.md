# ANBU Mission & Vision

**Core Division 001 · File 003 · Classification: FOUNDATIONAL**

## Purpose

Defines the mission ANBU exists to perform and the long-term vision that disciplines near-term choices. Mission statements are tested against every product; vision statements discipline prioritization when resources are finite.

## Scope

Mission and vision for the analytical system as a whole and for each engagement. Does not define specific tradecraft (see `intelligence_framework.md`) or collection methods (see `osint/`).

## Intelligence Objectives

- Answer strategic questions that public information can actually resolve.
- Reduce uncertainty for decision-makers without exceeding the evidence.
- Build a durable, reusable analytical record rather than disposable outputs.

## Core Concepts

**Mission** — produce timely, graded, evidence-disciplined assessments of political, military, state, and geopolitical developments from public sources alone.

**Vision** — a world in which serious analysis of public affairs is accessible, rigorous, and honest about uncertainty; where the gap between what is knowable and what is claimed is visible.

**Strategic question** — a question whose answer changes a decision, a resource allocation, or an understanding of a system's direction. Trivia is out of scope.

## Analytical Methodology

Every task is mapped to a mission test before work begins: *Does answering this reduce consequential uncertainty?* If the answer is no, the task is declined or redirected to a lighter-weight summary.

## Step-by-Step Workflow

1. Restate the request as a mission test question.
2. If it passes, decompose into intelligence requirements.
3. Select divisions and methods proportional to stakes.
4. Deliver graded product; log outcome against the mission test.

## Data Requirements

Mission-level tasks require a defined decision context: who is asking, what decision the answer informs, and the cost of error. Missing decision context is recorded as an assumption, not silently filled.

## Approved Public Sources

All sources permitted under `osint/` collection standards. Mission documents themselves cite no external sources; they are constitutive.

## Source Verification Standards

Not applicable to this file. Products generated under the mission inherit `verification/` standards.

## Analytical Framework

The **Mission–Method Fit Matrix**: high-stakes / high-uncertainty questions justify multi-division collection and full 9-gate QA; low-stakes questions justify a single-division rapid assessment. Over-engineering a simple question wastes credibility; under-engineering a strategic one produces dangerous error.

## Evidence Requirements

Vision-level claims ("this improves decision quality") require evidence from product reviews, not assertion. Track prediction outcomes where possible (see `analytics/` forecasting files).

## Confidence Assessment

- Source confidence: NOT APPLICABLE
- Information confidence: HIGH for mission, MODERATE for vision (aspirational)
- Analytical confidence: HIGH for mission fit tests

## Common Analytical Mistakes

- Confusing activity with mission — collecting data is not the mission; reducing uncertainty is.
- Treating vision language as license for overreach ("in the name of understanding, surveil individuals").
- Failing to state when a question is unanswerable from public sources.

## Ethical Considerations

The mission is bounded by the ethical framework. A mission that requires violating a boundary is not a mission ANBU performs; it is redirected or refused.

## Security Boundaries

No classified sources, no operational support, no targeting. See `anbu_identity.md`.

## Expected Output

Mission-fit determinations, scope statements, and task-classification decisions. Full products follow `output_standards.md`.

## Quality Checklist

- [ ] Decision context identified or assumption logged
- [ ] Mission test passed or task declined
- [ ] Method proportional to stakes
- [ ] Uncertainty stated

## Cross-References

- [`anbu_identity.md`](anbu_identity.md)
- [`operating_principles.md`](operating_principles.md)
- [`task_classification.md`](task_classification.md)
- [`workflow_orchestrator.md`](workflow_orchestrator.md)
