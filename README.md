# CSNet in Highly Efficient Salient Object Detection with100K Parameters
# **Non Profit Academic Research ONLY** And **DO NOT Distribute**
## Introduction
The repo is the light-weight Salient Object Detection model CSNet.

## Evaluation

You may refer to this repo for results evaluation: [SalMetric](https://github.com/Andrew-Qibin/SalMetric).

## Usage

### Prerequisites

- [Pytorch 1.0+](http://pytorch.org/) (We use PyTorch 1.0 for training, other version are not tested.)

### 1. Clone the repository

```shell
git clone https://github.com/MCG-NKU/SOD100K.git
cd SOD100K/CSNet
```

### 2. Download the datasets

Download the following datasets and unzip them into `dataset` folder.
Note that for each dataset, put images and GT into the folder 'images' and 'GT'.
Example:
```
SOD100K/CSNet/datasets/sal/DUTS-TE/GT
SOD100K/CSNet/datasets/sal/DUTS-TE/images
```

### 3. Testing

```
python test.py --config configs/csnet-L-x2.yml
```

### 4. Pre-trained models
Since the CSNet is extremely small, we just include the pre-trained model of CSNet in the `checkpoints` folder.

### 5. Training
**Non Profit Academic Research ONLY**

For commercial use, you can also email us to get more details.
```
python train.py --config configs/csnet-L-x2_train.yml

python finetune.py --config configs/csnet-L-x2_train.yml --epoch (the epoch you want to finetune)
```

```E-amil: shgao(at)live.com AND cmm(at)nankai.edu.cn```

## Citation
If you find this work or code is helpful in your research, please cite:
```
@InProceedings{gao2020sod100k,
  author = {Gao, Shang-Hua and Tan, Yong-Qiang and Cheng, Ming-Ming and Lu, Chengze and Chen, Yunpeng and Yan, Shuicheng},
  title = {Highly Efficient Salient Object Detection with 100K Parameters},
  booktitle = {ECCV},
  year = {2020},
}

```
