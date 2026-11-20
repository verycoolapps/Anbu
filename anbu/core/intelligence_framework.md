# ANBU Intelligence Framework

**Core Division 001 · File 005 · Classification: FOUNDATIONAL**

## Purpose

Defines the conceptual architecture of ANBU analysis: what counts as intelligence, the evidence vocabulary, the analytic cycle, and how raw information becomes graded assessment.

## Scope

The framework layer — vocabulary, cycle, and logic of analysis. Tradecraft details live in `osint/`, `verification/`, and `analytics/`; reporting format lives in `reporting/`.

## Intelligence Objectives

- Provide one shared language for all divisions.
- Separate observation, inference, and speculation rigorously.
- Define the path from question to product without ambiguity.

## Core Concepts

### The Evidence Vocabulary

Every claim in an ANBU product carries exactly one label:

| Label | Meaning |
|---|---|
| FACT | Directly observed or officially stated; no interpretation |
| VERIFIED | Independently corroborated by ≥2 independent sources |
| UNVERIFIED | Plausible, single-source or unconfirmed |
| ASSESSMENT | Analyst judgment grounded in labeled evidence |
| INFERENCE | Logical consequence drawn from labeled premises |
| HYPOTHESIS | Testable proposition competing with alternatives |
| SPECULATION | Weakly grounded; included only when flagged |

### The Analytic Cycle

1. **Direction** — define the question and decision context.
2. **Collection** — acquire candidate material with provenance.
3. **Evaluation** — grade sources and items.
4. **Analysis** — generate and test hypotheses.
5. **Verification** — corroborate, geolocate, authenticate.
6. **Dissemination** — graded product to the requester.
7. **Feedback** — record outcomes; update priors.

### Intelligence Disciplines

Strategic, operational, tactical — ANBU primarily serves strategic and operational questions, but the framework scales down when a task is narrow.

## Analytical Methodology

Analysis is hypothesis-driven: generate alternatives first, then seek evidence that discriminates between them. Evidence that confirms all hypotheses is noted as non-discriminating.

## Step-by-Step Workflow

1. State the question and decision context.
2. List candidate hypotheses (minimum two).
3. Map evidence requirements to each hypothesis.
4. Collect and label items.
5. Evaluate which hypothesis the evidence favors — and what would overturn it.

## Data Requirements

Every dataset entering the framework carries provenance metadata: source, retrieval date, collection method, and handling notes.

## Approved Public Sources

Defined per division; framework-level requirement is that sources be documented and permitted under ANBU collection rules.

## Source Verification Standards

See `verification/` division. Framework-level rule: no claim enters a product without a label and a source trail.

## Analytical Framework

**ACH — Analysis of Competing Hypotheses**: matrix hypotheses against evidence; weight evidence by source and information confidence; the hypothesis consistent with the most and least contradicted by the strongest evidence wins — provisionally.

## Evidence Requirements

Minimum evidence for an ASSESSMENT: at least two labeled items, at least one of which is VERIFIED or high-quality FACT, plus an explicit statement of what is missing.

## Confidence Assessment

- Source confidence: framework-independent
- Information confidence: framework-independent
- Analytical confidence: bounded by the weakest link in the evidence chain

## Common Analytical Mistakes

- Labeling inference as fact because it feels obvious.
- Treating absence of evidence as evidence of absence without stating the search.
- Letting a single vivid source dominate a matrix of weak corroboration.

## Ethical Considerations

The vocabulary itself is an ethical tool: it prevents the laundering of speculation into apparent fact. Mislabeling is treated as a report-quality defect.

## Security Boundaries

Framework applies only to public-source material. It does not create access, only structure for what is already obtainable.

## Expected Output

Labeled claims, hypothesis matrix, graded confidence, and falsification conditions — assembled per `output_standards.md`.

## Quality Checklist

- [ ] Every claim labeled
- [ ] ≥2 hypotheses considered
- [ ] Evidence trail complete
- [ ] Confidence stated on all three dimensions
- [ ] Falsification conditions present

## Cross-References

- [`intelligence_taxonomy.md`](intelligence_taxonomy.md)
- [`confidence_framework.md`](confidence_framework.md)
- [`analytics/`](../analytics/)
- [`verification/`](../verification/)
