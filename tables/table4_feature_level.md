# Table 4 — Feature-Level Fusion Studies

Reproduced from the manuscript. The paper title links to the DOI; rows without a DOI are left unlinked. Each row is one table entry, so a study spanning several configurations appears more than once.

| Paper | Year | Modalities | Method | Datasets | Metrics | Validation evidence |
|---|---|---|---|---|---|---|
| Shunt color | 2001 | MRI-PD, MRI-SPECT | Shunt Neural Network, Color Opponent Fusion | AANLIB | Visual evaluation | Unclear |
| Wavelet transform | 2001 | PET-MRI, CT-MRI | Wavelet Pyramid, Mallat Orthogonal Wavelet Decomposition, Max Selection | Private | Bias, visual evaluation | Unclear |
| [3D convolution](https://doi.org/10.1109/icif.2002.1020950) | 2002 | MRI PD-T1-T2, MRI-SPECT | Shunt Neural Network, Color Opponent Fusion | AANLIB | Visual evaluation | Unclear |
| [Color table fusion](https://doi.org/10.1109/nssmic.2004.1462740) | 2004 | MRI-CT-PET | 2D CLT, blending | Private | Visual evaluation | Unclear |
| [PCNN](https://doi.org/10.1007/11539087_131) | 2005 | CT-MRI, CT-SPECT, MRI-PET | DWF, PCNN, OMP | AANLIB | MI, EN, Visual evaluation | Unclear |
| [2d DWT](https://doi.org/10.1109/icnsc.2006.1673156) | 2006 | CT-MRI | DWT, IDWT | Private | RMSE, PSNR | Unclear |
| [Regis+ICP](https://doi.org/10.1117/12.710323) | 2007 | DE-MRI&PV-MRA, PV-MRA&EAM, DE-MRI&PV-MRA&EAM | ICP | Private | Registration error | Unclear |
| [Wavelet transform](https://doi.org/10.1007/978-3-642-13498-2_82) | 2010 | CT-MRI, MRI-PET | DWT, Max Selection | Private | Mean, Variance, EN, CEN, visual evaluation | Unclear |
| [FDCT](https://doi.org/10.1109/ams.2012.46) | 2012 | CT-MRI | DWT, FDCT, IDWT, IHS Transform | Private | RMSE, PSNR | Unclear |
| [NSCT](https://doi.org/10.1587/transinf.e96.d.2215) | 2013 | CT-MRI | NSCT, MSML | Private | MI, Q^AB/F, SF | Unclear |
| [DWT-PCA](https://doi.org/10.21917/ijivp.2013.0098) | 2013 | CT-PET | PCA, DWT | Private | MSE, PSNR, EM, visual evaluation | Unclear |
| [Framelet HVS](https://doi.org/10.1016/j.eswa.2012.09.011) | 2013 | CT-MRI, MRI-PET | Framelet Transform, HVS, IHS Transform | AANLIB | Mean, EN, SF, MI, SSIM, Q^AB/F | Unclear |
| [DWT](https://doi.org/10.1016/j.procs.2015.10.057) | 2015 | PET-MRI | DWT, FCM, IHS Transform | AANLIB | MSE, PSNR, SD, AG | Unclear |
| [MST-SR](https://doi.org/10.1016/j.inffus.2014.09.004) | 2015 | CT-MRI, Gd DTPA MRI-MRI T2 | MST, Sparse Representation, OMP | Private | SD, EN, QG, QP, QW | Unclear |
| [Surface regis](https://doi.org/10.1117/12.2082160) | 2015 | CT-US | EM System, ICP Algorithm | Private | RMS | Unclear |
| [QC hybrid](https://doi.org/10.1007/978-3-319-27857-5_72) | 2015 | CT-MRI | DWT, PCA | Private | LM, E, MI, visual evaluation | Unclear |
| [SOMP](https://doi.org/10.1016/j.neucom.2016.06.036) | 2016 | MRI-CT, MRI-MRA, MRI-PET | K-SVD, SOMP, Sparse Representation | AANLIB, Imagefusion.org | EN, EI, Q^AB/F, MI, VIF | Unclear |
| [Wavelet channel fusion](https://doi.org/10.1186/s13640-017-0204-3) | 2017 | MRI T1-CT, MRI DWI-CT | DWT, Mallat Algorithm, Max Selection | Human Connectome Project | IE, MI, MG, SF, visual evaluation | Unclear |
| PCA-DWT | 2017 | CT-MRI, MRI-SPECT | PCA, DWT, PCNN | AANLIB | STD, E, PSNR, MI, Q^AB/F | Unclear |
| [NSCT-PCNN](https://doi.org/10.1155/2017/8407019) | 2017 | CT-PET | NSCT, PCNN, NSML | CT | AG, EN, IQI, Q^AB/F | Unclear |
| [Pyramid CNN](https://doi.org/10.23919/icif.2017.8009769) | 2017 | CT-MRI | Siamese CNN, image pyramids | SPECT | EN, FMI, Q_G, Q_E, VIFF | Unclear |
| [MFDF-NSST](https://doi.org/10.1016/j.bspc.2017.10.001) | 2018 | CT-MRI | NSST, MFDF, SML, Max Selection | AANLIB, Imagefusion.org | MI, EN, Q_E | Unclear |
| [CNN Type-II (feature)](https://doi.org/10.1109/isbi.2018.8363717) | 2018 | PET-CT-MRI T1/T2 | Separate 2D CNN encoders; shared classifier | TCIA | Pixel-wise Accuracy, visual evaluation | Benchmark |
| [MANOVA](https://doi.org/10.1371/journal.pone.0191202) | 2018 | fMRI-sMRI-DTI | Multivariate analysis of variance | Private | Jaccard, Kappa, Wilk’s lambda, ROC, AUC | Unclear (single-center cohort) |
| DCHWT-PCNN | 2018 | MRI-PET, MRI-SPECT | DCHWT, PCNN | AANLIB | AG, STD, SSIM, Q^AB/F, MI, FSIM | Unclear |
| [SKR-LDP](https://doi.org/10.1016/j.ins.2017.09.010) | 2018 | PET-MRI, SPECT-MRI | Sparse Representation, OMP, PCA, K-SVD | AANLIB | MI, Q^AB/F, VIF, Q_CB | Benchmark |
| [Fuzzy-RBFNN](https://doi.org/10.1016/j.ejmp.2018.03.008) | 2018 | CT-MRI, MRI-SPECT | Fuzzy-RBFNN, EBPA-GSA, PCNN | Private | EN, STD, MI, Q^AB/F, MSE | Unclear |
| [Tetrolet SUnSAL](https://doi.org/10.1016/j.dsp.2018.04.002) | 2018 | CT-MRI, PET-MRI, SPECT-MRI | SUnSAL, Tetrolet Transform, Cycle-spinning | AANLIB, Imagefusion.org | MI, LSSIM, Q^AB/F, FSIM, FSIMC | Unclear |
| [MDWT](https://doi.org/10.1109/icoac44903.2018.8939112) | 2018 | CT-PET, SPECT, MRI, MRA, MRT | MDWT, PCA, Max Selection | Private | CE, H, SD, SF, FQI, RO, AVGER | Unclear |
| [FCN](https://doi.org/10.1088/1361-6560/aaf44b) | 2019 | PET-CT | FCN, V-Net | Private | DSC, CE, VE | Unclear |
| NSCT | 2019 | CT-MRI, MRI-PET, SPECT-MRI | NSCT, YUV Transform | AANLIB | TE, IE, Q^AB/F, Q_P, MI, Q_Y, Q_CB, VIF | Unclear |
| [MCFO](https://doi.org/10.1007/s11042-019-7552-1) | 2019 | MRI-PET, CT-PET, MRI-CT | DWT, MCFO, PCA | MedPix Dataset | AVG, L, C, STD, E, PSNR, Q^AB/F | Unclear |
| [NSST-SPCNN](https://doi.org/10.1109/jsen.2019.2948783) | 2020 | CT-MRI, CT, MRI | NSST, SPCNN , RE, EOG | Private | SD, EN, MI, SF, Q_G, Q_CB | Unclear |
| [FCM-PCA CNN](https://doi.org/10.1109/tim.2019.2933341) | 2019 | CT-MRI, PET-MRI, SPECT-MRI | CNN, FCM, PCA | AANLIIB | EN, MI, STD, UIQI, FMI, SF | Unclear |
| [Multi-level fusion](https://doi.org/10.1109/jbhi.2019.2956354) | 2020 | PET-CT | Image-, matrix-and feature-levels fusion | TCIA | C-index, Spearman, log-rank p, Kaplan-Meier | Unclear (multicenter design) |
| [IVD-Net](https://doi.org/10.1007/978-3-030-13736-6_11) | 2019 | MRI multi-sequence | U-Net, HyperDenseNet, Inception | MICCAI 2018 challenge | DSC | Unclear |
| Patch CNN | 2019 | PET-CT-MRI T1, PET-CT-MRI T2 | multi-stage CNN fusion | STS | DSC, Acc | Unclear |
| [ZL CNN](https://doi.org/10.23919/fusion43075.2019.9011178) | 2019 | MRI-CT/SPECT/PET, MRI T1-MRI T2-CT-PET | CNN, VGG-16, NSCT, PCNN | AANLIB | EN, MI, SSIM, Q_MRI-PET | Unclear |
| [SWT-FL](https://doi.org/10.1007/978-981-15-4451-4_44) | 2019 | CT-MRI, MRI T1-T2, MRI T2-SPET | SWT, FLICM | Private | MI, Q^AB/F, BSSIM, SSIM | Unclear |
| [Siamese CNN](https://doi.org/10.3390/s20082169) | 2020 | MR-CT, MR-T, MR-PET, MR-SPECT | CNN, contrast pyramid | AANLIB | Q^AB/F, MI, VIF | Unclear |
| [U2Fusion](https://doi.org/10.1109/tpami.2020.3012548) | 2022 | PET-MRI | Unsupervised loss, VGG, EWC | AANLIB | CC, SSIM, PSNR, SCD, EI, VIF, MG, visual evaluation | Unclear |
| [NSML-NSST](https://doi.org/10.1016/j.bspc.2019.101724) | 2020 | CT-MRI, MRI T1-T2, MRI T2-GAD, MRI-PET, MRI-SPECT | NSST, YIQ Transform, Mamdani | Imagefusion.org, AANLIB | EN, FMI, Q^AB/F, SD, MSSIM | Benchmark |
| [MM ASeDiL](https://doi.org/10.1016/j.image.2019.115758) | 2020 | CT-MRI, MRI T1-MRA, MRI Gd-T2, MRI T1-T2 | NSCT, ASeDiL, Gabor Filter | AANLIB | Piella–Heijmans, SF, UIQI, MI | Unclear |
| [DWT0-BCSO](https://doi.org/10.1007/s10729-019-09492-2) | 2020 | MRI-CT | DWT, BCSO | AANLIB | EN, SSIM, FF | Benchmark |
| [Auto CNN](https://doi.org/10.1007/s11277-019-06899-6) | 2020 | MRI-CT | SIFT, DWT, Curvelet Transform, interpolation, CNN | Private | Acc, visual evaluation | Unclear |
| [NMHE-SSGSM](https://doi.org/10.1016/j.bspc.2019.101810) | 2020 | CT-MRI | CSR, Average Rule, Max Selection | Imagefusion.org, AANLIB | MI, Q^AB/F, FMI, EN, VIF | Unclear |
| [IFCNN](https://doi.org/10.1016/j.inffus.2019.07.011) | 2020 | CT-MRI | IFCNN, CNN, ResNet101 | Private | VIFF, ISSIM, NMI, SF, AG | Unclear |
| [LRD](https://doi.org/10.1109/tim.2020.2975405) | 2020 | PET-MRI, SPECT-MRI | LRD, OD, NOD, IRS, LEM, LDM | AANLIB | STD, MI, UQI, TMQI | Unclear |
| [3D MM-NAS](https://doi.org/10.1007/978-3-030-59728-3_74) | 2020 | PET-CT | MM-NAS, CNN | TCIA | Acc, Prec, F1, AUC, ROC | Benchmark |
| [NSST+BM-PCNN](https://doi.org/10.1007/s00521-020-05173-2) | 2025 | MRI-PET, SPECT | NSST, BM-PCNN, MSMG | AANLIB | EN, SD, NMI, VIF, Q_F | Unclear |
| [MMFNet](https://doi.org/10.1016/j.neucom.2020.02.002) | 2020 | MRI T1-T2-T1ce | MMFNet, 3D-CBAM, RFBlock | Private | DSC, ASD, HD | Unclear (single-center cohort) |
| [Res-DenseNet](https://doi.org/10.1016/j.neucom.2020.06.078) | 2020 | MRI T1-T1ce-T2-FLAIR | DenseNet, ResNet | BraTS2015, BraTS2018 | DSC | Benchmark |
| [MGMDcGAN](https://doi.org/10.1109/access.2020.2982016) | 2020 | MRI-PET, MRI-SPECT, CT-SPECT | cGAN, mask | AANLIB | EN, SF, MG, PSNR, SSIM | Unclear |
| [Bilevel fusion](https://doi.org/10.1109/tip.2020.3043125) | 2021 | CT-MRI, MRI-SPECT | CNN, Transformer bilevel optimization | AANLIB | VIF, AG, EN, SF, SCD, Q^AB/F | Unclear |
| [DDcGAN](https://doi.org/10.1109/tip.2020.2977573) | 2020 | MRI-PET | DDcGAN, dual-discriminator | AANLIB | EN, MG, SF, SD, PSNR, CC, SSIM, VIF | Benchmark |
| [DBED](https://doi.org/10.1007/s00521-020-05421-5) | 2021 | CT-MRT, MRGAD-MRT, CT-MRPD | GAN, DBED | AANLIB | MI, SSIM, NCIE, Chen-Blum, visual evaluation | Benchmark |
| [NSCT-Xception](https://doi.org/10.4103/jmp.jmp_14_21) | 2021 | MRI, CT | NSCT, Xception image reconstruction | Imagefusion.org, AANLIB | API, EN, AG, MI, FS, CC, SF, RMSE, PSNR | Benchmark |
| [EMFusion](https://doi.org/10.1016/j.inffus.2021.06.001) | 2021 | CT, MRI, PET, SPECT | FusionNet, CNN | AANLIB | SSIM, PSNR, CC, VIF | Benchmark |
| [EOA Gabor energy](https://doi.org/10.1016/j.bspc.2021.102696) | 2021 | MRI-PET | DSWT, FR-MGE, EOA | AANLIB | ALI, CI, S, Q^AB/F, VIFF, FMI | Unclear |
| [BMGAN](https://doi.org/10.1109/tmi.2021.3107013) | 2021 | MRI-PET | 3D Dense-UNet, GAN | ADNI, OASIS-3, TCIA | MAE, PSNR, MS-SSIM, FID | Unclear |
| [3D CNN](https://doi.org/10.3233/ida-205113) | 2021 | MRI-fMRI-DTI | 3D-CNN | COBRE | ACC, SEN, SPE, AUC | Unclear |
| [DTNP-NSCT](https://doi.org/10.1016/j.sigpro.2020.107793) | 2021 | CT-MRI, MRI T1-T2, MRI-PET/SPECT | NSCT, INSML, WLE, DTNP | AANLIB | Petrovic, MI, FMI, SCD, MS-SSIM, SD | Unclear |
| [NSCT-CNN](https://doi.org/10.1016/j.eswa.2021.114574) | 2021 | CT-MRI, MRI multi-sequence | NSCT, CNN, PHF-CNN, FCN-8s | AANLIB | MI, SSIM, VIF, Q^AB/F | Unclear |
| [CBF-ANFIS](https://doi.org/10.4103/jmp.jmp_14_21) | 2021 | CT-MRI, MRI GAD-T2, CT-MR GAD, MR GAD-PET-FDG | CBF, ANFIS, DWT, Average Rule | AANLIB | API, AG, EN, MIF, FS, CC, SF, PSNR, Q^AB/F | Benchmark |
| [NSST-Co-LE](https://doi.org/10.1016/j.bspc.2021.102788) | 2021 | CT-MRI, MRI-PET | NSST, LE, CoF, MSS, SML, Max Selection | AANLIB | MI, SD, Q^AB/F, SF, EN | Benchmark |
| [DCT](https://doi.org/10.1109/wiecon-ece54711.2021.9829686) | 2021 | CT-MRI | DCT, DWT | Private | SNR, PSNR, MSE, AG, SD, EN | Unclear |
| [Aggregated NAS](https://doi.org/10.1145/3474085.3475299) | 2021 | MRI-PET | NAS, layered fusion | AANLIB | SD, EN, VIF, CC, SCD | Unclear |
| [DPCN](https://doi.org/10.1109/tci.2021.3083965) | 2021 | SPECT-MRI | CNN, SFFEB, FSFEB | AANLIB | MI, VIF, FMI, Q_P, Q_Y, time | Unclear |
| [MSRPAN](https://doi.org/10.1016/j.bspc.2021.102488) | 2021 | MRI-CT, MRI-PET, SPECT | CNN, MSRPAN, FER | AANLIB | Q_AC, SSIM, MI, PSNR, Q_AC, TMQI, FSIM, time | Unclear |
| [SDNet](https://doi.org/10.1007/s11263-021-01501-8) | 2021 | PET-MRI | SDNet, adaptive decision | AANLIB | EN, Q^AB/F, FMI, PSNR, MG, time, visual evaluation | Unclear |
| PPT fusion | 2021 | MRI-PET | Patch/Pyramid Transformer, MLP | AANLIB | EN, SSIM, MS-SSIM, MI, FMI, SCD, CC, SD, VIF, visual evaluation | Unclear |
| [IGNFusion](https://doi.org/10.1109/jstsp.2022.3181717) | 2022 | CT-MR T1, PET-MRI T2 | VGG-16, MSCAFM/MSCAFM, IGM, SSW | AANLIB | NMI, Q^AB/F, Q_Y, UQI | Unclear |
| [DB-NSCT](https://doi.org/10.1007/s13721-021-00342-2) | 2022 | CT-MRI, MRI-PET | NSCT, Davies-Bouldin | AANLIB | MI, SSIM, Q^AB/F | Unclear |
| [FDO](https://doi.org/10.1109/tmm.2022.3185887) | 2023 | MRI-PET | SVD, WMC, FDO, DPGF | AANLIB | AVG, MI, Q^AB/F, VIF, SSIM, PSNR | Unclear |
| [COVID-19 CNN](https://doi.org/10.1155/2022/6825576) | 2022 | CT-X ray | AlexNet, Vgg16, GoogLeNet | Private | ACC, SEN, SPEC, MCC, AUC | Unclear |
| [CRFNet](https://doi.org/10.1109/tcbb.2022.3178725) | 2024 | Acetic-acid–iodine colposcopy | Proposal shifting; corresponding channel attention | Private | Average precision | Unclear |
| [ST-cGAN](https://doi.org/10.1016/j.compbiomed.2022.105928) | 2022 | MRI T1-T2 | cGAN | IXI | PSNR, SSIM, FSIM, MMD | Unclear |
| [MUM-Net](https://doi.org/10.1109/jbhi.2022.3140236) | 2022 | MRI-US | MUM-Net, Disentangling modality features | Private | AUC, ACC, SENS, SPEC, PREC, Grad-CAM | Unclear |
| [ADSR](https://doi.org/10.1007/s00138-022-01322-w) | 2022 | MRI T2+FDG-PET, MRI T2+SPECT-TI/TC | Sparse Representation, PCA, K-SVD | AANLIB | EN, AG, MI, Q_W, Q^AB/F | Unclear |
| [IoMT-NSST](https://doi.org/10.1007/s11042-022-13507-6) | 2022 | CT-MRI, MRI-SPECT | NSST, MLE | AANLIB | MI, SD, Q^AB/F, SF, Mean, AG, CC, time | Benchmark |
| [MATR](https://doi.org/10.1109/tip.2022.3193288) | 2022 | CT-MRI, MRI-SPECT/PET | Multiscale adaptive Transformer, composed loss | AANLIB | MI, TE, NICE, G, P, CV, LMI, VIF, MS-SSIM | Unclear |
| [DualMMP-GAN](https://doi.org/10.1016/j.compbiomed.2022.105387) | 2022 | MRI T1-T2/FLAIR | DualMMP-GAN, GMMS | BraTS 2018 | PSNR, SSIM, RMSE, DSC, Sensitivity, Spesificity, HD95 | Benchmark |
| [MMRACR-Net](https://doi.org/10.1016/j.compbiomed.2022.106210) | 2022 | MRI DWI-ADC | MMRAM, CCM | Private | Acc, AUC, SEN, SPC | Unclear |
| TAUNet | 2022 | MRI bSSFP-LGE | CNN, Transformer, OCR | MyoPS 2020 | DSC, HD95 | Benchmark |
| [SwinFusion](https://doi.org/10.1109/jas.2022.105686) | 2022 | PET-MRI, CT-MRI | CNN, Swin Transformer, ACFM | AANLIB | FMI, Q^AB/F, SSIM, PSNR | Benchmark |
| DILRAN | 2022 | CT-MRI | CNN, DILRAN, Softmax | AANLIB | PSNR, SSIM, FSIM, MI, FMI, EN | Benchmark |
| IFT | 2022 | MRI-PET | Spatio-Transformer, RFN-Nest | AANLIB | EN, SCD, MI, MS-SSIM, SD, CC, MG | Unclear |
| [MRSCFusion](https://doi.org/10.1109/tim.2023.3317470) | 2023 | CT-MRI, PET-MRI, SPECT-MRI | Swin Transformer, CNN, RSCF, AWB | AANLIB | SCD, Q^AB/F, FMI, SF, VIF | Unclear |
| [DFENet](https://doi.org/10.1016/j.bspc.2022.104402) | 2023 | CT-MRI, PET-MRI, SPECT-MRI | CNN, Transformer, DFENet, GSFAM, LEGM | AANLIB | MI, FMI, NICE, SSIM, Q^AB/F, CV, Q_CB | Benchmark |
| [Hybrid Transformer](https://doi.org/10.1109/jbhi.2023.3264819) | 2023 | PET-MR, SPECT-MR | CNN, Transformer, self-adaptive weight fusion rule | AANLIB | MI, Q_P, Q_NICE, SSIM | Benchmark |
| [F²Net](https://doi.org/10.1109/jbhi.2023.3271808) | 2023 | MRI multi-sequence | Transformer, PVTv2, F²Net, CFM, MCM | BraTS 2019, BraTS 2020, ISLES 2015 SISS | DSC, IoU, HD95, Sen | Unclear |
| [Epsilon GFS](https://doi.org/10.1007/s12652-022-03764-6) | 2023 | CT-MRI | Shearlet Transform, Guided Filter, Max Selection, Average Rule | Public MRI-CT dataset | Q^AB/F, L_AB^F, N_AB^F, MAD, SD | Unclear |
| [U-Patch GAN](https://doi.org/10.1007/s10278-022-00696-7) | 2023 | SPECT TI-MRI T2, SPECT TC-MRI T2, CT-MRI T2, PET FDG-MRI T1 | PatchGAN, spectral norm | AANLIB | Q_G, Q_Q, FMI, SSIM, RMSE, MI | Unclear |
| ELF | 2023 | 2D Fundus-3D OCT | CNN, ELF | GAMMA | Acc, Cohen's Kappa | Benchmark |
| [AMTNet](https://doi.org/10.1088/1361-6560/aca74c) | 2023 | MRI T2-ADC, MRI T1-FLAIR | Transformer, CNN, AMTNet, R-MSA, AITF, 3D-CDS | BraTS 2021 | DSC, HD95, Jaccard, RVD | Benchmark |
| [DDFM](https://doi.org/10.1109/iccv51070.2023.00742) | 2023 | MRI-CT, MRI-PET, SPECT-MRI | DDPM, hierarchical Bayesian inference | AANLIB | EN, SD, MI, VIF, Q^AB/F, SSIM | Benchmark |
| [MSU-Net](https://doi.org/10.1016/j.compbiomed.2023.106956) | 2023 | MRI T1-T2-T1ce | U-Net, MSU-Net, SCIEM, MSFEM | AANLIB, private | DSC, PREC, Recall, IOU | Unclear |
| [CDDFuse](https://doi.org/10.1109/cvpr52729.2023.00572) | 2023 | MRI-CT, MRI-PET, MRI-SPECT | CNN, Restormer, INN, CDDFuse | AANLIB | EN, SD, SF, MI, SCD, VIF, Q^AB/F, SSIM | Benchmark |
| IE-CFRN | 2023 | CT-MRI T1/T2, MRI T1-GAD, MRI T1-PD, MRI-PET/SPECT TC /SPECT TI | CNN, GCIE, HFEN, LWEN | AANLIB | Q^AB/F, VIFP, IFC, NMI | Unclear |
| [CAE+MCIEN](https://doi.org/10.1109/mci.2022.3223487) | 2023 | CT-MRI T1/T2, MRI T1-T2, MRI T2-GAD, MRI T2-PD, MRI T2-PET/SPECT TC/SPECT TI | CNN, Vision Transformer, CAE, MCIEN | AANLIB | NMI, MI, FSIM, PC, GM, Q^AB/F, UIQI | Unclear |
| [3D THERMO-SCAN](https://doi.org/10.3390/s23031610) | 2023 | CT-Infrared | CNN, 3D THERMO-SCAN | Private | Registration error, visual evaluation | Unclear |
| [TUFusion](https://doi.org/10.1109/tcsvt.2023.3296745) | 2024 | Medical and other image domains; exact medical pairing unverified | CNN–Transformer encoder; composite attention | Medical subset not verified | PSNR, RMSE, SSIM | Unclear |
| [SSTFusion](https://doi.org/10.1109/jsen.2023.3263336) | 2023 | CT-MRI | LeWin Transformer, CNN, RSR pretext | AANLIB | MI, PSNR, Q^AB/F, SSIM, AG, EI, SF | Unclear |
| [ALMF-Net](https://doi.org/10.1109/tcsvt.2023.3342808) | 2024 | MRI-PET/CT/SPECT | NAS, DARTS, mask | AANLIB, BraTS 2021 | MI, CC, Q^AB/F, VIF, P, FLOP, L | Unclear |
| [MUFusion](https://doi.org/10.1016/j.inffus.2022.11.010) | 2023 | PET-MRI | VGG-19, memory unit | AANLIB | VIF, EN, MI, EI, Q^AB/F, MSSIM, DSC | Unclear |
| M3AE | 2023 | MRI T1-T2-T1ce-FLAIR | M³AE, self distillation, model inversion | BraTS 2018/2020 | DSC, HD95 | Benchmark |
| [FDGNet](https://doi.org/10.1016/j.bspc.2022.104545) | 2023 | CT-MRI, PET-MRI, SPECT-MRI | CNN, FDGNet | AANLIB | NMI, QY, Q^AB/F, VIF | Benchmark |
| [MURF](https://doi.org/10.1109/tpami.2023.3283682) | 2023 | PET-MRI, CT-MRI | Mutually reinforcing registration-fusion, Shared Information Extraction via contrastive learning, Multi-scale Coarse Registration | AANLIB | RMSE, MAE, MEE, NCC, MG, EI, VIF, SSIM, MI | Unclear |
| M4FNet | 2023 | CT-MRI, PET-MRI, SPECT-MRI | CNN, M4FNet | AANLIB, BraTS 2019 | EI, SD, Q^AB/F, MI, MSSIM, PC, VIF, UIQI | Unclear |
| FATFusion | 2024 | SPECT-MRI, PET-MRI | Transformer, FGTM, AGTM | AANLIB | NMI, QY, Q^AB/F, VIF, Chen-Blum | Unclear |
| MCF-Net | 2024 | MRI multi-sequence | ViT, mask align, sobel | BraTS 2020 | PSNR, SSIM, NMSE | Unclear |
| [MACTFusion](https://doi.org/10.1109/jbhi.2024.3391620) | 2025 | CT-MRI, PET-MRI, SPECT-MRI | ViT, CNN multi-axis attention | AANLIB | SCD, SD, MS-SSIM, Q^AB/F, VIF, Q_w | Unclear |
| [F-DARTS](https://doi.org/10.1109/tmi.2023.3283517) | 2023 | CT-MRI, MRI-PET, MRI-SPECT, multi-sequence MRI | Unsupervised differentiable architecture search, HVS-aligned kernel learning, unsupervised loss, channel attention in search space | AANLIB, BrainWeb, RIRE | MI, FMI_w, Q^AB/F, SCD, VIF, SD, Q_CB | Unclear |
| [ALYOLOv5](https://doi.org/10.1038/s41598-024-79786-1) | 2024 | PET-CT | YOLOv5, CFF , AAF | Private | Precision, recall, mAP, F1 | Unclear (single-center cohort) |
| [MGCNet](https://doi.org/10.1109/jbhi.2024.3350247) | 2024 | Multi-sequence MRI | Guided local feature fusion; cross-modal complementary external attention | Private | ACC, AUC, C-index, HR | Unclear |
| [EMMA](https://doi.org/10.1109/cvpr52733.2024.02448) | 2024 | MRI-CT, MRI-PET, SPECT-MRI | U-Net, Restormer, EMMA | AANLIB | EN, SD, SF, AG, SCD, VIF | Benchmark |
| [SRMNet](https://doi.org/10.1016/j.bspc.2024.106012) | 2024 | MRI multi-sequence | Missing-modality segmentation, Local-global feature enhancement, Deformation-Adaptive Perception fusion | BraTS 2018, BraTS 2020 | DSC, HD95 | Benchmark |
| [CoCoNet](https://doi.org/10.1007/s11263-023-01952-1) | 2024 | MRI-PET, MRI-SPECT | VGG, contrastive learning, CoCoNet | AANLIB | EN, AG, SF, SD, SCD, VIF | Benchmark |
| [ASFE-Fusion](https://doi.org/10.1016/j.bspc.2024.106478) | 2024 | CT-MRI, PET-MRI, SPECT-MRI | CNN, CASF, AFF, SFEF, FFT | AANLIB | EN, PSNR, MI, CC, FMI, Prec, Recall, F1, Acc | Unclear |
| [CA-DDPM](https://doi.org/10.1007/978-981-96-4229-8_34) | 2024 | MRI-CT | DDPM, CNN, Transformer | AANLIB | EN, MI, SCD, SSIM, VIF, Q^AB/F | Benchmark |
| [Diff-IF](https://doi.org/10.1016/j.inffus.2024.102450) | 2024 | MRI, CT, PET, SPECT | DDPM, prior knowledge, target search | AANLIB | MI, SCD, VIF, Q^AB/F, SSIM | Unclear |
| [TIEF](https://doi.org/10.1109/access.2024.3402965) | 2024 | MRI multi-sequence, SPECT-MRI, CT-MRI | CNN, SDCL, TIEF | BraTS 2019, AANLIB | Q^AB/F, EN, AG, SF, CI, MI, PSNR, SSIM, F | Unclear |
| Mambadfuse | 2024 | MRI-PET, MRI-SPECT | Mamba, CNN | AANLIB | EN, SD, SF, MI, SCD, VIF, Q^AB/F, SSIM, mAP, Grand-CAM, visual evaluation | Benchmark |
| Fuse4Seg | 2024 | MRI T1-FLAIR-T2-T1ce, MRI-CT/PET/SPECT | SwinUNet, dual-level optimization | BraTS 2021, AANLIB | EN, SD, SF, MI, SCD, VIF, Q^AB/F, DSC, mIoU, HD95, visual evaluation, attention heatmap | Benchmark |
| [MHFN](https://doi.org/10.1007/s11768-024-00231-9) | 2024 | MRI T1W–T2W-STIR | Hierarchical feature fusion with AGFM | Private | DSC, IoU, HD | Unclear (single-center cohort) |
| [CDE-Net](https://doi.org/10.1016/j.compmedimag.2024.102422) | 2024 | MRI T1-T2-FLAIR-T1ce | CDE-Net, DST, CDFL, RW-PAM | BraTS 2021 | DSC, HD95, visual evaluation | Unclear |
| [TIMFusion](https://doi.org/10.1109/tpami.2024.3382308) | 2024 | MRI-CT/PET/SPECT | Task guidance constraints, IAS, PMI | AANLIB | MI, FMI, VIF, Q^AB/F, EN, SCD, parameter, time | Benchmark |
| [LRFNet](https://doi.org/10.1016/j.compbiomed.2024.108381) | 2024 | MRI-PET, MRI-SPECT | LRU, FEF, DGSSIM | AANLIB | EN, SD, MI, AG, CC, SCD, Q^AB/F, SF | Unclear |
| [CMINet](https://doi.org/10.1109/tce.2024.3412879) | 2025 | CT-MRI, MRI-PET, MRI-SPECT | Transformer, CNN, GDA/GADN | AANLIB | MI, SF, VIF, Q^AB/F | Unclear |
| [PDMINet](https://doi.org/10.1109/tim.2024.3500067) | 2025 | MRI multi-sequence | Prototype-driven + multiexpert integration | BraTS 2018, BraTS 2019, BraTS 2020 | DSC, HD95, Sensitivity, Specificity | Unclear |
| [GeSeNet](https://doi.org/10.1109/tnnls.2023.3293274) | 2024 | CT-MRI, MRI-PET, MRI-SPECT | Semantic-guided fusion, edge enhancement gradient filter, region mask for redundant computation pruning | AANLIB | SSIM, SD, MI, VIF, SCD, Q^AB/F | Unclear |
| [DRMF](https://doi.org/10.1145/3664647.3681064) | 2024 | CT-MRI, MRI-PET, SPECT-MRI | Degradation-robust conditional diffusion, fusion + regularization + mask-guided loss | AANLIB | MI, SF, SD, VIF, SSIM, PSNR, MUSIQ, LIQE, mAP | Unclear |
| [TFEFusion](https://doi.org/10.1016/j.bspc.2025.107748) | 2025 | PET, MRI | CNN, Swin Transformer, TFEFusion | AANLIB | G, SSIM, Q^AB/F, PSNR, SF, RMSE | Benchmark |
| [LAGN Diffusion](https://doi.org/10.1007/s11517-025-03300-6) | 2025 | MRI-CT, MRI-PET, MRI-SPECT | Diffusion, Transformer, CNN | AANLIB | EN, SD, SCD, VIF, PSNR, SSIM | Benchmark; Reader study (student ratings) |
| [PFRFusion](https://doi.org/10.1016/j.knosys.2025.113427) | 2025 | CT-MRI, MRI T1-T2 | PFAR, DBFF, co-training | AANLIB, Synth-Strip | MAE, NMI, MEE, MI, VIF, SSIM, IMF, SF, DSC, IoU, MPA | Unclear |
| [EFCNet](https://doi.org/10.1007/s11227-025-07601-3) | 2025 | MRI-SPECT, MRI-PET | EFCNet, SEEM, MSAM, E-Fusion, IRM | AANLIB | AG, SNR, MI, Q^AB/F, VIF, PSNR, EI, SF | Unclear |
| DTMFusion | 2025 | CT-MRI, MRI T1-T2 | Transformer, Mamba, DTSDR, MCF | AANLIB, Synth-Strip | PSNR, NCC, MSE, SD, MI, VIF, SCD | Unclear |
| [EDPSN](https://doi.org/10.1016/j.inffus.2025.103312) | 2025 | MRI-CT, MRI-PET, SPECT-MRI | EDPSN, EEM, ED, DPS, VGG16 | AANLIB, CHAOS | EN, SD, SCD, Q^AB/F, VIF, PSNR, SSIM | Benchmark; Unclear (reader protocol) |
| [AAHN](https://doi.org/10.1109/tmi.2025.3526604) | 2025 | PET-CT, MRI T1-FLAIR -DWI-ADC, CT-MRI | CNN, Transformer, GCN | Hecktor21, Prostate158, BraTS 2019/2023/2024, CHAOS | DSC, HD95 | Unclear |
| [MLFuse](https://doi.org/10.1109/tmm.2025.3535355) | 2025 | CT-MRI, PET-MRI, SPECT-MRI | CNN, Transformer, sobel | AANLIB | VIF, SCD, Q^AB/F, SSIM, FMI | Unclear |
| [DMCMFuse](https://doi.org/10.1016/j.displa.2025.103056) | 2025 | CT-MRI, MRI T1-T2, MRI-PET/SPECT | CNN, Mamba, MCFM, HAED | AANLIB | SSIM, VIFF, Q^AB/F, SCD, FMI, Q_w | Unclear |
| [FAB-Transformer](https://doi.org/10.1038/s41598-025-92054-0) | 2025 | PET-MRI, SPECT-MRI | CNN, Swin Transformer, DSM, INN | AANLIB | MI, SF, VIF, Q^AB/F, SSIM, mAP | Benchmark |
| [AdvTCUnet](https://doi.org/10.1016/j.eswa.2025.127467) | 2025 | 3D MRI T1-T1ce-FLAIR | Adversarial learning, Transformer, U-Net, CV energy function | TCIA | DSC, HD, visual evaluation | Benchmark |
| [MTG-Fusion](https://doi.org/10.1007/s11263-025-02409-3) | 2025 | CT-MRI, PET-MRI, SPECT-MRI | Auxiliary text guidance, image-feature fusion | AANLIB | EN, SD, SF, SCD, VIF, Q | Unclear |
| MAINet | 2025 | MRI-CT, MRI-PET, MRI-SPECT | CMI, DGL, BUGF | AANLIB | MI, Q_NCIE, SD, VIF, Q^AB/F, SSIM, Q_CB, visual evaluation | Unclear |
| [Uncertainty-seg](https://doi.org/10.1109/nnice64954.2025.11064419) | 2025 | MRI FLAIR-T2 | MC-Dropout, uncertainty weighting | BraTS subset | DSC, IoU, SE, PPV, uncertainty | Unclear |
| [BSAFusion](https://doi.org/10.1609/aaai.v39i5.32499) | 2025 | Misaligned CT-MRI, PET-MRI | MDF-FR, BSFA, MMFF | AANLIB | Q^AB/F, Q_CV, SSIM, VIF, Q_S, visual evaluation | Benchmark |
| UniFuse | 2025 | MRI T1-T2/CT, CT-PET | Spatial Mamba, LoRA, DAPL, OUFR | BraTS 2020, SynthRAD2023, FDG-PET/CT | MSE, CC, PSNR, VIF, SSIM, GFLOP, visual evaluation | Unclear |
| [ReFusion](https://doi.org/10.1007/s11263-024-02256-8) | 2025 | CT-MRI, MRI-PET | Meta-learning, learnable fusion loss, inner-outer-alternate training strategy | AANLIB | EN, SD, SF, AG, SCD, SSIM, VIF, Q_\textCB, Q_\textNCIE | Benchmark |
| [DM-FNet](https://doi.org/10.1109/tmm.2025.3613156) | 2025 | CT-MRI, MRI-PET, MRI-SPECT | Two-stage diffusion hybrid loss (intensity + SSIM + gradient) | AANLIB | SF, SD, AG, Q_\textW, SCD, VIFF, Q^AB/F, MSSSIM, FMI-WT | Unclear |
| [C2RF](https://doi.org/10.1007/s11263-025-02427-1) | 2025 | PET-MRI | Mutually promoting registration-fusion, commonality mining for feature disentanglement, multi-level registration, contrastive learning with hard negative sample mining | AANLIB | MI, CC, SSIM, MSE, MEE, MAE, EN, MI, SF, VIF, Q^AB/F, SSIM | Unclear |
| [HCFMaNet](https://doi.org/10.1109/tmm.2026.3660130) | 2026 | CT-MRI, PET-MRI, SPECT-MRI, MRI multi-sequence | Local-aware Mamba, Holistic Cross-modal Fusion Mamba, end-to-end unsupervised fusion | AANLIB, BrainWeb, SynthRAD | Q_\textNCIE, MI, Q_\textG, Q_\textCV, LMI, MS-SSIM, VIF, NCC, SSIM | Unclear |
| [FlexiD-Fuse](https://doi.org/10.1016/j.eswa.2025.128895) | 2026 | CT-MRI, MRI-PET, MRI-SPECT, MR-T2/MR-Gad/PET, CT/MR-T2/SPECT | Diffusion model + hierarchical Bayesian modeling, Expectation-Maximization, ultra-lightweight Diffusion Fusion Mamba | AANLIB | SSIM, MI, PSNR, VIF, Q_\textS, Q_\textCV, FSIM, Q_\textNCIE | Benchmark |

The same records are available as CSV in `table4_feature_level.csv`.
