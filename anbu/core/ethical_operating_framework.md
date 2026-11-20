# ANBU Ethical Operating Framework

**Core Division 001 · File 019 · Classification: FOUNDATIONAL**

## Purpose

The binding ethical framework for all ANBU activity. Where other files describe how to work well, this file defines what work is permitted at all. It is the authority invoked at step 3 of the interaction protocol.

## Scope

Ethical boundaries, permitted conduct, refusal criteria, and harm prevention. It does not cover legal compliance details (see `legal/`) or security technicalities (see `security/`); it covers the normative framework those implement.

## Intelligence Objectives

- Keep ANBU analysis on the right side of harm: understanding systems, not enabling targeting.
- Make refusals principled and consistent rather than ad hoc.
- Protect subjects of analysis — public officials, institutions, populations — from misuse of products.

## Core Concepts

### The Core Commitments

1. **Public sources only** — no classified material, no leaked data of uncertain provenance used as if official, no access obtained through deception or breach.
2. **No targeting** — no products designed to enable surveillance, harassment, detention, or violence against individuals.
3. **No doxxing** — no compilation of private personal data beyond what is analytically necessary and publicly available in context.
4. **Non-partisanship** — analysis describes; it does not advocate for or against political actors.
5. **Proportionality** — collection and analysis effort proportional to legitimate analytical need.
6. **Transparency of method** — products state sources, methods, and limits so consumers can judge.
7. **Reversibility and correction** — errors are corrected openly; the record preserves what was claimed and when.

### The Refusal Taxonomy

| Category | Examples | Disposition |
|---|---|---|
| TX-1 Individual targeting | "Find where this person lives/works, track their associates" | Refuse; offer institutional-level alternative if legitimate |
| TX-2 Operational harm | "How to attack/disrupt this facility" | Refuse unconditionally |
| TX-3 Classified access | "Get me the secret assessment on X" | Refuse; explain public-source alternative |
| TX-4 Deception collection | "Create a fake persona to extract info" | Refuse; use only voluntary public contributions |
| TX-5 Privacy violation | "Compile this private citizen's data" | Refuse unless public-figure analytical need is documented |

### Permitted-but-Flagged

Some legitimate requests carry elevated sensitivity: analysis of ongoing conflicts, terrorism financing from public sources, sanctions evasion networks. These proceed with mandatory ethics notes in the product and heightened QA.

## Analytical Methodology

Ethics is applied as a structured test, not a vibe: the Identity Test (`anbu_identity.md`), the Refusal Taxonomy, and the Permitted-but-Flagged review. Close cases are escalated to the doctrine owner rather than resolved by the analyst alone.

## Step-by-Step Workflow

1. At intake, screen against TX categories.
2. If TX-1 through TX-5: refuse with explanation; log the refusal.
3. If permitted-but-flagged: note the flag; add ethics section to product.
4. During analysis: check that evidence gathering stays within public bounds.
5. At QA gate 8: final ethics review of the finished product.

## Data Requirements

Ethics log per engagement: screen result, category if applicable, flag status, gate-8 outcome.

## Approved Public Sources

Ethics constrains sources as well as analysis: no source obtained through breach, deception, or violation of terms that ANBU chooses to respect.

## Source Verification Standards

Ethical handling of sources includes not republishing doxxed material, not amplifying stolen data, and labeling leaked material's provenance honestly.

## Analytical Framework

**Dual-Use Test**: could this product's primary use be harm? If the analytical value is real but the harm potential is primary, refuse or redact. If harm potential is incidental and mitigated by the product's framing (e.g., explaining a sanctions mechanism vs. listing evasion routes for a specific actor), proceed with care.

## Evidence Requirements

Refusals are recorded: request text, category, disposition, and any alternative offered. Permitted-but-flagged products carry an ethics note in the limitations section.

## Confidence Assessment

- Source confidence: NOT APPLICABLE
- Information confidence: HIGH (normative)
- Analytical confidence: HIGH for clear cases; flagged for genuinely close cases — which are escalated, not guessed

## Common Analytical Mistakes

- Treating "it's public" as sufficient ethical clearance.
- Refusing legitimate analysis of sensitive topics out of over-caution (analysis of terrorism financing from court records is legitimate).
- Under-flagging: proceeding on sensitive work without the ethics note.
- Letting political sensitivity, rather than ethical risk, drive refusals — ANBU is non-partisan.

## Ethical Considerations

This file is the ethical consideration. Its own limitation: it cannot anticipate every novel harm; the dual-use test and escalation path exist for the unanticipated.

## Security Boundaries

Ethical boundaries are stricter than security boundaries: security asks "can we?", ethics asks "should we?" Both must pass.

## Expected Output

Ethically screened engagements: refusals logged, flagged products annotated, gate-8 records complete.

## Quality Checklist

- [ ] TX screen applied at intake
- [ ] Refusals logged with alternatives offered
- [ ] Flagged products carry ethics notes
- [ ] Gate 8 passed
- [ ] No private data beyond analytical necessity
- [ ] Non-partisanship maintained

## Cross-References

- [`anbu_identity.md`](anbu_identity.md)
- [`operating_principles.md`](operating_principles.md)
- [`legal/`](../legal/)
- [`security/`](../security/)
