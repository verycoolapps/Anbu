# Geospatial Ethics And Safety

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Ethical and safety framework for geospatial intelligence: privacy, dual-use risks, targeting concerns, vulnerable populations, and responsible publication of geographic analysis.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
All geospatial intelligence work. Applies to imagery, maps, location data, and derived geographic analysis.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Ensure geospatial intelligence serves legitimate purposes without enabling harm: privacy protection, dual-use risk mitigation, vulnerable population safeguards, and responsible publication standards.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Privacy in imagery (individuals, homes); dual-use risks (targeting, surveillance); vulnerable populations (displaced, informal settlements, conflict zones); military vs. civilian applications; publication risks (enabling harm); data minimization; proportionality; accountability.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
For each geospatial product: assess privacy implications → evaluate dual-use risk → consider vulnerable population impact → apply data minimization → determine publication level → document ethical review → escalate concerns.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Complete geospatial product. 2) Assess privacy implications (individuals identifiable?). 3) Evaluate dual-use risk (could enable targeting/surveillance?). 4) Consider vulnerable population impact. 5) Apply data minimization (aggregate where possible). 6) Determine publication level. 7) Document ethical review. 8) Escalate concerns.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Privacy impact assessment; dual-use risk evaluation; vulnerable population considerations; publication decision rationale; ethical review documentation.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
Ethical frameworks (Bello, Solon, etc.); humanitarian principles; international human rights law; professional intelligence ethics codes; ANBU internal policies.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Default to aggregation and minimization; when in doubt, reduce precision; consult ethical review for high-risk products; document all ethical decisions.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Ethical review checklist: privacy ☐ dual-use ☐ vulnerable populations ☐ proportionality ☐ publication level ☐ documentation.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
No individual-level targeting; no publication of precise sensitive locations; no imagery enabling identification of vulnerable persons; aggregate by default.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
Ethical review outcome: APPROVED / APPROVED WITH MODIFICATIONS / ESCALATED / PROHIBITED. All geospatial products require review before publication.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Publishing precise locations of vulnerable populations; enabling targeting through 'high-resolution' detail; ignoring dual-use implications; treating 'public' data as 'safe' data.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Geospatial data can enable serious harm—privacy invasion, targeting, surveillance. Default to protective posture; err on side of less precision, not more.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No publication of imagery enabling targeting; no precise location data for sensitive sites; no use of geospatial data for illegal surveillance; all products require security review.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Ethical review memo: product description, privacy assessment, dual-use evaluation, vulnerable population impact, publication recommendation, reviewer signature.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Privacy assessed ☐ Dual-use evaluated ☐ Vulnerable populations considered ☐ Data minimized ☐ Publication level determined ☐ Review documented ☐ Concerns escalated

## Additional guidance
Geospatial ethics requires balancing intelligence value against privacy and safety risks. Default to aggregation—analyze at neighborhood/facility level, not individual level. Consider dual-use risks: could this analysis enable targeting, surveillance, or harm? For vulnerable populations (displaced persons, informal settlements), apply extra caution. Respect that 'public' imagery does not mean 'safe' to publish. When in doubt, reduce precision. Document ethical review for sensitive products. Escalate concerns to ethics review board.

## Cross-reference links
`../legal/research_consent_and_ethics.md`; `../security/` publication review; `../reporting/` responsible publication; `../geoint/disaster_geospatial_assessment.md`.
## Implementation notes

This file is part of the ANBU geospatial intelligence corpus. Analysts should read the linked core standards before applying this guidance in operational products. Where this file conflicts with updated core standards, the core standards prevail. Suggestions for improvement should be submitted through the standard review process; do not modify this file directly without review.

Geospatial analysis products must always state the acquisition date of imagery and the vintage of any map or dataset used. 'Current' claims require evidence dated within the relevant period. Where imagery is unavailable for a required period, state the gap explicitly rather than interpolating.

All geospatial findings should be reproducible: another analyst with access to the same public sources should be able to verify the analysis using the documented method, sources, and parameters.

## Revision history

- v1.0 — Initial ANBU geospatial intelligence guidance (2026-11-20).
