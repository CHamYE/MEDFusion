# Repository Audit (R1)

Scope: every file on `main`, checked against the manuscript (`paper/MEDFusion.pdf`, 47 pp.) and the released per-study table (`studies_metric_coding.csv`).

## 1. Problems found

| # | Problem | Where | Action |
|---|---|---|---|
| 1 | 13 Markdown files were empty (0 bytes) | `Technical_System/README.md`, `Extended_Techniques/README.md`, `Extended_Techniques/Generative_Model_Fusion/README.md`, all four `Applications/` task pages and its `readme.md`, `Open_Source/README.md`, three tool lists, `paper/paper.md` | Written from the manuscript sections and Table 8/9 |
| 2 | Dataset list described 3 datasets; the manuscript reports 10 | `Open_Source/Datasets/dataset_list.md` | Rebuilt as a 10-row table (AANLIB, BraTS, TCIA, ADNI, Imagefusion.org, OASIS, IXI, CHAOS, SynthRAD 2023, HECKTOR 2021) with pairing status |
| 3 | Evaluation page used “full-reference”, the manuscript uses “source-referenced” | `Open_Source/Evaluation_and_visualization/evalvisual_list.md` | Terminology aligned, with the reason stated |
| 4 | Robust-fusion page was titled “Missing Modality Handling”, narrower than Section 4.3 | `Extended_Techniques/Low-quality_data-adaptive_fusion/readme.md` | Retitled to cover degraded inputs and missing modalities |
| 5 | No figures in the repository, although the README refers to Fig. 1–10 | root | `assets/fig1–fig10.png` added and referenced |
| 6 | Relative image paths would break at repository root level | `Technical_System/`, `Applications/`, `Open_Source/` | Paths corrected to `../assets/` or `../../assets/` by depth |
| 7 | Tool lists covered only part of the workflow | `Open_Source/*` | Preprocessing, training, deployment lists completed from Table 8 |

## 2. Content added

- `Technical_System/README.md`: pipeline overview, comparison of the three levels, folder map, reading rules for validation evidence.
- `Extended_Techniques/README.md`: four translation constraints and how they trade off.
- `Applications/`: task definitions, metrics, representative DOIs, and the controls a study must report.
- `Open_Source/`: toolchain map, dataset table, reproducibility protocol.
- `paper/paper.md`: title, authors, file list, section-to-folder map.

All DOIs are taken from `refs_R1.bib`; no reference was introduced beyond the manuscript.

## 3. Figure placement

| Figure | File | Used in |
|---|---|---|
| 1 | `assets/fig1.png` | root `README.md`, Figures table |
| 2 | `assets/fig2.png` | `Technical_System/README.md` |
| 3 | `assets/fig3.png` | `Technical_System/README.md` |
| 4 | `assets/fig4.png` | `Extended_Techniques/Interpretable_Fusion/README.md` |
| 5 | `assets/fig5.png` | `Extended_Techniques/Generative_Model_Fusion/README.md` |
| 6 | `assets/fig6.png` | `Extended_Techniques/Low-quality_data-adaptive_fusion/readme.md` |
| 7 | `assets/fig7.png` | `Extended_Techniques/Lightweight_generalized_fusion/readme.md` |
| 8 | `assets/fig8.png` | `Applications/readme.md` |
| 9 | `assets/fig9.png` | `Open_Source/README.md`, `Applications/Fused_image_generation/Fused_image_gen.md` |
| 10 | `assets/fig10.png` | root `README.md`, Figures table |

## 4. Known limits

- The per-method tables in `Technical_System/*` predate this audit and were not re-verified row by row against the publisher pages.
- `Applications/Classification/Cls.md` keeps its historic name; renaming it requires updating links in `Applications/readme.md`.

## 5. Tables added (2026-10-23, second pass)

All ten manuscript tables are now in [`tables/`](tables/README.md). Tables 3–5 are complete: 48 + 153 + 10 = **211 entries from 192 studies**, matching the manuscript; each is also released as CSV.

| Table | Rows | Check |
|---|---|---|
| 1 Comparison with prior surveys | 13 | 12 surveys + this review |
| 2 Configurations across three axes | 6 | all configurations in the paper |
| 3 Data-level studies | 48 | full table |
| 4 Feature-level studies | 153 | full table |
| 5 Decision-level studies | 10 | full table |
| 6 Cross-generation comparison | 8 | all methods compared |
| 7 Reported quantitative results | 16 | 16 methods on GLIS-RT |
| 8 Software components | 17 | all tools in Table 8 |
| 9 Public datasets | 10 | all datasets in Table 9 |
| 10 Evaluation system | 7 dimensions | structure + measures; formulas remain in the PDF |

Verification performed: column-count check on every row, no LaTeX residue (`\cite`, `\textbf`, `\begin`, `\multicolumn`), all relative links resolve, CSV rows/columns consistent, and totals match the manuscript.

## 6. Link pass (2026-10-23)

Every resource name now carries its own hyperlink:

- Paper titles in Tables 1, 3–6 link to the DOI (rows without a DOI stay unlinked: 9/48 in Table 3, 21/153 in Table 4, 2/10 in Table 5, 6/13 in Table 1, 2/8 in Table 6).
- Tool names in Table 8 and in the three `Open_Source/*` tool lists link to their official sites (17/17 in Table 8, 5 per tool list).
- Dataset names in Table 9 and `Open_Source/Datasets/dataset_list.md` link to the source portal (10/10).
- Method titles in `Technical_System/*`, `Extended_Techniques/*` and `Applications/*` link to the paper or code URL already recorded in the row (114 links in Data_Level, 31 in Feature_Level, 11 in Decision_Level, 7 in Preprocessing, plus 42 across the four direction/application pages).

Checks: column counts unchanged (0 bad rows), bracket balance 0, no LaTeX residue, all relative links resolve.
