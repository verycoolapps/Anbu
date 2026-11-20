# Public Satellite Imagery Context

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Defines use of public satellite imagery for contextual analysis: change detection, facility assessment, and event verification support.

## Scope

Publicly available satellite imagery from Sentinel-2, Landsat, Sentinel-1, commercial free tiers, and national programs, used as contextual evidence.

## Intelligence objectives

- Detect changes in facilities, infrastructure, and terrain over time
- Corroborate or contradict ground-level reports
- Assess construction, activity, and environmental changes
- Provide geospatial context for other OSINT findings

## Core concepts

- Optical versus radar imagery
- Spatial and temporal resolution tradeoffs
- Change detection methodology
- Imagery licensing and attribution
- Satellite revisit cycles and cloud cover

## Analytical methodology

Identify relevant imagery sources and coverage for the area of interest. Select appropriate resolution for the question. Acquire imagery for relevant dates. Perform change detection using band ratios, indices, or visual comparison. Correlate with ground reports and other sources. Document imagery dates, sources, and processing steps.

## Step-by-step workflow

1. Define area of interest and time window
2. Identify imagery sources and coverage
3. Acquire imagery for key dates
4. Process for change detection or analysis
5. Compare with ground reports
6. Document findings with imagery citations

## Data requirements

Area of interest coordinates; time window; analytical question; required resolution.

## Approved public sources

- Sentinel-2 (ESA/Copilot)
- Landsat (USGS EarthExplorer)
- Sentinel-1 SAR (Copernicus)
- MODIS (NASA)
- Commercial free tiers (Planet NICFI, Maxar Open Data)
- National satellite programs

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

Satellite imagery provides context, not proof. Changes are detected with defined thresholds and dates. Imagery is correlated with ground sources; discrepancies are flagged. Cloud cover and revisit cycles limit temporal precision.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Over-interpreting low-resolution imagery
- Ignoring cloud cover and revisit limitations
- Treating imagery as proof without corroboration
- Failing to document processing steps

## Ethical considerations

Use publicly available imagery under license terms. Respect attribution requirements. Do not use imagery for targeting or harm.

## Security boundaries

No use of classified or non-public imagery. No imagery-based targeting assistance.

## Expected output

Imagery analysis report with change detection results, dates, sources, and correlation with ground reports.

## Quality checklist

- [ ] Imagery sources documented
- [ ] Dates and processing recorded
- [ ] Resolution appropriate to question
- [ ] Corroborated with ground sources

## Cross-reference links

- `geospatial_open_data.md`
- `geoint/`
- `public_image_metadata_analysis.md`
- `public_video_analysis.md`
- `verification/`

