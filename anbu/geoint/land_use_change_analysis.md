# Land Use Change Analysis

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Analyzes land-use and land-cover change over time using satellite imagery, aerial photography, and open geospatial data—detecting conversion between categories (forest→agriculture, agriculture→urban, water→land), quantifying rates, and attributing drivers where evidence supports it.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
Public satellite archives (Landsat, Sentinel-2), aerial imagery where public, and open land-cover products (ESA WorldCover, Dynamic World, national land-use registries). Excludes classified imagery and proprietary high-resolution commercial archives unless publicly released.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
- Detect and map land-use transitions relevant to economic, environmental, or security questions.
- Quantify change rates (area per period) for trend assessment.
- Identify driver signals (deforestation fronts, urban sprawl, agricultural expansion, mining).
- Support environmental impact, development, and resource assessments.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
- Land cover vs. land use (physical cover vs. human purpose).
- Transition matrices (from-class × to-class).
- Change detection: post-classification comparison, image differencing, CVA, deep learning segmentation.
- Minimum mapping unit and scale dependence.
- Seasonal vs. secular change; phenology masking.
- Accuracy assessment: producer/user accuracy, confusion matrix, Kappa.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Classify or use existing land-cover products for each date → align classifications to a common legend → compute transition matrices → validate with reference samples → attribute drivers using ancillary evidence (roads, concessions, news) → report rates with uncertainty.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Define change question and period. 2) Acquire imagery/products for start and end dates. 3) Harmonize legend and resolution. 4) Run classification or load classified products. 5) Compute transitions per unit area. 6. Validate with ground/reference data. 7. Attribute drivers where evidence exists. 8. Report change maps, rates, confidence.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Imagery or classified products for ≥2 dates; reference validation data; ancillary driver data (concessions, infrastructure, news); AOI boundary; period definition.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
Landsat archive; Sentinel-2; ESA WorldCover; Dynamic World; Google Earth Engine public datasets; national land-cover inventories (where public); GLAD/UMD alerts; national cadastral/land registries where open.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Verify product version and classification legend; check classification accuracy reports; confirm date coverage; validate derived results against independent samples; cite product DOI/version.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Transition matrix: rows = start class, columns = end class, cells = area. Report net change, gross change, and persistence. Flag transitions exceeding expected rates for driver investigation.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Change claims need classified maps or imagery for both dates plus quantified area. Driver attribution requires independent evidence—correlation alone is insufficient.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: validated classification, clear transitions, corroborated drivers. MODERATE: good classification, partial validation. LOW: unvalidated or coarse classification. INSUFFICIENT: insufficient temporal coverage or data quality.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Comparing incompatible legends; ignoring seasonal vegetation as change; treating unvalidated classifications as accurate; attributing drivers without evidence; not stating minimum mapping unit.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Avoid enabling illegal land grabbing or resource exploitation; respect indigenous land rights in reporting; aggregate sensitive land-tenure information; support sustainable development analysis.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No classified land-use data; no publication enabling targeting of sensitive sites; no use for illegal resource extraction planning.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Land-use change report: period, methods, transition matrix, change maps, rates, driver assessment, confidence, limitations.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Dates and products verified ☐ Legend harmonized ☐ Transitions quantified ☐ Validation performed ☐ Drivers evidenced ☐ Confidence stated

## Additional guidance
Land-use change analysis requires careful legend harmonization—different products use different classification schemes. Validate classification accuracy before computing transitions. Distinguish seasonal vegetation changes from permanent land-use conversion. Use minimum mapping units appropriate to sensor resolution. For driver attribution, correlate with infrastructure development, policy changes, or economic activity—but label attribution as inference unless directly evidenced. Report both gross change (total area changed) and net change (directional).

## Cross-reference links
See `../geoint/historical_satellite_comparison.md`, `../geoint/environmental_change_analysis.md`, `../geoint/urban_development_analysis.md`, `../osint/`, `../reporting/`.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
