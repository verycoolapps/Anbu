# Historical Satellite Comparison

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Method for comparing satellite imagery across time to detect change: construction, demolition, land-use shift, environmental change, and activity patterns.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
Multi-temporal public imagery archives (Landsat since 1972/1984, Sentinel-2 since 2015, declassified Corona/KH programs where public). Excludes commercial historical archives unless publicly released.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Establish timelines of change; verify reported events (construction, disaster damage, military buildup); detect slow-onset change invisible in single scenes.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Temporal comparability: sensor differences (MSS vs OLI vs MSI), resolution changes, atmospheric conditions, seasonal vegetation, sun angle; co-registration accuracy; change detection methods (image differencing, post-classification, CVA); minimum detectable change; false positives from agriculture/phenology.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Select comparable pairs/triples → harmonize (surface reflectance, resample) → co-register → apply change detection → validate with high-res imagery/ground reports → quantify area/magnitude of change.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Define change question and period. 2) Inventory available dates. 3) Choose comparable sensors (prefer same sensor families). 4) Preprocess to common grid. 5) Run change detection. 6) Validate with independent evidence. 7) Report change magnitude and confidence.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Scene pairs with dates; sensor/platform; processing level; cloud cover; AOI; any ground-truth or news corroboration.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
USGS Landsat archive (1972–present); Copernicus Sentinel-2 archive; declassified Corona (USGS/FOIA releases); Hexagon KH-9; Corona via USGS; Soviet-era declassified via various archives; national archives' released imagery.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Verify acquisition dates precisely; note sensor differences affecting comparability; check for cloud/snow in either date; corroborate significant changes with non-imagery sources.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Change matrix: location × date range × change type × magnitude × confidence × corroboration.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Every detected change needs before/after scene IDs and, where possible, independent confirmation. False-positive rate must be stated.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: clear change in comparable imagery + corroboration; MODERATE: clear spectral/spatial change, single corroboration; LOW: ambiguous or poorly comparable; INSUFFICIENT: insufficient temporal coverage.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Comparing incompatible sensors without harmonization; ignoring seasonal vegetation; single-date 'change' claims; not quantifying detection limits.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Avoid publishing imagery enabling identification of individuals; respect privacy in residential change analysis; do not use historical imagery for targeting.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No use of classified historical imagery; no reconstruction of restricted archives; respect declassification terms.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Change assessment report: timeline, detected changes, confidence, corroboration, limitations.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Dates verified ☐ Sensors compatible ☐ Seasonality addressed ☐ Corroboration attempted ☐ Magnitude quantified

## Additional guidance
Historical comparison requires temporal comparability: prefer same-sensor comparisons (Landsat 8 vs. Landsat 9) over cross-sensor (Landsat vs. Sentinel-2) where possible. Harmonize processing levels (both L2 surface reflectance). Account for seasonal differences—compare same-season imagery or use phenology-resistant indices. Co-register images to sub-pixel accuracy. Quantify minimum detectable change based on sensor resolution and processing. Validate detected changes with independent sources. Document all preprocessing steps.

## Cross-reference links
`../geoint/public_satellite_data_sources.md`; `../geoint/geospatial_uncertainty_management.md`; `../geoint/disaster_geospatial_assessment.md`.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
