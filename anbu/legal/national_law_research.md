# National Law Research

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Research methods for national laws relevant to OSINT: privacy laws, data protection, computer crime statutes, official secrets laws, and FOI legislation across jurisdictions.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
Public national legislation, official gazettes, parliamentary records, court decisions, and regulatory guidance.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Identify legal constraints on intelligence activities in specific jurisdictions: what data can be collected, how it can be used, and what prohibitions apply.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Privacy/data protection laws (GDPR, national equivalents); computer misuse statutes; official secrets/espionage laws; FOI/access to information laws; surveillance laws; data localization requirements; extraterritorial application.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Identify jurisdiction → locate applicable laws → determine scope and extraterritorial reach → analyze prohibitions and permissions → assess compliance of proposed activity → document legal basis and risks.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Identify jurisdiction(s) involved. 2) Locate applicable national laws. 3) Determine scope/extraterritoriality. 4) Analyze prohibitions/permissions. 5) Assess proposed activity. 6) Document legal basis, risks, and recommendations.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
National legislation texts; official gazettes; court decisions; regulatory guidance; legal commentary; enforcement actions.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
National parliaments' official sites; official gazettes; data protection authority guidance; court databases; legal databases (Westlaw, Lexis where authorized); government legal portals.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Verify current version of laws (amendments); check enforcement practice; distinguish law from guidance; note extraterritorial provisions; consult local counsel for critical matters.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
National law analysis: jurisdiction, applicable laws, scope, prohibitions, permissions, compliance assessment, risks.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Every legal claim cites specific statute/section; distinguish law from policy; note enforcement risk; document assumptions about jurisdiction.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: clear statutory basis + enforcement practice; MODERATE: statutory basis, unclear enforcement; LOW: ambiguous or evolving law; INSUFFICIENT: insufficient legal research.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Assuming foreign laws don't apply; ignoring extraterritorial provisions; confusing guidance with law; not checking amendments.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Respect national laws; avoid activities clearly prohibited; seek legal review for high-risk jurisdictions; support rule-of-law compliance.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No evasion of national laws; no use of legal research to facilitate illegal activity; respect legal privileges and restrictions.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
National law memo: jurisdiction analysis, applicable laws, compliance assessment, risks, recommendations.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Jurisdiction identified ☐ Laws located and verified ☐ Scope analyzed ☐ Compliance assessed ☐ Risks documented ☐ Review completed where needed

## Additional guidance
National law research requires jurisdiction-specific analysis. Privacy laws vary significantly—GDPR applies extraterritorially to EU data subjects, while other jurisdictions have different scopes. Computer crime statutes may criminalize unauthorized access regardless of data sensitivity. Official secrets laws vary in scope and enforcement. FOI laws provide access rights but with exemptions. Data localization requirements may restrict cross-border transfer. Always check for extraterritorial provisions and enforcement practice. When in doubt, consult local counsel.

## Cross-reference links
`../legal/international_law_framework.md`; `../legal/privacy_protection_framework.md`; `../legal/lawful_osint_boundaries.md`.
## Implementation notes

This file is part of the ANBU legal intelligence corpus. It provides working guidance, not legal advice. Where a specific legal question arises, qualified legal counsel should be consulted. This document does not create attorney-client privilege.

Legal analysis must always identify the jurisdiction(s) concerned, the applicable instruments, and the date of the legal research. Laws change—verify currency before relying on any statement in this document. Where laws conflict across jurisdictions, document the conflict and analyze each separately.

All legal findings should note the level of confidence in the legal analysis itself, separate from confidence in underlying facts. Legal uncertainty is normal and should be reported honestly.

## Revision history

- v1.0 — Initial ANBU legal intelligence guidance (2026-11-20).
