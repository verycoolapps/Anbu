# Public Image Metadata Analysis

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Defines methods for analyzing public images: metadata (EXIF), geolocation, provenance, and contextual verification.

## Scope

Images from news media, social media, official sources, and open repositories, for verification and contextual analysis.

## Intelligence objectives

- Extract EXIF and technical metadata from public images
- Assess image provenance and authenticity
- Geolocate images where metadata supports it
- Detect manipulated or misattributed images

## Core concepts

- EXIF metadata: camera, timestamp, GPS, software
- Image provenance and chain of custody
- Reverse image search
- Error level analysis and manipulation detection
- Context versus content verification

## Analytical methodology

Extract metadata using EXIF tools; note that platforms strip metadata on upload. Use reverse image search to find earlier instances. Analyze visual content for context clues (geography, time, event). Apply manipulation detection where warranted. Cross-reference with text reports and satellite imagery. Grade authenticity based on provenance strength.

## Step-by-step workflow

1. Collect image and source attribution
2. Extract EXIF and technical metadata
3. Reverse image search for earliest instance
4. Analyze visual content for context
5. Check for manipulation artifacts
6. Cross-reference with reports and geospatial data

## Data requirements

Image files or URLs; source context; associated text claims; date and location hypotheses.

## Approved public sources

- News agency photo libraries
- Official government and institutional photo pages
- Social media public images
- Open image repositories
- Wire service photo archives

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

Images are graded on provenance (original source known), metadata completeness, corroboration with other sources, and manipulation assessment. An image without provenance is LOW confidence regardless of content plausibility.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Trusting image content without provenance
- Ignoring that platforms strip EXIF
- Failing to check for manipulation
- Treating geolocation as certain without corroboration

## Ethical considerations

Analyze images lawfully published. Do not create or distribute manipulated imagery. Do not use images to identify private individuals.

## Security boundaries

No extraction of personal data from image metadata beyond what's publicly visible. No facial recognition against private databases.

## Expected output

Image analysis report with metadata extract, provenance assessment, geolocation results, and confidence grade.

## Quality checklist

- [ ] Metadata extracted
- [ ] Provenance assessed
- [ ] Reverse search conducted
- [ ] Manipulation checked

## Cross-reference links

- `public_video_analysis.md`
- `public_satellite_imagery_context.md`
- `verification/`
- `geoint/`
- `osint_collection_ethics.md`

