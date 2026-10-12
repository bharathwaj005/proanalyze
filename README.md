ProAnalyze Web App
A static, browser-based protein sequence analyzer. Users can paste a raw sequence or FASTA content, or upload one or more .fasta, .fa, .faa, .fas, .fna, .pep, or .txt files. The browser performs calculations locally; sequence data is not sent to a server.
Run locally
Open index.html in a modern browser.
Publish with GitHub Pages
1.	Create a GitHub repository named proanalyze (or another available name).
2.	Upload index.html to the repository root.
3.	Open Settings → Pages.
4.	Select Deploy from a branch, choose main and /(root), then save.
5.	Wait for GitHub Pages to publish the URL.
Scientific limitations
This is an early prototype. Molecular weight, composition, GRAVY, aromaticity, aliphatic index and extinction coefficients are calculated in-browser. Theoretical pI uses an explicit approximate pKa model and may differ from Biopython or ExPASy. Results should be cross-checked before research-critical use. Structure prediction and molecular dynamics are not included.
