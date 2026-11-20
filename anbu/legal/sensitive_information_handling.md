# Sensitive Information Handling

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Framework for handling sensitive information in OSINT: identification, classification, protection, sharing, and disposal of sensitive data.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
All OSINT work involving sensitive information: personal data, confidential business information, security-sensitive data, or information that could cause harm if disclosed.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Handle sensitive information responsibly: identify, classify, protect, share appropriately, and dispose securely throughout the information lifecycle.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Sensitive information types; identification criteria; classification levels; protection measures; access controls; sharing protocols; retention schedules; disposal methods; breach response; personnel training; need-to-know.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Identify sensitive information → classify appropriately → implement protection measures → control access → share appropriately → retain per schedule → dispose securely → respond to breaches → document all handling.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Identify sensitive information. 2. Classify appropriately. 3. Implement protection. 4. Control access. 5. Share appropriately. 6. Retain per schedule. 7. Dispose securely. 8. Respond to breaches. 9. Document handling.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Sensitive info policies; classification guides; protection measures; access controls; sharing protocols; retention schedules; disposal procedures; breach response plans.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
Data protection laws; security policies; handling procedures; classification guides; training materials; case studies; legal requirements.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Identify sensitivity accurately; classify appropriately; protect adequately; control access; share appropriately; retain/dispose properly; respond to breaches; document everything.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Sensitive info handling assessment: identification, classification, protection, access control, sharing, retention, disposal, breach response, documentation.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Sensitive info identified; classified correctly; protected adequately; access controlled; sharing appropriate; retention/disposal proper; breaches handled; documentation complete.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: comprehensive handling + protection + documentation; MODERATE: handling with minor gaps; LOW: inadequate handling; INSUFFICIENT: insufficient handling analysis.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Failing to identify sensitive info; improper classification; inadequate protection; uncontrolled sharing; improper disposal; poor breach response.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Sensitive info handling protects individuals and organizations; prevent harm; support confidentiality; maintain trust; accountability for breaches.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No unauthorized access; no improper sharing; no insecure storage; no improper disposal; all handling documented and reviewed.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Sensitive info handling memo: identification, classification, protection, access, sharing, retention, disposal, breach response, documentation.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Info identified ☐ Classification correct ☐ Protection implemented ☐ Access controlled ☐ Sharing appropriate ☐ Retention proper ☐ Disposal secure ☐ Breaches handled ☐ Documentation complete

## Additional guidance
Sensitive information handling requires systematic approach throughout information lifecycle. Identify sensitive information accurately—personal data, confidential business info, security-sensitive data, information that could cause harm. Classify appropriately based on sensitivity and impact of disclosure. Implement protection measures: encryption, access controls, secure storage. Share only on need-to-know basis with appropriate authorization. Retain per schedule—don't keep indefinitely. Dispose securely—shred, wipe, or destroy. Respond to breaches promptly. Document all handling for audit. Train personnel on procedures. Sensitive information mishandling can have serious consequences.

## Cross-reference links
`../security/` sensitive info handling; `../legal/privacy_protection_framework.md`; `../legal/classified_information_exclusion.md`.
## Implementation notes

This file is part of the ANBU legal intelligence corpus. It provides working guidance, not legal advice. Where a specific legal question arises, qualified legal counsel should be consulted. This document does not create attorney-client privilege.

Legal analysis must always identify the jurisdiction(s) concerned, the applicable instruments, and the date of the legal research. Laws change—verify currency before relying on any statement in this document. Where laws conflict across jurisdictions, document the conflict and analyze each separately.

All legal findings should note the level of confidence in the legal analysis itself, separate from confidence in underlying facts. Legal uncertainty is normal and should be reported honestly.

## Revision history

- v1.0 — Initial ANBU legal intelligence guidance (2026-11-20).
