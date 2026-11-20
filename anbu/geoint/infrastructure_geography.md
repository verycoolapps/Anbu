# Infrastructure Geography

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Analysis of physical infrastructure geography: energy, water, transport, communications, industrial facilities, and their spatial relationships, using public imagery and open data.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
Public imagery and open infrastructure datasets (OpenStreetMap, national geoportals, company-published data, regulator filings). Excludes classified infrastructure data and restricted facility imagery.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Map and assess critical infrastructure: locations, capacity indicators, interdependencies, vulnerability, and change over time.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Infrastructure types (power, water, transport, telecom, industrial); facility footprints; capacity proxies (size, cooling structures, access roads); interdependencies; redundancy; strategic importance; construction activity; dual-use considerations.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Identify infrastructure assets from imagery/OpenStreetMap → attribute type and scale → assess interdependencies → evaluate change (expansion, new construction) → contextualize strategically → document with confidence.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Define infrastructure question. 2) Acquire imagery/open data for AOI. 3) Identify facilities via visual interpretation and attribute tables. 4) Classify by type/scale. 5) Map interconnections (power lines, pipelines, roads). 6) Compare with prior imagery for change. 7) Report findings.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Imagery scenes; OSM extracts; national infrastructure registers where public; company filings; regulatory documents; prior imagery for comparison.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
OpenStreetMap; national geoportals; Open Infrastructure Map; US EIA public data; national energy regulators' public filings; company sustainability reports; Maxar/Planet disaster imagery where released; Sentinel-2 time series.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Corroborate facility locations across sources; verify operating status where possible; note imagery date for 'current' claims; distinguish planned vs. existing infrastructure.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Infrastructure register: asset, type, location, evidence source, imagery date, confidence, strategic relevance.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Facility locations require imagery or authoritative map reference. Capacity estimates must be labelled as proxies, not measured values.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: multiple corroborating sources + recent imagery; MODERATE: clear imagery, single source; LOW: inferred from partial evidence; INSUFFICIENT: cannot verify.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Mistaking planned for existing infrastructure; over-interpreting shadows/signatures; ignoring imagery date; conflating dual-use civilian/military without evidence.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Avoid publishing precise targeting-grade detail of critical infrastructure; prefer strategic-level assessment; respect security of sensitive facilities.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No collection of restricted facility data; no imagery enhancement to reveal protected details; no publication of vulnerability specifics enabling attack.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Infrastructure assessment: asset inventory, interdependency map, change notes, strategic implications, confidence.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Assets corroborated ☐ Imagery dates noted ☐ Interdependencies mapped ☐ Capacity labelled as proxy ☐ Strategic context provided

## Additional guidance
Infrastructure analysis should distinguish between existing, under-construction, and planned facilities—imagery shows current state, not intent. Use multiple indicators: footprints, access roads, power connections, cooling structures, security features. For capacity assessment, use proxies (size, type) rather than claiming measured capacity. Map interdependencies (power, water, transport links). Compare with prior imagery for expansion or modification. Note that some infrastructure may be concealed or dual-use—avoid over-interpretation.

## Cross-reference links
`../geoint/geospatial_intelligence_overview.md`; `../geoint/transportation_network_analysis.md`; `../geoint/maritime_geographic_context.md`; `../security/` critical-infrastructure policy.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
