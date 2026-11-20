# Open Geospatial Data

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Catalogs and operational guidance for open geospatial datasets: vector, raster, elevation, land cover, administrative boundaries, and geocoding resources available without cost.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
Publicly licensed open data (CC-BY, ODbL, public domain). Excludes commercial datasets requiring licenses and any data of uncertain provenance.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Enable analysts to locate, evaluate, and use authoritative open geospatial data for any ANBU geographic task.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Data types (vector/raster/point cloud); licenses (CC-BY, ODbL, public domain); spatial resolution; temporal coverage; update frequency; formats (GeoTIFF, Shapefile, GeoPackage, COG); APIs and bulk download; quality/accuracy metadata.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Define need → search data catalogs → evaluate license/resolution/currency → download → validate topology/CRS → integrate into analysis → document version.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) State data requirement. 2) Query catalogs (Data.gov, EU data portal, national portals). 3) Compare candidates on resolution, currency, license. 4) Download and verify integrity. 5) Check CRS and topology. 6) Document dataset name, version, date.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Dataset name, publisher, version, license, download date, spatial extent, resolution, CRS, format.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
OpenStreetMap; Natural Earth; Copernicus Data Space; USGS EarthExplorer/3DEP; OpenTopography; ESA WorldCover; GHSL; geoBoundaries; GADM; GeoNames; national open data portals; Overture Maps Foundation.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Confirm license permits intended use. Check update frequency. Validate attribute tables against known features. Prefer versioned, citable datasets.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Dataset evaluation matrix: need × resolution × currency × license × quality.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Every dataset cited with version and retrieval date. Derived products must note source lineage.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: authoritative open dataset, current; MODERATE: reputable but aging; LOW: community-maintained, unversioned; INSUFFICIENT: no suitable open data.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Ignoring license terms; mixing incompatible CRS; using unversioned data; assuming completeness.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Attribute sources per license; do not republish restricted or personal data embedded in open sets; respect indigenous data sovereignty where flagged.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No credential sharing for gated open data; no bulk scraping violating portal terms.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Data source register with license and version for each dataset used.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ License verified ☐ Version recorded ☐ CRS checked ☐ Currency noted ☐ Attribution prepared

## Additional guidance
When evaluating open geospatial datasets, prioritize authoritative publishers (space agencies, national mapping organizations, UN bodies) over community-maintained sources. Check update frequency—some datasets are updated annually, others continuously. Document the dataset version used in analysis. For derived products, trace lineage to original sources. Respect license terms—some require attribution, others restrict commercial use. Maintain a data register listing all datasets used, their versions, licenses, and retrieval dates.

## Cross-reference links
`../geoint/public_map_research.md`; `../geoint/geographic_information_systems.md`; `../core/` data standards.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
