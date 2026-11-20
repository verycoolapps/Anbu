# Privacy Protection Framework

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Privacy protection framework for OSINT: GDPR awareness, privacy principles, data subject rights, and how privacy law constrains collection and use of personal data.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
GDPR and equivalent national laws, privacy principles (OECD), data protection authority guidance, case law on privacy in intelligence contexts.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Ensure OSINT collection and use respects privacy: minimize personal data collection, respect data subject rights, and comply with privacy law.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Privacy principles (lawfulness, fairness, transparency, purpose limitation, data minimization, accuracy, storage limitation, integrity, accountability); GDPR rights (access, rectification, erasure, restriction, portability, objection); lawful bases; special categories; international transfers; DPIAs; breaches.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Identify personal data involved → determine applicable privacy law → assess lawful basis → apply data minimization → respect data subject rights → implement safeguards → document compliance.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Identify personal data in collection/use. 2. Determine applicable privacy law. 3. Assess lawful basis. 4. Apply minimization. 5. Respect data subject rights. 6. Implement safeguards. 7. Document compliance.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Privacy laws; DPA guidance; case law; data protection assessments; consent records; privacy policies.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
GDPR text; EU DPA guidance; national privacy laws; EDPB guidelines; ICO guidance; court decisions; privacy literature.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Verify current law version; check territorial scope; distinguish personal from non-personal data; note special categories; consult DPO/legal for complex cases.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Privacy analysis: data identified, law applicable, lawful basis, minimization applied, rights respected, safeguards, compliance documented.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Every personal data use cites lawful basis; minimize data; respect rights; document all processing; flag special categories.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: clear lawful basis + compliance documented; MODERATE: lawful basis with safeguards; LOW: questionable basis or gaps; INSUFFICIENT: insufficient privacy analysis.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Treating all data as non-personal; ignoring GDPR extraterritorial scope; not minimizing data; ignoring data subject rights.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Privacy is fundamental right; minimize personal data; respect autonomy; support accountability for privacy violations.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No collection of personal data without lawful basis; no processing violating privacy law; no publication of personal data without authorization.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Privacy assessment: data identified, law applicable, basis, minimization, rights, safeguards, compliance.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Personal data identified ☐ Law applicable ☐ Lawful basis assessed ☐ Minimization applied ☐ Rights respected ☐ Safeguards implemented ☐ Compliance documented

## Additional guidance
Privacy protection requires understanding applicable law and principles. GDPR establishes comprehensive rights: access, rectification, erasure, restriction, portability, objection. Lawful bases include consent, contract, legal obligation, vital interests, public task, legitimate interests. Special categories (health, biometric, political opinions) require enhanced protection. Data minimization and purpose limitation are core principles. Extraterritorial application extends to non-EU entities processing EU residents' data. When privacy and security conflict, proportionality analysis determines balance. Document lawful basis for all personal data processing.

## Cross-reference links
`../legal/personal_data_minimization.md`; `../legal/public_information_law.md`; `../legal/national_law_research.md`.
## Implementation notes

This file is part of the ANBU legal intelligence corpus. It provides working guidance, not legal advice. Where a specific legal question arises, qualified legal counsel should be consulted. This document does not create attorney-client privilege.

Legal analysis must always identify the jurisdiction(s) concerned, the applicable instruments, and the date of the legal research. Laws change—verify currency before relying on any statement in this document. Where laws conflict across jurisdictions, document the conflict and analyze each separately.

All legal findings should note the level of confidence in the legal analysis itself, separate from confidence in underlying facts. Legal uncertainty is normal and should be reported honestly.

## Revision history

- v1.0 — Initial ANBU legal intelligence guidance (2026-11-20).
