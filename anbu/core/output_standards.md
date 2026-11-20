# ANBU Output Standards

**Core Division 001 · File 015 · Classification: FOUNDATIONAL**

## Purpose

Defines what every ANBU product must contain, how it is structured, and the minimum quality bar for delivery. This file is the contract between analysis and the consumer.

## Scope

Product structure and content requirements. Report format templates live in `reporting/`; this file defines the invariants every product must satisfy regardless of format.

## Intelligence Objectives

- Make products comparable across engagements.
- Ensure no product ships without uncertainty, sourcing, and confidence statements.
- Give consumers a predictable reading experience.

## Core Concepts

### Mandatory Product Elements

Every ANBU product, regardless of length or class, contains:

1. **Header block** — product ID, date, classification of task, evidence-label summary.
2. **Bottom line** — the assessment in 1–3 sentences, with confidence.
3. **Key judgments** — each labeled ASSESSMENT or INFERENCE with its evidence trail.
4. **Evidence basis** — sources cited with labels and confidence.
5. **Uncertainty statement** — what is unknown, what would change the assessment.
6. **Falsification conditions** — observations that would overturn key judgments.
7. **Confidence table** — source / information / analytical confidence.
8. **Limitations** — scope, source, and method limits.
9. **Distribution note** — who this product is for and handling caveats.

### Product Classes

| Class | Format | Length guide |
|---|---|---|
| T1 lookup | Answer block + source | < 1 page |
| T2 profile | Structured reference | 2–10 pages |
| T3 assessment | Standard assessment | 3–8 pages |
| T4 forecast | Assessment + forecast annex | 5–12 pages |
| T5 warning | Alert format | 1–3 pages |
| T6 audit | QA report | Variable |

### The 20-Section Report

Full strategic products use the ANBU INTELLIGENCE REPORT template (see `reporting/`). Shorter classes use the mandatory elements above in compact form.

## Analytical Methodology

Standards are enforced by the quality gates (`quality_assurance.md`), not by reviewer taste. A product missing a mandatory element fails gate 9 regardless of analytical quality.

## Step-by-Step Workflow

1. Draft product with all mandatory elements.
2. Verify every claim carries a label.
3. Verify confidence table is populated on all three dimensions.
4. Verify uncertainty and falsification sections are substantive, not boilerplate.
5. Run QA gates; fix failures; deliver.

## Data Requirements

Product metadata: product ID, task class, division tags, evidence-label counts, confidence summary, QA result.

## Approved Public Sources

Products cite only sources collected under ANBU rules; every citation resolves to a logged evidence item.

## Source Verification Standards

Citations must match logged provenance. A citation that cannot be traced to the evidence log is a defect.

## Analytical Framework

**Consumer-First Structure**: the bottom line comes first; supporting detail follows. Readers who stop after the bottom line still receive a correctly graded assessment.

## Evidence Requirements

Minimum evidence for delivery: all mandatory elements present, all claims labeled, confidence stated, QA gates passed.

## Confidence Assessment

- Source confidence: reported per citation
- Information confidence: reported per claim cluster
- Analytical confidence: stated for the bottom line

## Common Analytical Mistakes

- Writing the report as a narrative instead of a graded product.
- Boilerplate uncertainty sections ("more research is needed") — name the specific gaps.
- Confidence tables with only one dimension filled.
- Bottom lines that overstate what the body supports.

## Ethical Considerations

Output standards are an ethical safeguard: mandatory uncertainty and limitations sections prevent consumers from mistaking assessment for fact.

## Security Boundaries

Products contain analysis of public information only. No product includes personal data beyond what is analytically necessary and publicly available.

## Expected Output

A graded, structured, complete ANBU product ready for the requester.

## Quality Checklist

- [ ] All mandatory elements present
- [ ] Every claim labeled
- [ ] Confidence table complete (3 dimensions)
- [ ] Uncertainty statement specific
- [ ] Falsification conditions stated
- [ ] QA gates passed
- [ ] Citations traceable to evidence log

## Cross-References

- [`reporting/`](../reporting/)
- [`quality_assurance.md`](quality_assurance.md)
- [`confidence_framework.md`](confidence_framework.md)
- [`uncertainty_management.md`](uncertainty_management.md)
