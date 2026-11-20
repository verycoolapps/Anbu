# Disaster Geospatial Assessment

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Geospatial assessment of disasters—earthquakes, floods, fires, storms, industrial accidents—using pre/post-event imagery and open data for impact evaluation and response support.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
Pre/post-event public imagery (Maxar Open Data, Copernicus Emergency Management Service, Sentinel-1/2, Planet disaster imagery), open demographic/infrastructure data, official situation reports.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Assess disaster extent and impact: damaged areas, affected population, infrastructure damage, access constraints, and recovery progress.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Event detection vs. impact assessment; pre/post comparison; damage proxy indicators (building damage, flood extent, burn scar); population exposure; infrastructure impact; access/egress analysis; temporal monitoring of response.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Acquire pre-event baseline → acquire post-event imagery → register/co-register → detect change (flood extent, burn scar, damage) → overlay population/infrastructure → quantify impact → compare with official reports → update as new imagery arrives.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Define disaster event and AOI. 2) Acquire pre-event baseline. 3) Acquire post-event imagery (priority: all-weather SAR if clouds). 4) Co-register and detect change. 5) Overlay exposure data. 6) Quantify impact. 7) Compare with official reports. 8) Update with new acquisitions.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Pre/post event imagery with dates; event type/time; AOI; cloud conditions; population/infrastructure layers; official situation reports for validation.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
Copernicus Emergency Management Service; Maxar Open Data Program; Planet disaster response imagery; Sentinel-1 SAR (all-weather); Sentinel-2 optical; Landsat; NASA FIRMS (fire); Dartmouth Flood Observatory; national disaster agencies' public data.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Verify event timing vs. imagery acquisition; note cloud/smoke limitations; corroborate damage with ground reports; distinguish damage from pre-existing conditions; state detection method limitations.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Impact assessment: event timeline, affected area extent, exposed population estimate, infrastructure damage, access constraints, confidence.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Impact estimates need explicit methodology; population exposure figures must state data source and assumptions; avoid precision beyond data capability.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: pre/post imagery + official reports agree; MODERATE: clear imagery change, partial corroboration; LOW: single-source or cloud-limited; INSUFFICIENT: no usable imagery.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Ignoring pre-existing damage; confusing flood extent with permanent change; over-estimating population exposure; not noting imagery timing vs. event evolution.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Prioritize humanitarian use; avoid publishing sensitive victim information; respect affected communities' dignity; support relief, not exploitation.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No publication of imagery enabling targeting of vulnerable areas; no use of disaster data for non-humanitarian purposes; respect data sharing restrictions during active response.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Disaster impact report: event summary, affected area, population exposure, infrastructure impact, response considerations, confidence.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Pre/post imagery acquired ☐ Event timing verified ☐ Impact method stated ☐ Population exposure sourced ☐ Official reports compared ☐ Humanitarian focus maintained

## Additional guidance
Disaster assessment requires rapid but rigorous analysis: acquire pre-event baseline before post-event imagery. For cloud-affected events, prioritize SAR (Sentinel-1). Distinguish event damage from pre-existing conditions. Quantify affected area, not just 'damage occurred'. For population exposure, use current population data overlaid on affected areas. Infrastructure damage assessment requires pre/post comparison. Update assessments as new imagery arrives—events evolve. Coordinate with official situation reports but maintain independent assessment. Prioritize humanitarian application.

## Cross-reference links
`../geoint/historical_satellite_comparison.md`; `../geoint/geospatial_intelligence_overview.md`; `../osint/` crisis OSINT standards.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
