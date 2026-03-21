# Missing Modality Handling for Multi-Modality Medical Image Fusion
## 📌 Overview
Missing modality is a common challenge in clinical multi-modal medical image analysis: due to image damage, artifacts, acquisition protocol limitations, contrast agent allergy, or cost issues, one or more modalities are often missing in practical applications. Most existing multi-modal fusion/segmentation methods are designed for complete modalities, and their performance will drop sharply when modalities are missing.

This section summarizes the representative methods for handling missing modalities in multi-modal medical image fusion and downstream tasks, which mainly solve the problem through self-supervised pre-training, modality completion, generalizable feature learning, and other technical paths.

## 📑 Curated List of Methods
| Full Paper Title | Publication Venue & Year | Core Contributions | Paper Link | Open-Source Code |
|-------------------|---------------------------|--------------------|------------|------------------|
| M3AE: Multimodal Representation Learning for Brain Tumor Segmentation with Missing Modalities | arXiv, 2023 | Proposes a multi-modal mask autoencoder (M3AE) for brain tumor segmentation with missing modalities. In the pre-training stage, it masks random modality subsets and random 3D image patches simultaneously, and learns robust feature representations via mask recovery. It also uses model inversion for modality completion and memory-efficient self-distillation for optimization. | [Link](https://arxiv.org/abs/2303.05302) | [GitHub](https://github.com/ccarliu/m3ae) |
| Multi-Modality Uncertainty for Medical Image Segmentation | 5th International Conference on Neural Networks, Information and Communication Engineering (NNICE), 2025 | Mathematically proves that the multi-modal uncertainty is less than or equal to the maximum uncertainty of single modality in late fusion, theoretically explaining the performance advantage of multi-modal fusion. It proposes an uncertainty-driven feature fusion strategy, which converts feature uncertainty into confidence weights, and reduces the interference of low-reliability information when modalities are missing. | [Link](https://ieeexplore.ieee.org/abstract/document/11064419) | Not publicly available |
| Evidence modeling for reliability learning and interpretable decision-making under multi-modality medical image segmentation | Computerized Medical Imaging and Graphics (CMIG), 2024 | Proposes CDE-Net based on Dempster-Shafer evidence theory, which learns the category-level reliability coefficient of each modality via a context discount fusion layer (CDFL). It can adaptively adjust the fusion weight according to the reliability of the input modality, and has strong robustness to missing modalities. | [Link](https://www.sciencedirect.com/science/article/pii/S0895611124000995) | Not publicly available |




# Unaligned Multi-Modality Medical Image Fusion
## 📌 Overview
Spatial misalignment between multi-modal medical images is a common clinical problem, which is caused by respiratory motion, organ deformation, patient movement, different scanning positions, and other factors. Traditional multi-modal fusion methods rely on strictly pre-registered images, and the fusion quality will be seriously degraded when facing unaligned images. The two-stage "registration first, fusion later" method has high complexity and error accumulation problems.

This section summarizes the representative methods for unaligned multi-modal medical image fusion, which mainly realize end-to-end alignment and fusion through feature-level alignment, joint registration-fusion framework, deformable attention, and other technical paths.

## 📑 Curated List of Methods
| Full Paper Title | Publication Venue & Year | Core Contributions | Paper Link | Open-Source Code |
|-------------------|---------------------------|--------------------|------------|------------------|
| BSAFusion: A Bidirectional Stepwise Feature Alignment Network for Unaligned Medical Image Fusion | AAAI, 2025 | Proposes a single-stage BSAFusion framework for unaligned medical image fusion (CT-MRI/PET-MRI/SPECT-MRI). It designs a modality-difference-free feature representation (MDF-FR) module to eliminate modal differences, and a bidirectional stepwise feature alignment (BSFA) module to handle elastic deformation. It reduces the alignment error by 35% in elastic deformation scenarios, with 2.1x faster inference speed than two-stage methods. | [Link](https://arxiv.org/abs/2412.08050) | [GitHub](https://github.com/slrl123/BSAFusion) |
| Quasi-Conformal Hybrid Multi-modality Image Registration and its Application to Medical Image Fusion | International Symposium on Visual Computing (ISVC), 2015 | Proposes a quasi-conformal hybrid registration framework for multi-modal medical images, which ensures diffeomorphic transformation via Beltrami coefficient optimization, and combines landmark and intensity constraints to achieve high-precision registration. It then completes data-level fusion via DWT, solving the image folding problem in large deformation registration. | [Link](https://link.springer.com/chapter/10.1007/978-3-319-27857-5_72) | Not publicly available |
| Three-Dimensional Medical Image Fusion with Deformable Cross-Attention | International Conference on Neural Information Processing (ICONIP), 2023 | Proposes a 3D medical image fusion method with deformable cross-attention, which adaptively aligns the features of unaligned 3D medical images via deformable attention mechanism, and improves the fusion accuracy of 3D volume data without independent registration steps. | [Link](https://link.springer.com/chapter/10.1007/978-981-9981-31-3_45) | Not publicly available |




# Degraded Multi-Modality Medical Image Fusion
## 📌 Overview
Medical images often have various degradations in clinical scanning, such as motion artifacts, metal artifacts, noise, low dose, blurring, etc. These degradations will seriously affect the accuracy of multi-modal feature extraction and fusion, leading to the loss of pathological details and structural information in the fused image. Traditional fusion methods are designed for high-quality images, and their performance will drop sharply when facing degraded images.

This section summarizes the representative methods for degraded multi-modal medical image fusion, which mainly solve the problem through degradation-aware learning, joint restoration and fusion, adaptive degradation modeling, and other technical paths.

## 📑 Curated List of Methods
| Full Paper Title | Publication Venue & Year | Core Contributions | Paper Link | Open-Source Code |
|-------------------|---------------------------|--------------------|------------|------------------|
| UniFuse: A Unified All-in-One Framework for Multi-Modal Medical Image Fusion Under Diverse Degradations and Misalignments | arXiv, 2025 | Proposes a unified all-in-one framework UniFuse for multi-modal medical image fusion under diverse degradations (motion artifacts, metal artifacts, low-dose noise) and misalignments. It designs a degradation-aware prompt learning (DAPL) module to associate degradation with alignment-restoration, an omnidirectional unified feature representation (OUFR) module to eliminate modal differences, and an adaptive LoRA协同 network (ALSN) for lightweight adaptive restoration. It realizes degradation removal, alignment and fusion in a single stage. | [Link](https://arxiv.org/abs/2506.22736) | [GitHub](https://github.com/slrl123/UniFuse) |
| Multi-Modality Medical Image Fusion Using SWT & Speckle Noise Reduction with Bidirectional Exact Pattern Matching Algorithm | Disruptive Technologies for Society 5.0, 2021 | Proposes a non-deep learning fusion method combining stationary wavelet transformation (SWT) and speckle noise reduction (SNR) technology, which can effectively suppress speckle noise in ultrasound/MRI images while completing multi-modal fusion. | [Link](https://www.taylorfrancis.com/chapters/edit/10.1201/9781003154686-20/multi-modality-medical-image-fusion-using-swt-speckle-noise-reduction-bidirectional-exact-pattern-matching-algorithm-kapil-joshi-minakshi-memoria-laxman-singh-parag-verma-archana-barthwal) | Not publicly available |
| A robust mutual-reinforcing framework for 3d multimodal medical image fusion based on visual-semantic consistency | AAAI, 2024 | Proposes a robust mutual-reinforcing framework for 3D multi-modal medical image fusion, which optimizes the fusion performance of low-quality/degraded 3D medical images via visual-semantic consistency constraints, and improves the robustness of fusion to image degradations. | [Link](https://ojs.aaai.org/index.php/AAAI/article/view/28589) | Not publicly available |
