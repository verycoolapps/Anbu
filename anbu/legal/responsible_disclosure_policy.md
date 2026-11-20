# Responsible Disclosure Policy

## Purpose
This document is a working reference for ANBU analysts. It defines the topic's role within the broader intelligence workflow, the questions it answers, and the situations where it must be applied. It is intended to be used alongside the linked domain files and the core tradecraft standards.
Responsible disclosure policy: how to handle discovered vulnerabilities, security issues, or sensitive information that could cause harm if mishandled.

## Scope
This scope is deliberately bounded: only public sources, lawful methods, and evidence-linked analysis. Anything requiring restricted access, unlawful collection, or unverifiable claims falls outside this document and must be escalated or excluded. The scope statement should be checked before beginning any analysis in this domain.
All OSINT work that may uncover vulnerabilities, security issues, or sensitive information requiring careful handling.

## Intelligence objectives
Objectives should be stated as questions the analysis will answer, not as activities it will perform. Each objective maps to at least one approved source and one verification step. When objectives cannot be met with public data, the correct output is an explicit statement of the limitation rather than an inferred answer.
Ensure responsible disclosure: identify issues requiring disclosure, assess harm potential, determine appropriate recipients, coordinate disclosure, and protect those who discover issues.

## Core concepts
Core concepts are the vocabulary of the domain. Analysts should use these terms precisely and consistently in products. Where a term has multiple meanings across jurisdictions or disciplines, this document notes the preferred ANBU usage. New terms introduced by evolving practice should be added here with definitions.
Vulnerability disclosure; coordinated disclosure; responsible disclosure timelines; harm assessment; recipient identification; legal protections; whistleblower protections; disclosure channels; follow-up; documentation.

## Analytical methodology
The methodology section describes the reasoning chain, not just the steps. Each analytical choice should be justified: why this source over another, why this method over an alternative, why this confidence level. Methodology transparency allows reviewers to assess validity and allows the analysis to be repeated or challenged.
Identify issue requiring disclosure → assess harm potential → determine appropriate recipients → coordinate disclosure → protect discoverer → follow up → document → learn for prevention.

## Step-by-step workflow
Workflows are designed to be repeatable by any qualified analyst. Each step has an implicit quality gate: do not proceed to the next step until the current step's output meets the stated standard. Where a step fails, document the failure and either remediate or report INSUFFICIENT rather than proceeding on weak foundations.
1) Identify issue requiring disclosure. 2. Assess harm potential. 3. Determine recipients. 4. Coordinate disclosure. 5. Protect discoverer. 6. Follow up. 7. Document. 8. Learn for prevention.

## Data requirements
Data requirements list what must be in hand before analysis begins. Missing data is a finding in itself: note what is absent, why it is absent, and whether its absence affects the conclusion. Never fill data gaps with assumptions presented as facts.
Disclosure policies; vulnerability handling procedures; harm assessments; recipient lists; legal protections; whistleblower policies; documentation requirements.

## Approved public sources
Only sources listed here or in linked domain files may be used. If a needed source is not listed, analysts must request approval before use. Approved sources are those that are publicly accessible, lawfully obtained, and of sufficient reliability for intelligence purposes. Commercial sources require license verification before use.
Responsible disclosure frameworks; vulnerability disclosure policies; legal protections; whistleblower laws; professional standards; case studies.

## Source verification standards
Verification standards apply to every source before it informs analysis. Record retrieval date, source URL or identifier, and any authentication or access method. Prefer primary sources over secondary. Where sources conflict, document the conflict and resolve it or report both positions. Verification is a gate, not a formality.
Assess harm accurately; identify appropriate recipients; coordinate timing; protect discoverer; follow up; document; learn for improvement; respect legal requirements.

## Analytical framework
The analytical framework structures findings so reviewers can evaluate them. Every finding should map to a source, a date, a location or subject, and a confidence level. Frameworks prevent cherry-picking: all relevant evidence must be considered, not only evidence supporting the preferred conclusion.
Disclosure assessment: issue, harm potential, recipients, coordination, discoverer protection, follow-up, documentation, learning.

## Evidence requirements
Evidence requirements define the minimum standard for each type of claim. A claim about current activity requires recent evidence; a claim about historical events requires dated documentation; a claim about intent requires behavioral evidence, not just capability. Inferences must be labelled as inferences with stated reasoning.
Issues disclosed responsibly; harm minimized; recipients appropriate; discoverer protected; follow-up completed; documentation thorough; lessons learned.

## Confidence assessment
Confidence levels are standardized across ANBU: HIGH (multiple independent corroborations, strong provenance), MODERATE (two or more sources with minor gaps), LOW (single source or weak corroboration), INSUFFICIENT (cannot be assessed publicly). Confidence is per-finding, not per-product. State confidence for every substantive claim.
HIGH: coordinated disclosure + protection + follow-up; MODERATE: disclosure with minor gaps; LOW: inadequate disclosure; INSUFFICIENT: insufficient disclosure analysis.

## Common analytical mistakes
Common mistakes are documented because they recur across analysts and domains. Each mistake has a corresponding prevention measure in the workflow or quality checklist. When a mistake is identified in a product, it should be corrected and the correction documented. Mistakes that recur indicate a training or process gap.
Premature public disclosure; inadequate harm assessment; wrong recipients; failing to protect discoverer; no follow-up; no documentation.

## Ethical considerations
Ethical considerations are not optional. Every analysis should be reviewed for privacy impact, dual-use risk, vulnerable population effects, and proportionality. Ethical review is proportionate to risk: routine analysis may need only self-check, while sensitive analysis requires formal review. Ethical concerns that cannot be resolved must be escalated.
Responsible disclosure prevents harm; protects discoverers; supports security improvement; maintains trust; ethical obligation.

## Security boundaries
Security boundaries define what must never be done: no classified data, no unauthorized access, no publication of sensitive details, no evasion of security controls. These boundaries are absolute. Work that would cross a boundary must be redesigned or abandoned. Security breaches must be reported immediately through the appropriate channel.
No premature disclosure; no harm to affected parties; no legal violations; discoverers protected; all disclosures coordinated.

## Expected output
Expected outputs define what a completed analysis looks like. They include the analytical product itself, supporting documentation, source lists, confidence assessments, and limitations statements. Outputs must be reviewable: another analyst should be able to verify the reasoning and reproduce the result from the documented sources.
Disclosure memo: issue, harm assessment, recipients, coordination, discoverer protection, follow-up, documentation, recommendations.

## Quality checklist
The quality checklist is the final gate before a product leaves the analyst. Each item must be verified, not assumed. If any item fails, the product is not complete. Checklist results should be documented—unchecked items require explanation. The checklist applies to drafts as well as final products.
☐ Issue identified ☐ Harm assessed ☐ Recipients determined ☐ Disclosure coordinated ☐ Discoverer protected ☐ Follow-up completed ☐ Documentation thorough ☐ Lessons learned

## Additional guidance
Responsible disclosure balances security improvement with harm prevention. When vulnerabilities or security issues are discovered, assess harm potential—could disclosure enable attacks? Identify appropriate recipients—vendor, CERT, affected parties. Coordinate timing—disclose when fix is available or risk is mitigated. Protect discoverer—ensure legal protection and recognition. Follow up—verify fix, assess residual risk. Document all steps. Learn for prevention—improve processes. Responsible disclosure is ethical obligation and often legally protected. Premature or irresponsible disclosure can cause serious harm.

## Cross-reference links
`../security/` vulnerability disclosure; `../legal/sensitive_information_handling.md`; `../legal/research_consent_and_ethics.md`.
## Implementation notes

This file is part of the ANBU legal intelligence corpus. It provides working guidance, not legal advice. Where a specific legal question arises, qualified legal counsel should be consulted. This document does not create attorney-client privilege.

Legal analysis must always identify the jurisdiction(s) concerned, the applicable instruments, and the date of the legal research. Laws change—verify currency before relying on any statement in this document. Where laws conflict across jurisdictions, document the conflict and analyze each separately.

All legal findings should note the level of confidence in the legal analysis itself, separate from confidence in underlying facts. Legal uncertainty is normal and should be reported honestly.

## Revision history

- v1.0 — Initial ANBU legal intelligence guidance (2026-11-20).
