# Generative models
This is a collection of generative models

## Variational Auto Encoder (VAE)

**1. Variational Auto Encoder (VAE)**

This is an implementation of **Auto-Encoding Variational Bayes** using Pytorch.

Reference paper:
-  [Auto-Encoding Variational Bayes](https://arxiv.org/abs/1312.6114).

Code: [apaszke](https://github.com/pytorch/examples/blob/master/vae/main.py), which is changed some part to implement in Jupyter notebook.

**2. Conditional VAE**

This is an extension of VAE using an extra input label y to generate new instances.

Reference paper:
-  [Semi-Supervised Learning with Deep Generative Models](https://arxiv.org/abs/1406.5298).

Code: [wiseodd](https://github.com/wiseodd/generative-models/tree/master/VAE/conditional_vae).

**3. Denoising VAE**

This is an extension of VAE with noise injected into input.

Reference paper [Denoising criterion for variational auto-encoding framework](https://arxiv.org/abs/1511.06406).

The code is adopted from [wiseodd](https://github.com/wiseodd/generative-models/blob/master/VAE/denoising_vae/dvae_pytorch.py).

Loss is averaged by using [PyTorchNet](https://github.com/pytorch/tnt). To install ```PyTorchNet```, we can run following command:
```sh
pip install git+https://github.com/pytorch/tnt.git@master
```

**3. Adversarial Autoencoders**
- Reference paper: 
- [Adversarial autoencoders](https://arxiv.org/abs/1511.05644)

- Article and code: 
- [Adversarial autoencoders with Pytorch](https://blog.paperspace.com/adversarial-autoencoders-with-pytorch/)

## Generative Adversarial Networks (GANs)

**1. Generative Adversarial Networks (GAN)**

GAN is a neural networks that is composed of 2 separate deep neural networks trying to compete each other during training time: the generator and the discriminator.

Reference paper: 
- [Generative Adversarial Networks](https://arxiv.org/abs/1406.2661)

Article:
- [Hackernoon](https://hackernoon.com/how-do-gans-intuitively-work-2dda07f247a1#.4ppap66hn)
- [Arthur Juliani](https://medium.com/@awjuliani/generative-adversarial-networks-explained-with-a-classic-spongebob-squarepants-episode-54deab2fce39#.w5pqccvbr)

Code: [wiseodd](https://github.com/wiseodd/generative-models/blob/master/GAN/vanilla_gan/gan_pytorch.py)

**2. Deep Convolutional Generative Adversarial Networks (DCGAN)**

In order to understand Deconvolutional network, refer to this [Convolution arithmetic](https://github.com/vdumoulin/conv_arithmetic).

In general case, with **W**: the input volume size, **F**: the filter/kernel size, **S**: the stride and **P**: the amount of zero padding used, the architecture of Deconv layer can be computed as following:

**(W + (W-1)*(S-1)) + (F-1) -2P)**

Reference paper: 
- [Unsupervised representation learning with deep convolutional generative adverarial networks](https://arxiv.org/pdf/1511.06434.pdf)

Code: [Pytorch DCGAN](https://github.com/pytorch/examples/blob/master/dcgan/main.py)


**3. Conditional Generative Adversarial Networks**