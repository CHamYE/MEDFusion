# Table 3 — Data-Level Fusion Studies

Reproduced from the manuscript. The paper title links to the DOI; rows without a DOI are left unlinked. Each row is one table entry, so a study spanning several configurations appears more than once.

| Paper | Year | Modalities | Method | Datasets | Metrics | Validation evidence |
|---|---|---|---|---|---|---|
| Fusion system | 1993 | CT-MR | Color channel mapping | Private | Point displacement error, spatial dimension accuracy, visual evaluation | Unclear |
| 3D voxel fusion | 2004 | CT-MRI, MRI multi-sequences | 3D reconstruction, color coding | Private | Fusion accuracy, FPS | Unclear |
| [3D spinal fusion](https://doi.org/10.1016/j.compmedimag.2003.08.001) | 2004 | 3D CT-MRI | Registration, voxel merging, Semi-Boundary | Private | Visual evaluation | Unclear |
| [Color table fusion](https://doi.org/10.1109/nssmic.2004.1462740) | 2004 | CT-PET-MRI | Anatomy specific color fusion, Observer oriented fusion | Private | Visual evaluation | Unclear |
| [Regis+ICP](https://doi.org/10.1117/12.710323) | 2007 | DE-MRI&PV-MRA, PV-MRA&EAM, DE-MRI&PV-MRA&EAM | Intensity-based rigid registration, ICP | Private | Registration error | Unclear |
| TRUS-MRI fusion | 2007 | TRUS-MRI | Manual registration method for 3D US reconstruction | Private | Hausdorff, TRE, FRE | Unclear |
| [AWT+curvelet transform](https://doi.org/10.1080/09500340903541056) | 2010 | MRI-CT | Curvelet transform | Private | Similarity, PSNR | Unclear |
| [PCA+DWT](https://doi.org/10.21917/ijivp.2013.0098) | 2013 | CT-PET | PCA, DWT | Private | MSE, PSNR, Entropy, visual evaluation | Unclear |
| [Improved ICP](https://doi.org/10.1155/2014/348740) | 2014 | CT& Blue-Ray | ICP, improved Voronoi | Private | Registration average Euclidean distance | Unclear |
| DCxWT | 2014 | CT-MRI, T1w MRI-MRA | DCxWT, multi-scale max fusion | Imagefusion.org | Entropy, Q_AB^F , FF, SD, FS | Unclear |
| [Block PCNN](https://doi.org/10.1109/icsess.2015.7339067) | 2015 | CT-MRI | S-PCNN, OFG, Image block processing | Private | FD, MI, Q_AB^F , MV, RMSE | Unclear |
| [QC hybrid](https://doi.org/10.1007/978-3-319-27857-5_72) | 2015 | CT-MRI | Pseudo conformal mapping, mixed criteria | Private | e_max/e_mean , Beltrami, MI, visual evaluation | Unclear |
| CMA-ES | 2016 | CT-MRI | Morphological filtering, evolutionary optimization | Private | Registration error, time, visual evaluation | Unclear |
| Union LAP | 2016 | CT-MRI, PET-MRI, SPECT-MRI | Laplacian pyramid multi-scale decomposition, multi feature fusion, image statistics | AANLIB | PSNR, STD, SSIM, TMQI | Benchmark |
| [QPSO-PCNN](https://doi.org/10.1016/j.asoc.2016.03.028) | 2016 | CT-MR, MR T1-FDG, MR T2-SPET | QPSO-PCNN | Private | STD, SF, MI, SSIM, Sharpness | Unclear |
| [Wavelet channel fusion](https://doi.org/10.1186/s13640-017-0204-3) | 2017 | MR T1-CT, MR DWI-CT | Wavelet-Pseudo color-α channel | Human Connectome Project | IE, MI, MG, SF, visual evaluation | Unclear |
| [MRR](https://doi.org/10.1016/j.bj.2017.09.002) | 2017 | CT-MRI | B-spline deformable registration | Kasturba Hospital | MI, visual evaluation | Reader study (radiologist ratings) |
| PCA-DWT | 2017 | CT-MRI, MRI-SPECT | PCA, DWT, PCNN | AANLIB | PSNR, STD, Entropy, MI, Q_AB^F , visual evaluation | Unclear |
| [LR sparse dictionary fusion](https://doi.org/10.1016/j.patcog.2018.02.005) | 2018 | CT-MRI, MRI-T1/MRI-T2, MRI-PET, SPECT-MRI | Discriminative low-rank sparse dictionary learning, low-rank and sparse component decomposition, weighted nuclear norm regularization, max-absolute component fusion | AANLIB, imagefusion.org, private training samples | MI, Q_\textTE, Q_\textNCIE, Q_\textM, Q_\textP, Q_\textS, Q_\textG | Unclear |
| [CNN Type-I (input)](https://doi.org/10.1109/isbi.2018.8363717) | 2018 | PET-CT-MRI T1/T2 | 2D patch stacking across modalities; channel-spanning kernels | TCIA | Pixel-wise Accuracy, visual evaluation | Benchmark |
| [Fuzzy logic](https://doi.org/10.1109/cccs.2018.8586829) | 2018 | CT-MRI-PD | T-S fuzzy reasoning system | AANLIB | MSE, PSNR, SNR, visual evaluation | Unclear |
| [Tetrolet SUnSAL](https://doi.org/10.1016/j.dsp.2018.04.002) | 2018 | CT-MRI, PET-MRI, SPECT-MRI | Tetrolet transform, SUnSAL, cycle-spinning, MDC, WSML | Imagefusion.org, AANLIB | Visual evaluation, LSSIM, MI, Q_AB^F , FSIM/FSIMC | Unclear |
| [NSST PCNN](https://doi.org/10.1007/s11760-018-1303-z) | 2018 | CT-MRI T2 | NSST, PCNN | PGIMER, AANLIB | STD, MI, SF, Q_AB^F , Mean | Benchmark; Unclear (cohort design) |
| [NSST S-PCNN](https://doi.org/10.1016/j.sigpro.2018.08.002) | 2018 | CT-MRI-PET | HSV, NSST, ICM S-PCNN | AANLIB | AG, SF, MV, SD | Unclear |
| DRT | 2018 | MRI-PET | DRT, SSF | AANLIB | MI, SF, ASSIM, Q_AB^F | Benchmark |
| [S-ICP](https://doi.org/10.1117/12.2512775) | 2019 | 3D coronary artery-vein anatomy SPECT | S-ICP, CRT | Private | Registration error | Unclear |
| [BWT](https://doi.org/10.1016/j.ijleo.2018.12.028) | 2019 | CT-MRI, MRI T1-MRA | BWT, GFS rules | Imagefusion.org | FF, FS, Entropy, Q_AB^F | Unclear |
| [CS-MCA](https://doi.org/10.1109/lsp.2019.2895749) | 2019 | CT-MRI T2, MRI T1-T2 | CSR, MCA | AANLIB | LMI, Q_AB^F , Q_HVS , Q_E | Unclear |
| [CNN-DCSCM](https://doi.org/10.1007/s11517-018-1935-8) | 2019 | CT-MRI | VGG, DCSCM | AANLIB | MSSIM, IE, MI, SF, Q_AB^F | Benchmark |
| [Siamese CNN](https://doi.org/10.3390/s20082169) | 2020 | MRI-CT, MRI T1-T2, MRI-PET/SPECT | CNN, contrast pyramid | AANLIB | TE, MI, VIF, Q_AB^F , visual evaluation | Unclear |
| [PMGI](https://doi.org/10.1609/aaai.v34i07.6975) | 2020 | MRI-PET | PGMI | AANLIB | CC, EN, FMI, MI, SF, SSIM, SD | Benchmark |
| [MIEE-PCNN](https://doi.org/10.1109/tcsvt.2020.2998696) | 2021 | CT-MRI, PET-MRI | MIEE, PCNN, PSO | AANLIB, Imagefusion.org | Visual evaluation, NMI, SSIM, Q^AB/F, FSIM | Unclear |
| [BMGAN](https://doi.org/10.1109/tmi.2021.3107013) | 2021 | MRI-PET | 3D Dense-UNet, GAN | ADNI, OASIS-3, TCIA | PSNR, FID, MS-SSIM, MAE | Unclear |
| [AISA-NSST](https://doi.org/10.1016/j.bspc.2021.102480) | 2021 | CT-PET, MRI-CT, MR T1-T2 | NSST, AISA, MG | AANLIB | PSNR, SSIM, SD, EN, MI, Q^AB/F, time, visual evaluation | Benchmark |
| [ECLAHE](https://doi.org/10.3233/XST-210851) | 2021 | CT-MRI | SNNE, ECLAHE | AANLIB, BraTS 2015 | MSE, PSNR, SSIM, EN, F1, accuracy, recall | Benchmark |
| [CS-PCA](https://doi.org/10.1007/s12065-020-00551-0) | 2021 | MRI DW-FLAIR, DW-T1, FLAIR-T1, DW-FLAIR-T1 | CS, PCA, Tsallis WSS | ISLES 2015 | DSC, JI, PR, AC, SE | Benchmark |
| [DCT](https://doi.org/10.1109/wiecon-ece54711.2021.9829686) | 2021 | CT-MRI | DWT, DCT | Private | MSE, AG, PSNR, EN, SD, SNR | Unclear |
| [Lambert](https://doi.org/10.1016/j.radonc.2022.06.021) | 2022 | MRI-Fundus | 2D-3D Lambert | Private | NCC, VR, AR, distance, visual evaluation | Unclear |
| [Variational optimization](https://doi.org/10.1007/s11760-022-02220-4) | 2022 | CT-MRI | Variational optimization fusion | Harvard Whole Brain Atlas | MI, Q_W , Q^G | Benchmark |
| [IST-NSST](https://doi.org/10.1016/j.bspc.2022.103717) | 2022 | PET-CT | WAGLE, IST | AANLIB | VIF, EDGE, FD, AG, SF, SD | Unclear |
| [CDF 9/7 NSST](https://doi.org/10.18280/ts.390432) | 2022 | CT-MRI, MRI-PET, MRI-SPECT | CDF 9/7 NSST, MPCNN | AANLIB | VIF, SS, EN, SD | Unclear |
| [SIFI](https://doi.org/10.1016/j.bspc.2022.103762) | 2022 | CT-MRI, MRI T1-T2, MRI-Gad-T2 | SIFS, fuzzy set | AANLIB | AG, MI, Entropy, SD, Mean, visual evaluation | Unclear |
| [CBF-DTF-RGF](https://doi.org/10.1016/j.eswa.2022.118283) | 2022 | CT-MRI | DTF, RGF, CBF | MATLAB Central File Exchange | CC, EN, SD, MI, AG, API | Benchmark |
| [SwinFusion](https://doi.org/10.1109/jas.2022.105686) | 2022 | PET-MRI, CT-MRI | Swin Transformer, CNN | AANLIB | PSNR, SSIM, Q_AB^F , FMI | Benchmark |
| [PAULPCNN](https://doi.org/10.1016/j.bspc.2023.104659) | 2023 | PET-MRI, SPECT-MRI | PAULPCNN, NSST, DWRE | AANLIB | UQI, Edge, AG, MIF, SSIM, Q_AB^F | Unclear |
| M3AE | 2023 | MRI T1-T1c-T2-FLAIR | M^3AE, model inversion, self-distillation | BraTS 2018, 2020 | DSC, HD95 | Benchmark |
| [3D U-Net](https://doi.org/10.1063/5.0209009) | 2024 | MRI T1-T1ce-T2-FLAIR | 3D U-Net, attention | BraTS 2018 | DSC, IoU | Unclear |
| [MHFN input baseline](https://doi.org/10.1007/s11768-024-00231-9) | 2024 | MRI T1W–T2W-STIR | Raw-input concatenation; baseline in the MHFN study | Private | DSC, IoU, HD | Unclear (single-center cohort) |

The same records are available as CSV in `table3_data_level.csv`.
