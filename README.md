# EfficientSAM

[XetHub](about.xethub.com) hosted fork of EfficientSAM using the [GitHub plugin](https://github.com/apps/xetdata).

EfficientSAM: Leveraged Masked Image Pretraining for Efficient Segment Anything

## News
[Dec.5 2023] We release the torchscript version of EfficientSAM and share the Google colab notebook.

## Online Demo & Examples
Online demo and examples can be found in the [project page](https://yformer.github.io/efficient-sam/).

## EfficientSAM Instance Segmentation Examples

<img width="848" alt="Screenshot 2023-12-06 at 1 16 13 PM" src="https://github.com/xetdata/EfficientSAM/assets/801507/6a4586e6-94cc-4eea-94e7-e78a6f57dcfe">


## Using the models

The model files live in this repo itself:

- EfficientSAM-S:[models/efficientsam_s_gpu.jit](models/efficientsam_s_gpu.jit)
- EfficientSAM-Ti: [models/efficientsam_ti_gpu.jit](models/efficientsam_ti_gpu.jit)

<img width="971" alt="Screenshot 2023-12-06 at 1 19 26 PM" src="https://github.com/xetdata/EfficientSAM/assets/801507/72374016-2b6f-4617-881a-9b7b45059a35">


**Instructions**

1. Install the [git-xet](https://xethub.com/assets/docs/getting-started/install) extension.

2. Clone the repo:

```
# Using SSH
git clone git@github.com:xetdata/EfficientSAM.git

cd EfficientSAM/
```

2. Activate your Python virtual environment and install the requirements:

```
pip install -r requirements.txt
```

3. Start Jupyter Notebook:

```
# jupyter lab
jupyter lab

# jupyter notebook
jupyter notebook
```

4. You can directly use EfficientSAM:

```
import torch

efficientsam = torch.jit.load(models/efficientsam_s_gpu.jit)
```

## Google Colab

You can also use this [Google Colab notebook](https://colab.research.google.com/drive/150dvh_lwbliC3020fWO9qASgy-so6sUZ?usp=sharing)


## Acknowledgement

+ [SAM](https://github.com/facebookresearch/segment-anything)
+ [MobileSAM](https://github.com/ChaoningZhang/MobileSAM)
+ [FastSAM](https://github.com/CASIA-IVA-Lab/FastSAM)
+ [U-2-Net](https://github.com/xuebinqin/U-2-Net)

If you're using EfficientSAM in your research or applications, please cite using this BibTeX:
```bibtex


@article{xiong2023efficientsam,
  title={EfficientSAM: Leveraged Masked Image Pretraining for Efficient Segment Anything},
  author={Yunyang Xiong, Bala Varadarajan, Lemeng Wu, Xiaoyu Xiang, Fanyi Xiao, Chenchen Zhu, Xiaoliang Dai, Dilin Wang, Fei Sun, Forrest Iandola, Raghuraman Krishnamoorthi, Vikas Chandra},
  journal={arXiv:2312.00863},
  year={2023}
}
```
