# ResNet-ResNeXt-Model-Builder-Tensorflow-Keras
This repository contains One-Dimentional (1D) and Two-Dimentional (2D) versions of ResNet (original) and ResNeXt (Aggregated Residual Transformations on ResNet) developed in Tensorflow-Keras. The models in this repository have been built following the original papers' implementation guidances (as much as possible) except adding commonly accepted beneficial blocks such as BatchNormalization.  
Read more about ResNets in this original preprint: https://arxiv.org/pdf/1512.03385.  
Read more about ResNeXts in this original preprint: https://arxiv.org/abs/1611.05431.  

Supprted Models:  
1. ResNet18 - ResNeXt18
2. ResNet34 - ResNeXt34
3. ResNet50 - ResNeXt50
4. ResNet101 - ResNeXt101
5. ResNet152 - ResNeXt152

![ResNet Architecture Params](https://github.com/Sakib1263/ResNet-Model-Builder-KERAS/blob/main/Documents/Images/ResNet_Model.png "ResNet Architecture") 

On the contrary, the models contain BatchNormalization (BN) blocks after Convolutional blocks and before activation, which is deviant from the original implementation. Read more about BN in this paper: https://arxiv.org/abs/1502.03167v3.

## ResNet Architectures
A table from the original paper containing the architectures of the ResNet models developed is shown below:  
![ResNet Architecture Params](https://github.com/Sakib1263/1DResNet-KERAS/blob/main/Documents/Images/ResNet.png "ResNet Parameters")  
The original implementation comes up with a fixed number of 1000 classification due to using ImageNet dataset for training and evaluation purposes. The developed ResNet model is flexible enough to accept any number of classed according to the user's requirements.  

Mentionable that ResNet18 and ResNet34 uses a lighter residual block that other three deeper models as shown in the Figure below where the deeper residual block with a bottleneck structure is for ResNet50, ResNet101 and ResNet152.
![Residual Blocks](https://github.com/Sakib1263/1DResNet-KERAS/blob/main/Documents/Images/Residual_Block.png "Residual Blocks")  

## ResNeXt Architectures


## Supported Features
The speciality about this model is its flexibility. The user has the option for: 
1. Choosing any of 5 available ResNet models for either 1D or 2D tasks.
2. Varying number of input kernel/filter, commonly known as the Width of the model.
3. Varying number of classes for Classification tasks and number of extracted features for Regression tasks.
4. Varying number of Channels in the Input Dataset.
Details of the process are available in the DEMO provided in the codes section. The datasets used in the DEMO as also available in the 'Documents' folder.
