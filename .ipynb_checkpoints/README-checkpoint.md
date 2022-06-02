# FastDeploy

**简体中文**🀄 | [English🌎](./README_en.md)

</p>

------------------------------------------------------------------------------------------

<p align="center">
    <a href="./LICENSE"><img src="https://img.shields.io/badge/license-Apache%202-dfd.svg"></a>
    <a href="https://github.com/PaddlePaddle/FastDeploy/releases"><img src="https://img.shields.io/github/v/release/PaddlePaddle/FastDeploy?color=ffa"></a>
    <a href=""><img src="https://img.shields.io/badge/python-3.6.2+-aff.svg"></a>
    <a href=""><img src="https://img.shields.io/badge/os-linux%2C%20win%2C%20mac-pink.svg"></a>
    <a href="https://github.com/PaddlePaddle/FastDeploy/graphs/contributors"><img src="https://img.shields.io/github/contributors/PaddlePaddle/FastDeploy?color=9ea"></a>
    <a href="https://github.com/PaddlePaddle/FastDeploy/commits"><img src="https://img.shields.io/github/commit-activity/m/PaddlePaddle/FastDeploy?color=3af"></a>
    <a href="https://pypi.org/project/FastDeploy/"><img src="https://img.shields.io/pypi/dm/FastDeploy?color=9cf"></a>
    <a href="https://github.com/PaddlePaddle/FastDeploy/issues"><img src="https://img.shields.io/github/issues/PaddlePaddle/FastDeploy?color=9cc"></a>
    <a href="https://github.com/PaddlePaddle/FastDeploy/stargazers"><img src="https://img.shields.io/github/stars/PaddlePaddle/FastDeploy?color=ccf"></a>
</p>


<h4 align="center">
  <a href=#特性> 特性 </a> |
  <a href=#安装> 安装 </a> |
  <a href=#快速开始> 快速开始 </a> |
  <a href=#api文档> API文档 </a> |
  <a href=#社区交流> 社区交流 </a>
</h4>

**FastDeploy**是一款**简单易用**的推理部署工具箱。覆盖业界主流**优质预训练模型**并提供**开箱即用**的开发体验，包括[图像分类]()、[目标检测]()、[图像分割]()、[人脸检测]()、[文字识别]()等多任务，覆盖**云、边、端**多场景，多硬件、多部署环境要求，可满足开发者**快速部署**的需求。

## News 📢

* 🔥 2022.6.22 B站[飞桨直播课](https://space.bilibili.com/476867757)，FastDeploy首发，手把手入门快速部署能力


* 🔥 2022.6.20 [**FastDeploy v0.1**](https://github.com/PaddlePaddle/FastDeploy/releases/tag/v0.1)全新发布！🎉
  * 💎 第一批发布对于40个重点模型在8种重点软硬件环境的支持
  * 😊 支持网页端、pip包两种使用方式


## 特性

#### <a href=#开箱即用的推理部署工具集> 📦 开箱即用的推理部署工具集 </a>

#### <a href=#覆盖丰富的预训练模型> 🤗 覆盖丰富的预训练模型 </a>

#### <a href=#支持云边端、多硬件、多操作系统部署> 🎛️ 支持云边端、多硬件、多操作系统部署 </a>



### 开箱即用的推理部署工具集


<p align="center">
  <img src="./docs/imgs/paddlenlp.png" align="middle"  width="500" />
</p>
home/FastDeploy/docs/pictures/easytouse.png


### 覆盖丰富的预训练模型


<font size=0.5>

|<font size=2>   model name| <font size=2> Type |<font size=2>  Size/MB |<font size=2>  Speed |<font size=2>  Jetson | <font size=2> X86 CPU |<font size=2>  X86 CPU | <font size=2> Nvidia GPU |<font size=2> Nvidia GPU |<font size=2> ARM CPU |<font size=2>  ARM CPU  |<font size=2>  ARM CPU  |
|---|---|---|---|---|---|---|---|---|---|---|---|
|----- | ---- |---|----- |<font size=2> Linux | <font size=2>Windows | <font size=2>Linux |<font size=2> Windows |<font size=2>Linux |<font size=2>IOS | <font size=2>Android |<font size=2> Linux |
| <font size=2> [PP-LCNetv1](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 11.9 |---|✅|✅|✅|✅|✅|✅|✅|✅|
| <font size=2> [PP-LCNetv2](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 26.6 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [EfficientNet](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication |31.4 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [GhostNet](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 20.8 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [MobileNetv1](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 17 |---|✅|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [MobileNetv2](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 14.2 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [MobileNetv3](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 22 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [ShuffleNetv2](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md)|Classfication | 9.2 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [SqueezeNetv1.1](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication |5 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [Inceptionv3](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication |95.5 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [PP-HGNet](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 59 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [ResNet50](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 102.5 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [Swin-Transform](https://github.com/PaddlePaddle/PaddleClas/blob/release/2.3/docs/zh_CN/models_training/classification.md) |Classfication | 352.7 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [Picodet_s_320_coco](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 4.1 |---|✅|✅|✅|✅|✅|✅|✅|✅|
|<font size=2>  [Picodet_s_320lcnet](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 4.9 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [TinyPose](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 5.5 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [CenterNet](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection |4.8 |---|✅|✅|✅|✅ |✅ |/|/|/|
|<font size=2>  [Yolov3_Mobilenet_v3](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 94.6 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [ppyolo_tiny_650e_coco](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection |4.4 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [ssd_mobilenet_v1_300_120e_voc](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 23.3 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [yolox_nano](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 3.7 |---|✅|✅|✅|✅|✅ |/|/|/|
|<font size=2> [ppyolo_ResNet50vd](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 188.5|—|✅ |✅ |✅ |✅ |✅ |/|/|/|
|<font size=2>  [ppyolov2_ResNet50vd](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 218.7 |---|✅|✅|✅|✅|✅ |/|/|/|
|<font size=2>  [ppyoloe_crn_l_300e_coco](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 209.1 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [faster_rcnn_r50_fpn_1x_coco](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 167.2 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [mask_rcnn_r50_fpn_1x_coco](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Detection | 177.8 |---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2> [yolov5s](https://github.com/Sharpiless/PaddleDetection-Yolov5) |Detection | 29.3|—|✅|✅|✅|✅|✅|/|/|/|
|<font size=2>  [blazeface](https://github.com/PaddlePaddle/PaddleDetection/blob/develop/docs/tutorials/GETTING_STARTED_cn.md) |Face Detection |1.5|---|✅|✅|✅|✅|✅|/|/|/|
|<font size=2> [retinaface](https://github.com/GuoQuanhao/RetinaFace-Paddle) |Face Localisation |1.7|——— |/|/|/|/|/|/|/|/|
|<font size=2>  [PP-OCRv1](https://github.com/PaddlePaddle/PaddleOCR/blob/release%2F2.5/doc/doc_ch/ppocr_introduction.md) |OCR | 2.3+4.4 |---|/|/|/|/|/|✅|✅|✅|
|<font size=2>  [PP-OCRv2](https://github.com/PaddlePaddle/PaddleOCR/blob/release%2F2.5/doc/doc_ch/ppocr_introduction.md) |OCR | 2.3+4.4 |---|/ |/|/ |/ |/ |/ |/ |/ |
| <font size=2> [PP-OCRv3](https://github.com/PaddlePaddle/PaddleOCR/blob/release%2F2.5/doc/doc_ch/PP-OCRv3_introduction.md) |OCR | 2.4+10.6 |---|/ |/ |/ |/ |/ |✅ |✅ |✅ |
| <font size=2> [PP-OCRv3-tiny](https://github.com/PaddlePaddle/PaddleOCR/blob/release%2F2.5/doc/doc_ch/models_list.md) |OCR |2.4+10.7 |---|/ |/ |/ |/ |/|/ |/ |/ |
|<font size=2>  [PP-LiteSeg(STDC1)](https://github.com/PaddlePaddle/PaddleSeg/blob/develop/configs/pp_liteseg/README.md)|Seg | 32.2|——— |/|/|/|/|/|/|/|/|
|<font size=2>  [PP-HumanSeg-lite](https://github.com/PaddlePaddle/PaddleSeg/blob/develop/contrib/PP-HumanSeg/README_cn.md) |Seg | 556KB|——— |/|/|/|/|/|/|/|/|
|<font size=2>  [HRNet-w18](https://github.com/PaddlePaddle/PaddleSeg/blob/develop/docs/train/train_cn.md) |Seg | 38.7|——— |/|/|/|/|/|/|/|/|
|<font size=2> [PP-HumanSeg-server](https://github.com/PaddlePaddle/PaddleSeg/blob/develop/contrib/PP-HumanSeg/README_cn.md)|Seg | 107.2|——— |/|/|/|/|/|/|/|/|
|<font size=2> [Unet](https://github.com/PaddlePaddle/PaddleSeg/blob/develop/docs/train/train_cn.md) |Seg | 53.7|——— |/ |/ |/ |/ |/|/ |/ |/ |
|<font size=2> [Deeplabv3-resnet50](https://github.com/PaddlePaddle/PaddleSeg/blob/develop/docs/train/train_cn.md)|Seg |156.5|——— |/ |/ |/ |/ |/|/ |/ |/ |

</font>

    
    
#### 环境依赖

- python >= 3.6
- paddlepaddle >= 2.2

### pip安装

```shell
pip install --upgrade FastDeploy
```


## 快速开始

这里以信息抽取-命名实体识别任务，UIE模型为例，来说明如何快速使用PaddleNLP:

### 一键预测

PaddleNLP提供[一键预测功能](./docs/model_zoo/taskflow.md)，无需训练，直接输入数据即可开放域抽取结果：

```python
>>> from pprint import pprint
>>> from paddlenlp import Taskflow

>>> schema = ['时间', '选手', '赛事名称'] # Define the schema for entity extraction
>>> ie = Taskflow('information_extraction', schema=schema)
>>> pprint(ie("2月8日上午北京冬奥会自由式滑雪女子大跳台决赛中中国选手谷爱凌以188.25分获得金牌！"))
