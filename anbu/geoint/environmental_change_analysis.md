# Environmental Change Analysis

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Analysis of environmental change using satellite time series: deforestation, land degradation, water change, coastal erosion, glacial retreat, and pollution indicators.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
Long-term satellite archives (Landsat since 1972, Sentinel-2 since 2015), MODIS/VIIRS time series, GEDI LiDAR, national environmental monitoring data where public.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Detect and quantify environmental change; assess drivers; support environmental impact and climate-related intelligence analysis.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Change detection over long time series; land cover classification; vegetation indices (NDVI, EVI); deforestation alerts (GLAD, RADD); water extent change; coastal change; glacial mass balance proxies; fire history; environmental degradation indicators.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Select indicator appropriate to question → acquire long time series → apply classification/index → detect change → attribute drivers where possible → validate with ground data → quantify rates and confidence.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Define environmental question. 2) Select indicator and time range. 3) Acquire time series. 4) Apply detection method. 5) Validate with reference data. 6) Quantify change rates. 7) Assess drivers. 8) Report.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Time series imagery; classification reference data; ground validation points; ancillary data (climate, land use); known disturbance events.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
Landsat archive; Sentinel-2; MODIS/VIIRS (NASA); GLAD/RADD deforestation alerts; Global Forest Watch; Copernicus Land Monitoring; national environmental agencies; GEDI; GRACE for water storage.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Verify time series continuity (sensor transitions); validate classifications with ground data; distinguish natural variability from anthropogenic change; note cloud contamination in tropical regions.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Environmental change report: indicator, time series, detected changes, rates, drivers, confidence, validation.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Every change rate needs stated method and uncertainty; driver attribution requires evidence, not just correlation; distinguish detection from attribution.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: validated classification + long time series + corroboration; MODERATE: clear trend, partial validation; LOW: ambiguous signal; INSUFFICIENT: insufficient data quality/coverage.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Ignoring sensor transition artifacts; confusing seasonal with long-term change; attributing drivers without evidence; not stating classification accuracy.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Avoid enabling environmental targeting or harassment; respect indigenous land rights in change reporting; support conservation, not exploitation.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No use of environmental data for illegal resource extraction planning; no publication of sensitive ecological sites' precise locations.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Environmental change assessment: indicators, trends, drivers, confidence, data quality.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Time series continuity verified ☐ Classification validated ☐ Change rates quantified ☐ Drivers evidenced ☐ Uncertainty stated

## Additional guidance
Environmental change detection requires long time series to distinguish trends from variability. Validate classifications with ground reference data. For deforestation, use alerts (GLAD, RADD) plus imagery confirmation. Distinguish natural disturbances (fire, storm) from anthropogenic change. For water bodies, account for seasonal variation—use dry-season imagery for consistent comparison. Vegetation indices (NDVI, EVI) are sensitive to atmospheric conditions—use corrected products. Attribute drivers cautiously—correlation is not causation. Report rates with uncertainty bounds.

## Cross-reference links
`../geoint/historical_satellite_comparison.md`; `../geoint/geospatial_intelligence_overview.md`; `../geoint/land_use_change_analysis.md`.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
