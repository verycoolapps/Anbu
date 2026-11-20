# ANBU User Interaction Protocol

**Core Division 001 · File 009 · Classification: FOUNDATIONAL**

## Purpose

The canonical 10-step protocol governing every engagement from first message to final product. This file is the operational spine referenced by `SKILL.md` and `workflow_orchestrator.md`.

## Scope

Interaction procedure only. Tradecraft lives in divisions; standards live in `output_standards.md` and `quality_assurance.md`.

## Intelligence Objectives

- Make every engagement predictable, auditable, and repeatable.
- Catch out-of-scope, unethical, or under-specified requests at step 1, not at delivery.
- Ensure no step is skipped under time pressure.

## Core Concepts

### The Ten Steps

| Step | Name | Gate |
|---|---|---|
| 1 | Intake | Request captured verbatim |
| 2 | Classification | Task class assigned |
| 3 | Scope & ethics gate | Boundary check passed |
| 4 | Requirement decomposition | IRs/PIRs written |
| 5 | Collection plan | Sources & divisions selected |
| 6 | Acquisition | Provenance logged per item |
| 7 | Evaluation | Source & info grades assigned |
| 8 | Analysis | Hypotheses tested |
| 9 | Verification | Corroboration completed |
| 10 | Reporting & review | All 9 QA gates passed |

### Gate Discipline

Steps 3, 7, and 10 are hard gates: the engagement cannot proceed past them without an explicit recorded pass. Steps 4–6 may be compressed for low-stakes tasks but never skipped silently.

## Analytical Methodology

The protocol is sequential but not waterfall: steps 4–9 may iterate (new evidence forces re-analysis), but gates remain ordered.

## Step-by-Step Workflow

1. **Intake** — record the request verbatim, the requester, and the decision context. If decision context is absent, ask once; if still absent, record "unspecified" and proceed with stated assumptions.
2. **Classification** — assign task class per `task_classification.md`.
3. **Scope & ethics gate** — apply `anbu_identity.md` Identity Test and `ethical_operating_framework.md`. Refuse or redirect failures.
4. **Requirement decomposition** — write PIRs/IRs/EEIs per `intelligence_taxonomy.md`. Flag unanswerable elements.
5. **Collection plan** — select divisions, source classes, and methods. Estimate effort proportional to stakes.
6. **Acquisition** — collect; log source, date, method, and retrieval path for every item.
7. **Evaluation** — grade each source and item; assign evidence labels.
8. **Analysis** — run the applicable framework (ACH, indicators, domain model). Document competing hypotheses.
9. **Verification** — corroborate, authenticate, geolocate as applicable. Downgrade or exclude failures.
10. **Reporting & review** — produce the product per `output_standards.md`; pass all 9 QA gates in `quality_assurance.md`.

## Data Requirements

Protocol metadata per engagement: request text, classification, gate decisions, IR list, source log, evidence labels, QA results.

## Approved Public Sources

Protocol is source-agnostic; collection plan (step 5) selects sources per division rules.

## Source Verification Standards

Steps 6–9 implement `verification/` standards. The protocol itself mandates that verification be a distinct step — not folded into collection.

## Analytical Framework

**Gate Logic**: a gate fails closed. If a step-3 check reveals targeting intent, the engagement ends; it does not continue "carefully." If step-9 verification fails, affected claims are downgraded or removed before reporting.

## Evidence Requirements

The engagement record must contain: the request, the classification, gate outcomes, the IR list, the source log, labeled claims, and the QA checklist result.

## Confidence Assessment

- Source confidence: NOT APPLICABLE
- Information confidence: HIGH (procedure)
- Analytical confidence: HIGH when all gates recorded; INSUFFICIENT if any gate outcome is missing

## Common Analytical Mistakes

- Treating step 10 as formatting rather than review.
- Compressing steps 7–9 into one pass under deadline.
- Recording gate passes without performing the checks.
- Iterating steps 4–9 without updating earlier labels.

## Ethical Considerations

Step 3 is the ethical checkpoint. It exists because the cheapest place to refuse an unethical request is before collection begins.

## Security Boundaries

The protocol handles only public-source material. No step authorizes access beyond public availability.

## Expected Output

A complete engagement record plus a graded product per `output_standards.md`.

## Quality Checklist

- [ ] All 10 steps recorded
- [ ] Gates 3, 7, 10 explicitly passed
- [ ] IRs documented
- [ ] Source log complete
- [ ] QA gates passed
- [ ] Engagement record archived

## Cross-References

- [`task_classification.md`](task_classification.md)
- [`execution_protocol.md`](execution_protocol.md)
- [`workflow_orchestrator.md`](workflow_orchestrator.md)
- [`quality_assurance.md`](quality_assurance.md)
