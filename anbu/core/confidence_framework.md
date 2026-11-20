# ANBU Confidence Framework

**Core Division 001 · File 017 · Classification: FOUNDATIONAL**

## Purpose

Defines the three-dimensional confidence model: SOURCE, INFORMATION, and ANALYTICAL confidence — how each is assessed, combined, and reported. Confidence is the system's honesty mechanism.

## Scope

Confidence doctrine only. Per-domain confidence cues live in division files; this file defines the model they feed into.

## Intelligence Objectives

- Prevent false precision: confidence must track evidence, not rhetorical need.
- Let consumers see *where* uncertainty lives — source, item, or inference.
- Enable calibration over time via prediction logging.

## Core Concepts

### The Three Dimensions

**SOURCE CONFIDENCE** — reliability of the origin.
- HIGH: official record, established institution, track record of accuracy.
- MODERATE: reputable journalism, established expert, consistent past performance.
- LOW: single unverified claim, unknown outlet, demonstrated errors.
- INSUFFICIENT: cannot be assessed (anonymous, no provenance).

**INFORMATION CONFIDENCE** — reliability of this specific item.
- HIGH: directly observed, officially documented, independently confirmed.
- MODERATE: single credible source, plausible but unconfirmed.
- LOW: hearsay, single weak source, internally inconsistent.
- INSUFFICIENT: cannot be evaluated.

**ANALYTICAL CONFIDENCE** — soundness of the inference.
- HIGH: strong evidence base, competing hypotheses tested, method appropriate.
- MODERATE: reasonable inference, material gaps remain.
- LOW: weak evidence, untested alternatives, method stretched.
- INSUFFICIENT: analysis cannot be supported (should not ship).

### Combination Rules

- Product confidence = the *weakest necessary* dimension for the claim's weight. A HIGH-source/HIGH-info claim with LOW analytical confidence is reported as LOW-confidence assessment.
- Confidence is never averaged into a single number in the body; the table reports all three.
- INSUFFICIENT on any blocking dimension stops delivery (per `quality_assurance.md`).

### Confidence Language

Use the four levels verbatim. Avoid "likely," "probably," "almost certainly" without mapping to a level — or better, state the level and the reasoning.

## Analytical Methodology

Confidence is assigned per claim cluster, not per product globally. The bottom line carries the analytical confidence of its weakest supporting chain.

## Step-by-Step Workflow

1. Grade each source (source confidence).
2. Grade each significant item (information confidence).
3. After analysis, grade each conclusion (analytical confidence).
4. Report all three in the confidence table.
5. Check combination rules; downgrade where required.

## Data Requirements

Confidence grades require documented reasoning: *why* HIGH, *why* LOW. Unreasoned grades are treated as absent.

## Approved Public Sources

Confidence assessment is method, not source — applies to any public source.

## Source Verification Standards

Source confidence feeds from `verification/` grading; information confidence from corroboration results.

## Analytical Framework

**Weakest-Link Reporting**: the consumer sees the binding constraint. If sources are excellent but inference is thin, the product says so — that is more useful than blanket confidence.

## Evidence Requirements

Every confidence grade in a product must cite the evidence or reasoning behind it. "MODERATE because single-source but credible" is acceptable; "MODERATE" alone is not.

## Confidence Assessment

- Source confidence: this framework IS the standard
- Information confidence: HIGH (constitutive)
- Analytical confidence: HIGH for the model; per-product grades vary

## Common Analytical Mistakes

- Collapsing three dimensions into one vague "confidence: medium."
- Upgrading confidence because the conclusion is important.
- Treating confidence as a property of the writer rather than the evidence.
- Reporting HIGH analytical confidence on a hypothesis that wasn't tested against alternatives.

## Ethical Considerations

Confidence honesty is the core ethical obligation: consumers make decisions on these labels. Inflated confidence is a harm even when conclusions are correct.

## Security Boundaries

Confidence labels do not create access or authorize action; they describe epistemic state only.

## Expected Output

Products with complete, reasoned, three-dimensional confidence tables.

## Quality Checklist

- [ ] All three dimensions graded
- [ ] Grades reasoned, not asserted
- [ ] Weakest-link rule applied
- [ ] INSUFFICIENT blocks delivery
- [ ] Language matches levels

## Cross-References

- [`uncertainty_management.md`](uncertainty_management.md)
- [`operating_principles.md`](operating_principles.md)
- [`output_standards.md`](output_standards.md)
- [`analytics/`](../analytics/)
