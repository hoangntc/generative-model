# Generative models
This is a collection of generative models

**1. Variational Auto Encoder (VAE)**

This is an implementation of **Auto-Encoding Variational Bayes** using Pytorch.

Reference paper [Auto-Encoding Variational Bayes](https://arxiv.org/abs/1312.6114).

The code is adopted from [apaszke](https://github.com/pytorch/examples/blob/master/vae/main.py), which is changed some part to implement in Jupyter notebook.

**2. Conditional VAE**

This is an extension of VAE using an extra input label y to generate new instances.

Reference paper [Semi-Supervised Learning with Deep Generative Models](https://arxiv.org/abs/1406.5298).

The code is adopted from [wiseodd](https://github.com/wiseodd/generative-models/tree/master/VAE/conditional_vae).

**3. Denoising VAE**

This is an extension of VAE with noise injected into input.

Reference paper [Denoising criterion for variational auto-encoding framework](https://arxiv.org/abs/1511.06406).

The code is adopted from [wiseodd](https://github.com/wiseodd/generative-models/blob/master/VAE/denoising_vae/dvae_pytorch.py).

Loss is averaged by using [PyTorchNet](https://github.com/pytorch/tnt). To install ```PyTorchNet```, we can run following command:
```sh
pip install git+https://github.com/pytorch/tnt.git@master
```

**4. Generative Adversarial Networks**

GAN is a neural networks that is composed of 2 separate deep neural networks trying to compete each other during training time: the generator and the discriminator.

Reference paper:
- [Generative Adversarial Networks](https://arxiv.org/abs/1406.2661)
- [Unsupervised representation learning with deep convolutional generative adverarial networks](https://arxiv.org/pdf/1511.06434.pdf)

Article:
- [Hackernoon](https://hackernoon.com/how-do-gans-intuitively-work-2dda07f247a1#.4ppap66hn)
- [Arthur Juliani](https://medium.com/@awjuliani/generative-adversarial-networks-explained-with-a-classic-spongebob-squarepants-episode-54deab2fce39#.w5pqccvbr)

The code is adopted from [wiseodd](https://github.com/wiseodd/generative-models/blob/master/GAN/vanilla_gan/gan_pytorch.py)

