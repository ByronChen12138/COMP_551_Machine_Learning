# COMP 551 Project 4 (Fall 2021)

## Acknowledgements

This repository is for **COMP 551** at **McGill University** for **Fall 2021**. Thanks to Byron Chen, Yicong Hao, and Kevin Li, without whom this project cannot be accomplished.

## Description
To find an algorithm that can train sparse neural networks (SNN) without being bounded to specific architectures, this project aims to reproduce part of the 
paper: "A Bregman Learning Framework for Sparse Neural Networks". In this study, we use the codes provided by the authors in this repository to reproduce
the results in a two-hidden-layer MLP, a ConvNet and ResNet-18. To further investigate ifthe algorithms can perform well in other models, VGG-16 and VGG-13 are implemented in
this study. In the end, the results is found to be unstable, since we cannot reproduce the results
even the codes are provided by the researchers. Apart from this, the Bregman algorithms fail to work in VGG-16 and VGG-13 which shows that 
they are model-dependent, thus not general.

## Project Structure

```console
├── paper.pdf
├── Project Description.pdf
├── report.pdf
└── codes
    ├── Bregman.ipynb
    └── Bregman Learning
        ├── model
        │   ├── aux_funs.py
        │   ├── fully_connected.py
        │   ├── mnist_conv.py
        │   ├── resnet.py
        │   └── vgg.py
        ├── notebooks
        │   ├── ConvNet-Classification.ipynb
        │   ├── DenseNet.ipynb
        │   ├── MLP-Classification.ipynb
        │   ├── ResNet-Classification.ipynb
        │   └── Skip-Encoder.py
        ├── utils
        │   ├── configuration.py
        │   └── datasets.py
        ├── .gitignore
        ├── LICENSE
        ├── optimizers.py
        ├── README.md
        ├── requirements.txt
        └── train.py
```
