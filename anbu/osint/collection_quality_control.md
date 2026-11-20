# Collection Quality Control

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Defines quality control procedures for collection: completeness checks, provenance verification, and reliability assessment.

## Scope

All collection activity, ensuring collected information meets quality standards before entering analysis.

## Intelligence objectives

- Verify collection completeness against requirements
- Validate provenance and source reliability
- Check for errors and inconsistencies
- Ensure quality standards are met before hand-off

## Core concepts

- Quality control checkpoints
- Completeness metrics
- Provenance validation
- Reliability scoring
- Error detection and correction

## Analytical methodology

QC is performed at collection cycle end. Check: log completeness (all fields filled), provenance validity (URLs accessible, timestamps accurate), source reliability (assessments current), content accuracy (spot checks), and requirement coverage (success criteria met). Document QC findings and corrective actions.

## Step-by-step workflow

1. Review collection log for completeness
2. Validate provenance records
3. Spot-check content accuracy
4. Assess source reliability
5. Check requirement coverage
6. Document QC findings and actions

## Data requirements

Collection log; collection requirement; source reliability assessments; spot-check samples.

## Approved public sources

- Collection log
- Collection requirement
- Source reliability database
- Verification division findings

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

QC uses checklist-based assessment. Completeness threshold: 95% of items with all fields. Provenance threshold: all URLs validated. Reliability threshold: all sources rated. Failures trigger corrective action or collection review.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Skipping QC before analysis hand-off
- Incomplete spot-checking
- Ignoring QC failures
- Not documenting corrective actions

## Ethical considerations

QC must not compromise source protection or expose collection methods.

## Security boundaries

QC findings must not reveal sensitive collection tradecraft.

## Expected output

QC report with findings, corrective actions, and quality metrics.

## Quality checklist

- [ ] Log completeness checked
- [ ] Provenance validated
- [ ] Reliability assessed
- [ ] Coverage confirmed

## Cross-reference links

- `source_collection_log.md`
- `osint_methodology.md`
- `information_gap_analysis.md`
- `verification/`
- `security/`

