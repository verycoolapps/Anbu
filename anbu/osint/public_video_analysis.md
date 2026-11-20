# Public Video Analysis

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Defines methods for analyzing public video: verification, geolocation, timeline reconstruction, and content analysis.

## Scope

Videos from news outlets, social media, official channels, and open repositories, for event verification and reconstruction.

## Intelligence objectives

- Verify video authenticity and provenance
- Geolocate and timestamp video content
- Reconstruct events from video sequences
- Detect manipulation and misattribution

## Core concepts

- Video provenance and chain of custody
- Keyframe analysis and visual geolocation
- Audio and speech analysis
- Frame-by-frame timeline reconstruction
- Deepfake and manipulation detection

## Analytical methodology

Extract keyframes and metadata. Reverse search keyframes for earliest publication. Analyze visual content for geolocation clues (architecture, signage, terrain). Check audio for speech and ambient sound consistency. Build frame-level timeline. Cross-reference with satellite imagery, maps, and other reports. Grade authenticity.

## Step-by-step workflow

1. Collect video and source attribution
2. Extract metadata and keyframes
3. Reverse image search keyframes
4. Analyze visual and audio content
5. Build timeline and geolocation
6. Cross-reference with other sources
7. Grade authenticity and confidence

## Data requirements

Video files or URLs; source context; associated claims; date and location hypotheses.

## Approved public sources

- News outlet video pages
- Official broadcaster and government channels
- Social media public videos
- YouTube and video platforms
- Open video repositories
- Wire service video archives

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

Videos are graded on provenance, geolocation confidence, temporal consistency, and manipulation assessment. A video without verified provenance is LOW confidence. Multiple videos of the same event are compared for consistency.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Trusting video content without provenance
- Ignoring audio-visual inconsistencies
- Failing to check for deepfakes
- Missing that videos can be recut and recontextualized

## Ethical considerations

Analyze publicly available videos. Do not distribute manipulated versions. Do not use video analysis to identify private individuals.

## Security boundaries

No creation or distribution of deepfakes. No use of facial recognition against private databases.

## Expected output

Video analysis report with provenance assessment, geolocation results, timeline reconstruction, and confidence grade.

## Quality checklist

- [ ] Provenance verified
- [ ] Keyframes reverse-searched
- [ ] Geolocation corroborated
- [ ] Manipulation assessed

## Cross-reference links

- `public_image_metadata_analysis.md`
- `public_satellite_imagery_context.md`
- `public_event_reconstruction.md`
- `verification/`
- `geoint/`

