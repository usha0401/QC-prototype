PDF Document QC Prototype

Goal: Build a prototype that scans PDFs and flags basic document quality issues. Use any publicly available sample PDFs (e.g., forms, letters, contracts) or small synthetic PDFs you create.

QC checks (pick ≥5, implement well):

Legibility: blurred/low-resolution or faint text.

Page integrity: cut-off margins, blank pages, unexpected page count.

Orientation: upside-down or rotated pages.

Signatures/attestations: pages with signature blocks/labels but no apparent signature.

Draft vs final labeling: content contains “Draft” while filename/metadata suggests final.

Dates & validity (basic): missing dates near signatures; obviously expired dates if applicable.

Language detection (basic): flag non-English if your pipeline expects English.

Deliverables:

A CLI or notebook that ingests a folder of PDFs and outputs CSV/Excel:
document_id, check_name, severity, evidence (page#, snippet), confidence

Short README: approach, libraries/models (OCR, layout, image quality), how to run.

Nice-to-have (optional):

Simple HTML report per document.

Config to enable/disable checks.

Evaluation: Accuracy of flags, clear evidence, code quality, reproducibility, and handling of real-world scans (noise, skew, mixed content).
