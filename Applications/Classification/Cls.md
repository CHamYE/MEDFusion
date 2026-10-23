# Fusion for Classification

## Task definition

Classification assigns a label to a case, a slice or a region. In MMIF it usually appears as disease classification (tumour grade, Alzheimer disease stage) or as a downstream check that fused features retain diagnostic information.

## Metrics

Accuracy alone is not sufficient. Report AUC, sensitivity and specificity at the operating point, and state the class balance. For multi-class tasks, report per-class recall and the confusion matrix.

## Representative studies

| Title | Venue, Year | DOI |
|---|---|---|
| Ensemble of Deep Convolutional Neural Networks Based Multi-Modality Images for Alzheimer's Disease Diagnosis | IET Image Processing, 2020 | [10.1049/iet-ipr.2019.0617](https://doi.org/10.1049/iet-ipr.2019.0617) |
| Automated Medical Diagnosis System Based on Multi-Modality Image Fusion and Deep Learning | Wireless Personal Communications, 2020 | [10.1007/s11277-019-06899-6](https://doi.org/10.1007/s11277-019-06899-6) |
| MURF: Mutually Reinforcing Multi-Modal Image Registration and Fusion | IEEE Transactions on Pattern Analysis and Machine Intelligence, 2023 | [10.1109/tpami.2023.3283682](https://doi.org/10.1109/tpami.2023.3283682) |
| BSAFusion: A Bidirectional Stepwise Feature Alignment Network for Unaligned Medical Image Fusion | Proceedings of the AAAI Conference on Artificial Intelligence, 2025 | [10.1609/aaai.v39i5.32499](https://doi.org/10.1609/aaai.v39i5.32499) |
| Fuse4Seg: Image-Level Fusion Based Multi-Modality Medical Image Segmentation | arXiv preprint arXiv:2409.10328,  | NR |
| One Model for All: Low-Level Task Interaction Is a Key to Task-Agnostic Image Fusion | Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, 2025 | [10.1109/cvpr52734.2025.02617](https://doi.org/10.1109/cvpr52734.2025.02617) |
| Brain Tumour Segmentation using Multimodal MRI | BMVC Workshop on Deep Learning-based Information Fusion and Its Applications (DIFA), 2025 | NR |

## What to check in an entry

- Whether the classifier was trained on fused images or on separate modalities, and whether a no-fusion control is reported.
- Whether the split is patient-level; slice-level splits inflate accuracy when adjacent slices overlap.
- Whether the label definition is clinical (pathology, follow-up) or proxy (image-derived).

## Note

Classification studies often reuse segmentation or detection backbones. Record the backbone and the pretraining data, because a strong backbone can mask a weak fusion module.
