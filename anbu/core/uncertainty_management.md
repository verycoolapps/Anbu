# ANBU Uncertainty Management

**Core Division 001 · File 018 · Classification: FOUNDATIONAL**

## Purpose

Defines how ANBU identifies, characterizes, and communicates uncertainty — the discipline that keeps honest analysis honest under pressure to be definitive.

## Scope

Uncertainty doctrine: types, expression, and management. Confidence grading is `confidence_framework.md`; this file covers what to do with what remains unknown.

## Intelligence Objectives

- Make uncertainty specific and actionable rather than vague and ignored.
- Turn unknowns into collection requirements where possible.
- Prevent uncertainty from being hidden by confident prose.

## Core Concepts

### Types of Uncertainty

| Type | Definition | Management |
|---|---|---|
| **Evidential** | Required evidence doesn't exist or isn't accessible | State the gap; lower confidence; flag as collection requirement |
| **Source** | Sources conflict or are unreliable | Report the conflict; weight by source confidence |
| **Analytical** | Multiple explanations fit the evidence | Present competing hypotheses with discriminating tests |
| **Temporal** | Situation is changing faster than analysis | Timestamp everything; shorten shelf-life; add monitoring triggers |
| **Structural** | The system itself is opaque (closed regimes, secret budgets) | State the opacity as a finding; bound estimates accordingly |

### Uncertainty Expression

Uncertainty is expressed three ways, all required:

1. **In the body** — at the point of the uncertain claim, not just in an appendix.
2. **In the uncertainty statement** — the dedicated section naming specific gaps.
3. **In confidence labels** — the three-dimensional table.

### What Uncertainty Is Not

- Not an apology or a hedge-word habit ("it could be argued that…").
- Not a reason to omit analysis — bounded analysis with stated uncertainty beats false precision.
- Not symmetric: some unknowns matter more than others; rank them.

## Analytical Methodology

Uncertainty is managed by decomposition: a vague "we don't know" becomes "we don't know X specifically, and here's what would resolve it." Each named unknown gets a resolution path or an explicit statement that none exists from public sources.

## Step-by-Step Workflow

1. List all unknowns encountered during analysis.
2. Classify each by type.
3. Rank by decision impact.
4. For each: state resolution path or declare it unresolvable publicly.
5. Write the uncertainty statement from this list — not from memory.
6. Verify the statement names *specific* gaps, not generic caveats.

## Data Requirements

Uncertainty register per engagement: `unknown | type | impact | resolution_path | status`.

## Approved Public Sources

Uncertainty about source availability is itself assessed from public information about the information environment.

## Source Verification Standards

Unverified items are uncertainty made visible: they stay labeled UNVERIFIED in products rather than being silently dropped or promoted.

## Analytical Framework

**Uncertainty Budgeting**: allocate analytical effort to the unknowns that most change the conclusion. An unknown that wouldn't change the assessment gets a line, not a paragraph.

## Evidence Requirements

The uncertainty statement must contain at least one *specific* unknown with a named resolution path, or an explicit statement that no public resolution exists. "Further research needed" fails this standard.

## Confidence Assessment

- Source confidence: NOT APPLICABLE
- Information confidence: HIGH for the framework
- Analytical confidence: the framework *produces* analytical confidence ratings; it does not have one itself beyond HIGH

## Common Analytical Mistakes

- Treating uncertainty as a defect to minimize rather than a property to report.
- Hiding uncertainty in footnotes while the body reads confidently.
- Listing unknowns without ranking or resolution paths.
- Confusing "we haven't looked" with "it cannot be known" — different statements, different confidence.

## Ethical Considerations

Downplaying uncertainty is the most common analytical dishonesty. Consumers act on stated confidence; hiding doubt transfers risk to them invisibly.

## Security Boundaries

Uncertainty management does not authorize collection beyond public bounds; it only describes what is not known.

## Expected Output

Products with specific, ranked, actionable uncertainty statements and honest confidence tables.

## Quality Checklist

- [ ] Unknowns listed and typed
- [ ] Ranked by decision impact
- [ ] Resolution paths named or unresolvability declared
- [ ] Uncertainty stated in body, not just appendix
- [ ] No generic caveats

## Cross-References

- [`confidence_framework.md`](confidence_framework.md)
- [`operating_principles.md`](operating_principles.md)
- [`output_standards.md`](output_standards.md)
- [`analytics/`](../analytics/)
