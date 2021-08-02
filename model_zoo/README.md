# InsightFace Model Zoo

## 0. Python Package models

To check the detail of insightface python package, please see [here](../python-package).

To install: ``pip install -U insightface``


| Name           | Detection Model | Recognition Model   | Alignment    | Attributes |
| -------------- | --------------- | ------------------- | ------------ | ---------- |
| **antelopev2** | SCRFD-10GF      | ResNet100@Glint360K | 2d106 & 3d68 | Gender&Age |

##  1. Face Recognition models.

| Backbone | Dataset | Method  | LFW   | CFP-FP | AgeDB-30 | MegaFace | link(mxnet)                                                  |
| -------- | ------- | ------- | ----- | ------ | -------- | -------- | ------------------------------------------------------------ |
| R100     | MS1MV2  | ArcFace | 99.77 | 98.27  | 98.28    | 98.47    | [BaiduDrive](https://pan.baidu.com/s/1wuRTf2YIsKt76TxFufsRNA) |
| MFN      | MS1MV1  | ArcFace | 99.50 | 88.94  | 95.91    | -        | [BaiduDrive](https://pan.baidu.com/s/1If28BkHde4fiuweJrbicVA) |

| Backbone | Dataset   | Method  | LFW  | CFP-FP | AgeDB-30 | African | Caucasian | South Asian | East Asian | MR-All | link(onnx)                                                   |
| -------- | --------- | ------- | ---- | ------ | -------- | ------- | --------- | ----------- | ---------- | ------ | ------------------------------------------------------------ |
| R100     | Casia     | ArcFace |      |        |          | 39.666  | 53.933    | 47.807      | 21.572     | 42.735 | [download](https://1drv.ms/u/s!AswpsDO2toNKrUJpk8zC61HVN7Kg?e=zE9JDd) |
| R100     | MS1MV2    | ArcFace |      |        |          | 79.117  | 87.176    | 85.501      | 55.807     | 80.725 | [download](https://1drv.ms/u/s!AswpsDO2toNKrUTlYEHJCHg3UYM-?e=ihxMpS) |
| R18      | MS1MV3    | ArcFace |      |        |          | 62.613  | 75.125    | 70.213      | 43.859     | 68.326 | [download](https://1drv.ms/u/s!AswpsDO2toNKrTxlT6w1Jo02yzSh?e=KDhFAA) |
| R34      | MS1MV3    | ArcFace |      |        |          | 71.644  | 83.291    | 80.084      | 53.712     | 77.365 | [download](https://1drv.ms/u/s!AswpsDO2toNKrT2O5pgyVtwnjeMq?e=16S8LI) |
| R50      | MS1MV3    | ArcFace |      |        |          | 75.488  | 86.115    | 84.305      | 57.352     | 80.533 | [download](https://1drv.ms/u/s!AswpsDO2toNKrUUWd5i3a5OlFpM_?e=ExBDBN) |
| R100     | MS1MV3    | ArcFace |      |        |          | 81.083  | 89.040    | 88.082      | 62.193     | 84.312 | [download](https://1drv.ms/u/s!AswpsDO2toNKrUPwyqWvNXUlNd3P?e=pTLw9A) |
| R18      | Glint360K | ArcFace |      |        |          | 68.230  | 80.575    | 75.852      | 47.831     | 72.074 | [download](https://1drv.ms/u/s!AswpsDO2toNKrT5ey4lCqFzlpzDd?e=VWP28J) |
| R34      | Glint360K | ArcFace |      |        |          | 79.907  | 88.620    | 86.815      | 60.604     | 83.015 | [download](https://1drv.ms/u/s!AswpsDO2toNKrUBcgGkiuUS11Hsd?e=ISGDnP) |
| R50      | Glint360K | ArcFace |      |        |          | 85.272  | 91.617    | 90.541      | 66.813     | 87.077 | [download](https://1drv.ms/u/s!AswpsDO2toNKrT8jbvHxjqCY0d08?e=igfdrd) |
| R100     | Glint360K | ArcFace |      |        |          | 89.488  | 94.285    | 93.434      | 72.528     | 90.659 | [download](https://1drv.ms/u/s!AswpsDO2toNKrUFgLEIj-mnkb51b?e=vWqy2q) |



## 2. Face Detection models.

### 2.1 RetinaFace

In RetinaFace, mAP was evaluated with multi-scale testing.

| Impelmentation           | Easy-Set | Medium-Set | Hard-Set | Link                                                         |
| ------------------------ | -------- | ---------- | -------- | ------------------------------------------------------------ |
| RetinaFace-R50           | 96.5     | 95.6       | 90.4     | [BaiduDrive](https://pan.baidu.com/s/1C6nKq122gJxRhb37vK0_LQ) |
| RetinaFace-m025(yangfly) | -        | -          | 82.5     | [BaiduDrive](https://pan.baidu.com/s/1P1ypO7VYUbNAezdvLm2m9w)(nzof) |

### 2.2 SCRFD

In SCRFD, mAP was evaluated with single scale testing, VGA resolution.

|      Name      | Easy  | Medium | Hard  | FLOPs | Params(M) | Infer(ms) | Link                                                         |
| :------------: | ----- | ------ | ----- | ----- | --------- | --------- | ------------------------------------------------------------ |
|   SCRFD_500M   | 90.57 | 88.12  | 68.51 | 500M  | 0.57      | 3.6       | [download](https://1drv.ms/u/s!AswpsDO2toNKqyYWxScdiTITY4TQ?e=DjXof9) |
|    SCRFD_1G    | 92.38 | 90.57  | 74.80 | 1G    | 0.64      | 4.1       | [download](https://1drv.ms/u/s!AswpsDO2toNKqyPVLI44ahNBsOMR?e=esPrBL) |
|   SCRFD_2.5G   | 93.78 | 92.16  | 77.87 | 2.5G  | 0.67      | 4.2       | [download](https://1drv.ms/u/s!AswpsDO2toNKqyTIXnzB1ujPq4th?e=5t1VNv) |
|   SCRFD_10G    | 95.16 | 93.87  | 83.05 | 10G   | 3.86      | 4.9       | [download](https://1drv.ms/u/s!AswpsDO2toNKqyUKwTiwXv2kaa8o?e=umfepO) |
|   SCRFD_34G    | 96.06 | 94.92  | 85.29 | 34G   | 9.80      | 11.7      | [download](https://1drv.ms/u/s!AswpsDO2toNKqyKZwFebVlmlOvzz?e=V2rqUy) |
| SCRFD_500M_KPS | 90.97 | 88.44  | 69.49 | 500M  | 0.57      | 3.6       | [download](https://1drv.ms/u/s!AswpsDO2toNKri_NDM0GIkPpkE2f?e=JkebJo) |
| SCRFD_2.5G_KPS | 93.80 | 92.02  | 77.13 | 2.5G  | 0.82      | 4.3       | [download](https://1drv.ms/u/s!AswpsDO2toNKqyGlhxnCg3smyQqX?e=A6Hufm) |
| SCRFD_10G_KPS  | 95.40 | 94.01  | 82.80 | 10G   | 4.23      | 5.0       | [download](https://1drv.ms/u/s!AswpsDO2toNKqycsF19UbaCWaLWx?e=F6i5Vm) |



## 3. Face Alignment models.

### 2.1 2D Face Alignment

### 2.2 3D Face Alignment

### 2.3 Dense Face Alignment

## 4. Face Attribute models.

### 4.1 Gender&Age 


### 4.2 Expression