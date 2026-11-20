# Timeline Analysis

**ANBU Division 008 · Analytics**

---

## Purpose

Timeline analysis reconstructs the sequence of events from public sources, resolves timing disputes, and establishes the temporal structure on which causal and intent assessments depend. A wrong timeline corrupts everything built on it. This file defines how ANBU builds defensible event chronologies.

## Scope

Applied to any question involving sequence: what happened before what, how long between events, whether claimed timelines are possible, reconstructing incidents, tracking policy evolution, establishing alibis for institutional claims, and testing causal precedence.

## Intelligence objectives

- Establish verified event ordering from heterogeneous sources.
- Resolve conflicting timestamps and account for timezone/local-time issues.
- Identify gaps in the timeline that represent collection or reporting failures.
- Provide the temporal skeleton for causal, intent, and pattern analysis.

## Core concepts

- **Event anchor.** A firmly dated event (official statement, legislation signed, image verified) that other events are positioned relative to.
- **Time precision tiers.** Exact timestamp > date > "early/mid/late" period > sequence-only ordering. Products must preserve precision honestly.
- **Source time basis.** Publication time ≠ event time; timezone, embargo, and filing delays distort apparent ordering.
- **Simultaneity and overlap.** Events may overlap; forcing strict sequence can falsify reality.
- **Timeline gaps.** Absence of events in a window is itself data — or evidence of collection failure; distinguish which.
- **Reconstruction vs. reporting.** Sources report when they learned of events, not always when they occurred.

## Analytical methodology

1. Collect all dated claims about the events in scope.
2. Normalize times: timezone, date precision, publication vs. event time.
3. Anchor the timeline on the most verifiable events.
4. Position remaining events relative to anchors; flag ordering conflicts.
5. Resolve conflicts by source reliability, not convenience.
6. Mark gaps and assess whether they are real or observational.
7. Output the timeline with per-event confidence and source citations.

## Step-by-step workflow

1. Define the timeline scope: which events, which period, which question.
2. Harvest dated items from collection; log source, timestamp, precision.
3. Normalize to a single time standard (UTC) with original local time preserved.
4. Build the master chronology; identify anchors.
5. For each ordering conflict, apply source-verification standards to adjudicate.
6. Annotate each entry: verified date / reported date / inferred position.
7. Identify gaps; task collection to fill critical ones.
8. Publish timeline annex with confidence per entry.

## Data requirements

- Dated source material: official timestamps, gazette dates, meeting minutes, video metadata, court filings.
- Timezone documentation for all sources.
- Awareness of publication delays (news cycles, embargoes, FOI queues).
- Where images/video exist: verification of capture time per `../verification/` and `../geoint/`.

## Approved public sources

Official gazettes and government calendars; parliamentary records with timestamps; central bank release schedules; court dockets; corporate filing timestamps (EDGAR, national equivalents); official social-media posts with platform timestamps; satellite imagery with acquisition timestamps via `../geoint/`; verified news archives.

## Source verification standards

Timestamps from primary sources outrank secondary reporting. Social-media timestamps are platform-generated but context (posting vs. event) must be assessed. See `../verification/timestamp_verification.md` and `../geoint/imagery_timestamp_verification.md`.

## Analytical framework

Timeline entry standard:

| Field | Requirement |
|---|---|
| Event | Precise description of what occurred |
| Time | Normalized UTC + original stated time |
| Precision | Exact / date / period / inferred order |
| Source | Primary preferred; citation recorded |
| Confidence | Per-entry confidence grade |
| Notes | Conflicts, caveats, gap markers |

## Evidence requirements

- Every timeline entry cites its source.
- Ordering conflicts are disclosed with adjudication reasoning.
- Inferred positions are labeled as inferred, not stated.
- Gap analysis included: which windows lack coverage and why.

## Confidence assessment

- **HIGH** — all key events anchored on primary sources; ordering unambiguous.
- **MODERATE** — core sequence solid; some entries rely on secondary sources or inferred positions.
- **LOW** — significant ordering conflicts unresolved; many inferred positions.
- **INSUFFICIENT** — too few dated items to establish sequence; report what is known and the gap.

## Common analytical mistakes

- Treating publication time as event time.
- Ignoring timezone differences between sources.
- Forcing a linear sequence when events overlapped.
- Using a convenient timeline that fits the preferred narrative.
- Resolving timestamp conflicts by picking the source that agrees with the hypothesis.
- Treating absence of reporting as absence of events.

## Ethical considerations

Timelines involving individuals must be built only from public, verified sources and must not fabricate or compress time to imply guilt. Sequence reconstruction for accountability purposes is legitimate; for targeting purposes it is not.

## Security boundaries

Timeline construction uses public timestamps and records only. No access to non-public communications, location data, or surveillance records. Products must not enable doxxing via reconstructed movements.

## Expected output

Timeline annex: master chronology table with confidence per entry, conflict log, and gap analysis. Main product references timeline conclusions (precedence, simultaneity, gaps) where relevant.

## Quality checklist

- [ ] All times normalized with source basis preserved.
- [ ] Anchors identified and verified.
- [ ] Conflicts disclosed and adjudicated by source quality.
- [ ] Precision tiers preserved honestly.
- [ ] Gaps analyzed (real vs. observational).
- [ ] Every entry cited.

## Cross-reference links

- [`causal_analysis.md`](causal_analysis.md) — precedence is causal evidence.
- [`pattern_analysis.md`](pattern_analysis.md) — periodicity in sequences.
- [`hypothesis_testing.md`](hypothesis_testing.md) — time-bounded propositions.
- [`indicators_and_signposts.md`](indicators_and_signposts.md) — timing of triggers.
- [`analytical_reasoning.md`](analytical_reasoning.md) — reasoning foundation.
- [`../verification/timestamp_verification.md`](../verification/timestamp_verification.md) — time standards.
- [`../geoint/imagery_timestamp_verification.md`](../geoint/imagery_timestamp_verification.md) — imagery timing.
- [`../reporting/timeline_template.md`](../reporting/timeline_template.md) — output format.
