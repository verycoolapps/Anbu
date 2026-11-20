# Terrain Context Analysis

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Analysis of terrain and its military/geographic significance: elevation, slope, landform, drainage, and their implications for movement, observation, and operations.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
Public DEM data (SRTM, Copernicus DEM, ALOS), topographic maps, geological surveys where public, and satellite-derived terrain products.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Characterize terrain for movement analysis, observation/cover assessment, infrastructure siting implications, and disaster risk context.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Elevation models (DEM/DSM/DTM); slope and aspect; landform classification; drainage patterns; relief; rock type/soil where public; terrain ruggedness indices; line-of-sight considerations; seasonal terrain changes.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Acquire DEM → derive slope/aspect/roughness → classify landforms → analyze drainage → overlay with activity/ infrastructure → assess terrain constraints → document with resolution and accuracy notes.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Define terrain question. 2) Acquire appropriate DEM (resolution matched to need). 3) Derive terrain parameters. 4) Analyze drainage/landforms. 5) Overlay with relevant features. 6) Assess implications. 7) Document data resolution and limitations.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
DEM source and resolution; vertical accuracy; AOI extent; any ground-truth for validation; intended analysis use.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
Copernicus DEM (GLO-30/GLO-90); NASA SRTM; ALOS World 3D; USGS 3DEP; national DEMs where public; OpenTopography; GMTED2010; ETOPO1 for bathymetry.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Check DEM resolution vs. analysis scale (30m DEM cannot support trench-level analysis); note void-filling artifacts; verify vertical datum; corroborate critical terrain features with imagery.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Terrain profile: elevation stats, slope distribution, landform map, drainage analysis, operational implications.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Terrain claims must state DEM resolution and source. Line-of-sight or mobility claims need explicit terrain parameter basis.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: high-res DEM + imagery corroboration; MODERATE: standard DEM, reasonable use; LOW: coarse DEM for fine-scale claims; INSUFFICIENT: no suitable data.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Using 90m DEM for tactical-scale claims; ignoring void-fill artifacts; confusing DSM with DTM; not stating resolution limitations.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Avoid publishing high-precision terrain data enabling targeting; prefer strategic-level terrain description; respect military terrain data sensitivities.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No classified terrain data; no high-precision data publication beyond public-source resolution; no use of restricted survey data.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Terrain assessment: parameters, landforms, constraints, implications, data quality notes.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ DEM source/resolution stated ☐ Vertical accuracy noted ☐ Analysis scale appropriate ☐ Implications evidence-based ☐ Limitations documented

## Additional guidance
Terrain analysis should match DEM resolution to analysis scale: 30m DEM for regional assessment, 12m or better for tactical-scale. Note that SRTM has voids in steep terrain—check void-fill artifacts. Distinguish DSM (includes vegetation/buildings) from DTM (bare earth). For mobility analysis, compute slope, aspect, and ruggedness indices. For observation analysis, consider line-of-sight and cover. Terrain is dynamic—seasonal changes (snow, vegetation) affect accessibility. Document vertical datum and horizontal accuracy.

## Cross-reference links
`../geoint/geographic_context_analysis.md`; `../geoint/infrastructure_geography.md`; `../military/` terrain doctrine.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
