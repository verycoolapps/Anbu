# Lawful Osint Boundaries

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Framework for lawful OSINT boundaries: what is permitted, prohibited, or requires authorization across different jurisdictions and contexts.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
National laws, international law, platform terms of service, professional ethics, and organizational policies governing OSINT.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Define clear boundaries for lawful OSINT: distinguish public vs. restricted sources, authorized vs. unauthorized access, ethical vs. unethical collection.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Public vs. restricted sources; authorized vs. unauthorized access; platform ToS; national laws (privacy, computer crime, secrets); international law; professional ethics; organizational policies; proportionality; necessity; accountability.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Identify activity → determine applicable laws/ToS → assess authorization requirements → evaluate proportionality/necessity → implement safeguards → document compliance → escalate concerns.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Define OSINT activity. 2. Identify applicable laws/ToS. 3. Assess authorization requirements. 4. Evaluate proportionality/necessity. 5. Implement safeguards. 6. Document compliance. 7. Escalate concerns.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
National laws; platform ToS; international law; professional codes; organizational policies; authorization records; compliance assessments.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
National legislation; platform ToS; international law instruments; professional ethics codes; organizational policies; legal guidance; case law.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Check all applicable constraints; distinguish public from restricted; verify authorization where needed; document compliance; escalate novel/uncertain activities.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Boundary analysis: activity, applicable constraints, authorization, proportionality, safeguards, compliance, escalation.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Every activity assessed against all constraints; document compliance; flag concerns; escalate novel activities for review.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: clearly lawful with documentation; MODERATE: lawful with safeguards; LOW: questionable legality; INSUFFICIENT: insufficient legal analysis.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Assuming 'public' = 'lawful'; ignoring platform ToS; not checking national laws; treating ethics as optional.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Lawful boundaries protect sources and organizations; respect legal and ethical constraints; support accountability; err on side of caution.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No activities violating law/ToS/ethics; no unauthorized access; no evasion of restrictions; all activities documented and reviewed.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Boundary memo: activity, constraints, authorization, proportionality, safeguards, compliance, escalation, recommendations.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Activity defined ☐ Constraints identified ☐ Authorization assessed ☐ Proportionality evaluated ☐ Safeguards implemented ☐ Compliance documented ☐ Concerns escalated

## Additional guidance
Lawful OSINT boundaries are defined by multiple constraints: national laws (privacy, computer crime, secrets), international law (sovereignty, human rights), platform terms of service, professional ethics, and organizational policies. 'Public' data is not automatically 'lawful'—access method matters. Unauthorized access to restricted systems is illegal regardless of data sensitivity. Platform ToS may prohibit scraping even when data is technically accessible. Proportionality and necessity tests apply—collect only what's needed for legitimate purpose. When constraints conflict, document analysis and escalate concerns.

## Cross-reference links
`../legal/national_law_research.md`; `../legal/international_law_framework.md`; `../legal/research_consent_and_ethics.md`.
## Implementation notes

This file is part of the ANBU legal intelligence corpus. It provides working guidance, not legal advice. Where a specific legal question arises, qualified legal counsel should be consulted. This document does not create attorney-client privilege.

Legal analysis must always identify the jurisdiction(s) concerned, the applicable instruments, and the date of the legal research. Laws change—verify currency before relying on any statement in this document. Where laws conflict across jurisdictions, document the conflict and analyze each separately.

All legal findings should note the level of confidence in the legal analysis itself, separate from confidence in underlying facts. Legal uncertainty is normal and should be reported honestly.

## Revision history

- v1.0 — Initial ANBU legal intelligence guidance (2026-11-20).
