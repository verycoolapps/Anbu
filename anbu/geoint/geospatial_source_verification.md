# Geospatial Source Verification

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Verification standards for geospatial sources: how to authenticate imagery, maps, and geospatial claims before using them in intelligence products.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
All public geospatial sources—satellite portals, map services, crowd-sourced maps, archived imagery, and derived products.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Ensure every geospatial claim in ANBU products is traceable to a verified source with documented provenance and appropriate confidence.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Source authority tiers (official space agencies, national mapping, reputable commercial, community); metadata completeness; processing level verification; scene ID verification; coordinate verification; temporal verification; manipulation detection (for imagery); cross-source corroboration.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
For each geospatial source: identify authority → verify metadata completeness → confirm processing level → check scene/date accuracy → validate coordinates → cross-check with independent source → assign confidence.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Record source URL/portal and scene/product ID. 2) Verify acquisition datetime and sensor. 3) Check processing level and product type. 4) Validate coordinates against known features. 5) Cross-check with independent source where possible. 6) Document verification steps and confidence.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Source URL; scene/product ID; acquisition datetime; sensor/platform; processing level; coordinates; retrieval timestamp; verification notes.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
Copernicus Data Space; USGS EarthExplorer; NASA Earthdata; ESA portals; national mapping agency portals; OpenStreetMap; commercial portals' public products; archive.org for historical maps.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Official portals preferred; verify scene IDs resolve correctly; check metadata consistency (date vs. sun angle vs. orbit); flag community-edited maps needing corroboration; test coordinates against known landmarks.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Verification log: source, identifiers, checks performed, corroboration, confidence assigned.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Unverified geospatial claims must be labelled; imagery without metadata is LOW confidence at best; derived products need lineage documentation.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: official source + metadata complete + corroborated; MODERATE: reputable source, minor gaps; LOW: community/derived without full verification; INSUFFICIENT: cannot verify.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Accepting metadata at face value; not checking processing level; ignoring coordinate errors; treating crowd-sourced maps as authoritative.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Do not manipulate or enhance imagery to mislead; disclose all processing; respect source licensing in verification documentation.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No verification using restricted data; no bypassing portal authentication; no scraping violating terms.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Verification appendix for each geospatial product: sources verified, methods, confidence, limitations.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Source identified ☐ Metadata complete ☐ Scene/date verified ☐ Coordinates checked ☐ Corroboration attempted ☐ Confidence stated

## Additional guidance
Geospatial source verification requires checking metadata completeness: acquisition datetime, sensor/platform, processing level, coordinates, cloud cover. Verify scene IDs resolve to correct products. For maps, check edition date and publisher authority. For crowd-sourced data (OSM), verify critical features against authoritative sources. For derived products, trace lineage to original data. Test coordinates against known landmarks. Document all verification steps—unverified sources should be flagged as LOW confidence minimum.

## Cross-reference links
`../osint/source_verification.md`; `../geoint/geospatial_uncertainty_management.md`; `../reporting/` evidence standards.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
