# Generative models
This is a collection of generative models

1. Variational Auto Encoder (VAE)

This is an implementation of **Auto-Encoding Variational Bayes** using Pytorch.

Reference paper [Auto-Encoding Variational Bayes](https://arxiv.org/abs/1312.6114).

The code is adopted from [apaszke](https://github.com/pytorch/examples/blob/master/vae/main.py), which is changed some part to implement in Jupyter notebook.

2. Conditional VAE

This is an extension of VAE using an extra input label y to generate new instances.

Reference paper [Semi-Supervised Learning with Deep Generative Models](https://arxiv.org/abs/1406.5298).

The code is adopted from [wiseodd](https://github.com/wiseodd/generative-models/tree/master/VAE/conditional_vae).

3. Denoising VAE

This is an extension of VAE with noise injected into input.

Reference paper [Denoising criterion for variational auto-encoding framework](https://arxiv.org/abs/1511.06406).

The code is adopted from [wiseodd](https://github.com/wiseodd/generative-models/blob/master/VAE/denoising_vae/dvae_pytorch.py).

Loss is averaged by using [PyTorchNet](https://github.com/pytorch/tnt).

```pip install git+https://github.com/pytorch/tnt.git@master```
