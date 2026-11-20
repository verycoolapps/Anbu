# Maritime Geographic Context

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Analysis of maritime geography: coastlines, ports, shipping lanes, EEZs, straits, and maritime chokepoints using public nautical charts, AIS-derived public data, and imagery.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
Public nautical charts (where released), open AIS aggregators' public layers, satellite imagery of ports/coasts, national maritime boundary deposits at UN.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Assess maritime strategic context: port capacity indicators, shipping lane chokepoints, naval access, boundary disputes, and maritime activity patterns.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Maritime zones (territorial sea, EEZ, continental shelf); straits and canals; port infrastructure; shipping lanes; AIS anomalies; bathymetry (where public); maritime boundaries; naval facilities (where publicly visible); search and rescue regions.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Acquire nautical/base layers → identify maritime features → assess port/stratigraphic chokepoints → analyze AIS patterns where public → examine boundary claims → corroborate with imagery → assess strategic relevance.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Define maritime question. 2) Gather charts/boundary data/AIS public layers. 3) Map features and chokepoints. 4) Analyze activity patterns. 5) Compare with historical data. 6) Corroborate with imagery/news. 7) Report.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Nautical charts or public equivalents; UN maritime boundary deposits; AIS public data; satellite imagery; port authority public information; maritime news.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
IMO public data; UN Division for Ocean Affairs (maritime boundary deposits); national hydrographic offices' open charts; MarineTraffic/VesselFinder public layers; Copernicus Maritime Service; Sentinel-1/2 for port/coastal monitoring; OpenSeaMap.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Verify chart editions and dates; distinguish official boundaries from claimed limits; check AIS data licensing; corroborate vessel activity with imagery where possible.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Maritime assessment: zones, chokepoints, port analysis, activity patterns, boundary status, strategic implications.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Boundary claims must cite the specific treaty/deposit/claimant position. AIS patterns need time-window context.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: official charts + treaty data + corroboration; MODERATE: public data with minor gaps; LOW: inferred patterns; INSUFFICIENT: no reliable public data.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Treating claimed EEZ as settled boundary; ignoring AIS data gaps (transponders off); over-reading port imagery; confusing naval and commercial activity.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Avoid publishing real-time vessel tracking that could enable targeting; respect privacy of crews; do not assist sanctions evasion analysis beyond public-interest.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No use of classified AIS or naval data; no real-time tracking publication; respect vessel privacy where applicable.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Maritime context brief: zones/chokepoints, port assessment, activity analysis, boundary status, confidence.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Boundaries sourced to treaties/deposits ☐ AIS limitations noted ☐ Port features verified ☐ Claims vs. settled distinguished ☐ Strategic balance maintained

## Additional guidance
Maritime analysis requires understanding maritime zones: territorial sea (12nm), contiguous zone (24nm), EEZ (200nm), continental shelf. Distinguish treaty-established boundaries from claimed limits. For ports, assess capacity indicators: berth length, crane type, draft depth, storage area. Shipping lanes follow depth, currents, and traffic separation schemes. AIS data has gaps (transponders off, coverage limits)—note these limitations. For naval analysis, distinguish commercial from military vessels where possible. Respect that some maritime activities are intentionally concealed.

## Cross-reference links
`../geoint/geographic_context_analysis.md`; `../geoint/infrastructure_geography.md`; `../osint/` maritime OSINT standards.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
