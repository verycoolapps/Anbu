# Public Map Research

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Covers systematic research using publicly available maps: web maps, historical maps, topographic maps, nautical charts, aeronautical charts, and crowd-sourced maps.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
Publicly accessible map products and archives. Excludes paywalled or restricted map services and any map whose use violates terms.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Extract locations, routes, boundaries, infrastructure, and named features; verify place names and coordinates; build map-based evidence for reports.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Map scale and accuracy; projection distortions; map currency vs. ground truth; gazetteers and place-name authority; historical map comparison; symbol interpretation; map generalization; crowd-sourced error rates; gazetteer ambiguity.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Identify map need → select appropriate map type/scale → acquire → georeference if needed → extract features → corroborate with imagery/other maps → record provenance.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Define what the map must show. 2) Select map source(s) matching scale and theme. 3) Extract features with coordinates. 4) Cross-check names against gazetteers. 5) Compare multiple map vintages where change matters. 6) Document source, edition, and retrieval date.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Map title, publisher, edition/date, scale, projection, sheet/tile ID, URL, retrieval timestamp.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
OpenStreetMap; Google Earth/Maps public view (respect ToS for extraction); USGS topo quads; national topo services; NGA/public nautical charts where released; David Rumsey Map Collection; British Library map archive; national gazetteers; GeoNames.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Check edition date and currency. Distinguish gazetteer names from map labels. Flag crowd-sourced features needing corroboration. Record scale—small-scale maps misplace features.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Map evidence table: feature, coordinate, map source, edition, confidence, corroboration.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Coordinates must include CRS. Named features require gazetteer confirmation. Historical maps require date context.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: official current map + corroboration; MODERATE: reputable map, single source; LOW: crowd-sourced or old map; INSUFFICIENT: unverifiable.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Reading small-scale maps for precise location; ignoring map projection; treating old maps as current; misinterpreting map symbols.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Respect map publisher licensing; do not bulk-scrape violating ToS; avoid reproducing restricted map content verbatim.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No bypassing paywalls or access controls; no unauthorized scraping; respect robots/ToS.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Map research log + extracted feature table with provenance.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Map edition/date recorded ☐ Scale noted ☐ Coordinates with CRS ☐ Corroboration attempted ☐ ToS respected

## Additional guidance
Map research requires attention to map type and scale: a 1:50,000 topographic map reveals different features than a 1:1,000,000 political map. Always record the map's publication date, edition, and publisher. Historical maps are valuable for change detection but must be interpreted in their historical context. Crowd-sourced maps like OpenStreetMap vary in completeness by region—verify critical features against authoritative sources. When georeferencing historical maps, document control points used and resulting accuracy.

## Cross-reference links
`../osint/` open-source collection; `../geoint/open_geospatial_data.md`; `../reporting/` map annexes.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
