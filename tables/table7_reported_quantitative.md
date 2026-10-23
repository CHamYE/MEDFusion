# Table 7 — Reported Quantitative Results (GLIS-RT)

CT–T1-Gd MRI fusion and contouring results reported by Safari et al. (mean ± SD).

| Method | Backbone / principle | EN | SSIM | Q^AB/F | Contouring Dice | Params / FLOPs |
|---|---|---|---|---|---|---|
| GTF | Gradient transfer | 5.25±0.42 | 0.29±0.37 | 0.60±0.06 | NR | NR / NR |
| [5pt] DDCT-PCA | Transform + PCA | 5.13±0.30 | 0.33±0.16 | 0.60±0.06 | 0.91±0.07 | NR / NR |
| [5pt] FPDE | Fourth-order PDE | 4.77±0.34 | 0.25±0.26 | 0.37±0.10 | NR | NR / NR |
| [5pt] HMSD | Multiscale decomposition | 5.58±0.23 | 0.32±0.17 | 0.60±0.07 | 0.85±0.08 | NR / NR |
| [5pt] GFDF | Traditional fusion | 2.07±0.51 | 0.66±0.33 | 0.46±0.04 | NR | NR / NR |
| [5pt] IVF | Traditional fusion | 2.74±0.57 | 0.13±0.05 | 0.54±0.04 | 0.88±0.07 | NR / NR |
| [5pt] MEF | Multi-exposure fusion | 2.06±0.48 | 0.81±0.03 | 0.61±0.06 | 0.89±0.09 | NR / NR |
| [5pt] CNN-Fuse | CNN | 2.06±0.50 | 0.66±0.31 | 0.51±0.07 | NR | NR / NR |
| [5pt] SESF-Fuse | CNN autoencoder | 2.06±0.51 | 0.58±0.25 | 0.46±0.04 | NR | NR / NR |
| [5pt] SwinFusion | Swin Transformer | 2.05±0.46 | 0.67±0.16 | 0.60±0.04 | 0.89±0.07 | NR / NR |
| [5pt] IFCNN | CNN | 2.11±0.48 | 0.78±0.04 | 0.60±0.05 | 0.92±0.04 | NR / NR |
| [5pt] U2Fusion | CNN | 2.14±0.49 | 0.15±0.06 | 0.54±0.07 | 0.90±0.07 | NR / NR |
| [5pt] DSAGAN | GAN | 2.19±0.39 | 0.11±0.05 | 0.40±0.05 | 0.72±0.14 | NR / NR |
| [5pt] CU-Net | Coupled unrolling | 2.83±0.55 | 0.40±0.09 | 0.31±0.04 | NR | NR / NR |
| [5pt] FusionGAN | GAN | 1.64±0.30 | 0.59±0.18 | 0.35±0.03 | NR | NR / NR |
| [5pt] MedFusionGAN | Residual CNN / GAN | 5.20±0.38 | 0.62±0.22 | 0.64±0.10 | 0.96±0.02 | NR / NR |
