# Geographic Context Analysis

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Builds the geographic context layer for any intelligence topic: terrain, climate, hydrology, vegetation, and human geography that shape behavior and events. Context is the frame against which anomalies and activities are interpreted.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
Public geographic data and open physical/environmental datasets. Excludes site-specific classified geography and any data requiring field access.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Provide analysts with an accurate, current geographic baseline: what the land looks like, how it is used, what infrastructure exists, and what environmental factors constrain activity.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Physical geography (relief, hydrology, climate zones); human geography (settlement patterns, land use, infrastructure density); accessibility (roads, rivers, airfields); environmental constraints (forest, desert, permafrost, flood zones); seasonal variation; scale dependence.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Start from small-scale context (country/region) then zoom to AOI. Layer physical and human geography. Identify chokepoints, corridors, and constraints. Compare with historical baselines for change.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Define AOI and scale. 2) Acquire base layers (terrain, land cover, hydro, roads). 3) Overlay human activity layers. 4) Identify constraints and corridors. 5) Note seasonal/temporal factors. 6) Summarize context relevant to the question.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
AOI extent; required thematic layers; currency of data; resolution; license terms; coordinate consistency.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
Natural Earth (1:10m/50m); OpenStreetMap; ESA WorldCover; Copernicus DEM; USGS 3DEP/SRTM; HydroSHEDS; FAO GAUL/GeoNetwork; national open geoportals; Global Human Settlement Layer.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Check dataset currency and license. Verify coordinate systems. Prefer authoritative sources (national mapping agencies) over community data for contested areas.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Context matrix: physical constraint × human element × temporal factor × relevance to question.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Every context statement cites dataset, version, and date. Anomalies noted only when deviation from context is documented.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: authoritative recent data; MODERATE: mixed-vintage or community-sourced; LOW: stale or coarse data; INSUFFICIENT: no coverage.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Assuming static geography; ignoring seasonal changes; over-relying on one data vintage; treating absence of data as absence of features.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Do not publish precise locations of sensitive sites; respect indigenous land and restricted areas; avoid militarizing public geographic data.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No scraping of restricted mapping services; respect OSM usage policies and national geo-data restrictions.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Geographic context brief: layers used, key constraints, corridors, seasonal notes, limitations.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Layers sourced and dated ☐ CRS consistent ☐ Constraints identified ☐ Seasonal factors noted ☐ Limitations stated

## Additional guidance
Context analysis should proceed from macro to micro: begin with country or regional geography, then narrow to the area of interest. Note that geographic context is dynamic—seasonal changes, conflict, development, and environmental events alter the baseline. Analysts should maintain a context log documenting each layer added, its vintage, and its relevance to the intelligence question. Where context is contested (e.g., disputed boundaries), present all positions neutrally.

## Cross-reference links
`../core/` context standards; `../geoint/public_map_research.md`; `../geoint/terrain_context_analysis.md`; `../osint/` collection standards.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
