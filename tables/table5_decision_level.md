# Table 5 — Decision-Level Fusion Studies

Reproduced from the manuscript. The paper title links to the DOI; rows without a DOI are left unlinked. Each row is one table entry, so a study spanning several configurations appears more than once.

| Paper | Year | Modalities | Method | Datasets | Metrics | Validation evidence |
|---|---|---|---|---|---|---|
| [DST-cls](https://doi.org/10.1016/0167-8655(96)00039-6) | 1996 | Double echo MRI | DS theory, mass function, composite hypothesis | Private | K, decision consistency, visual evaluation | Unclear |
| [CNN Type-III (decision)](https://doi.org/10.1109/isbi.2018.8363717) | 2018 | PET-CT-MRI T1/T2 | CNN, Majority voting | TCIA | Pixel-wise Accuracy, visual evaluation | Benchmark |
| Patch CNN | 2019 | PET-CT-MRI T1 | Voting, CNN | STS | DSC, Pixel-wise Accuracy | Unclear |
| [DCMA](https://doi.org/10.1049/iet-ipr.2019.0617) | 2020 | MRI-PET | DCNN ensemble, Adaboost, dropout | ADNI | Acc, Sen, Spe, AUC | Benchmark |
| [Evidence fusion](https://doi.org/10.1007/978-3-031-16443-9_39) | 2022 | MRI T1-T1Gd-T2-FLAIR | DST, contextual discounting, MMEF module | BraTS 2021 | DSC, HD, ECE, visual evaluation | Benchmark |
| ETSCL | 2024 | CFP-OCT-Vascular | Supervised contrastive loss, DST-based fusion | GAMMA | Cohen's kappa, Accuracy | Benchmark |
| [MHFN decision baseline](https://doi.org/10.1007/s11768-024-00231-9) | 2024 | MRI T1W–T2W-STIR | Combines modality-specific segmentation outputs; baseline in the MHFN study | Private | DSC, IoU, HD | Unclear (single-center cohort) |
| [Deep evidential fusion](https://doi.org/10.1016/j.inffus.2024.102648) | 2025 | PET-CT, MRI multi-sequence | DST, evidence mapping, contextual discounting | PET-CT lymphoma dataset, BraTS 2021 | DSC, Brier score, NLL, ECE | Benchmark; Retrospective |
| [MAMS](https://doi.org/10.1007/s40747-025-02013-5) | 2025 | FFDM-DBT | cGAN, MAMS fusion | NFH, GDHCM | RMSE, PSNR, UQI, MS-SSIM, Acc, AUC, F1-Score | Retrospective (two centers) |
| [Uncertainty-seg](https://doi.org/10.1109/nnice64954.2025.11064419) | 2025 | MRI FLAIR-T2 | MC-Dropout, uncertainty weighting | BraTS subset | DSC, IoU, SE, PPV, uncertainty | Unclear |

The same records are available as CSV in `table5_decision_level.csv`.
