# Impact Assessment

**ANBU Division 008 · Analytics**

---

## Purpose

Impact assessment estimates the consequences if an event occurs — who is affected, how severely, over what timeframe, and whether effects cascade. Probability without impact is incomplete; impact without probability is alarmism. Together they produce risk: probability × consequence. This file defines how ANBU analysts assess impacts from public evidence and communicate them proportionately.

## Scope

Applied to risk matrices, contingency planning, strategic assessments, and any question of "what happens if X?" Covers humanitarian, economic, political, security, and institutional impacts. Focuses on assessing impact magnitude and distribution, not predicting impact with false precision.

## Intelligence objectives

- Estimate impact magnitude across relevant dimensions.
- Identify who bears impacts — distribution matters as much as magnitude.
- Assess cascading and second-order effects.
- Enable proportional response: impact severity drives resource allocation.
- Communicate impact honestly without catastrophizing or minimizing.

## Core concepts

- **Impact dimensions.** Human (lives, displacement, health), economic (GDP, budgets, livelihoods), political (stability, legitimacy, institutions), security (conflict, crime, order), environmental (where relevant).
- **Direct vs. cascading impact.** Immediate effects vs. downstream consequences through systems.
- **Impact distribution.** Who bears the impact — aggregate numbers hide distributional reality.
- **Threshold effects.** Impacts may be nonlinear: small changes crossing critical thresholds produce outsized effects.
- **Recovery trajectory.** Impact includes duration and reversibility, not just initial severity.
- **Second-order effects.** Effects on actors who respond to the initial impact — refugees affecting neighbors, sanctions affecting third parties.
- **Counterfactual.** What would have happened anyway? Impact is measured against baseline, not zero.

## Analytical methodology

1. Define the event whose impact is assessed.
2. Identify affected populations and systems.
3. Estimate direct impact per dimension using comparable cases and data.
4. Assess distribution: who bears it, who benefits, who is protected.
5. Model cascading effects through relevant systems.
6. Evaluate thresholds and nonlinearity.
7. Estimate duration and recovery trajectory.
8. Combine with probability via `risk_probability_assessment.md` for risk rating.
9. Report impact statement with confidence and uncertainty.

## Step-by-step workflow

1. Define the event and timeframe.
2. Identify affected populations: who, how many, where.
3. Pull baseline data: current conditions, recent trends, existing vulnerabilities.
4. Estimate direct impacts per dimension using comparable cases.
5. Assess distribution: which groups bear disproportionate impact?
6. Identify cascade pathways: economic → political → security → humanitarian.
7. Check thresholds: what tipping points exist?
8. Estimate duration: immediate, medium-term, long-term.
9. Write impact assessment with confidence and comparison cases.

## Data requirements

- Baseline statistics: population, economy, institutions, security conditions.
- Comparable case data: similar events and their documented impacts.
- Vulnerability indicators: poverty, conflict exposure, institutional weakness.
- System interdependency data: trade links, infrastructure, supply chains.
- Historical recovery data for duration estimates.

## Approved public sources

UN OCHA and humanitarian datasets; World Bank and IMF assessments; national statistics offices; conflict datasets (ACLED, UCDP); economic indicators; health surveillance; market and trade data; government contingency plans; academic disaster/conflict impact studies.

## Source verification standards

Impact estimates must cite comparable cases or baseline data. Early-impact reporting is often incomplete and revised; analysts must note estimate vintage. See `../verification/` standards for data quality.

## Analytical framework

Impact assessment matrix:

| Dimension | Magnitude | Distribution | Duration | Confidence |
|---|---|---|---|---|
| Human | [estimate] | [who bears] | [timeframe] | [grade] |
| Economic | [estimate] | [who bears] | [timeframe] | [grade] |
| Political | [estimate] | [who bears] | [timeframe] | [grade] |
| Security | [estimate] | [who bears] | [timeframe] | [grade] |

Magnitude scale: negligible / minor / moderate / major / catastrophic — defined per context, not universal.

## Evidence requirements

- Baseline data cited for affected populations.
- Comparable cases cited for magnitude estimates.
- Distribution analysis shows who bears impact.
- Cascade effects identified and sourced.
- Uncertainty acknowledged: early estimates are provisional.
- Counterfactual considered: impact vs. baseline.

## Confidence assessment

- **HIGH** — impact well-documented from comparable cases; distribution clear; cascades understood.
- **MODERATE** — impact direction clear; magnitude uncertain; some cascades speculative.
- **LOW** — limited comparable cases; distribution unclear; cascades unknown.
- **INSUFFICIENT** — cannot estimate impact reliably; report what is known and gaps.

## Common analytical mistakes

- Aggregate numbers hiding distributional reality.
- Ignoring cascades and second-order effects.
- Confusing initial impact with total impact (duration matters).
- Catastrophizing rare worst cases as expected outcomes.
- Minimizing impacts on vulnerable groups.
- Ignoring counterfactual — what would happen anyway.
- Treating early estimates as final (they are revised).
- Missing threshold effects and nonlinearity.

## Ethical considerations

Impact assessment must center the people affected, not just systems. Human impacts require the highest evidentiary care. Analysts must not minimize humanitarian consequences for political convenience, nor inflate them for advocacy. Vulnerable populations' disproportionate impacts must be highlighted.

## Security boundaries

Public data only. No impact assessments used to justify targeting or collective punishment. Humanitarian impact analysis must serve protection, not operational planning against civilians.

## Expected output

Impact annex: impact matrix per dimension, distribution analysis, cascade map, duration estimate, comparison cases, confidence. Main product states impact magnitude and key vulnerabilities.

## Quality checklist

- [ ] All impact dimensions assessed.
- [ ] Distribution analyzed — who bears it.
- [ ] Cascades identified.
- [ ] Duration and recovery considered.
- [ ] Comparable cases cited.
- [ ] Counterfactual addressed.
- [ ] Confidence reflects estimate quality.

## Cross-reference links

- [`risk_probability_assessment.md`](risk_probability_assessment.md) — probability component.
- [`trend_analysis.md`](trend_analysis.md) — baseline trends.
- [`strategic_warning_analysis.md`](strategic_warning_analysis.md) — impact per scenario.
- [`strategic_warning_analysis.md`](strategic_warning_analysis.md) — warning impact.
- [`political_economy_analysis.md`](political_economy_analysis.md) — economic impacts.
- [`../security/threat_assessment.md`](../security/threat_assessment.md) — security impacts.
- [`../reporting/risk_matrix_template.md`](../reporting/risk_matrix_template.md) — output format.
