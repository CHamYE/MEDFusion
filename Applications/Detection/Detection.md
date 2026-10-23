# Fusion for Detection

## Task definition

Detection localizes lesions or abnormalities and assigns a confidence. In MMIF it is used for lung nodules, brain metastases, and lesion screening on fused PET/CT or PET/MRI.

## Metrics

Report mAP at a stated IoU threshold, sensitivity at fixed false positives per case, and the lesion-size distribution. Small lesions dominate the clinical risk and are usually where fusion helps or hurts most.

## Representative studies

| Title | Venue, Year | DOI |
|---|---|---|
| Yolo-SG: Salience-Guided Detection of Small Objects in Medical Images | 2022 IEEE International Conference on Image Processing (ICIP), 2022 | [10.1109/icip46576.2022.9898077](https://doi.org/10.1109/icip46576.2022.9898077) |
| Artificial Intelligence Empowered Coronary Artery Imaging: A Review | Computerized Medical Imaging and Graphics, 2026 | NR |
| A Corresponding Region Fusion Framework for Multi-Modal Cervical Lesion Detection | IEEE/ACM Transactions on Computational Biology and Bioinformatics, 2024 | [10.1109/tcbb.2022.3178725](https://doi.org/10.1109/tcbb.2022.3178725) |
| An Adaptive and Lightweight YOLOv5 Detection Model for Lung Tumor in PET/CT Images | Scientific Reports, 2024 | [10.1038/s41598-024-79786-1](https://doi.org/10.1038/s41598-024-79786-1) |

## What to check in an entry

- Whether detection was performed on the fused image or on the source channels.
- Whether the reference standard is pathology, follow-up imaging, or a single reader.
- Whether false positives are reported per image or per patient.

## Note

Detection papers frequently report only mAP. Without a fixed operating point, mAP cannot be translated into a clinical reading workflow.
