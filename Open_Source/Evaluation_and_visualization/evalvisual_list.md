# Evaluation Metrics for Multi-Modality Medical Image Fusion
## 📌 Overview
Evaluation metrics are the core basis for quantitatively comparing the performance of different MMIF methods. They are mainly divided into two categories: **full-reference metrics** (with source images as reference) and **no-reference metrics** (without reference images). In addition, for fusion methods for downstream tasks, the performance improvement of downstream tasks (segmentation, detection, diagnosis) is also an important clinical evaluation indicator.

This section systematically sorts out the commonly used evaluation metrics in the MMIF field, with detailed information such as metric definition, core function, and value trend (better when larger/smaller).

## 📑 Curated List of Evaluation Metrics
### 1. Full-Reference Metrics (Most Commonly Used)
| Metric Full Name | Abbreviation | Core Definition & Function | Value Trend |
|-------------------|--------------|------------------------------|-------------|
| Structural Similarity Index Measure | SSIM | Evaluates the structural consistency between the fused image and the source images from three dimensions: brightness, contrast, and structure. It is the most commonly used metric to measure the structural retention of fused images. | Larger is better (0~1) |
| Peak Signal-to-Noise Ratio | PSNR | Measures the pixel-level distortion between the fused image and the source images, reflecting the noise level of the fused image. | Larger is better (unit: dB) |
| Mutual Information | MI | Quantifies the amount of information transferred from the source images to the fused image, reflecting the degree of information retention of the fused image. | Larger is better |
| Visual Information Fidelity | VIF | Evaluates the visual information fidelity of the fused image based on the human visual system (HVS), which is highly consistent with the subjective evaluation of clinicians. | Larger is better |
| Edge Preservation Index | Q_abf / Q_AB/F | Calculates the degree of edge information transfer from the source images to the fused image, reflecting the retention of pathological edges and tissue boundaries in the fused image. | Larger is better (0~1) |
| Correlation Coefficient | CC | Measures the linear correlation between the fused image and the source images, reflecting the consistency of the overall intensity distribution. | Larger is better (0~1) |
| Feature Similarity Index Measure | FSIM | Evaluates the similarity between the fused image and the source images based on phase consistency and gradient amplitude, focusing on the retention of feature-level information. | Larger is better (0~1) |
| Difference Correlation Sum | SCD | Quantifies the correlation between the difference of the fused image and each source image, reflecting the complementary information integration ability of the fusion method. | Larger is better |

### 2. No-Reference Metrics
| Metric Full Name | Abbreviation | Core Definition & Function | Value Trend |
|-------------------|--------------|------------------------------|-------------|
| Entropy | EN / Ent | Measures the amount of information contained in the fused image based on information theory. The higher the entropy, the richer the details and information of the fused image. | Larger is better |
| Standard Deviation | SD | Reflects the discrete degree of the gray value of the fused image, and the larger the SD, the higher the contrast of the fused image. | Larger is better |
| Average Gradient | AG / MG | Evaluates the richness of texture details of the fused image by calculating the average gradient of the image, reflecting the clarity of the fused image. | Larger is better |
| Spatial Frequency | SF | Measures the gray change rate of the fused image in the spatial domain, reflecting the richness of edge and texture details. | Larger is better |

### 3. Downstream Task Evaluation Metrics (Clinical-Oriented)
| Metric Full Name | Abbreviation | Core Definition & Function | Applicable Downstream Task | Value Trend |
|-------------------|--------------|------------------------------|-----------------------------|-------------|
| Dice Similarity Coefficient | DSC / Dice | Measures the overlap between the segmentation result based on the fused image and the ground truth, reflecting the accuracy of tumor/organ segmentation. | Medical Image Segmentation | Larger is better (0~1) |
| Intersection over Union | IoU | Calculates the intersection over union between the predicted segmentation area and the ground truth, which is a core metric for segmentation performance evaluation. | Medical Image Segmentation | Larger is better (0~1) |
| 95th Percentile Hausdorff Distance | HD95 | Measures the maximum distance between the boundary of the segmentation result and the ground truth (95th percentile to suppress outliers), reflecting the boundary alignment accuracy. | Medical Image Segmentation | Smaller is better (unit: mm) |
| Average Symmetric Surface Distance | ASD | Calculates the average distance between the surfaces of the segmentation result and the ground truth, reflecting the overall surface proximity. | Medical Image Segmentation | Smaller is better (unit: mm) |
| Mean Average Precision | mAP | Measures the accuracy of target detection based on the fused image, reflecting the ability of the fused image to assist lesion localization. | Lesion Detection | Larger is better (0~1) |
| Area Under the Curve | AUC | Evaluates the performance of disease diagnosis based on the fused image, reflecting the diagnostic accuracy. | Clinical Diagnosis | Larger is better (0~1) |
