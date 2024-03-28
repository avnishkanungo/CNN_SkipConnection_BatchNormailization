# Skip Connection and Batch Normalization in CNNs

## Overview
This project implements skip connections (also known as residual connections) and batch normalization techniques in Convolutional Neural Networks (CNNs) to address the vanishing gradient problem. These techniques enable the training of deeper networks by mitigating the degradation problem associated with increasing network depth.
Refer to the associated PDF for more details.

## Motivation
As CNNs grow deeper, they encounter difficulties in training due to the vanishing gradient problem. Skip connections and batch normalization are two widely used techniques to alleviate this issue and facilitate the training of deep networks.

## Implementation Details
- **Skip Connections**: 
  - Skip connections allow the gradients to flow directly through the network, bypassing several layers. This helps in mitigating the vanishing gradient problem by providing shorter paths for gradient flow during backpropagation.
  - Implementation involves adding identity mappings between layers or using residual blocks to pass the input directly to the output of a later layer.

- **Batch Normalization**:
  - Batch normalization normalizes the activations of each layer, reducing internal covariate shift and providing a regularization effect.
  - It stabilizes the training process, accelerates convergence, and allows for the use of higher learning rates.

## Requirements
- Python 3.x
- PyTorch
- torchvision
- Other dependencies (specified in imports in the .ipynb file)
