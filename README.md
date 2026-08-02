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
  - `template.tex` — the manuscript text.
  - `bibliography.bib` — references (author-year/natbib style; must move
    to numbered format per the editor's requirements).
  - `agsm.bst` — current author-year bibliography style.
  - `figures/` — the four figures currently used in the manuscript
    (`RIGEL.png`, `Example_experiment2.png`, `sc_bulk.png`,
    `Popular_Task.png`; the last is used only in the "Potential
    Applications" section slated for removal).
- `reviews/` — the editor decision letter and both reviewers' comments.
  - `Feedback from the Editor.docx` — original file as received.
  - `editor_and_reviewer_comments.md` — plain-text/markdown transcription
    of the same, for easy reading and diffing.
- `JASA_HR_VILAGE.zip` — the original Overleaf project export, kept as a
  provenance snapshot of the manuscript as submitted (before revision).

## Required revision

The editor requires reframing the paper as a **Data Descriptor**: no
results, analyses, or general conclusions outside the Background and
Summary, Methods, Data Records, and Technical Validation sections. See
`reviews/editor_and_reviewer_comments.md` for the full list of editor
action items and Reviewer 1 / Reviewer 2 comments, each of which needs a
response in the eventual "response to comments" file required for
resubmission.
