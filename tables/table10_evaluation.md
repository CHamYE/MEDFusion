# Table 10 — Evaluation System for MMIF

The manuscript organises evaluation into four dimensions and their measures. The full descriptions and metric formulas are in the manuscript table and in Section 6.4; this page records the structure so that the repository and the paper use the same vocabulary.

| Dimension | Measures |
|---|---|
| Clinical qualitative validation | Professional physician assessment; structural detail preservation; artifact control; clinical auxiliary value |
| User study | Information completeness; visual comfort; reading time and decision confidence |
| Objective quantitative — source-referenced | SSIM, PSNR, MI, CC, Q^AB/F, N^AB/F, RMSE, SCD |
| Objective quantitative — output statistics | EN, SF, SD, AG |
| Objective quantitative — task performance | Dice, IoU, HD95, ACC, AUC, mAP |
| Engineering-oriented — efficiency | Model size, FLOPs, FPS |
| Engineering-oriented — robustness | Stability under noise, artifacts, low dose and spatial misalignment |

## Reading note

Source-referenced measures compare the fused image with the specified source images; they do not measure fidelity to a ground-truth fused target, because MMIF has none. Output statistics can be inflated by noise, which is why they are reported alongside task-level or reader evidence rather than alone.
