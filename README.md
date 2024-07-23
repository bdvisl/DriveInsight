# DriveInsight

> Jiankun Li, Hao Li, Jiangjiang Liu, Zhikang Zou, Xiaoqing Ye&#8224;, Fan Wang, Jizhou Huang&#8224;, Hua Wu, Haifeng Wang
>
> Baidu Inc.
>
> <sup>&#8224;</sup> Corresponding author

[arXiv link](https://arxiv.org/abs/2407.06546)

## Overview
We present a debugging and analyzing tool for black-box end-to-end autonomous driving models.

![11111](https://github.com/bdvisl/DriveInsight/assets/174320502/4d2d6b75-20e9-4369-8b50-521d68371206)
Overall architecture of our DriveInsight framework. 

## Evaluation

Closed-loop evaluation on the Town05 Long & Short benchmarks. Our method achieve a
competitive driving score while also achieving the highest route completion. The sign * denotes that
we exclude data from town05 in the training set.


|Method|Modality|Reference|Training frames|Town05 Long DS|Town05 Long RC | Town05 Short DS| Town05 Short RC|
|---|---|---|---|---|---|---|---|
LBC| C | CoRL 20 | 150K | 12.3 | 31.9 | 31.0 | 55.0
Transfuser| C+L | TPAMI 22 | 150K | 31.0 | 47.5 | 54.5 | 78.4
ST-P3 | C | ECCV 22 | 150K | 11.5 | 83.2 | 55.1 | 86.7
VAD | C | ICCV 23 | 3.0M | 30.3 | 75.2 | 64.3 | 87.3
ThinkTwice | C+L | CVPR 23 | 2.2M | 70.9 | 95.5 | - | -
MILE | C | NeurIPS 22 | 2.9M | 61.1 | 97.4 | - | -
Interfuser | C | CoRL 22 | 3.0M | 68.3 | 95.0 | 94.9 | 95.2
DriveAdapter | C+L | ICCV 23 | 2.0M | **71.9** | 97.3 | - | -
Ours | C+L | - | 1.8M | 66.6 | **100.0** | **95.3** | **99.2**
Ours* | C+L | - | 1.5M | 64.4 | **100.0** | 93.2 | 95.8


## Citation
If you find this project helpful, please consider citing the following paper:
```
@article{li2024exploring,
  title={Exploring the Causality of End-to-End Autonomous Driving},
  author={Jiankun, Li and Hao, Li and Jiangjiang, Liu and Zhikang, Zou and Xiaoqing, Ye and Fan, Wang and Jizhou, Huang and Hua, Wu and Haifeng, Wang},
  journal={arXiv preprint arXiv:2407.06546},
  year={2024}
}
```

