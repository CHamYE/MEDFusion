# MEDFusion

# Medical Image Fusion: Fusion Paradigms, Clinical Applications, and Open Resources — Companion Repository

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![GitHub Stars](https://img.shields.io/github/stars/CHamYE/MEDFusion?style=social)](https://github.com/CHamYE/MEDFusion)

This is the official companion repository for the survey **"Medical Image Fusion: Fusion Paradigms, Clinical Applications, and Open Resources"** by Junxin Chen, Zhiheng Ye, Mingzhi Wang, Jiawei Zhang, Jun Mou, Xu Xu, Yongfei Wu, and Wei William Wang.

The repository mirrors the structure of the manuscript: every directory corresponds to a section, and every entry follows the same record template so that a method, dataset, or tool can be traced back to the paragraph that discusses it.

## Table of Contents

- [Repository Structure](#-repository-structure)
- [Study Corpus and Metric Extraction](#-study-corpus-and-metric-extraction)
- [Quick Start](#-quick-start)
- [Entry Format](#-entry-format)
- [How to Contribute](#-how-to-contribute)
- [Maintenance](#-maintenance)
- [Citation](#-citation)
- [Contact](#-contact)
- [License](#-license)

## Repository Structure

```
MEDFusion/
├── README.md
├── CITATION.cff
├── LICENSE
├── studies_metric_coding.csv        # Per-study extraction behind Fig. 9 (192 studies)
├── paper/                           # Survey manuscript and supplementary material
├── Technical_System/                # Section 3: preprocessing and data/feature/decision fusion
│   ├── Preprocessing/
│   ├── Data_Level_Fusion/
│   ├── Feature_Level_Fusion/
│   └── Decision_Level_Fusion/
├── Extended_Techniques/             # Section 4: interpretable, generative, robust, lightweight
│   ├── Interpretable_Fusion/
│   ├── Generative_Model_Fusion/
│   ├── Low-quality_data-adaptive_fusion/
│   └── Lightweight_generalized_fusion/
├── Applications/                    # Section 5: fused-image generation, segmentation, detection, classification
│   ├── Fused_image_generation/
│   ├── Segmentation/
│   ├── Detection/
│   └── Classification/
└── Open_Source/                     # Section 6: datasets, frameworks, evaluation, visualization, deployment
    ├── Data_Preprocessing/
    ├── Datasets/
    ├── Model_design_and_training_frameworks/
    ├── Evaluation_and_visualization/
    └── Deployment_and_inference/
```

## Study Corpus and Metric Extraction

`studies_metric_coding.csv` contains the per-study extraction used for the metric-frequency analysis in **Fig. 9** of the manuscript. It covers the **192 distinct studies** catalogued in Tables 3–5 (211 table entries, because 17 studies appear in more than one configuration).

Columns:

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

Visual assessment, runtime, registration error, and other task-specific measures are retained in the raw column but are not among the 13 families.

**Reproducing Fig. 9.** With the `uses_*` columns:

```python
import pandas as pd

df = pd.read_csv("studies_metric_coding.csv")
counts = df.filter(like="uses_").sum().sort_values(ascending=False)
print(len(df))       # 192 studies
print(counts)
```

Expected counts: MI 88, Q_AB/F 71, SSIM 66, VIF 59, EN 55, SD 51, SF 40, PSNR 39, SCD 27, DSC 25, FMI 19, Acc 15, MSE 9.

## Quick Start

1. **Browse by manuscript section.** Each directory corresponds to a section of the survey; start with the `README.md` in that directory.
2. **Find a method, dataset, or tool.** Use the directory corresponding to the fusion level or pipeline stage, or search the repository for the method name.
3. **Check the extraction table.** `studies_metric_coding.csv` links each catalogued study to its reported metrics and validation evidence.

## Entry Format

Research papers:

```markdown
## [Paper Title]
- **Publication**: Journal/Conference, Year
- **Authors**: Author List
- **Core Contributions**: ...
- **Modalities**: MRI-CT / MRI-PET / ...
- **Fusion Hierarchy**: Data-level / Feature-level / Decision-level
- **Reported Metrics**: ...
- **Links**:
  - [Paper DOI](https://doi.org/...)
  - [Official Code](https://github.com/...)
```

Tools and datasets:

```markdown
## [Tool/Dataset Name]
- **Type**: Registration Tool / Dataset / Framework
- **Applicable Modalities**: CT / MRI / PET / All
- **License**: Apache 2.0 / MIT / Commercial (Free Academic)
- **Links**:
  - [Official Repository/Documentation](https://...)
```

## How to Contribute

Contributions that keep the collection current are welcome:

1. Open an issue describing the proposed addition or correction.
2. Fork the repository and follow the entry format above.
3. Submit a pull request with a short description and the source link.

Please include a DOI or publisher link for every paper, and the official repository link for every tool.

## Maintenance

The repository is maintained by the author team, with **Zhiheng Ye** as the designated maintainer. Updates are released annually and after the major medical-imaging conferences (MICCAI, ISBI, MIDL). Community corrections are handled through issues and pull requests. Each release records the date on which the links were checked; the links in the current release were verified on **29 September 2026**.

## Citation

If you use this repository or the survey, please cite:

```bibtex
@article{chen2026mmif_survey,
  title   = {Medical Image Fusion: Fusion Paradigms, Clinical Applications, and Open Resources},
  author  = {Chen, Junxin and Ye, Zhiheng and Wang, Mingzhi and Zhang, Jiawei and Mou, Jun and Xu, Xu and Wu, Yongfei and Wang, Wei William},
  journal = {Information Fusion},
  year    = {2026},
  note    = {Manuscript}
}
```

Machine-readable metadata are provided in [`CITATION.cff`](CITATION.cff).

## Contact

- **Corresponding author**: Jun Mou (moujun@dlpu.edu.cn)
- **Repository maintainer**: Zhiheng Ye (175299084@mail.dlut.edu.cn)
- **Issues**: [GitHub Issues](https://github.com/CHamYE/MEDFusion/issues)

## License

The repository content is released under the MIT License. All links point to external resources maintained by their respective authors; we do not host or redistribute third-party code, datasets, or tools. Please refer to the original sources for their license terms.
