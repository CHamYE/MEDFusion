# Fusion for Segmentation

## Task definition

Segmentation assigns a label to every voxel. It is the most common downstream task in MMIF because tumour, organ and lesion boundaries are clinically meaningful and can be annotated.

## Metrics

Dice similarity coefficient (DSC) and the 95th percentile Hausdorff distance (HD95) are the standard pair. Report both: DSC is insensitive to boundary error, HD95 is sensitive to outliers. For small structures, add per-class DSC.

## Representative studies

| Title | Venue, Year | DOI |
|---|---|---|
| MedFusion-TransNet: Multi-Modal Fusion via Transformer for Enhanced Medical Image Segmentation | Frontiers in Medicine, 2025 | NR |
| Deep Fusion of Multi-Modal Features for Brain Tumor Image Segmentation | Heliyon, 2023 | [10.1016/j.heliyon.2023.e19266](https://doi.org/10.1016/j.heliyon.2023.e19266) |
| Multi-Modality Hierarchical Fusion Network for Lumbar Spine Segmentation with Magnetic Resonance Images | Control Theory and Technology, 2024 | [10.1007/s11768-024-00231-9](https://doi.org/10.1007/s11768-024-00231-9) |
| Fuse4Seg: Image-Level Fusion Based Multi-Modality Medical Image Segmentation | arXiv preprint arXiv:2409.10328,  | NR |
| Deep Evidential Fusion with Uncertainty Quantification and Reliability Learning for Multimodal Medical Image Segmentation | Information Fusion, 2025 | [10.1016/j.inffus.2024.102648](https://doi.org/10.1016/j.inffus.2024.102648) |
| M3AE: Multimodal Representation Learning for Brain Tumor Segmentation with Missing Modalities | , 2023 | NR |

## What to check in an entry

- Whether segmentation used the fused image or a multi-channel input; the latter is a strong baseline that fusion must beat.
- Whether the train/test split is patient-level and whether an external cohort was used.
- Whether the reported Dice is per-class or averaged, and whether HD95 is in millimetres.

## Note

A frequent inconsistency is to compare a fusion-plus-segmentation pipeline against a segmentation model trained on a single modality. That comparison confounds fusion with the additional input channel. The control should be the same network with concatenated sources.
