# ANBU Master Reference Index

**Core Division 001 · File 020 · Classification: REFERENCE**

## Purpose

The master index of the ANBU system: every file, its division, its function, and the reading order for different task types. This is the navigation layer for the whole skill.

## Scope

System-wide index. It lists files and their roles; it does not duplicate their content. As divisions are populated, this index is updated.

## Intelligence Objectives

- Let any analyst or consumer locate the right file for a given need.
- Define canonical reading orders per task class.
- Provide the checklist for system completeness (333 files across 15 divisions).

## Core Concepts

### Reading Orders

**Minimum viable context** (any task):
`SKILL.md` → `core/anbu_identity.md` → `core/user_interaction_protocol.md` → task-class files → division files → `core/output_standards.md` → `core/quality_assurance.md`

**T1 lookup**: SKILL.md → task_classification → relevant division file → output_standards

**T3 assessment**: full minimum viable context + intelligence_framework + confidence_framework + uncertainty_management + ethics + relevant divisions + reporting template

**T4 forecast**: T3 set + analytics/ forecasting files + prediction log requirements

**T6 audit**: quality_assurance + the audited product's own evidence log + verification/ files

### Division Status

| Division | Path | Status | Planned focus |
|---|---|---|---|
| Core | `core/` | COMPLETE (20 files) | Doctrine, protocols, standards |
| OSINT | `osint/` | PLANNED | Collection tradecraft, source classes |
| Political | `political/` | PLANNED | Elections, parties, institutions |
| Military | `military/` | PLANNED | Posture, procurement, doctrine |
| State | `state/` | PLANNED | Governance, bureaucracy, services |
| Geopolitical | `geopolitical/` | PLANNED | Alliances, conflict, sanctions |
| Verification | `verification/` | PLANNED | Authenticity, corroboration, geolocation |
| Analytics | `analytics/` | PLANNED | SATs, indicators, forecasting |
| Geoint | `geoint/` | PLANNED | Imagery, terrain, movement analysis |
| Legal | `legal/` | PLANNED | Treaties, regulation, accountability |
| Security | `security/` | PLANNED | Threats, protective intelligence, cyber |
| Reporting | `reporting/` | PLANNED | Templates, formats, dissemination |
| Workflows | `workflows/` | PLANNED | Pipelines, repeatable procedures |
| Manifests | `manifests/` | PLANNED | Inventories, versioning, config |

### File Inventory — Core Division (Complete)

| # | File | Function |
|---|---|---|
| 001 | `SKILL.md` (root) | Entry point, division map, protocol overview |
| 002 | `core/anbu_identity.md` | What ANBU is and is not |
| 003 | `core/mission_and_vision.md` | Mission test, vision discipline |
| 004 | `core/operating_principles.md` | Durable behavioral doctrine |
| 005 | `core/intelligence_framework.md` | Evidence vocabulary, analytic cycle |
| 006 | `core/intelligence_taxonomy.md` | Requirement & product classification |
| 007 | `core/system_architecture.md` | Layers, components, data flow |
| 008 | `core/capability_matrix.md` | What ANBU can/cannot do |
| 009 | `core/user_interaction_protocol.md` | The 10-step engagement protocol |
| 010 | `core/execution_protocol.md` | Execution states, evidence log |
| 011 | `core/task_classification.md` | T1–T6 task classes, TX triggers |
| 012 | `core/workflow_orchestrator.md` | Workflow selection & composition |
| 013 | `core/intelligence_glossary.md` | ANBU-specific terms |
| 014 | `core/terminology_dictionary.md` | General analytical vocabulary |
| 015 | `core/output_standards.md` | Mandatory product elements |
| 016 | `core/quality_assurance.md` | The 9 quality gates |
| 017 | `core/confidence_framework.md` | Three-dimensional confidence |
| 018 | `core/uncertainty_management.md` | Types, expression, budgeting |
| 019 | `core/ethical_operating_framework.md` | Binding ethical boundaries |
| 020 | `core/master_reference_index.md` | This file — system navigation |

## Analytical Methodology

The index is maintained as divisions are built. A file not listed here does not exist; a listed file that doesn't exist is a defect.

## Step-by-Step Workflow

1. Identify task class.
2. Consult the reading order for that class.
3. Load files in order; do not skip doctrine for tradecraft.
4. After task completion, note any files that were missing or inadequate — feed back into division planning.

## Data Requirements

Index maintenance requires: file list per division, function summary, status, and cross-reference validation.

## Approved Public Sources

Not applicable.

## Source Verification Standards

Index accuracy is verified mechanically: every listed file must exist; every existing file must be listed.

## Analytical Framework

**Progressive Disclosure Enforcement**: the index exists so that no task loads the entire system. Loading order is part of the methodology, not a convenience.

## Evidence Requirements

System completeness is measured against the 333-file target: core = 20, remaining 313 across 14 divisions.

## Confidence Assessment

- Source confidence: NOT APPLICABLE
- Information confidence: HIGH for core; INSUFFICIENT for unbuilt divisions
- Analytical confidence: HIGH

## Common Analytical Mistakes

- Loading all files regardless of task (violates progressive disclosure).
- Citing division files that are planned but not yet written.
- Letting the index drift from the actual file tree.

## Ethical Considerations

The index makes the system's boundaries visible: a reader can see exactly what exists and what doesn't — no implied capabilities.

## Security Boundaries

Index entries describe file functions only; no sensitive operational detail is stored here.

## Expected Output

Navigation-ready system map; completeness tracking against the 333-file target.

## Quality Checklist

- [ ] Every existing file listed
- [ ] Every listed file exists
- [ ] Reading orders defined per task class
- [ ] Division status current
- [ ] Cross-references resolve

## Cross-References

- [`system_architecture.md`](system_architecture.md)
- [`SKILL.md`](../SKILL.md)
- [`manifests/`](../manifests/)
- All division directories
