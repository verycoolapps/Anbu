# Strategic Warning Analysis

**ANBU Division 008 · Analytics**

---

## Purpose

Strategic warning analysis detects and assesses developments that could significantly affect national, regional, or global security and stability — early enough for decision-makers to act. It is the forward-looking edge of intelligence: not reporting what happened, but identifying what is building toward consequences that matter. This file defines how ANBU conducts strategic warning from public sources, structures warning products, and maintains the credibility that makes warnings actionable rather than noise.

## Scope

Applied to developments with strategic significance: potential conflicts, state instability, proliferation, economic crises with security implications, alliance shifts, and other events whose consequences could reshape the strategic environment. Covers both specific-event warning and trend-based early warning.

## Intelligence objectives

- Identify developments that could produce strategic consequences.
- Assess probability and time horizon of warned events.
- Provide sufficient lead time for decision-makers to consider options.
- Avoid warning fatigue: maintain signal-to-noise ratio.
- Structure warnings so they are actionable, not merely alarming.

## Core concepts

- **Strategic significance.** The consequence test: would this event materially change the strategic balance, state stability, or regional order?
- **Warning vs. forecast.** Warning identifies that something may happen and signals urgency; forecast estimates probability and timing. Warnings are triggers; forecasts are estimates.
- **Indicators and signposts.** The observable markers that an event is approaching — see `indicators_and_signposts.md`.
- **Warning timeline.** The window between detection and consequence; warning is useless if it arrives after the event.
- **False alarm cost.** Warnings that don't materialize erode credibility; the cost of false alarms must be weighed against missed warnings.
- **Warning thresholds.** Pre-defined criteria for issuing warnings at different levels — prevents both under- and over-warning.
- **Strategic surprise.** The failure mode warning exists to prevent: being caught unprepared by an event that was detectable in principle.

## Analytical methodology

1. Monitor indicators and trends across strategic domains.
2. Identify developments crossing warning thresholds.
3. Assess probability and time horizon per `risk_probability_assessment.md`.
4. Assess potential impact per `impact_assessment.md`.
5. Determine warning level per threshold criteria.
6. Structure the warning product: what, why it matters, probability, timeframe, indicators, recommended attention.
7. Disseminate to appropriate consumers.
8. Track outcome: did the warned event occur? Was the warning timely?

## Step-by-step workflow

1. **Monitoring.** Continuously collect indicators per `indicators_and_signposts.md` and `../workflows/monitoring_and_warning.md`.
2. **Detection.** Identify developments crossing predefined thresholds.
3. **Assessment.** Evaluate probability (`risk_probability_assessment.md`), impact (`impact_assessment.md`), and timeframe.
4. **Warning decision.** Determine if thresholds met for warning issuance; assign warning level.
5. **Product.** Write warning per `../reporting/warning_product_template.md`.
6. **Dissemination.** Route to appropriate consumers with appropriate urgency.
7. **Tracking.** Monitor indicators for event development or warning resolution.
8. **Review.** After event resolution or timeout, review warning accuracy and timeliness.

## Data requirements

- Continuous indicator monitoring infrastructure.
- Baseline data for threshold calibration.
- Probability assessment capability.
- Impact assessment capability.
- Defined warning thresholds and levels.
- Consumer feedback mechanism.

## Approved public sources

All OSINT sources — warning depends on breadth. Priority: official military/diplomatic signals, economic indicators, political instability markers, conflict datasets, proliferation indicators, alliance behavior.

## Source verification standards

Warning-triggering indicators require verified observation. Single unverified reports may trigger "watch" status but not formal warning. See `../verification/indicator_verification.md`.

## Analytical framework

Warning levels:

| Level | Criteria | Action |
|---|---|---|
| WATCH | Indicators present; development possible | Monitor; no formal warning |
| CAUTION | Multiple indicators; probability rising | Issue caution to relevant consumers |
| WARNING | Thresholds met; probability moderate-high | Issue formal warning with timeframe |
| CRITICAL | High probability; imminent or high impact | Issue urgent warning; recommend action |

Warning product structure:

1. What is being warned about (precise event).
2. Why it matters (strategic significance).
3. Probability and timeframe.
4. Key indicators observed.
5. What would confirm or disconfirm.
6. Recommended consumer attention.

## Evidence requirements

- Indicator observations verified and dated.
- Probability estimate with reference class.
- Impact assessment with comparable cases.
- Threshold criteria documented.
- Warning level justified.
- Consumer feedback tracked.

## Confidence assessment

Warning confidence reflects indicator quality and assessment rigor:

- **HIGH** — multiple verified indicators; robust probability and impact assessment; thresholds clearly met.
- **MODERATE** — indicators present; assessment reasonable; some uncertainty in timing or magnitude.
- **LOW** — early indicators only; significant uncertainty; issue as WATCH/CAUTION not WARNING.
- **INSUFFICIENT** — cannot assess; report monitoring status and gaps.

## Common analytical mistakes

- Warning fatigue: too many warnings, too little discrimination.
- Warning on vibes rather than indicators.
- Missing warnings because thresholds too high.
- Not tracking outcomes — no learning from false alarms or misses.
- Conflating warning with prediction: warning says "be ready," not "it will happen."
- Failing to specify timeframe — warning without deadline is useless.
- Not providing disconfirmers — consumer doesn't know what would cancel the warning.
- Single-source warning triggers.
- Warning about everything, prioritizing nothing.

## Ethical considerations

Warnings must be issued responsibly: sufficient evidence, calibrated language, acknowledgment of uncertainty. Must not be used to manufacture consent for preferred policies or to alarm without basis. False warnings carry real costs — credibility, resources, civil liberties.

## Security boundaries

Public indicators only. No warnings based on classified intelligence. No warnings framed as targeting or incitement. Warnings serve protective and decision-support purposes.

## Expected output

Warning product per template, with indicator annex, probability/impact assessment, and tracking plan. Post-event review documenting accuracy and timeliness.

## Quality checklist

- [ ] Indicators verified and documented.
- [ ] Warning thresholds defined and applied.
- [ ] Probability and impact assessed.
- [ ] Warning level appropriate to evidence.
- [ ] Timeframe specified.
- [ ] Disconfirmers stated.
- [ ] Consumer feedback mechanism in place.
- [ ] Outcome tracking scheduled.

## Cross-reference links

- [`indicators_and_signposts.md`](indicators_and_signposts.md) — indicator foundation.
- [`risk_probability_assessment.md`](risk_probability_assessment.md) — probability.
- [`impact_assessment.md`](impact_assessment.md) — consequences.
- [`trend_analysis.md`](trend_analysis.md) — trend-based warning.
- [`strategic_intent_assessment.md`](strategic_intent_assessment.md) — intent signals.
- [`capability_assessment.md`](capability_assessment.md) — capability context.
- [`../workflows/monitoring_and_warning.md`](../workflows/monitoring_and_warning.md) — monitoring pipeline.
- [`../reporting/warning_product_template.md`](../reporting/warning_product_template.md) — output format.
