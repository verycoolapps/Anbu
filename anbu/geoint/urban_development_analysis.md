# Urban Development Analysis

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Analysis of urban development patterns: growth, land-use change, infrastructure expansion, informal settlements, and urban planning using satellite time series and open data.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
Satellite time series (Landsat, Sentinel-2), GHSL built-up layers, national urban planning documents, municipal open data where available.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Track urban growth and change; assess development patterns; identify informal settlements; evaluate infrastructure adequacy; detect rapid/unplanned expansion.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Urban growth detection; land-use classification (residential, commercial, industrial, informal); built-up area change; infrastructure coverage; urban heat/island effects; planning compliance; density gradients; peri-urban expansion.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Acquire multi-temporal imagery → classify land use → derive built-up change → overlay infrastructure → identify informal vs. planned areas → assess growth drivers → document with temporal sequence.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Define urban question and AOI. 2) Acquire imagery time series. 3) Classify/classify change. 4) Map built-up expansion. 5) Overlay infrastructure/services. 6) Identify informal settlements. 7) Assess drivers and implications.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Imagery time series with dates; GHSL layers; municipal plans; infrastructure datasets; population data for context.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
Sentinel-2/Landsat time series; GHSL; World Settlement Footprint; Global Human Settlement Layer; national urban databases; municipal open data; VIIRS night lights for activity proxy.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Verify classification accuracy with ground reference; distinguish new construction from seasonal vegetation; note imagery resolution limits for informal settlement detection; corroborate with population/field data where available.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Urban change analysis: growth timeline, land-use maps, infrastructure gaps, informal settlement estimates, drivers.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Change claims need before/after imagery; informal settlement estimates must state method and uncertainty; avoid precise household-level mapping.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: multi-temporal imagery + corroborating data; MODERATE: clear imagery change; LOW: ambiguous classification; INSUFFICIENT: insufficient temporal coverage.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Confusing vegetation change with construction; over-interpreting low-res imagery; treating night lights as direct population measure; ignoring informal settlement detection limits.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Avoid mapping informal settlements at household level; respect resident privacy; do not enable forced eviction targeting; aggregate to neighborhood level.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No publication of vulnerable population locations enabling harm; no use of urban data for surveillance; respect informal settlement residents' rights.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Urban development report: growth analysis, land-use change, infrastructure assessment, informal settlement notes, implications.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Time series adequate ☐ Classification validated ☐ Change dated ☐ Informal settlement method stated ☐ Privacy protected

## Additional guidance
Urban analysis should distinguish planned vs. informal development—formal areas follow planning regulations, informal settlements grow organically. Use multiple indicators: building density, road patterns, infrastructure coverage, land-use mix. Night lights (VIIRS) provide activity proxy but not direct population measure. For growth detection, use multi-temporal imagery with consistent methodology. Note that rapid urbanization often outpaces infrastructure—assess service gaps. Respect that informal settlements house vulnerable populations—avoid enabling harm.

## Cross-reference links
`../geoint/historical_satellite_comparison.md`; `../geoint/population_geography.md`; `../geoint/land_use_change_analysis.md`.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
