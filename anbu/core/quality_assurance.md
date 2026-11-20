# ANBU Quality Assurance

**Core Division 001 · File 016 · Classification: FOUNDATIONAL**

## Purpose

Defines the 9 quality gates every ANBU product must pass before delivery, plus the QA process that applies them. QA is step 10 of the interaction protocol made concrete.

## Scope

Quality gates and review procedure. It does not define analytical methods; it judges whether methods were applied correctly.

## Intelligence Objectives

- Catch defects that individual analyst judgment misses.
- Make quality auditable: every delivered product has a recorded gate result.
- Protect consumers from plausible-looking but unsound analysis.

## Core Concepts

### The Nine Gates

| # | Gate | Question it answers |
|---|---|---|
| 1 | RELEVANCE | Does the product answer the classified requirement? |
| 2 | SOURCE QUALITY | Are sources appropriate to the claim's weight? |
| 3 | AUTHENTICITY | Is the material what it claims to be? |
| 4 | CORROBORATION | Is each significant claim independently confirmed? |
| 5 | ANALYTICAL RIGOR | Were sound methods applied and documented? |
| 6 | UNCERTAINTY | Is uncertainty stated specifically and honestly? |
| 7 | BIAS CONTROL | Were known biases identified and countered? |
| 8 | ETHICAL SAFETY | Does the product respect all boundaries? |
| 9 | REPORT QUALITY | Does the product meet output standards? |

### Gate Severity

- **Blocking** — gates 3, 4, 8: failure stops delivery until resolved.
- **Corrective** — gates 1, 2, 5, 6, 7, 9: failure requires revision; delivery may proceed only with documented waiver and reason.

### The QA Record

Every product carries a QA record: gate-by-gate result, reviewer, date, waivers with justification. The record is part of the product.

## Analytical Methodology

QA is a separate pass, ideally by a different analyst or a fresh-context review. Self-review is permitted only for T1–T2 products and must be labeled as such.

## Step-by-Step Workflow

1. Assemble the product and evidence log.
2. Apply gates 1–9 in order.
3. Record PASS / FAIL / WAIVED per gate with notes.
4. Resolve blocking failures; document corrective waivers.
5. Attach QA record; deliver.

## Data Requirements

QA record schema: `gate | result | reviewer | notes | waiver_reason`.

## Approved Public Sources

QA judges the product, not the sources' legality — but gate 3 (authenticity) and gate 8 (ethics) do examine source handling.

## Source Verification Standards

Gate 4 operationalizes `verification/` standards: significant claims need independent corroboration or explicit downgrade.

## Analytical Framework

**Gate Independence**: passing eight gates does not compensate for failing one. Gates are conjunctive, not compensatory.

## Evidence Requirements

A product without a QA record is undelivered regardless of content quality.

## Confidence Assessment

- Source confidence: NOT APPLICABLE
- Information confidence: HIGH for gate definitions
- Analytical confidence: HIGH when QA record is complete; INSUFFICIENT when review was skipped

## Common Analytical Mistakes

- Treating QA as proofreading.
- Waiving gates without recorded justification.
- Reviewing only the product, not the evidence log behind it.
- Letting deadline pressure convert blocking failures into waivers.

## Ethical Considerations

Gate 8 is the ethical checkpoint at delivery: it catches harm that survived earlier gates — e.g., a technically sound product that enables targeting.

## Security Boundaries

QA records contain no sensitive data beyond the product itself; they are stored with the engagement record.

## Expected Output

Delivered product + attached QA record showing all gates resolved.

## Quality Checklist

- [ ] All 9 gates evaluated
- [ ] Blocking failures resolved or delivery stopped
- [ ] Waivers documented with reasons
- [ ] QA record attached
- [ ] Review performed as separate pass

## Cross-References

- [`output_standards.md`](output_standards.md)
- [`user_interaction_protocol.md`](user_interaction_protocol.md)
- [`verification/`](../verification/)
- [`ethical_operating_framework.md`](ethical_operating_framework.md)
