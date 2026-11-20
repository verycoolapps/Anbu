# Tertiary Source Handling

**Division 007 · Verification · ANBU OSINT**

## 1. Purpose

Tertiary sources are material three or more steps removed from the event: user-generated posts, memes, comment threads, forum claims, anonymous uploads, and aggregated content farms. They are indispensable for early warning and on-the-ground texture but carry the highest fabrication and manipulation risk of any tier. This file defines the minimum handling standard for tertiary material.

## 2. Scope

Covers: social media posts, anonymous image/video dumps, forum and chat claims, content-farm articles, AI-generated or AI-assisted material, unattributed "insider" claims, and crowd-sourced compilations. Anything whose author, origin, and custody cannot be established is tertiary by default.

## 3. Intelligence Objectives

- Capture early signals from the open web without being poisoned by them.
- Establish origin and custody for every tertiary item before it influences analysis.
- Distinguish genuine eyewitness material from coordinated inauthentic behavior.
- Convert promising tertiary leads into verifiable secondary or primary records.

## 4. Core Concepts

- **Epistemic humility:** tertiary sources are leads with timestamps, not evidence.
- **Velocity vs. verification:** tertiary material travels fastest and verifies slowest; treat early viral items as presumptively suspect.
- **Attribution vacuum:** anonymous or pseudonymous authorship means reliability cannot be graded — score content only.
- **Amplification asymmetry:** a single tertiary post can appear as "many sources" through reposts. See `cross_source_corroboration.md`.

## 5. Analytical Methodology

1. **Snapshot immediately:** capture URL, timestamp, content hash, author handle, and engagement metrics before deletion or edit.
2. **Provenance attempt:** trace the earliest discoverable instance; record the chain in `source_provenance_tracking.md`.
3. **Content authentication:** apply `image_authenticity_assessment.md` and `video_authenticity_assessment.md` where media is present.
4. **Origin analysis:** assess whether the post shows signs of coordinated inauthentic amplification (`disinformation_detection.md`).
5. **Lead conversion:** attempt to anchor the claim to a primary or secondary record; if impossible, retain as unverified signal only.

## 6. Step-by-Step Workflow

1. Acquire and archive the item (screenshot + raw file where possible; Wayback capture).
2. Record author account metadata: creation date, follower graph signals, posting history consistency.
3. Run reverse-image/video checks per media authenticity files.
4. Search for earlier instances of the content (distinctive phrases, frame matching).
5. Check platform integrity signals: sudden engagement spikes, identical captions, bot-like timing.
6. Assign a provisional label: UNVERIFIED LEAD / PARTIALLY CORROBORATED / DISPROVEN; log in audit trail.

## 7. Data Requirements

- Timestamped capture with hash.
- Author handle and account metadata snapshot.
- Media files in original quality where obtainable.
- Earliest-known-instance search results.
- Platform propagation metrics at capture time.

## 8. Approved Public Sources

Public social platforms (read-only), public forums, public video platforms, open web archives, public leak repositories that are lawfully accessible, and crowd documentation projects with published methodology. Nothing behind login walls is accessed without authorization; private groups are out of scope entirely.

## 9. Source Verification Standards

A tertiary item graduates only when it is anchored: either the author is identified and credible, or the content is corroborated by independent records, or the media is authenticated. Until then, every downstream use must carry the label "unverified tertiary report."

## 10. Analytical Framework

Use the **Tertiary Funnel**: capture → provenance → authentication → corroboration → anchoring. Items may exit the funnel at any stage as DISPROVEN or DEPRIORITIZED; only anchored items enter claim cards. Funnel stage is recorded per item.

## 11. Evidence Requirements

Every retained tertiary item needs: capture hash, earliest-known timestamp, author metadata snapshot, authenticity check results, corroboration attempts with outcomes, and a current label. Items failing authenticity checks are retained for the audit trail but quarantined from analysis.

## 12. Confidence Assessment

Tertiary items cap at LOW by default. MODERATE requires either authenticated media plus corroboration or an identified credible author with track record. HIGH is effectively unreachable for anonymous tertiary content; reaching it means the item is no longer tertiary — reclassify it.

## 13. Common Analytical Mistakes

- Treating engagement metrics as credibility signals.
- Assuming a viral video is authentic because "too big to fake."
- Counting reposts as independent sources.
- Retaining disproven items in analysis "for balance" — disproven material belongs in the audit trail, not the assessment.
- Ignoring that sophisticated actors deliberately seed plausible tertiary content.

## 14. Ethical Considerations

Do not amplify unverified claims, do not name private individuals based on tertiary material, and do not harass or investigate private citizens beyond public posts relevant to a legitimate intelligence question. Respect platform terms; document any automated collection.

## 15. Security Boundaries

No interaction with authors, no sock-puppet engagement, no doxxing of pseudonymous accounts, no access to private groups or leaked credentials. Geolocation of posters' physical locations is prohibited unless directly required for a documented threat assessment and reviewed under `legal/`.

## 16. Expected Output

A tertiary-item register with per-item funnel stage and label; promoted items enter the standard claim-card pipeline; quarantined items remain in the audit trail with reasons.

## 17. Quality Checklist

- [ ] Item captured with hash and timestamp before it can be deleted
- [ ] Earliest-known instance identified or absence noted
- [ ] Media authenticity checks run where applicable
- [ ] Amplification analysis completed
- [ ] Label assigned; quarantine applied where needed
- [ ] Promotion path documented for anchored items

## 18. Cross-Reference Links

- Authentication: `image_authenticity_assessment.md`, `video_authenticity_assessment.md`, `manipulated_media_assessment.md`
- Threat context: `misinformation_detection.md`, `disinformation_detection.md`, `propaganda_analysis.md`
- Records: `source_provenance_tracking.md`, `evidence_chain_management.md`, `verification_audit_trail.md`
- Divisions: `osint/` (collection), `security/` (threat context), `legal/` (privacy), `reporting/` (labeling)
