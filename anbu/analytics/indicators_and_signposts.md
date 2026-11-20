# Indicators and Signposts

**ANBU Division 008 · Analytics**

---

## Purpose

Indicators and signposts translate analysis into observable tripwires. An indicator is a specific, measurable phenomenon whose presence signals that a hypothesis or scenario is unfolding; a signpost is the decision point where a consumer should act on it. This file defines how ANBU builds indicator sets that are observable in public sources, specific enough to be meaningful, and timely enough to matter.

## Scope

Applied to warning products, scenario analyses, and monitoring tasks. Covers political, military, economic, and security developments where public indicators can plausibly precede or accompany the event of interest.

## Intelligence objectives

- Convert analytical judgments into monitorable conditions.
- Provide early warning that survives contact with ambiguous reality.
- Enable consumers to trigger contingency actions on defined criteria rather than vibes.
- Track which scenario of a scenario-planning exercise is materializing.

## Core concepts

- **Indicator.** A concrete observable: a named official's travel pattern, a procurement category appearing in budgets, a statistical series crossing a threshold, a rhetorical shift in official statements.
- **Signpost.** The threshold or conjunction of indicators that constitutes actionable warning.
- **Specificity vs. sensitivity trade-off.** Specific indicators rarely false-alarm but may miss events; sensitive ones catch more but generate noise.
- **Diagnostic vs. ambient indicators.** Diagnostic indicators point at a specific hypothesis; ambient indicators describe the environment and may support many hypotheses.
- **Decay.** Indicators have shelf lives; an indicator valid last year may be meaningless after a structural change.

## Analytical methodology

1. Identify the hypothesis, scenario, or event the indicators should track.
2. Ask: what would be observably different in the world if this were happening?
3. Convert each expected difference into a public-source-observable indicator.
4. Specify each indicator precisely: what, where observed, threshold, expected baseline.
5. Define signpost conditions: single strong indicator or combinations.
6. Assign collection frequency and source responsibility.
7. Re-validate indicators periodically; retire decayed ones.

## Step-by-step workflow

1. Take the assessment or scenario product.
2. For each key hypothesis, list expected observable signatures.
3. Filter signatures through the public-observability test — can an OSINT analyst actually see this?
4. Write indicator cards: name | definition | source | baseline | trigger threshold | collection cadence.
5. Group indicators into signpost rules (e.g., "any two of A, B, C within 30 days").
6. Issue to `../workflows/monitoring_and_warning.md` for ongoing collection.
7. Review on schedule; adjust thresholds based on observed noise.

## Data requirements

- The underlying assessment or scenarios.
- Baseline data for each indicator (normal levels, seasonal patterns).
- Identified public sources capable of observing each indicator.
- A monitoring cadence matched to the warning timeline.

## Approved public sources

Official gazettes and procurement portals; parliamentary/legislative records; central bank and statistics publications; official statements and state media; court dockets; corporate filings and earnings calls; satellite imagery tasking via `../geoint/`; reputable news wires for corroboration only.

## Source verification standards

Indicator triggers require verified observation, not rumor. A single unverified report may be logged as "possible" but cannot fire a signpost alone. See `../verification/indicator_verification.md`.

## Analytical framework

Indicator quality test — every indicator must answer:

| Test | Question |
|---|---|
| Observable | Can we actually see it in public sources? |
| Specific | Does it distinguish the target event from routine noise? |
| Timely | Does it appear early enough to matter? |
| Stable | Is the baseline measurable and the threshold meaningful? |
| Attributable | Can we cite exactly where it was observed? |

## Evidence requirements

- Baseline measurements cited to public statistical sources.
- Trigger events documented with date, source, and verification grade.
- Signpost firings recorded with the indicator set state at the time.

## Confidence assessment

Confidence attaches to the indicator set's design, not to individual observations:

- **HIGH** — indicators are specific, baselines well-established, multiple corroborating sources exist.
- **MODERATE** — indicators plausible but baselines thin or sources single.
- **LOW** — indicators largely speculative or observability marginal.
- **INSUFFICIENT** — no reliable public indicators exist; say so and recommend collection requirements.

## Common analytical mistakes

- Writing indicators that are technically true but unobservable ("intent to escalate").
- Setting thresholds so loose they always fire, or so tight they never do.
- Ignoring base rates — an indicator that fires often tells little.
- Treating indicator absence as evidence of absence without checking observability.
- Never retiring decayed indicators.

## Ethical considerations

Indicators must target events and institutions, not private individuals' private behavior. Where an indicator would require monitoring a private person's communications or movements, it is out of scope. Warning products must not be framed to enable pre-emptive action against lawful political activity.

## Security boundaries

All indicator observation uses public sources only. No tasking of intrusive collection, no monitoring of non-public channels, no use of indicators to profile individuals beyond what public institutional analysis permits.

## Expected output

An indicator annex: indicator cards, signpost rules, monitoring cadence, and a short warning protocol stating who is notified when a signpost fires and what confidence attaches.

## Quality checklist

- [ ] Every indicator passes the five tests in the framework.
- [ ] Baselines are cited and current.
- [ ] Signpost rules are explicit (which indicators, what combination).
- [ ] Cadence matches the warning timeline.
- [ ] Decay review scheduled.
- [ ] Single-source triggers flagged as "possible" not "confirmed."

## Cross-reference links

- [`trend_analysis.md`](trend_analysis.md) — trends supply indicator candidates.
- [`pattern_analysis.md`](pattern_analysis.md) — patterns become signposts.
- [`strategic_warning_analysis.md`](strategic_warning_analysis.md) — scenarios need indicators.
- [`intelligence_synthesis.md`](intelligence_synthesis.md) — synthesis consumes indicator state.
- [`strategic_warning_analysis.md`](strategic_warning_analysis.md) — warning doctrine.
- [`../verification/indicator_verification.md`](../verification/indicator_verification.md) — trigger standards.
- [`../workflows/monitoring_and_warning.md`](../workflows/monitoring_and_warning.md) — collection loop.
- [`../reporting/warning_product_template.md`](../reporting/warning_product_template.md) — warning format.
