# MEDFusion
# Multi-modality Medical Image Fusion Survey - Official GitHub Repository

[![DOI](https://img.shields.io/badge/DOI-10.1016/j.inffus.2025.xxxxxx-blue)](https://doi.org/10.1016/j.inffus.2025.xxxxxx)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![GitHub Stars](https://img.shields.io/github/stars/your-username/MMIF-Survey?style=social)](https://github.com/CHamYe/MEDFusion)

This is the official companion GitHub repository for the survey paper **"Information Fusion for Medical Image Analysis: Methods, Open Tools, and Trends"**.

## 📋 Table of Contents
- [Repository Structure](#-repository-structure)
- [Quick Start](#-quick-start)
- [How to Contribute](#-how-to-contribute)
- [Citation](#-citation)
- [Contact](#-contact)

---

## 📁 Repository Structure

The repository is organized **exactly following the structure of the survey paper** to ensure seamless navigation between the manuscript and practical resources:

```
MMIF-Survey/
├── README.md                          # This file
├── LICENSE                            # MIT License
├── CITATION.cff                       # Standardized citation file
├── paper/                             # Survey paper and supplementary materials
│   ├── MEDFusion.pdf
│   └── Supplementary_Material.pdf
├── Technical_System/               # Section 3: Full-chain fusion methods
│   ├── README.md
│   ├── Preprocessing/
│   │   ├── registration_tools.md
│   │   ├── segmentation_tools.md
│   │   └── bias_correction_augmentation.md
│   ├── Data_Level_Fusion/
│   │   ├── traditional_methods.md
│   │   └── deep_learning_methods.md
│   ├── Feature_Level_Fusion/
│   │   ├── traditional_methods.md
│   │   └── deep_learning_methods.md
│   └── Decision_Level_Fusion/
│       ├── traditional_methods.md
│       └── deep_learning_methods.md
├── Extended_Techniques/            # Section 4: Advanced fusion techniques
│   ├── README.md
│   ├── Interpretable_Fusion/
│   ├── Generative_Model_Fusion/
│   ├── Low_Quality_Data_Fusion/
│   └── Lightweight_Architectures/
├── Applications/                   # Section 5: Clinical applications
│   ├── README.md
│   ├── Fused_Image_Generation/
│   ├── Segmentation/
│   ├── Detection/
│   └── Classification/
├── Open_Source_Toolchain/          # Section 6: Full-process open-source tools
│   ├── README.md
│   ├── Data_Preprocessing/
│   │   └── tool_list.md
│   ├── Datasets/
│   │   └── dataset_list.md
│   ├── Model_Design_Frameworks/
│   │   └── framework_list.md
│   ├── Evaluation_Visualization/
│   │   └── tool_list.md
│   └── Deployment_Inference/
│       └── tool_list.md
├── Challenges_Future_Trends/       # Section 7: Challenges and future directions
│   ├── README.md
│   ├── core_challenges.md
│   └── future_trends_tracking.md
└── assets/                             # Figures and visual resources
    ├── taxonomy_figure.png
    ├── pipeline_figure.png
    └── benchmark_visualization.png
```

---

## 🚀 Quick Start

### 1. Browse by Survey Section
Each directory corresponds to a section in the survey paper. Start with the `README.md` in each directory for an overview, then explore the specific content files.

### 2. Find a Specific Method or Tool
- **For fusion methods**: Navigate to `03_Technical_System/` or `04_Extended_Techniques/` and select the appropriate category
- **For datasets**: Go to `06_Open_Source_Toolchain/06b_Datasets/`
- **For tools**: Check `06_Open_Source_Toolchain/` for the complete toolchain

### 3. Content Format
All resources are provided as **structured pointers** (links) to original sources, including:
- Paper DOIs/arXiv links
- Official code repositories
- Tool documentation pages
- Dataset download portals

---

## 📝 Example Content Structure

Each method/tool entry follows a standardized format:

### For Research Papers
```markdown
## [Paper Title]
- **Publication**: Journal/Conference, Year
- **Authors**: Author List
- **Core Contributions**:
  - Contribution 1
  - Contribution 2
- **Modalities**: MRI-CT / MRI-PET / All modalities
- **Fusion Hierarchy**: Data-level / Feature-level / Decision-level
- **Links**:
  - [Paper DOI](https://doi.org/xxx)
  - [arXiv Preprint](https://arxiv.org/abs/xxx)
  - [Official Code](https://github.com/xxx/xxx)
```

### For Tools/Datasets
```markdown
## [Tool/Dataset Name]
- **Type**: Registration Tool / Dataset / Framework
- **Applicable Modalities**: CT / MRI / PET / All
- **License**: Apache 2.0 / MIT / Commercial (Free Academic)
- **Links**:
  - [Official Repository/Documentation](https://xxx)
  - [Quick Start Guide](https://xxx)
```

---

## 🤝 How to Contribute

We welcome contributions from the community to keep this repository up-to-date and comprehensive!

### Ways to Contribute
1. **Add new papers**: Include recently published MMIF methods
2. **Update resources**: Add new tools, datasets, or frameworks
3. **Fix broken links**: Report or fix outdated URLs
4. **Improve documentation**: Clarify explanations or add examples

### Contribution Process
1. Open an Issue describing your proposed addition
2. Fork the repository
3. Make your changes following our standardized format
4. Submit a Pull Request with a clear description

Please see our [Contribution Guidelines](.github/CONTRIBUTING.md) for detailed instructions.

---

## 📄 Citation

If you find this survey or repository useful for your research, please cite our paper:

```bibtex
@article{chen2025mmif_survey,
  title={Information Fusion for Medical Image Analysis: Methods, Open Tools, and Trends},
  author={Chen, Junxin and Ye, Zhiheng and Zhang, Jiawei and Li, Qiankun and Zhang, Yudong and Chen, Yang and Mou, Jun and García, Salvador and Camacho, David},
  journal={},
  year={2026},
  publisher={},
  doi={}
}
```

Also, please ⭐ this repository to help others discover it!

---

## 📮 Contact

- **Corresponding Author**: Jun Mou (moujun@dlpu.edu.cn)
- **Repository Maintainer**: Zhiheng Ye (175299084@mail.dlut.edu.cn)
- **Issues**: [GitHub Issues](https://github.com/CHamYe/MEDFusion/issues)

---

## ⚠️ Disclaimer

This repository is for academic research purposes only. All links point to external resources maintained by their respective authors. We do not host or distribute third-party code, datasets, or tools. Please refer to the original sources for license terms and usage restrictions.

---

**Last Updated**: March 2026
