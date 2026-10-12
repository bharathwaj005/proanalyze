# ProAnalyze — Browser-only protein sequence analysis

ProAnalyze is a static website. Users do not need to install Python or download the source code. The calculations run in the browser.

## Features
- Paste raw amino-acid sequence or FASTA records.
- Upload multiple FASTA/plain-text sequence files.
- Validate against the 20 standard amino acids.
- Calculate sequence length, molecular weight, approximate theoretical pI, GRAVY, aromaticity, aliphatic index, extinction estimates, and amino-acid composition.
- Export an Excel workbook (`.xlsx`) with `Analysis Summary`, `AA Composition`, and `Methods & Notes` sheets.

## Publish with GitHub Pages
Upload `index.html` and `README.md` to the root of the repository's `main` branch. In **Settings → Pages**, choose **Deploy from a branch**, branch `main`, folder `/(root)`.

## Important scientific limitations
- The theoretical pI is an approximate pKa-based estimate; validate important results against a reference implementation such as Biopython ProtParam or ExPASy.
- The cystine extinction estimate assumes all cysteine residues form pairs; the sequence alone does not establish disulfide bonding.
- Results are sequence-derived estimates, not experimental measurements.
- This version does not perform structure prediction or molecular dynamics.
- The SheetJS library is loaded from a CDN, so Excel export requires internet access. Core calculations can run locally in the browser.

## Privacy
Sequence text and files are processed in the user's browser and are not sent to a ProAnalyze backend. The Excel library is fetched from a third-party CDN.
