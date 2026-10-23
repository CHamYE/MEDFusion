<div align="center">

<img src="assets/banner.svg" alt="Medical Image Fusion — companion repository" width="100%">

# MEDFusion

**Companion repository to the survey “Medical Image Fusion: Fusion Paradigms, Clinical Applications, and Open Resources”**

[![License: MIT](https://img.shields.io/badge/License-MIT-2a9d8f.svg)](LICENSE)
[![Stars](https://img.shields.io/github/stars/CHamYE/MEDFusion?style=social)](https://github.com/CHamYE/MEDFusion)
[![Studies](https://img.shields.io/badge/studies-192-1d4e89)](studies_metric_coding.csv)
[![Tables](https://img.shields.io/badge/manuscript%20tables-10-1d4e89)](tables/README.md)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-2a9d8f)](.github/CONTRIBUTING.md)

Junxin Chen · Zhiheng Ye · Mingzhi Wang · Jiawei Zhang · Jun Mou · Xu Xu · Yongfei Wu · Wei William Wang

[**Manuscript (PDF)**](paper/MEDFusion.pdf) · [**Study table (CSV)**](studies_metric_coding.csv) · [**All tables**](tables/README.md) · [**Figures**](#figures) · [**Citation**](#citation)

</div>

---

## Why this repository

Reading a survey tells you what the field looks like; it does not tell you where the code, the datasets, or the numbers are. This repository closes that gap. Every folder follows one section of the manuscript, every entry follows the same record template, and every paper, dataset and tool name links to its source.

The repository is meant to be **checked**, not just browsed: the per-study extraction behind Fig. 9 is released, the ten manuscript tables are reproduced in Markdown, and the figures can be read without opening the PDF.

## At a glance

| | |
|---|---|
| **192** studies · **211** table entries | Corpus of the survey, catalogued in Tables 3–5 |
| **3** fusion levels | Data, feature, decision |
| **4** clinical translation directions | Interpretable, generative, robust, lightweight |
| **4** downstream tasks | Generation, segmentation, detection, classification |
| **13** metric families | Frequency analysis in Fig. 9 |
| **10** datasets · **17** tools | Tables 9 and 8 |
| **10** manuscript tables | Reproduced in [`tables/`](tables/README.md) |

## News

- **2026-10** — Repository restructured to follow the R1 manuscript; all ten tables added; every resource name linked to its source.
- **2026-10** — `studies_metric_coding.csv` released (192 studies, 23 columns); Fig. 9 reproducible from the `uses_*` columns.
- **2026-09** — Link audit completed; verification date recorded in the captions and in Section 6 of the manuscript.

## Contents

- [Repository structure](#repository-structure)
- [Figures](#figures)
- [Tables](#tables)
- [Study corpus and metric extraction](#study-corpus-and-metric-extraction)
- [Quick start](#quick-start)
- [Entry format](#entry-format)
- [How to contribute](#how-to-contribute)
- [Maintenance](#maintenance)
- [Citation](#citation)
- [Contact](#contact)
- [License](#license)

## Repository structure

```
MEDFusion/
├── README.md
├── CITATION.cff                     # Machine-readable citation metadata
├── LICENSE                          # MIT
├── CONTRIBUTING.md                  # Entry template and review rules (.github/)
├── studies_metric_coding.csv        # Per-study extraction behind Fig. 9 (192 studies)
├── studies_metric_coding.xlsx
├── assets/                          # Banner and figures reproduced from the manuscript
├── tables/                          # All ten manuscript tables (3–5 also as CSV)
├── paper/                           # Manuscript PDF
├── Technical_System/                # Section 3: preprocessing and the three fusion levels
│   ├── Preprocessing/
│   ├── Data_Level_Fusion/
│   ├── Feature_Level_Fusion/
│   └── Decision_Level_Fusion/
├── Extended_Techniques/             # Section 4: interpretable, generative, robust, lightweight
│   ├── Interpretable_Fusion/
│   ├── Generative_Model_Fusion/
│   ├── Low-quality_data-adaptive_fusion/
│   └── Lightweight_generalized_fusion/
├── Applications/                    # Section 5: generation, segmentation, detection, classification
│   ├── Fused_image_generation/
│   ├── Segmentation/
│   ├── Detection/
│   └── Classification/
└── Open_Source/                     # Section 6: datasets, frameworks, evaluation, deployment
    ├── Data_Preprocessing/
    ├── Datasets/
    ├── Model_design_and_training_frameworks/
    ├── Evaluation_and_visualization/
    └── Deployment_and_inference/
```

## Figures

Reproduced from the manuscript so that the repository can be read without the PDF.

| Figure | Content | Where it is used |
|---|---|---|
| [Fig. 1](assets/fig1.png) | Annual PubMed records, 1988–2026 | Corpus description |
| [Fig. 2](assets/fig2.png) | Three fusion hierarchies | [Technical_System](Technical_System/README.md) |
| [Fig. 3](assets/fig3.png) | Overall MMIF pipeline | [Technical_System](Technical_System/README.md) |
| [Fig. 4](assets/fig4.png) | Interpretable fusion | [Interpretable_Fusion](Extended_Techniques/Interpretable_Fusion/README.md) |
| [Fig. 5](assets/fig5.png) | Generative paradigms | [Generative_Model_Fusion](Extended_Techniques/Generative_Model_Fusion/README.md) |
| [Fig. 6](assets/fig6.png) | Robust fusion | [Low-quality data](Extended_Techniques/Low-quality_data-adaptive_fusion/readme.md) |
| [Fig. 7](assets/fig7.png) | Lightweight fusion | [Lightweight fusion](Extended_Techniques/Lightweight_generalized_fusion/readme.md) |
| [Fig. 8](assets/fig8.png) | Downstream applications | [Applications](Applications/readme.md) |
| [Fig. 9](assets/fig9.png) | Metric frequency over 192 studies | [Open_Source](Open_Source/README.md) |
| [Fig. 10](assets/fig10.png) | Challenges and future trends | Section 7 of the manuscript |

<p align="center">
  <img src="assets/fig3.png" alt="Overall MMIF pipeline" width="92%">
</p>

## Tables

All ten manuscript tables are reproduced in [`tables/`](tables/README.md). Tables 3–5 — the complete study corpus — are also released as CSV with the same columns.

| Table | Content | Rows |
|---|---|---|
| [1](tables/table1_comparison.md) | Comparison with prior surveys | 13 |
| [2](tables/table2_mapping.md) | Configurations across the three axes | 6 |
| [3](tables/table3_data_level.md) | Data-level studies | 48 |
| [4](tables/table4_feature_level.md) | Feature-level studies | 153 |
| [5](tables/table5_decision_level.md) | Decision-level studies | 10 |
| [6](tables/table6_cross_generation.md) | Cross-generation comparison | 8 |
| [7](tables/table7_reported_quantitative.md) | Reported quantitative results (GLIS-RT) | 16 |
| [8](tables/table8_tools.md) | Software components | 17 |
| [9](tables/table9_datasets.md) | Public datasets | 10 |
| [10](tables/table10_evaluation.md) | Evaluation system | 7 dimensions |

## Study corpus and metric extraction

`studies_metric_coding.csv` contains the per-study extraction used for the metric-frequency analysis in **Fig. 9**. It covers the **192 distinct studies** catalogued in Tables 3–5 (211 table entries, because 17 studies appear in more than one configuration).

| Column | Meaning |
|---|---|
| `study_id` | Sequential identifier in the released table |
| `citation_key` | BibTeX key used in the manuscript |
| `first_author`, `year`, `title`, `venue`, `doi` | Bibliographic record |
| `fusion_level` | Data-level / Feature-level / Decision-level (a study may span more than one) |
| `reported_metrics_raw` | Metrics as recorded from the study, before family merging |
| `validation_evidence` | Benchmark / Retrospective / External / Reader study / Prospective / Unclear |
| `uses_*` | Binary indicator (1/0) for each of the 13 metric families in Fig. 9 |

**Counting rule.** A study contributes at most one count per metric family, regardless of the number of datasets, configurations, or variants it reports. Variants are merged at the family level:

| Family | Merged variants |
|---|---|
| MI | MI, NMI, LMI |
| SSIM | SSIM, MSSIM, MS-SSIM, LSSIM |
| Q_AB/F | Q^AB/F, Q_AB^F |
| SD | SD, STD |
| EN | EN, entropy |
| DSC | DSC, Dice |
| Acc | Acc, accuracy, pixel-wise accuracy |

Visual assessment, runtime, registration error and other task-specific measures are retained in the raw column but are not among the 13 families.

**Reproducing Fig. 9.**

```python
import pandas as pd

df = pd.read_csv("studies_metric_coding.csv")
counts = df.filter(like="uses_").sum().sort_values(ascending=False)
print(len(df))       # 192 studies
print(counts)
```

Expected counts: MI 88, Q_AB/F 71, SSIM 66, VIF 59, EN 55, SD 51, SF 40, PSNR 39, SCD 27, DSC 25, FMI 19, Acc 15, MSE 9.

## Quick start

1. **Browse by manuscript section.** Each directory corresponds to a section of the survey; start with its `README.md`.
2. **Find a method, dataset or tool.** Use the folder for the fusion level or pipeline stage, or search the repository for the name.
3. **Check the evidence.** `studies_metric_coding.csv` links each study to its reported metrics and validation label; `tables/` gives the manuscript table it came from.

## Entry format

Research papers:

```markdown
## [Paper Title](https://doi.org/...)
- **Publication**: Journal/Conference, Year
- **Authors**: Author list
- **Core contributions**: ...
- **Modalities**: MRI-CT / MRI-PET / ...
- **Fusion hierarchy**: Data-level / Feature-level / Decision-level
- **Reported metrics**: ...
- **Links**: paper DOI · official code
```

Tools and datasets:

```markdown
## [Tool or Dataset](https://...)
- **Type**: Registration tool / Dataset / Framework
- **Applicable modalities**: CT / MRI / PET / All
- **License**: Apache 2.0 / MIT / Commercial (free for academic use)
- **Links**: documentation · quick start
```

## How to contribute

1. Open an issue describing the addition or correction.
2. Fork the repository and follow the entry format above.
3. Submit a pull request with a short description and the source link.

Include a DOI or publisher link for every paper, and the official repository link for every tool. New entries should state the dataset, the metric family and the validation evidence, not only the reported score. See [CONTRIBUTING.md](.github/CONTRIBUTING.md).

## Maintenance

Maintained by the author team, with **Zhiheng Ye** as the designated maintainer. Updates are released annually and after the major medical-imaging conferences (MICCAI, ISBI, MIDL). Community corrections are handled through issues and pull requests. Each release records the date on which the links were checked; the current release was verified on **29 September 2026**.

## Citation

```bibtex
@article{chen2026mmif_survey,
  title   = {Medical Image Fusion: Fusion Paradigms, Clinical Applications, and Open Resources},
  author  = {Chen, Junxin and Ye, Zhiheng and Wang, Mingzhi and Zhang, Jiawei and Mou, Jun and Xu, Xu and Wu, Yongfei and Wang, Wei William},
  journal = {Information Fusion},
  year    = {2026},
  note    = {Manuscript}
}
```

Machine-readable metadata: [`CITATION.cff`](CITATION.cff).

## Contact

- **Corresponding author**: Jun Mou (moujun@dlpu.edu.cn)
- **Repository maintainer**: Zhiheng Ye (175299084@mail.dlut.edu.cn)
- **Issues**: [GitHub Issues](https://github.com/CHamYE/MEDFusion/issues)

## License

Content released under the MIT License. All links point to external resources maintained by their respective authors; this repository does not host or redistribute third-party code, datasets or tools. Please refer to the original sources for their license terms.

<div align="center">

[![Star History Chart](https://api.star-history.com/svg?repos=CHamYE/MEDFusion&type=Date)](https://star-history.com/#CHamYE/MEDFusion&Date)

<sub>If this repository helps your work, please consider citing the survey.</sub>

</div>
