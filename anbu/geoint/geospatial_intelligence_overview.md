# Geospatial Intelligence Overview

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Defines GEOINT as the analysis of imagery and geospatial data to describe, assess, and visually depict physical features and geographically referenced activities. Establishes ANBU's scope for public-source geospatial analysis: satellite imagery, aerial imagery, maps, terrain data, and derived products. Distinguishes GEOINT from remote sensing science and from pure cartography.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
Covers public imagery and geospatial sources only. Excludes classified imagery, restricted government feeds, and any task requiring unlawful access. Applies to all ANBU analysts producing geographic or infrastructure assessments.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Map physical and human geography relevant to the intelligence question; establish baseline geographic context; identify change over time; support event verification (disasters, military activity, infrastructure development).

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Spatial resolution vs. spectral resolution; revisit time vs. temporal resolution; orthorectification; coordinate reference systems (WGS84, UTM); raster vs. vector data; change detection; georeferencing and ground control; spatial accuracy (CE90/CE95); temporal uncertainty; metadata standards (STAC, ISO 19115).

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Hypothesis-driven: form geographic question → select appropriate sensor/product → acquire with known acquisition parameters → preprocess (orthorectify, atmospherically correct where needed) → analyze (visual interpretation, spectral indices, change detection) → validate against independent sources → quantify uncertainty.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Frame geographic question and area of interest (AOI). 2) Inventory available public imagery for AOI and timeframe. 3) Acquire and record metadata. 4) Preprocess to common CRS. 5) Perform interpretation/analysis. 6) Cross-check with maps, ground reports, other imagery. 7) Document findings with confidence and limitations.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
AOI boundary definition; acquisition dates; sensor/platform; spatial/spectral resolution; cloud cover; processing level (L1/L2); coordinate reference; any ground-truth or reference data for validation.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
Copernicus Browser / Sentinel Hub (Sentinel-1 SAR, Sentinel-2 MSI); USGS LandsatLook / EarthExplorer (Landsat 8/9 OLI, Landsat 4/5 MSS archive); Maxar Open Data Program (disaster events); Planet public NICFI basemaps and disaster imagery; ESA WorldCover; OpenStreetMap; Natural Earth; OpenTopography; USGS 3DEP; national mapping agencies' open data.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Record sensor, platform, acquisition datetime, processing level, and source URL for every scene. Prefer analysis-ready (L2A/L2SP) products. Note cloud cover and sun angle. Verify AOI alignment against reference data. Flag scenes where metadata is incomplete.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Layer model: baseline geography → human activity → change signal → corroborating evidence. Weight recency and resolution against the question. Apply change-detection only where temporal comparability is adequate.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Each geographic claim requires an imagery reference (scene ID, date), a map reference where applicable, or a documented inference. Spectral indices must state formula and thresholds used.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: multiple independent sensors/dates corroborate; MODERATE: one good source plus plausible corroboration; LOW: single low-resolution or poorly dated scene; INSUFFICIENT: AOI not covered or imagery unusable.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Single-scene over-interpretation; ignoring revisit gaps; confusing surface reflectance with activity; failing to account for cloud/snow/seasonal vegetation; treating pixel resolution as ground-truth precision; not documenting negative findings.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Avoid publishing imagery that enables targeting of individuals; aggregate to facility/neighborhood level where possible; respect national imagery restrictions; do not use imagery to violate privacy of private property beyond public-interest justification.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
Never purchase or use leaked imagery; do not attempt to defeat cloud-cover or tasking restrictions on commercial platforms; no use of satellite tasking APIs without authorization; store imagery per data-handling policy.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Geospatial findings memo: AOI description, imagery inventory, method, findings by confidence, limitations, source appendix.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ AOI and timeframe defined ☐ All scenes have metadata ☐ CRS consistent ☐ Corroboration attempted ☐ Confidence per finding ☐ Limitations stated ☐ No restricted data

## Additional guidance
Operational notes: GEOINT differs from IMINT (which may include non-geographic imagery) in that every product must be geographically referenced. All GEOINT work should record the coordinate reference system used, the acquisition parameters of any imagery, and the analyst's interpretation confidence. When fusing multiple sources, document the fusion method and any conflicts between sources. Imagery-derived observations should be distinguished from map-derived and report-derived observations in the analytical framework.

## Cross-reference links
`../osint/` source verification; `../security/` imagery handling; `../reporting/` geospatial annex format; `../geoint/geospatial_source_verification.md`; `../geoint/geospatial_uncertainty_management.md`.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
