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
- General CVAE arichitecture
![image](https://user-images.githubusercontent.com/39685317/124267851-5e98fc00-db6b-11eb-8c3e-35f0846fc01f.png)
- Experimental Setup
  - dataset: MNIST dataset in torchvision.datasets
  - Batchsize: 100
  - Activation function: Relu(x)
  - Optimizer: Adam
  - Epochs = 50 
  - Layers:
    - ![image](https://user-images.githubusercontent.com/39685317/124268193-cb13fb00-db6b-11eb-9bb1-76a6046e8622.png)

- Training and testing:
  - ![image](https://user-images.githubusercontent.com/39685317/124267929-76708000-db6b-11eb-90cd-313a6beed13c.png)
  - Record of last three epoches:
    - ![image](https://user-images.githubusercontent.com/39685317/124268331-f565b880-db6b-11eb-8583-f90c94ca3363.png)

- Demos:
  - ![image](https://user-images.githubusercontent.com/39685317/124267956-7f615180-db6b-11eb-8ca1-6262ed47f4ca.png)
  - Comparing to randomly sampled VAE output
  - ![image](https://user-images.githubusercontent.com/39685317/124268031-94d67b80-db6b-11eb-9d7a-116972510360.png)

## References
[1] Kihyuk Sohn, Honglak Lee, and Xinchen Yan. ‘Learning structured output representation using deep conditional generative models.’  _In NIPS_, 2015.

[2] Carl Doersch, ‘Tutorial on Variational Autoencoders’, _arXiv:1606.05908_, 2016

[3] Deng, L., 'The mnist database of handwritten digit images for machine learning research.' _IEEE Signal Processing Magazine_, 29(6), 141–142, 2012.

[4] https://github.com/lyeoni/



