# Fused-Image Generation

## Task definition

Fused-image generation is the direct output of MMIF: a single image that carries the complementary information of two or more sources. It is the task most often reported in the corpus, and the one with the weakest clinical endpoint.

## Metrics

Source-referenced measures (MI, Q^AB/F, SSIM, VIF, SCD), output statistics (EN, SD, SF, AG), and reader preference. Report the metric family and the implementation; MI and EN are sensitive to normalization and quantization, and a higher value is not always better.

![Metric frequency in the corpus](../../assets/fig9.png)

*Figure 9 of the manuscript: application frequency of the 13 metric families over 192 studies.*

## Representative studies

| Title | Venue, Year | DOI |
|---|---|---|
| [MGMDcGAN: Medical Image Fusion using Multi-Generator Multi-Discriminator Conditional Generative Adversarial Network](https://doi.org/10.1109/access.2020.2982016) | IEEE Access, 2020 | [10.1109/access.2020.2982016](https://doi.org/10.1109/access.2020.2982016) |
| Anatomical-Functional Image Fusion by Information of Interest in Local Laplacian Filtering Domain | IEEE Transactions on Image Processing, 2017 | NR |
| [A New Approach of Multi-Modal Medical Image Fusion using Intuitionistic Fuzzy Set](https://doi.org/10.1016/j.bspc.2022.103762) | Biomedical Signal Processing and Control, 2022 | [10.1016/j.bspc.2022.103762](https://doi.org/10.1016/j.bspc.2022.103762) |
| [A Multiscale Residual Pyramid Attention Network for Medical Image Fusion](https://doi.org/10.1016/j.bspc.2021.102488) | Biomedical Signal Processing and Control, 2021 | [10.1016/j.bspc.2021.102488](https://doi.org/10.1016/j.bspc.2021.102488) |
| [MACTFusion: Lightweight Cross Transformer for Adaptive Multimodal Medical Image Fusion](https://doi.org/10.1109/jbhi.2024.3391620) | IEEE Journal of Biomedical and Health Informatics, 2025 | [10.1109/jbhi.2024.3391620](https://doi.org/10.1109/jbhi.2024.3391620) |

## What to check in an entry

- Whether the method has a ground-truth fused target; if not, source-referenced metrics are the only quantitative option.
- Whether the metric implementation and parameters are stated; MI and EN are not comparable across implementations without them.
- Whether any reader evaluation was performed, and how many readers.

## Note

A fused image with a high MI can still lose a small lesion. The entry should say which structures the method is claimed to preserve: bone, soft tissue, vessels, or metabolic uptake.
