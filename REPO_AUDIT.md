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
