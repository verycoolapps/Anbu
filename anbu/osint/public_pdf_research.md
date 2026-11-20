# Public PDF Research

> ANBU OSINT Division 002 — Collection Tradecraft

## Purpose

Covers research and analysis of public PDF documents: reports, filings, forms, scanned documents, and digital publications.

## Scope

PDF documents from government, corporate, academic, and institutional sources, including scanned and form-based PDFs.

## Intelligence objectives

- Extract text and data from PDF collections
- Handle scanned, form-based, and image-heavy PDFs
- Verify document authenticity and metadata
- Build searchable corpora from PDF sources

## Core concepts

- Native versus scanned PDF
- PDF metadata: author, creation date, software
- Form fields and embedded data
- PDF as container for documents, data, and images

## Analytical methodology

Inventory PDF sources and download lawfully. Extract text via PDF tools; use OCR for scanned documents. Check metadata for authorship and creation context. Validate document structure and signatures where applicable. Build searchable corpus with source attribution. For forms, extract field data systematically.

## Step-by-step workflow

1. Collect PDF sources from identified portals
2. Extract text and metadata
3. OCR scanned documents where needed
4. Validate authenticity markers
5. Build searchable corpus
6. Index findings with document citations

## Data requirements

PDF source list; document types; OCR requirements; metadata analysis needs.

## Approved public sources

- Government publication portals
- Corporate filings and reports
- Academic repositories
- Court document systems
- Institutional archives
- Regulatory filing systems

## Source verification standards

Every source is evaluated for authority, proximity to the event or subject, currency, and internal consistency before its content is used analytically. Primary sources are preferred over secondary accounts. Where sources conflict, the conflict is preserved and reported rather than silently resolved. Source reliability is rated on the ANBU reliability scale and recorded in the collection log.

## Analytical framework

PDFs are analyzed for content, metadata, and authenticity markers. Creation metadata is treated as evidence but not proof. Scanned documents are labeled as such; OCR errors are flagged. Document structure (form fields, embedded files) is examined for completeness.

## Evidence requirements

Every analytical claim must be traceable to a logged collection item. Evidence requirements: (1) verbatim quotation or precise paraphrase with page/section reference; (2) source attribution including URL or archive identifier; (3) collection timestamp; (4) access method; (5) confidence grade per the ANBU scale. Claims without logged evidence are marked INSUFFICIENT and excluded from analytical products.

## Confidence assessment

HIGH: multiple independent primary sources, direct documentation, no material contradictions. MODERATE: credible sources with minor gaps or single-source primary documentation. LOW: indirect, derivative, or partially corroborated reporting. INSUFFICIENT: evidence does not support a judgment; collection gap or contested sources prevent assessment.

## Common analytical mistakes

- Treating OCR output as verbatim
- Ignoring PDF metadata that reveals authorship
- Missing embedded files and attachments
- Failing to check document signatures

## Ethical considerations

Extract only from lawfully accessed PDFs. Respect document copyright; quote minimally.

## Security boundaries

No extraction from access-controlled PDFs. No malware execution from PDF content; scan before opening.

## Expected output

PDF research corpus with extracted text, metadata reports, authenticity assessments, and indexed findings.

## Quality checklist

- [ ] Text extraction verified
- [ ] Metadata analyzed
- [ ] Scanned documents OCR'd and flagged
- [ ] Authenticity markers checked

## Cross-reference links

- `public_document_analysis.md`
- `public_registry_research.md`
- `academic_research_collection.md`
- `verification/`
- `osint_methodology.md`

