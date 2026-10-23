# Emerging Directions for Clinical Translation

## 📌 Overview

This folder mirrors Section 4 of the survey. The four directions here are not new fusion levels; they are requirements that decide whether a fusion model can leave the benchmark and enter a clinical workflow.

| Direction | Clinical question | Representative methods | Figure |
|---|---|---|---|
| [Interpretable fusion](Interpretable_Fusion/README.md) | Can the contribution of each modality be traced? | Bilevel integrated optimization, CDDFuse, DDFM, CDE-Net | Fig. 4 |
| [Generative fusion](Generative_Model_Fusion/README.md) | Can a learned prior supply missing or degraded information? | DDcGAN, U-Patch GAN, AdvTCUnet, DDFM, DM-FNet, Mask-DiFuser | Fig. 5 |
| [Robust fusion](Low-quality_data-adaptive_fusion/readme.md) | Does performance hold under noise, artifacts and misalignment? | U-Fusion, LR-FNet, M3AE, MEI-Net | Fig. 6 |
| [Lightweight fusion](Lightweight_generalized_fusion/readme.md) | Can the model run on clinical hardware? | NAS-based fusion, M4FNet, DMCMFuse, MambaDFuse | Fig. 7 |

## 🔗 How the directions interact

Interpretability and robustness are often traded against each other: a module that exposes modality contributions usually adds branches and parameters, which raises inference cost. Generative priors improve restoration and missing-modality synthesis but introduce a fidelity risk, because a plausible output is not necessarily a faithful one. Lightweight design reduces cost but can remove the redundancy that makes a model robust.

The survey therefore treats these four directions as constraints to be reported together, not as independent improvements. Each folder records the constraint, the representative methods, and the evidence that the claim was tested.

## ✅ Evidence standard

A method listed here is not endorsed because it reports a high score. The entry should state the dataset, the metric family, the validation evidence, and whether code or data are available. Studies without a quantitative evaluation are marked as such rather than being ranked.
