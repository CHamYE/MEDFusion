# Public Datasets for MMIF

The ten datasets below are the ones used most often in the surveyed corpus. They differ in what they provide: paired modalities, segmentation labels, or a repository from which a pair must be assembled.

| Dataset | Primary objective | Modality composition | Release and scale | Source |
|---|---|---|---|---|
| AANLIB / Whole Brain Atlas | Brain anatomy and neurological disease examples | CT, MRI, PET, SPECT; combinations vary by case | Case-based atlas | https://www.med.harvard.edu/AANLIB/ |
| BraTS | Brain-tumour segmentation with expert annotations | Co-registered T1, T1ce, T2, FLAIR | 2020: 369 training cases, four sequences each | https://www.med.upenn.edu/cbica/brats/ |
| TCIA | Cancer imaging collections; fusion depends on collection | Collection-dependent; multiparametric MRI, PET/CT | Collection-dependent (e.g., TCGA-GBM, 262 subjects) | https://www.cancerimagingarchive.net/ |
| ADNI | Longitudinal imaging and biomarkers for aging and Alzheimer disease | Structural MRI and PET; sequences depend on phase | Phase- and visit-dependent cohort | https://adni.loni.usc.edu/ |
| Imagefusion.org | Legacy image-fusion examples | Study-specific pairs; medical subset provenance unverified | No verified current release | http://www.imagefusion.org/ |
| OASIS | Cross-sectional and longitudinal imaging of aging | OASIS-1: T1; OASIS-3: T1, T2, FLAIR, PET | Cross-sectional and longitudinal cohorts | https://www.oasis-brains.org/ |
| IXI | Healthy-subject brain MRI | T1, T2, PD, MRA, diffusion | About 600 subjects from three London hospitals | https://brain-development.org/ixi-dataset/ |
| CHAOS | Abdominal organ segmentation; CT and MRI cohorts not paired | CT; MRI T1-DUAL and T2-SPIR | 40 CT and 40 MRI patients (separate) | https://chaos.grand-challenge.org/ |
| SynthRAD 2023 | Synthetic CT generation for radiotherapy | Task 1: MRI-CT; Task 2: CBCT-CT | 540 pairs per task (360/60/120) | https://synthrad2023.grand-challenge.org/ |
| HECKTOR 2021 | Head-and-neck tumour segmentation and outcome | Registered FDG-PET and CT | 224 training and 101 test cases | https://hecktor.grand-challenge.org/ |

## Pairing status

Only some of these datasets provide true paired acquisitions. BraTS, SynthRAD 2023 and HECKTOR 2021 provide registered pairs; CHAOS provides CT and MRI cohorts that are not paired across modalities; AANLIB provides case-level combinations. A study that reports a fusion score on unpaired data is measuring a different task, and the entry should say so.

## Links and licences

Each dataset is governed by its own data-use agreement. Check the licence before redistributing any image. This repository links to the official portals and does not host imaging data.
