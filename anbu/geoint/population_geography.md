# Population Geography

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Analysis of population distribution, density, and demographics using public census data, GHSL, WorldPop, and related open datasets.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
Public census data, UN population datasets, GHSL, WorldPop, national statistical offices' open data. Excludes restricted demographic data and any data enabling individual identification.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Map population distribution and density; assess demographic patterns relevant to stability, development, disaster risk, and urbanization.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Population distribution vs. density; settlement hierarchy; urban/rural classification; demographic transition; age structure; displacement/migration patterns; data aggregation levels and privacy constraints.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Identify demographic question → select dataset at appropriate aggregation → analyze spatial patterns → compare with infrastructure/service data → assess trends → document aggregation level and privacy safeguards.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Define demographic question. 2) Select dataset (census/GHSL/WorldPop). 3) Analyze distribution/density. 4) Compare with land use/infrastructure. 5) Assess trends/changes. 6) Document aggregation and limitations.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Dataset name, year, aggregation level (admin unit, grid), methodology, license, privacy protections.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
UN World Population Prospects; national census data (where public); GHSL; WorldPop; GRUMP; national statistical offices; DHS surveys (public use files); UNHCR refugee data.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Check census year and methodology comparability; note modeled vs. enumerated data; verify aggregation level protects privacy; distinguish urban definition variations.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Demographic analysis: distribution maps, density stats, urban/rural breakdown, trends, implications.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Only aggregate-level data; no individual-level analysis; cite dataset year and methodology; note modeled data uncertainty.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: recent census or high-quality modeled data; MODERATE: older census or modeled; LOW: coarse or conflicting sources; INSUFFICIENT: no reliable public data.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Treating modeled data as census counts; ignoring aggregation level; comparing incompatible urban definitions; publishing small-area data risking re-identification.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Strict privacy—aggregate only; no small-area analysis enabling identification; respect census confidentiality; avoid demographic profiling for targeting.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No access to restricted demographic data; no re-identification attempts; no publication of small-area sensitive data.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Population analysis: distribution, density, urban patterns, trends, implications, data quality notes.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Aggregation level appropriate ☐ Privacy protected ☐ Census year noted ☐ Methodology documented ☐ Trends evidence-based

## Additional guidance
Population analysis requires understanding data aggregation levels—census data may be by administrative unit, gridded products (GHSL, WorldPop) provide finer resolution but are modeled. Distinguish enumerated counts from modeled estimates. Note census year and methodology comparability. For displacement analysis, use UNHCR and IOM data. Respect privacy—aggregate to protect individuals. Urban/rural definitions vary by country—note definitions used. Population data supports exposure analysis for disasters, conflict, and development but must be current.

## Cross-reference links
`../geoint/urban_development_analysis.md`; `../geoint/geographic_context_analysis.md`; `../legal/personal_data_minimization.md`.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
