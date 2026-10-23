# Table 2 — Configurations Across Input, Fusion Stage and Output

Representative configurations mapped to the three axes used in the manuscript.

| Example | Input composition | Fusion stage and operation | Output purpose |
|---|---|---|---|
| Raw-channel concatenation (illustrative configuration) | Multi-sequence MRI; no explicit temporal fusion; no auxiliary text | Data: concatenate raw input channels before a shared encoder | Segmentation |
| SwinFusion | CT-MRI or PET-MRI; no explicit temporal fusion; no auxiliary text | Feature: cross-attention integrates image representations | Fused image |
| Deep residual feature fusion | T1, T1ce, T2, FLAIR MRI; no explicit temporal fusion; no auxiliary text | Feature: combine modality-specific residual features | Brain tumor segmentation |
| Deep evidential fusion | PET-CT or multi-sequence MRI; no explicit temporal fusion; no auxiliary text | Decision: combine reliability-discounted modality-specific belief masses | Tumor segmentation and uncertainty |
| MTG-Fusion | Multiple medical images (e.g., CT-MRI); no explicit temporal fusion; generated text guidance | Feature: text-guided extraction and weighting of image features | Fused image |
| MTFN (temporal boundary example) | One DCE-MRI sequence, phases 1 and 3 of one examination; no auxiliary text | Feature: co-attention integrates temporal representations | Synthesis of phase 8; related supporting task |
