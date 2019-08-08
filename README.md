### This is the code base for the paper: "Weight Standardized Residual Learning for Image Recognition"

# Train CIFAR10 with ResNet18, ResNet50 and ResNet101 by implementing Weight Standardization on PyTorch

I'm playing with [PyTorch](http://pytorch.org/) on the CIFAR10 dataset.

## Prerequisites
- Python 3.6+
- PyTorch 1.0+

## 3 type of networks are provided in 3 different folders:
*ResNet18
*ResNet50
*ResNet101

## Weight Standardization (WS) has been implemented seperately in 'resnet_WS.py' modules under the folder 'Model' in each ResNet folders.
To run the ResNet with WS, just edit the 'resnet' portion and rewrite 'resnet_WS' in the 'main.py' file of each ResNet folder.

## Learning rate adjustment
I manually change the `lr` during training:
- `0.1` for epoch `[0,150)`
- `0.01` for epoch `[150,250)`
- `0.001` for epoch `[250,350)`

Start the training with 'python main.py --lr=0.1'

## The graphs can be plotted using 'Resnet_plot.ipynb' file
