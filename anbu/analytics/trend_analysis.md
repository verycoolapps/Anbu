# Trend Analysis

**ANBU Division 008 · Analytics**

---

## Purpose

Trend analysis identifies the direction, rate, and durability of change in political, economic, military, and social phenomena — and assesses whether an observed trend will continue, accelerate, stall, or reverse. In OSINT, trends are often asserted from headlines; this file requires them to be demonstrated from data and qualified by structural analysis.

## Scope

Applied to quantitative and qualitative time series: budgets, election results, force sizes, price levels, opinion series, conflict incidence, institutional outputs. Also covers qualitative trends (rhetorical escalation, doctrinal evolution) where repeated observations establish direction.

## Intelligence objectives

- Establish whether a change is a trend, a cycle, or noise.
- Estimate trend direction and rough trajectory.
- Identify trend drivers and likely inflection points.
- Produce signposts for trend continuation or reversal.

## Core concepts

- **Trend.** Sustained directional change over multiple observations, not a single data point.
- **Cycle vs. trend.** Cycles oscillate around a mean; trends persist in one direction. Misreading a cycle peak as a trend produces bad forecasts.
- **Inflection point.** Where trend direction or rate changes; often driven by structural breaks.
- **Base rate of change.** Historical pace of change sets expectations; extrapolation must respect it.
- **Leading vs. lagging indicators.** Some series move before the phenomenon they indicate; others confirm after.
- **Saturation/ceiling effects.** Trends cannot continue indefinitely; approaching limits changes dynamics.

## Analytical methodology

1. Define the trend precisely: variable, direction, timeframe, scope.
2. Assemble the time series; check data quality, definitional consistency, and gaps.
3. Plot or tabulate; identify direction, rate, volatility, and breaks.
4. Distinguish trend from cycle and noise using multiple observations.
5. Identify candidate drivers via `causal_analysis.md` and `political_economy_analysis.md`.
6. Assess durability: what structural factors support or constrain continuation?
7. Define inflection indicators and project scenarios per `strategic_warning_analysis.md`.
8. Report trend statement with confidence and signposts.

## Step-by-step workflow

1. Receive the trend question (e.g., "is military spending rising?").
2. Identify the authoritative public series; document source, frequency, definitions.
3. Extract the full available series, not a convenient window.
4. Compute direction and rate; note anomalies, revisions, and definitional breaks.
5. Check against alternative explanations: cycle, one-off shock, data artifact.
6. Identify drivers and constraints from structural analysis.
7. Write the trend statement: direction, rate, confidence, key drivers, reversal conditions.
8. Attach indicators for continuation vs. inflection.

## Data requirements

- Long, consistent time series from authoritative sources.
- Documentation of definitions and methodology changes.
- For qualitative trends: dated corpus of comparable statements or events.
- Enough observations to distinguish trend from noise — rule of thumb: 3+ cycles or 10+ points for slow phenomena.

## Approved public sources

National statistics offices; central banks; defense budget publications and SIPRI/IISS databases; UN agencies; electoral commissions; official gazettes; reputable longitudinal datasets; court and parliamentary records for institutional trends.

## Source verification standards

Trend claims must cite the underlying series, not commentary about it. Check for definitional changes (e.g., what counts as "military spending"), revisions, and missing years. See `../verification/statistical_source_review.md`.

## Analytical framework

Trend assessment table:

| Element | Content |
|---|---|
| Variable | Precisely defined measure |
| Direction | Rising / falling / stable / U-shaped |
| Rate | Per-period change, recent vs. historical |
| Volatility | Stability of the movement |
| Drivers | Structural factors identified |
| Constraints | Limits, ceilings, countervailing forces |
| Inflection risk | What could reverse or accelerate it |

## Evidence requirements

- Full series cited with source and retrieval date.
- Data gaps and definitional breaks disclosed.
- Drivers linked to evidence, not assumed.
- Extrapolation limited and labeled as such.

## Confidence assessment

- **HIGH** — long consistent series, clear direction, understood drivers, no pending structural break.
- **MODERATE** — clear recent direction but limited history or uncertain drivers.
- **LOW** — short series, volatile movement, or conflicting indicators.
- **INSUFFICIENT** — no reliable series; qualitative impression only, say so.

## Common analytical mistakes

- Extrapolating a short-term move into a "trend."
- Ignoring base rates and saturation limits.
- Treating data revisions or definitional changes as real change.
- Cherry-picking the window that shows the preferred direction.
- Confusing cycle peaks/troughs with trend turns.
- Attributing trend to a single cause when multiple drivers operate.

## Ethical considerations

Trend claims about social groups can feed harmful narratives; present them with appropriate context and avoid essentializing. Long-range forecasts must carry uncertainty proportional to their horizon.

## Security boundaries

Trend analysis uses public statistical and documentary sources only. No projections may be framed as targeting or threat lists against individuals or lawful groups.

## Expected output

Trend annex: series citation, direction/rate statement, driver analysis, inflection indicators. Main product: 1–2 paragraph trend assessment with confidence and signposts.

## Quality checklist

- [ ] Series is authoritative, consistent, and fully cited.
- [ ] Direction and rate quantified, not just asserted.
- [ ] Cycle vs. trend distinguished.
- [ ] Drivers evidenced, constraints noted.
- [ ] Reversal/inflection conditions stated.
- [ ] Confidence matches series quality and horizon.

## Cross-reference links

- [`pattern_analysis.md`](pattern_analysis.md) — patterns within trends.
- [`indicators_and_signposts.md`](indicators_and_signposts.md) — trend signposts.
- [`strategic_warning_analysis.md`](strategic_warning_analysis.md) — trend-based scenarios.
- [`causal_analysis.md`](causal_analysis.md) — why trends move.
- [`correlation_vs_causation.md`](correlation_vs_causation.md) — trend drivers are causal claims.
- [`../verification/statistical_source_review.md`](../verification/statistical_source_review.md) — series quality.
- [`../reporting/assessment_template.md`](../reporting/assessment_template.md) — output format.
