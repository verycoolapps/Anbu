# Transportation Network Analysis

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Analysis of transportation networks—roads, rail, pipelines, air corridors, maritime routes—using public maps, imagery, and open data to assess connectivity, chokepoints, and change.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
Public map data (OSM, national road/rail registers, AIS-derived public data, aeronautical charts where public). Excludes classified transport infrastructure data and restricted port/airfield imagery.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Assess network topology, identify chokepoints and alternative routes, detect new construction or closures, and evaluate strategic mobility implications.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Network representation (graph theory: nodes, edges, centrality); road/rail classes; chokepoints (bridges, tunnels, passes, canals); seasonal access; capacity indicators; construction activity; alternative routing; multimodal connections.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Build network graph from open data → compute centrality/connectivity → overlay chokepoints → compare with historical maps/imagery for changes → assess strategic implications → validate against ground reports where available.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Define network question. 2) Acquire network data (OSM, national registers). 3) Clean and build graph. 4) Analyze connectivity/chokepoints. 5) Compare vintages for change. 6) Corroborate with imagery/news. 7) Report.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Network datasets with versions; imagery for verification; news/event reports for ground truth; historical map comparisons.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
OpenStreetMap; national road/rail authorities' open data; Eurocontrol/NATS public flight data summaries; MarineTraffic/ VesselFinder public AIS summaries (where permitted); national canal/port authorities' public info; Sentinel-2 for construction detection.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Check data currency—OSM varies by region. Verify chokepoint locations against imagery. Distinguish permanent vs. seasonal routes. Corroborate closures with official notices.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Network analysis: graph metrics, chokepoint list, change timeline, strategic assessment.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Route claims require map or imagery evidence. Chokepoint analysis must cite the specific geographic feature.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: authoritative network data + imagery corroboration; MODERATE: OSM + plausible corroboration; LOW: partial coverage; INSUFFICIENT: no reliable data.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Treating OSM as complete in low-coverage regions; ignoring seasonal closures; over-reading construction imagery; confusing planned vs. built infrastructure.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Avoid publishing detailed vulnerability of transport chokepoints; respect critical infrastructure sensitivities; do not aid targeting.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No access to restricted transport databases; no AIS data obtained illegally; no publication of route vulnerabilities.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Transport network brief: topology summary, chokepoints, changes, strategic implications, confidence.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Network data sourced ☐ Chokepoints verified ☐ Changes dated ☐ Seasonal factors noted ☐ Strategic assessment balanced

## Additional guidance
Transportation network analysis benefits from graph theory: model networks as nodes (intersections, stations) and edges (segments). Compute centrality measures to identify chokepoints. Distinguish road classes (highway vs. local) and rail types (passenger vs. freight). Note seasonal access variations (winter closures, monsoon impacts). For maritime transport, distinguish commercial shipping lanes from naval routes. Validate network data against imagery—OSM may miss new construction or include abandoned features. Report network resilience and alternative routing options.

## Cross-reference links
`../geoint/infrastructure_geography.md`; `../geoint/maritime_geographic_context.md`; `../geoint/border_geography_analysis.md`.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
