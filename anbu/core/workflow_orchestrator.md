# ANBU Workflow Orchestrator

**Core Division 001 · File 012 · Classification: FOUNDATIONAL**

## Purpose

Defines how multi-step analytical work is orchestrated: which workflows exist, how they compose, and how state moves between them. The orchestrator sits above individual workflows and below the interaction protocol.

## Scope

Workflow selection, composition, and state management. Individual workflow procedures live in `workflows/`; this file governs their coordination.

## Intelligence Objectives

- Prevent ad-hoc process drift: every engagement runs a known workflow or a documented variant.
- Enable parallel work where divisions are independent.
- Make workflow choice explicit so it can be reviewed.

## Core Concepts

### Canonical Workflows

| Workflow | Steps compressed | Typical classes |
|---|---|---|
| WF-LOOKUP | Intake → source → report | T1 |
| WF-PROFILE | Intake → multi-source collection → synthesis → report | T2 |
| WF-ASSESS | Full 10-step protocol | T3 |
| WF-FORECAST | WF-ASSESS + forecasting framework + prediction log | T4 |
| WF-WARNING | WF-ASSESS expedited + monitoring triggers | T5 |
| WF-AUDIT | Load prior product → re-verify → quality report | T6 |

### Orchestration Rules

1. Every engagement instantiates exactly one canonical workflow or a declared composite.
2. Composite workflows name their component workflows and the merge point.
3. A workflow may not skip a hard gate defined in `user_interaction_protocol.md`.
4. Parallel division work merges at the analysis step, never at collection (each collector logs independently).

### State Model

Orchestration state = interaction protocol state + per-division substates. The orchestrator tracks division completion; the protocol tracks phase completion.

## Analytical Methodology

Workflow choice follows task class: higher classes get fuller workflows. The orchestrator's job is fit, not maximization — a T1 lookup does not run WF-ASSESS.

## Step-by-Step Workflow

1. Receive classified task.
2. Select canonical workflow; declare composite if needed.
3. Instantiate state; assign division owners.
4. Run phases; log transitions.
5. Merge division outputs at analysis.
6. Single verification pass over merged material.
7. Report; close state.

## Data Requirements

Orchestration record: workflow ID, component list, division assignments, state transitions, merge decisions.

## Approved Public Sources

Workflow-agnostic; source rules live in division files.

## Source Verification Standards

Merged material undergoes one consolidated verification pass — per-division verification happens during collection, cross-division verification happens at merge.

## Analytical Framework

**Merge Discipline**: when division outputs combine, conflicting claims are not averaged — they are both preserved, labeled, and resolved by evidence weight or reported as a genuine disagreement.

## Evidence Requirements

The orchestration record must show: workflow chosen, why, who owned what, where merges happened, and how conflicts were resolved.

## Confidence Assessment

- Source confidence: NOT APPLICABLE
- Information confidence: HIGH (procedure)
- Analytical confidence: HIGH for workflow fit; degraded if composite is undeclared

## Common Analytical Mistakes

- Running the heaviest workflow for every task (wasted effort, delayed output).
- Merging division outputs without a conflict-resolution rule.
- Losing orchestration state on session boundaries.

## Ethical Considerations

Orchestration must not become a mechanism for parallelizing out-of-scope work: each branch still passes its own step-3 gate.

## Security Boundaries

Workflow composition does not expand source permissions. All branches remain inside public-source bounds.

## Expected Output

Coordinated multi-division product with intact provenance and a complete orchestration record.

## Quality Checklist

- [ ] Workflow declared
- [ ] Gates preserved
- [ ] Merge rule applied
- [ ] State transitions logged
- [ ] Conflicts preserved, not averaged

## Cross-References

- [`execution_protocol.md`](execution_protocol.md)
- [`user_interaction_protocol.md`](user_interaction_protocol.md)
- [`workflows/`](../workflows/)
- [`system_architecture.md`](system_architecture.md)
