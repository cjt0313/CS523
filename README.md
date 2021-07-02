## CS523
# An application of CVAE on MINIST dataset

This project focuses on the Conditional Variantional Auto-encoder, a member of VAE family that is enabled to sampling new data conditional on a specific input.
- Traditional VAE model generates plausible looking fake samples while it could not control the model output. 
- The goal of this project aims to build up an auto-encoder model that could generate specific output.

## Conditional Variational Auto-encoder (CVAE)
In a one-sentence description, CVAE proceeds as conditioning the entire generative process on an input with the loss function as a sumation of KL divergence and cross-entropy loss.
- Dependencies
  - pytorch
  - matlabplotlib
  - keras
- Model arichitecture
https://github.com/lz10/CS523/blob/main/picture/architecture%201.png

- Experimental Setup
  - dataset: MNIST dataset in torchvision.datasets
  - Batchsize: 100
  - Activation function: Relu(x)
  - Optimizer: Adam
  - Epochs = 50
- Training and testing:
- Demos:

## References
[1] Kihyuk Sohn, Honglak Lee, and Xinchen Yan. ‘Learning structured output representation using deep conditional generative models.’  _In NIPS_, 2015.

[2] Carl Doersch, ‘Tutorial on Variational Autoencoders’, _arXiv:1606.05908_, 2016

[3] Deng, L., 'The mnist database of handwritten digit images for machine learning research.' _IEEE Signal Processing Magazine_, 29(6), 141–142, 2012.

[4] https://github.com/lyeoni/pytorch-mnist-CVAE



