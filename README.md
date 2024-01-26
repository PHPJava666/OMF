# Overlay Left Atrium Mantle-Free for Semi-Supervised Medical Image Segmentation
by Jiacheng Liu[0009−0000−3354−6139], Wenhua Qian, Jinde Cao and Peng Liu.
[fig1.pdf](https://github.com/vigilliu/OMF/files/14062173/fig1.pdf)
[fig2.pdf](https://github.com/vigilliu/OMF/files/14062175/fig2.pdf)

## Introduction
Official code for "[Overlay Left Atrium Mantle-Free for Semi-Supervised Medical Image Segmentation](https://arxiv.org/)".
## Requirements
This repository is based on PyTorch 1.8.0, CUDA 11.1 and Python 3.6.13. All experiments in our paper were conducted on NVIDIA GeForce RTX 3090 GPU with an identical experimental setting.
## Usage
Data could be got at [LA](https://github.com/yulequan/UA-MT/tree/master/data).

[fig3.pdf](https://github.com/vigilliu/OMF/files/14062177/fig3.pdf)
<img width="654" alt="截屏2024-01-26 16 45 52" src="https://github.com/vigilliu/OMF/assets/129838909/5bf7713e-3bb2-4064-8800-397e126246e8">
<img width="890" alt="截屏2024-01-26 16 46 19" src="https://github.com/vigilliu/OMF/assets/129838909/855c96e6-1d1a-47e2-998b-1eb85c0373af">

To train a model,
```
python ./code/LA_BCP_train.py --exp=OMF_lab8 --base_lr=0.1 --labelnum=8  #for LA training
python ./code/LA_BCP_train.py --exp=OMF_lab16 --base_lr=0.1 --labelnum=16  #for LA training
``` 

To test a model,
```
python ./code/test_LA.py --exp=OMF_lab8 --labelnum=8 #for LA testing
python ./code/test_LA.py --exp=OMF_lab16 --labelnum=16 #for LA testing
```

## Acknowledgements
Our code is largely based on [BCP:Bidirectional Copy-Paste for Semi-Supervised Medical Image Segmentation]. Thanks for these authors for their valuable work, hope our work can also contribute to related research.

## Questions
If you have any questions, welcome contact me at '.edu.cn'



