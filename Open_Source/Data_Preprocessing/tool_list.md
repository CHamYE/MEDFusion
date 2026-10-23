# Preprocessing Tools

Preprocessing determines whether a fusion result is meaningful. Registration error, intensity mismatch and inconsistent orientation propagate into every downstream metric.

| Tool | Role | Input to output | License | Link |
|---|---|---|---|---|
| SimpleITK | Registration and resampling | Images and masks to aligned images and transforms | Apache 2.0 | https://simpleitk.org/ |
| ANTs | Registration and bias correction | Image volumes to affine transforms and deformation fields | Apache 2.0 | https://github.com/ANTsX/ANTs |
| 3D Slicer | Inspection and ROI editing | Volumes, labels and transforms to scenes and masks | BSD-style | https://www.slicer.org/ |
| MONAI | Medical-image transforms and loading | Images and metadata to transformed tensors | Apache 2.0 | https://github.com/Project-MONAI/MONAI |
| TorchIO | Patch sampling and augmentation | Subject images and labels to transformed volumes and patches | Apache 2.0 | https://github.com/TorchIO-project/torchio |

## Minimum record for a preprocessing step

State the registration method and its parameters, the resampling grid and spacing, the intensity normalization, and whether augmentation was applied before or after splitting. Without these, a reported fusion score cannot be reproduced even with the same code.

## Common failure

Applying augmentation before the train/test split leaks subject identity across splits. For paired modalities, any spatial transform must be applied identically to both sources and to the label.
