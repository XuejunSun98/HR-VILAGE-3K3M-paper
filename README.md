# HR-VILAGE-3K3M — Scientific Data Revision

Manuscript and peer-review materials for the *Scientific Data* (Nature)
submission of **HR-VILAGE-3K3M**, a curated, harmonized transcriptomic
resource (microarray, bulk RNA-seq, scRNA-seq) covering 3,178 subjects
across 66 respiratory viral vaccination, inoculation, and mixed-exposure
studies.

- Dataset: [huggingface.co/datasets/xuejun72/HR-VILAGE-3K3M](https://huggingface.co/datasets/xuejun72/HR-VILAGE-3K3M)
- Analysis code: [github.com/XuejunSun98/HR-VILAGE-3K3M](https://github.com/XuejunSun98/HR-VILAGE-3K3M)
- Submission ID: `acf167d6-60f5-442f-9760-05d400c4dabd`

This repository holds only the paper-revision materials, not the dataset
build pipeline or analysis notebooks (those live in the separate main
project).

## Layout

- `manuscript/` — current manuscript source (originally exported from
  Overleaf, JASA template).
  - `template.tex` — the manuscript text. References are numbered
    (natbib `numbers` option + `unsrtnat` bibliography style, in
    citation order), section numbering is off, the title no longer
    includes the dataset name, and the "Potential Applications" section
    has been removed, per the editor's requirements.
  - `bibliography.bib` — references.
  - `figures/` — the three figures used in the manuscript (`RIGEL.png`,
    `Example_experiment2.png`, `sc_bulk.png`).
- `reviews/` — the editor decision letter and both reviewers' comments.
  - `Feedback from the Editor.docx` — original file as received.
  - `editor_and_reviewer_comments.md` — plain-text/markdown transcription
    of the same, for easy reading and diffing.
- `JASA_HR_VILAGE.zip` — the original Overleaf project export, kept as a
  provenance snapshot of the manuscript as submitted (before revision).
- `response/response_to_comments.tex` — the point-by-point "response to
  comments" document required for resubmission. Quotes every Editor
  action item (E1–E14, including the third-party-data Q1–Q3 sub-points),
  every Reviewer 1 major comment (R1-1–R1-8), and every Reviewer 2 major
  and minor comment (R2-1–R2-6, R2-m1–R2-m11), each followed by a blank
  `Response:` block to fill in. General Comments (no response required
  per the editor) are listed separately as a checklist. Compiles cleanly
  with `pdflatex` (verified, 18 pages).

## Required revision

The editor requires reframing the paper as a **Data Descriptor**: no
results, analyses, or general conclusions outside the Background and
Summary, Methods, Data Records, and Technical Validation sections. See
`reviews/editor_and_reviewer_comments.md` for the full list of editor
action items and Reviewer 1 / Reviewer 2 comments, and
`response/response_to_comments.tex` to fill in and submit alongside the
revised manuscript.
