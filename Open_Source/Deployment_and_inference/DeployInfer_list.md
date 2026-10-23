# Deployment and Inference Tools

| Tool | Role | Input to output | License | Link |
|---|---|---|---|---|
| [ONNX](https://github.com/onnx/onnx) | Model exchange format | Supported model graph to portable graph file | Apache 2.0 | https://github.com/onnx/onnx |
| [TensorRT](https://developer.nvidia.com/tensorrt) | GPU inference optimization | Supported model to optimized engine | NVIDIA SDK terms | https://developer.nvidia.com/tensorrt |
| [OpenVINO](https://github.com/openvinotoolkit/openvino) | CPU/edge inference | Converted model to runtime outputs | Apache 2.0 | https://github.com/openvinotoolkit/openvino |
| [MONAI Deploy App SDK](https://github.com/Project-MONAI/monai-deploy-app-sdk) | Clinical application packaging | Operators and models to packaged application | Apache 2.0 | https://github.com/Project-MONAI/monai-deploy-app-sdk |
| [Docker Engine](https://docs.docker.com/engine/) | Environment packaging | Build recipe to container image | Apache 2.0 | https://docs.docker.com/engine/ |

## Minimum record

State the target hardware, the batch size, the precision (FP32/FP16/INT8), and the measured latency distribution rather than a single best-case number. A model that meets a frame-rate target on a workstation may not run on a clinical console.
