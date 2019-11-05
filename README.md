# WSCNet: Weakly Supervised Coupled Networks for Visual Sentiment Classification and Detection

By Dongyu She, Jufeng Yang, Ming-Ming Cheng, Yu-Kun Lai, Paul L. Rosin and Liang Wang

### Introduction

We propose a framework for weakly supervised sentiment detection and classification. The detection branch detects a sentiment specific soft map by training a fully convolutional network with the cross spatial pooling strategy, which only requires image-level labels, thereby significantly reducing the annotation burden. The classification branch utilizes both the holistic and localized information by coupling the sentiment map with deep features for robust classification. The proposed WSCNet performs favorably against the state-ofthe-art methods for visual sentiment analysis.

### Citations

If you find our framework useful in your research, please consider citing:

    @article{She_2019_TMM,
    	Author = {She, Dongyu and Yang, Jufeng and Cheng, Ming-Ming and Lai, Yu-Kun and Rosin, Paul L. and Wang, Liang},
    	Title = {WSCNet: Weakly Supervised Coupled Networks for Visual Sentiment Classification and Detection},
    	journal = {IEEE Transactions on Multimedia},
    	Year = {2019}
    }

    @InProceedings{Yang_2018_CVPR,
    	Author = {Yang, Jufeng and She, Dongyu and Lai, Yu-Kun and Rosin, Paul L. and Yang, Ming-Hsuan},
    	Title = {Weakly Supervised Coupled Networks for Visual Sentiment Analysis},
    	booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition},
    	Year = {2018}
    }


### Architecture
<p align="left">
<img src="images/framework.jpg" alt="framework" width="900px">
</p>

### Requirements

Our code is written by Python, based on [Pytorch](https://pytorch.org/) (Version ≥ 1.0)

NVIDIA GTX TITANX (~12G of memory)


### Dataset config

Train/val/test split is available [here](https://pan.baidu.com/s/1YLludq6JYQZcCIEXgiMH2Q) (password: r2bm) for the FI. And splits for other dataset can be downloaded [here](https://pan.baidu.com/s/1GNqdmGzPpd7YLfqkJQpxwQ) (password: xay5).


### Usage

1. Clone the repository
    ```Shell
    git clone https://github.com/sherleens/WSCNet.git
    ```

2. Download dataset config and put the split images into `$ROOT_DIR/dataset/FI/` folder. The folders are arranged like this:
    ```Shell
    FI
    ├── train
    │   ├── classname1
    │   │   ├──xx.jpg
    │   │   ├──...
    │   ├── classname2
    │   │   ├──...
    │   ├── ...
    ├── val
    │   ├── classname1
    │   │   ├──xx.jpg
    │   │   ├──...
    │   ├── classname2
    ```

3. Go into the folder `$ROOT_DIR/scripts/`. Then you can train the deep network by running `WSCNet-Res101_train.ipynb` on the FI dataset.


### Our trained models

Coming soon.
