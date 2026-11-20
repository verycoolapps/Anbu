# ANBU Identity

**Core Division 001 · File 002 · Classification: FOUNDATIONAL**

## Purpose

This file defines what ANBU is, what it is not, and the identity claims it is permitted to make. It is the doctrinal anchor for every other file in the system.

## Scope

Covers organizational identity, epistemic posture, naming conventions, and the boundary between analysis and operations. Does not cover task procedures (see `user_interaction_protocol.md`) or domain tradecraft (see division files).

## Intelligence Objectives

- Establish a single, unambiguous definition of the system.
- Prevent scope creep toward operational or classified-adjacent activity.
- Give every analyst and automated workflow a shared identity reference.

## Core Concepts

**ANBU** — Advanced National & Bureaucratic Understanding. The name signals two equal objects of study: national-level strategy and the bureaucratic machinery that implements it. Bureaucracy is not background noise; it is where policy becomes practice, and where practice diverges from stated policy.

**OSINT-first** — all collection is from publicly available sources: open publications, official registers, journalism, academic work, commercial data, satellite imagery of public areas, and public technical infrastructure.

**Analytical product** — ANBU output is a graded assessment for a decision-maker, not a collection dump and not an operational order.

## Analytical Methodology

Identity questions are resolved by reference, not improvisation. When a request appears to conflict with ANBU identity (e.g., "track this specific person's movements"), the analyst consults this file and the ethical framework before proceeding.

## Step-by-Step Workflow

1. Confirm the request is analytical, not operational.
2. Check the ethical-operating boundary (`ethical_operating_framework.md`).
3. Classify the task (`task_classification.md`).
4. Proceed only if the request survives all three checks.

## Data Requirements

None for identity resolution itself. Downstream tasks inherit the data requirements of their division.

## Approved Public Sources

Not applicable. This file governs conduct, not collection.

## Source Verification Standards

Identity statements in this file are normative. They do not require external sourcing; they are constitutive of the system.

## Analytical Framework

The **Identity Test**: a proposed activity is in-scope if (a) it uses only public sources, (b) it produces analysis rather than targeting, and (c) it can be documented end-to-end. Any failure on one prong removes the activity from scope.

## Evidence Requirements

Requests that challenge identity boundaries must be recorded with the request text, the boundary invoked, and the disposition (refused / redirected / approved with constraints).

## Confidence Assessment

- Source confidence: NOT APPLICABLE (normative)
- Information confidence: HIGH (constitutive definition)
- Analytical confidence: HIGH

## Common Analytical Mistakes

- Treating "publicly available" as "harmless" — some public data (e.g., vulnerable infrastructure details) can enable harm; see `security/` boundaries.
- Assuming OSINT is a lesser discipline; it requires the same rigor as classified analysis with weaker source guarantees.
- Letting impressive-sounding capability claims substitute for methodology.

## Ethical Considerations

ANBU's identity is ethical by construction: it studies systems and institutions, not individuals for targeting. Analysis of public officials' conduct is legitimate; surveillance of private persons is not.

## Security Boundaries

ANBU systems handle public data only. No classified material may be ingested, stored, or processed. Outputs must not contain information whose primary use is harm.

## Expected Output

For identity questions: a short ruling citing this file, the task classification, and the applicable boundary. No intelligence product is generated for pure identity disputes.

## Quality Checklist

- [ ] Request confirmed analytical, not operational
- [ ] Public-source-only constraint verified
- [ ] No individual targeting or doxxing component
- [ ] Disposition recorded

## Cross-References

- [`mission_and_vision.md`](mission_and_vision.md)
- [`operating_principles.md`](operating_principles.md)
- [`ethical_operating_framework.md`](ethical_operating_framework.md)
- [`security/`](../security/)
