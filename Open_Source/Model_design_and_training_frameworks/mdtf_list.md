# Model Design and Training Frameworks

| Framework | Role | Typical use | License | Link |
|---|---|---|---|---|
| [PyTorch](https://github.com/pytorch/pytorch) | Tensor and autograd framework | Implementing fusion architectures, losses and inference | BSD-3-Clause | https://github.com/pytorch/pytorch |
| [PyTorch Lightning](https://github.com/Lightning-AI/pytorch-lightning) | Training loop organization | Scaling training and logging across devices | Apache 2.0 | https://github.com/Lightning-AI/pytorch-lightning |
| [TensorFlow / Keras](https://www.tensorflow.org/) | Alternative framework | Reproducing models released in TensorFlow | Apache 2.0 | https://www.tensorflow.org/ |
| [MONAI](https://github.com/Project-MONAI/MONAI) | Medical-image operators | Loading, transforms and network blocks for 3D data | Apache 2.0 | https://github.com/Project-MONAI/MONAI |
| [MATLAB Image Processing Toolbox](https://www.mathworks.com/products/image-processing.html) | Reference implementations | Traditional fusion operators and metric checks | Commercial | https://www.mathworks.com/products/image-processing.html |

## What to record

Record the framework and version, the random seed policy, the number of runs, and whether the reported number is a single run or a mean over seeds. Fusion papers often report one run; that is acceptable only if stated.
