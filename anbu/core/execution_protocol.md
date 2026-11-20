# ANBU Execution Protocol

**Core Division 001 · File 010 · Classification: FOUNDATIONAL**

## Purpose

Defines how an approved engagement is executed after the interaction protocol's planning steps: the operational discipline for collection, analysis, verification, and handoff. Where `user_interaction_protocol.md` governs the conversation, this file governs the work.

## Scope

Execution discipline: sequencing, logging, iteration rules, and handoff standards. It does not redefine the 10 steps; it specifies how steps 5–9 are carried out.

## Intelligence Objectives

- Make execution auditable: every analytical act is reconstructible from the log.
- Prevent silent scope changes mid-engagement.
- Ensure handoffs between analysts or sessions preserve state.

## Core Concepts

### Execution States

`PLANNED → COLLECTING → EVALUATING → ANALYZING → VERIFYING → REPORTING → CLOSED`

Each transition is logged with timestamp and actor. Regressions (e.g., ANALYZING → COLLECTING when new evidence demands it) are permitted and logged as iterations.

### The Evidence Log

The single authoritative record of the engagement. Every collected item, every label assignment, every hypothesis revision is appended. The log — not memory — is the state of the analysis.

### Iteration Rules

- New evidence that contradicts a labeled claim triggers re-evaluation of that claim and its dependents.
- Hypotheses are never deleted; they are marked CONFIRMED / WEAKENED / ELIMINATED with the evidence that did it.
- Scope changes require re-passing the step-3 ethics gate.

## Analytical Methodology

Execution follows the plan from step 5 unless evidence demands deviation; deviations are logged with reason. Improvisation is allowed; unlogged improvisation is not.

## Step-by-Step Workflow

1. Confirm PLANNED state; load the collection plan.
2. COLLECTING: acquire items; append each to the evidence log with provenance.
3. EVALUATING: assign source grade and information grade per item; assign evidence label.
4. ANALYZING: populate the hypothesis matrix; document reasoning chains.
5. VERIFYING: run corroboration checks; adjust labels and confidence.
6. REPORTING: assemble product per `output_standards.md`.
7. CLOSED: archive log, product, and QA checklist.

## Data Requirements

Evidence log schema: `item_id | source | source_class | retrieved | method | label | source_conf | info_conf | notes`. Hypothesis matrix schema: `hypothesis | supporting_evidence | contradicting_evidence | status`.

## Approved Public Sources

Per the collection plan; execution may not introduce sources outside the approved classes without logging the addition and re-checking ethics.

## Source Verification Standards

Verification is a state, not an afterthought: items remain UNVERIFIED until the verifying pass completes.

## Analytical Framework

**State Machine Discipline**: the execution state reflects the furthest completed phase. A product cannot be marked REPORTING while items remain unevaluated.

## Evidence Requirements

At handoff, the log must support a full reconstruction: what was collected, how it was graded, what was concluded, and what remains uncertain.

## Confidence Assessment

- Source confidence: per item, logged
- Information confidence: per item, logged
- Analytical confidence: per conclusion, stated in product

## Common Analytical Mistakes

- Losing state between sessions (log not updated).
- Treating the plan as fixed when evidence demands iteration.
- Handoff without the evidence log — the next analyst starts blind.

## Ethical Considerations

The log is also the ethics record: it shows what was collected, so out-of-scope acquisition is detectable and auditable.

## Security Boundaries

Logs contain public-source derivatives only. No credentials, no classified references, no personal data beyond what public sources legitimately contain and the task requires.

## Expected Output

Complete evidence log, hypothesis matrix, labeled claim set, and the graded product.

## Quality Checklist

- [ ] State transitions logged
- [ ] Evidence log complete and append-only
- [ ] Iterations recorded with reasons
- [ ] Handoff package complete
- [ ] No unlogged scope changes

## Cross-References

- [`user_interaction_protocol.md`](user_interaction_protocol.md)
- [`workflow_orchestrator.md`](workflow_orchestrator.md)
- [`uncertainty_management.md`](uncertainty_management.md)
- [`quality_assurance.md`](quality_assurance.md)
