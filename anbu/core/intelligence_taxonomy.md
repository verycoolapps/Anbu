# ANBU Intelligence Taxonomy

**Core Division 001 · File 006 · Classification: FOUNDATIONAL**

## Purpose

Defines the classification system for intelligence requirements, products, sources, and analytic outputs. Taxonomy ensures every task and product lands in a known category with known standards.

## Scope

Classification of *what kind of intelligence work this is*. It complements `task_classification.md` (which classifies the engagement) by classifying the objects of analysis.

## Intelligence Objectives

- Route tasks to the correct division and method.
- Standardize product types so consumers know what they are reading.
- Enable retrieval and comparison across the analytical record.

## Core Concepts

### Requirement Types

| Type | Definition | Example |
|---|---|---|
| PIR | Priority Intelligence Requirement — answers a standing decision need | "Will Country X impose energy sanctions this quarter?" |
| IR | Intelligence Requirement — decomposed sub-question | "What is X's current oil import dependency?" |
| EEI | Essential Elements of Information — facts needed to answer an IR | "Monthly crude import volumes, last 12 months" |

### Product Types

- **Strategic assessment** — long-horizon, system-level.
- **Operational estimate** — near-term, action-relevant.
- **Tactical note** — narrow, time-sensitive.
- **Warning product** — flags a developing risk or opportunity.
- **Reference product** — durable knowledge base entry (profiles, datasets).

### Source Classes

See `osint/` for the full source taxonomy. Framework-level classes: official, journalistic, academic, commercial, technical, social-media-derived (lowest default confidence).

### Analytic Output Types

- **Description** — what happened (facts only).
- **Explanation** — why it likely happened (inference + hypotheses).
- **Prediction** — what is likely next (forecast with confidence).
- **Warning** — what to watch for.

## Analytical Methodology

Classification happens at intake and again at reporting. Mismatches (a "tactical note" request that requires strategic analysis) trigger re-scoping before work proceeds.

## Step-by-Step Workflow

1. Identify the requirement type (PIR/IR/EEI).
2. Identify the product type the requester actually needs.
3. Identify the output type the evidence supports.
4. Route to divisions per the mapping table.

## Data Requirements

Classification metadata: requirement ID, product type, output type, division tags, confidence dimensions.

## Approved Public Sources

Taxonomy is source-neutral; per-class source rules live in `osint/` and `verification/`.

## Source Verification Standards

Not applicable to classification itself; inherited by all classified products.

## Analytical Framework

**Requirement Decomposition**: PIR → IRs → EEIs. Each level must be answerable from public sources; unanswerable EEIs are flagged rather than silently dropped.

## Evidence Requirements

A classified requirement without at least one mapped EEI and one candidate source class is incomplete and returned for refinement.

## Confidence Assessment

- Source confidence: NOT APPLICABLE
- Information confidence: HIGH for classification decisions
- Analytical confidence: HIGH when decomposition is complete

## Common Analytical Mistakes

- Answering a different question than the one classified (scope drift).
- Classifying a prediction request as a description because prediction is harder.
- Over-classifying (assigning PIR weight to trivia) — inflates effort and false precision.

## Ethical Considerations

Classification prevents mission creep: a request classified as targeting-adjacent is refused at intake rather than discovered at reporting.

## Security Boundaries

Classification labels are internal metadata; they do not affect data handling boundaries, which are fixed by `anbu_identity.md`.

## Expected Output

A requirement card: type, product, output, divisions, EEIs, source classes, confidence expectations.

## Quality Checklist

- [ ] Requirement type assigned
- [ ] Product type matches requester need
- [ ] Output type matches evidence reality
- [ ] Divisions mapped
- [ ] Unanswerable elements flagged

## Cross-References

- [`task_classification.md`](task_classification.md)
- [`intelligence_framework.md`](intelligence_framework.md)
- [`workflow_orchestrator.md`](workflow_orchestrator.md)
- [`osint/`](../osint/)
