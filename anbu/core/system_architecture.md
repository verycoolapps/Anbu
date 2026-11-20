# ANBU System Architecture

**Core Division 001 · File 007 · Classification: FOUNDATIONAL**

## Purpose

Describes the logical and functional architecture of ANBU: components, their responsibilities, data flows, and the interfaces between core doctrine and division tradecraft.

## Scope

System-level design. Implementation details (file formats, tooling) belong to `manifests/` and `workflows/`; this file defines the shape those implementations must respect.

## Intelligence Objectives

- Make the system's structure explicit so extensions don't contradict doctrine.
- Define clear ownership: every function belongs to exactly one division.
- Enable progressive disclosure: modules load only when needed.

## Core Concepts

### Layered Architecture

```
┌─────────────────────────────────────┐
│  INTERACTION LAYER                  │
│  SKILL.md · user_interaction_protocol│
├─────────────────────────────────────┤
│  DOCTRINE LAYER (core/)             │
│  identity · principles · framework  │
│  taxonomy · confidence · QA         │
├─────────────────────────────────────┤
│  TRADECRAFT LAYER (divisions/)      │
│  osint · political · military ·     │
│  state · geopolitical · verification│
│  analytics · geoint · legal ·       │
│  security · reporting · workflows   │
├─────────────────────────────────────┤
│  RECORD LAYER                       │
│  manifests/ · evidence logs ·       │
│  assessment history                 │
└─────────────────────────────────────┘
```

### Component Responsibilities

| Component | Owns | Must not own |
|---|---|---|
| core/ | Doctrine, vocabulary, standards | Domain tradecraft |
| osint/ | Collection methods, source classes | Analysis judgments |
| verification/ | Authenticity, corroboration | Collection, reporting |
| analytics/ | Structured techniques, forecasting | Source acquisition |
| division domains | Domain-specific frameworks | Cross-domain doctrine |
| reporting/ | Product formats | Analytical content |
| workflows/ | Pipelines, orchestration | Standards |

### Data Flow

Question → classification → collection plan → acquisition (provenance logged) → evaluation → analysis → verification → graded report → record.

## Analytical Methodology

Architecture is enforced through the cross-reference graph: files link to the doctrine they depend on. A division file that contradicts core doctrine is defective regardless of local quality.

## Step-by-Step Workflow

1. Intake at the interaction layer.
2. Load doctrine files for the task class.
3. Load division files per scope.
4. Execute the workflow; log evidence.
5. Report per standards; record outcome.

## Data Requirements

Every data object carries: provenance, evidence label, confidence triple, and division tag.

## Approved Public Sources

Architecture constrains flow, not sources. Source approval is per-division.

## Source Verification Standards

See `verification/` and `quality_assurance.md`.

## Analytical Framework

**Separation of Duties**: collection, analysis, and verification are distinct functions. Where a single analyst performs all three, the verification pass is performed as a separate, later step with fresh eyes — never inline during collection.

## Evidence Requirements

Architectural integrity check: every file must (a) declare its division, (b) cross-reference its doctrine dependencies, and (c) respect the layered boundaries above.

## Confidence Assessment

- Source confidence: NOT APPLICABLE
- Information confidence: HIGH (design specification)
- Analytical confidence: HIGH

## Common Analytical Mistakes

- Letting a division file redefine doctrine locally ("in this file, FACT means…").
- Bypassing verification because collection felt thorough.
- Building workflow shortcuts that skip evidence logging.

## Ethical Considerations

Layered separation exists partly for ethics: the verification layer is the checkpoint where harmful or out-of-scope material is caught. Collapsing layers removes the checkpoint.

## Security Boundaries

No layer handles classified data. The record layer stores public-source derivatives only, with provenance intact.

## Expected Output

Architecturally compliant products: correct division routing, complete provenance, verified claims, doctrine-consistent language.

## Quality Checklist

- [ ] Division ownership respected
- [ ] Doctrine loaded before tradecraft
- [ ] Provenance logged end-to-end
- [ ] Verification pass completed separately
- [ ] Cross-references resolve

## Cross-References

- [`capability_matrix.md`](capability_matrix.md)
- [`workflow_orchestrator.md`](workflow_orchestrator.md)
- [`master_reference_index.md`](master_reference_index.md)
- [`manifests/`](../manifests/)
