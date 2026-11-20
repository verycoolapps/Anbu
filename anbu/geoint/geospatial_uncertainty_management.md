# Geospatial Uncertainty Management

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Framework for identifying, quantifying, and communicating uncertainty in geospatial analysis: positional accuracy, temporal uncertainty, classification error, and interpretive uncertainty.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
All geospatial analysis products. Applies uncertainty budgets to every geographic claim.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Ensure analysts communicate the limits of geospatial claims honestly; prevent over-confidence in location, timing, and interpretation.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Positional uncertainty (CE90/CE95, RMSE); temporal uncertainty (acquisition time vs. event time); classification uncertainty (producer vs. user accuracy); interpretation uncertainty (analyst subjectivity); scale uncertainty; propagation of uncertainty through analysis.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Identify uncertainty sources for each claim → quantify where possible → propagate through analysis → communicate as ranges/categories → flag claims exceeding data capability → document assumptions.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) For each geospatial claim, identify uncertainty sources. 2) Quantify positional/temporal/classification uncertainty. 3) Propagate through analysis steps. 4) Express final uncertainty. 5) Flag claims beyond data capability. 6) Document all assumptions.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Sensor accuracy specs; metadata completeness; classification accuracy reports; analyst assumptions; known data gaps.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
Sensor/platform documentation; product metadata; accuracy assessment literature; national mapping standards; analyst judgment documented explicitly.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Never state precision beyond data capability; distinguish accuracy (closeness to truth) from precision (repeatability); use ranges or categories for uncertain values; document all assumptions.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Uncertainty budget: claim × uncertainty sources × magnitude × impact on conclusion × communication method.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Every quantitative claim needs uncertainty bounds; qualitative claims need confidence category; 'unknown' is a valid and important answer.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
The confidence levels themselves: HIGH (uncertainty low, corroborated), MODERATE (bounded uncertainty), LOW (high uncertainty), INSUFFICIENT (cannot assess). Uncertainty must always be stated, not implied.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Reporting point estimates without uncertainty; ignoring temporal gaps; treating classification accuracy as perfect; not documenting assumptions.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Honest uncertainty communication protects sources and prevents misuse; avoid false precision that could enable harm.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No suppression of uncertainty for political convenience; no overstating confidence to please stakeholders.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Uncertainty statement for each finding: sources of uncertainty, magnitude, impact on confidence, recommended caution.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Uncertainty sources identified ☐ Magnitude estimated ☐ Propagation considered ☐ Communication appropriate ☐ Assumptions documented

## Additional guidance
Uncertainty management requires identifying all uncertainty sources: positional (CE90/CE95), temporal (acquisition vs. event), classification (producer/user accuracy), interpretation (analyst subjectivity), scale (resolution limits). Propagate uncertainty through analysis—don't ignore it. Express results as ranges or confidence categories, not false precision. Distinguish accuracy (closeness to truth) from precision (repeatability). Document all assumptions. When uncertainty exceeds acceptable levels, report 'INSUFFICIENT' rather than guessing. Honest uncertainty communication protects sources and prevents misuse.

## Cross-reference links
`../geoint/geospatial_source_verification.md`; `../osint/uncertainty_management.md`; `../reporting/` confidence standards.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
