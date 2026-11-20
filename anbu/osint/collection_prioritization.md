# Collection Prioritization

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Defines methods for prioritizing collection activities: ranking source classes, queries, and collection slices under constraints.

## Scope

All collection planning, ensuring effort is allocated to highest-value collection activities first.

## Intelligence objectives

- Rank collection slices by expected value
- Optimize effort under time and access constraints
- Balance coverage across source classes
- Identify quick wins versus deep collection

## Core concepts

- Expected value of collection
- Effort versus yield tradeoffs
- Source class coverage balance
- Quick wins identification
- Collection slicing and phasing

## Analytical methodology

Collection slices are ranked by: expected yield (probability of relevant findings), access cost, verification burden, and time sensitivity. Quick wins (high yield, low cost) are prioritized. Deep collection (high cost, high value) is scheduled for dedicated cycles. Coverage balance ensures no source class is neglected if relevant.

## Step-by-step workflow

1. Identify collection slices from requirement
2. Score each slice on yield, cost, time
3. Rank slices by expected value
4. Schedule quick wins first
5. Plan deep collection cycles
6. Document prioritization rationale

## Data requirements

Collection requirement; source class inventory; access constraints; time window.

## Approved public sources

- Collection requirement definition
- Source discovery results
- Prior collection logs
- Access constraint assessments

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

Prioritization uses weighted scoring: yield (40%), access cost (30%), time sensitivity (20%), verification burden (10%). Slices scoring high on yield and low on cost are scheduled first. Coverage balance is checked to ensure all relevant source classes are addressed.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Prioritizing by ease rather than value
- Ignoring coverage balance
- Over-investing in low-yield sources
- Failing to document prioritization rationale

## Ethical considerations

Prioritization must not deprioritize ethically required collection or over-prioritize ethically sensitive sources.

## Security boundaries

No prioritization that leads to unlawful or unethical collection.

## Expected output

Prioritized collection plan with ranked slices, scheduling rationale, and coverage balance check.

## Quality checklist

- [ ] Slices scored
- [ ] Ranking documented
- [ ] Coverage balanced
- [ ] Quick wins identified

## Cross-reference links

- `collection_requirement_definition.md`
- `osint_methodology.md`
- `source_discovery.md`
- `information_gap_analysis.md`
- `collection_quality_control.md`

