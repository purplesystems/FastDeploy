# ⚡️FastDeploy

</p>

------------------------------------------------------------------------------------------

<p align="center">
    <a href="./LICENSE"><img src="https://img.shields.io/badge/license-Apache%202-dfd.svg"></a>
    <a href="https://github.com/PaddlePaddle/FastDeploy/releases"><img src="https://img.shields.io/github/v/release/PaddlePaddle/FastDeploy?color=ffa"></a>
    <a href=""><img src="https://img.shields.io/badge/python-3.7+-aff.svg"></a>
    <a href=""><img src="https://img.shields.io/badge/os-linux%2C%20win%2C%20mac-pink.svg"></a>
    <a href="https://github.com/PaddlePaddle/FastDeploy/graphs/contributors"><img src="https://img.shields.io/github/contributors/PaddlePaddle/FastDeploy?color=9ea"></a>
    <a href="https://github.com/PaddlePaddle/FastDeploy/commits"><img src="https://img.shields.io/github/commit-activity/m/PaddlePaddle/FastDeploy?color=3af"></a>
    <a href="https://pypi.org/project/FastDeploy-python/"><img src="https://img.shields.io/pypi/dm/FastDeploy-python?color=9cf"></a>
    <a href="https://github.com/PaddlePaddle/FastDeploy/issues"><img src="https://img.shields.io/github/issues/PaddlePaddle/FastDeploy?color=9cc"></a>
    <a href="https://github.com/PaddlePaddle/FastDeploy/stargazers"><img src="https://img.shields.io/github/stars/PaddlePaddle/FastDeploy?color=ccf"></a>
</p>


<h4 align="center">
  <a href=#特性> 特性 </a> |
  <a href=#SDK安装> 安装 </a> |
  <a href=#SDK使用> 快速开始 </a> |
  <a href=#社区交流> 社区交流 </a>
</h4>

**⚡️FastDeploy** FastDeployis an easy-to-use inference deployment toolbox. It covers the mainstream high-quality pre-trained models in the industry and provides out-of-the-box development experience, including image classification, object detection, image segmentation, face detection, human body key point recognition, text recognition and other multi-tasking, to meet the rapid deployment needs of developers in multiple scenarios, multi-hardware and multi-platform.

## News 📢

* 🔥 2022.6.30 晚20:30，⚡️FastDeploy angel users invite test communication meetings, discuss the pain points of reasoning deployment with developers, and welcome everyone to scan the code to sign up for the conference link.。
<div align="center">
<img src="https://user-images.githubusercontent.com/54695910/175854075-2c0f9997-ed18-4b17-9aaf-1b43266d3996.jpeg"  width = "150" height = "150" />
</div>

* 🔥 2022.6.27 [**⚡️FastDeploy v0.1.0**](https://github.com/PaddlePaddle/FastDeploy/releases/tag/release%2F0.1.0)Beta release! 🎉
  * 💎 Released 40 key models supported SDKs in 8 key hardware and software environments
  * 😊 Supports two ways to download and use web pages and pip packages


## About


### 📦**Out-of-the-box inference deployment toolchain, supporting cloud-edge, multi-hardware, and multi-platform deployments**
- Click download and PIP install a single line command for the web terminal to quickly download various types of SDK installation packages
- Cloud (including servers, data centers):
    - Supports one-line command to start Serving service (including graphical display of web pages)
    - Supports one-line command to start image, local video stream, local camera, network video stream prediction
    - Supports Window, Linux operating systems
    - Support for Python, C++ programming languages
- Edge end:
    - Support for edge devices such as NVIDIA Jetson and support for video stream prediction services
- End side (including mobile end)
    - Support iOS, Android mobile terminal
    - Support for ARM CPU side-side devices
    - Supports mainstream hardware
    - Support for Intel CPU series (including Core, Xeon, etc.)
    - Supports the entire range of ARM CPUs (including Qualcomm, MTK, RK, etc.)
    - Supports the full range of NVIDIA GPUs (including V100, T4, Jetson, etc.)

### 🤗**Rich pre-trained models, easy to download SDK to get the inference deployment**


<font size=0.5>

|<font size=2>   model| <font size=2> Task  |<font size=2>  Size(MB)  | <font size=2>End | <font size=2>Mobile |<font size=2> Mobile |<font size=2>Edge |<font size=2>Server+Cloud | <font size=2>Server+Cloud |<font size=2> Server+Cloud |<font size=2> Server+Cloud |
|---|---|---|---|---|---|---|---|---|---|---|
|----- | ---- |----- |<font size=2>  Linux | <font size=2> Android |<font size=2>  iOS | <font size=2> Linux |<font size=2> Linux |<font size=2> Linux |<font size=2>  Windows  |<font size=2>  Windows  |
|----- | ---- |--- | <font size=2> ARM CPU |<font size=2>  ARM CPU | <font size=2> ARM CPU |<font size=2> Jetson |<font size=2> X86 CPU |<font size=2>  GPU  |<font size=2> X86 CPU |<font size=2>  GPU  |
| <font size=2> [PP-LCNet](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 11.9 |✅|✅|✅|✅|✅|✅|✅|✅|
| <font size=2> [PP-LCNetv2](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 26.6 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [EfficientNet](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication |31.4 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [GhostNet](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 20.8 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [MobileNetV1](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 17 |✅|✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [MobileNetV2](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 14.2 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [MobileNetV3](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 22 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [ShuffleNetV2](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md)|Classfication | 9.2 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [SqueezeNetV1.1](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication |5 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [Inceptionv3](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication |95.5 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [PP-HGNet](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 59 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [ResNet50_vd](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 102.5 |❌|❌|❌|✅|✅|✅|✅|✅|
|<font size=2>  [SwinTransformer_224_win7](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 352.7 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [PP-PicoDet_s_320_coco](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 4.1 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [PP-PicoDet_s_320_lcnet](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 4.9 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [CenterNet](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection |4.8 |✅|✅|✅|✅ |✅ |✅|✅|✅|
|<font size=2>  [YOLOv3_MobileNetV3](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 94.6 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [PP-YOLO_tiny_650e_coco](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection |4.4 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [SSD_MobileNetV1_300_120e_voc](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 23.3 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [YOLOX_Nano_300e_coco](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 3.7 |❌|❌|❌|✅|✅ |✅|✅|✅|
|<font size=2> [PP-YOLO_ResNet50vd](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 188.5|✅ |✅ |✅ |✅ |✅ |✅|✅|✅|
|<font size=2>  [PP-YOLOv2_ResNet50vd](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 218.7 |✅|✅|✅|✅|✅ |✅|✅|✅|
|<font size=2>  [PP-YOLO_crn_l_300e_coco](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 209.1 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2> [YOLOv5s](https://github.com/ultralytics/yolov5) |Detection | 29.3|✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [Faster R-CNN_r50_fpn_1x_coco](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 167.2 |❌|❌|❌|✅|✅|✅|✅|✅|
|<font size=2> [BlazeFace](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Face Detection |1.5|✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2> [RetinaFace](https://github.com/biubug6/Pytorch_Retinaface) |Face Localisation |1.7| ✅|❌|❌|✅|✅|✅|✅|✅|
|<font size=2>  [PP-TinyPose](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Keypoint Detection| 5.5 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2> [PP-LiteSeg(STDC1)](https://github.com/PaddlePaddle/PaddleSeg/blob/develop/configs/pp_liteseg/README.md)|Segmentation | 32.2|✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [PP-HumanSeg-Lite](https://github.com/PaddlePaddle/PaddleSeg/blob/develop/contrib/PP-HumanSeg/README_cn.md) |Segmentation | 0.556|✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [HRNet-w18](https://github.com/PaddlePaddle/PaddleSeg/blob/develop/docs/train/train_cn.md) |Segmentation | 38.7|✅|✅|✅|❌|✅|✅|✅|✅|
|<font size=2> [Mask R-CNN_r50_fpn_1x_coco](https://github.com/PaddlePaddle/PaddleSeg/blob/develop/contrib/PP-HumanSeg/README_cn.md)|Segmentation| 107.2|❌|❌|❌|✅|✅|✅|✅|✅|
|<font size=2> [PP-HumanSeg-Server](https://github.com/PaddlePaddle/PaddleSeg/blob/develop/contrib/PP-HumanSeg/README_cn.md)|Segmentation | 107.2|✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2> [Unet](https://github.com/PaddlePaddle/PaddleSeg/blob/develop/docs/train/train_cn.md) |Segmentation | 53.7|❌|✅|❌|❌|✅|✅|✅|❌|
|<font size=2> [Deeplabv3-ResNet50](https://github.com/PaddlePaddle/PaddleSeg/blob/develop/docs/train/train_cn.md)|Segmentation |156.5|❌|❌|❌|❌|✅|✅|✅|✅|
|<font size=2>  [PP-OCRv1](https://github.com/PaddlePaddle/PaddleOCR/blob/release%2F2.5/doc/doc_ch/ppocr_introduction.md) |OCR | 2.3+4.4 |✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [PP-OCRv2](https://github.com/PaddlePaddle/PaddleOCR/blob/release%2F2.5/doc/doc_ch/ppocr_introduction.md) |OCR | 2.3+4.4 |✅|✅|✅|✅|✅|✅|✅|✅|
| <font size=2> [PP-OCRv3](https://github.com/PaddlePaddle/PaddleOCR/blob/release%2F2.5/doc/doc_ch/PP-OCRv3_introduction.md) |OCR | 2.4+10.6 |✅|✅|✅|✅|✅|✅|✅|✅|
| <font size=2> [PP-OCRv3-tiny](https://github.com/PaddlePaddle/PaddleOCR/blob/release%2F2.5/doc/doc_ch/models_list.md) |OCR |2.4+10.7 |✅|✅|✅|✅|✅|✅|✅|✅|
</font>


## SDK Installation

### Method 1: Download and install the web version

- Log In to [EasyEdge网页端](https://ai.baidu.com/easyedge/app/openSource) to download SDK

### Mode 2: pip installation

Developers can get the latest download links through pip installation `fastdeploy-python`

- Environment dependencies

    python >= 3.6  

- Installation mode

```
pip install fastdeploy-python --upgrade
```

- 使用方式

    - Lists all models currently supported by FastDeploy
    ```
    fastdeploy --list_models
    ```
    - Download the model's deployment SDK on specific platforms and corresponding hardware, as well as examples
    ```
    fastdeploy --download_sdk \
               --model PP-PicoDet-s_320 \
               --platform Linux \
               --soc x86 \
               --save_dir .
    ```

    - Parameter description
        - `list_models`: Lists all models currently supported by FastDeploy
        - `download_sdk`: Download the sdk and examples of the model's deployment on specific platforms and corresponding hardware
        - `model`: Model name, such as "PP-PicoDet-s_320", can be viewed by viewing all the optionslist_models
        - `platform`: Deployment platform with support for Windows/Linux/Android/iOS
        - `soc`: Deploy hardware with x86/x86-NVIDIA-GPU/ARM/Jetson support
        - `save_dir`: SDK download and save directory

## SDK Usage
### 1 Cloud + server deployment
- Linux systems (X86 CPUs, NVIDIA GPUs)
    - C++ Inference deployment (with video streaming)
    - C++ serviced deployment
    - Python Inference deployment
    - Python serviced deployment
- Window System (X86 CPU, NVIDIA GPU)
    - C++ Inference deployment (with video streaming)
    - C++ serviced deployment
    - Python Inference deployment
    - Python serviced deployment
2 Edge-side deployment
- ArmLinux system (NVIDIA Jetson Nano/TX2/Xavier)
    - C++ Inference deployment (with video streaming)
    - C++ serviced deployment
3-side deployment
- ArmLinux System (ARM CPU)
    - C++ Inference deployment (with video streaming)
    - C++ serviced deployment
    - Python Inference deployment
    - Python serviced deployment
4 Mobile deployment
- iOS system deployment
- Android system deployment
5 Custom model deployment
- Quickly implement personalized model replacement

## Community communication
   - Join the community👬： After Scanning the QR code on WeChat, fill in a questionnaire to join the communication group and discuss the pain points of reasoning deployment with developers

<div align="center">
<img src="https://user-images.githubusercontent.com/54695910/175854075-2c0f9997-ed18-4b17-9aaf-1b43266d3996.jpeg"  width = "200" height = "200" />
</div>



## Acknowledge

本项目中SDK生成和下载使用了[EasyEdge](https://ai.baidu.com/easyedge/app/openSource)中的免费开放能力，再次表示感谢。

## License

FastDeploy follows the [Apache-2.0 Open Source License](./LICENSE)。
