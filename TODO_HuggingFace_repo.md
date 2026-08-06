# TODO for Ruilie — Hugging Face repo changes (for editor comment E9)

Editor comment E9 requires that HR-VILAGE-3K3M not mirror original third-party
input files on Hugging Face — only the newly created/derived data product.

Decision (2026-08-06): delete the raw data from the HF repo and instead point
users to the original source for raw files.

Action items on `xuejun72/HR-VILAGE-3K3M`:

1. **Delete** the `bulk_gene_expr_raw/` folder (raw/unprocessed expression
   files) from the repo.
2. **Add a raw-data link** per study so users can still retrieve the original
   raw files from the source repository (GEO/ArrayExpress/ImmPort) — e.g.
   populate/repurpose the `raw_data` column in `study_meta.csv` to link out
   to the source accession page, rather than flagging local file presence.
3. Once done, double check `study_meta.csv`'s `raw_data` column semantics
   match what's now described in the manuscript (`template.tex`, Data
   Records section): raw data is *not* stored in this repository; where
   available, it can be obtained from the original source cited in
   Supplementary Table 1.

The manuscript text (Data Records section) and the E9 response letter have
already been updated to reflect this decision, assuming the above repo
changes are made to match.

## For editor comment E14 (repository requirements)

DOI is done: `10.57967/hf/9892` (already added to the manuscript and
`bibliography.bib`). Still needed on the HF repo itself:

4. **License**: set the dataset card's license to CC-BY. This is a YAML
   metadata field at the top of the repo's `README.md`:
   ```yaml
   ---
   license: cc-by-4.0
   ---
   ```
   Can be edited directly in the README or via the "Edit dataset card"
   metadata UI on the repo page.
5. **Repository metadata**: make sure the dataset card lists the full
   author list and title (matching the manuscript's author list).
6. **Dataset card citation**: add a "Citation" section to the README
   referencing the DOI-based citation (`10.57967/hf/9892`) so readers can
   find how to cite the dataset directly from the repo page.

