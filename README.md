### My personal paper reading notes
> Last updated 03/28/2018
>
> Lian qing (lianqinglalala@gmail.com)

## Table of Contents

  - [Architecture search](architecture-search)

## Architecture search

- Learning Transferable Architectures for Scalable Image Recognition [[pdf]](https://arxiv.org/abs/1707.07012)
[[code]](https://github.com/tensorflow/models/tree/8652f38d668b69cb2203fda6eade94d8fb05a551/research/slim/nets/nasnet)
  - Barret Zoph, Vijay Vasudevan, Jonathon Shlens, Quoc V. Le
  > Use NASNet's architecture and do some improvement
  > 1. use block structure(like Inception or resnet) and only search the block to improve searching time
  > 2. improve searching process that first search the network on a small dataset (cifar) and then use that network to test on larger dataset(Imagenet)
  > 3. make a comparison between random search and use reinforcement learning and show the benefit from reinforcement learning
  > 4. Do a experiment that transfer the network from classification task to detection task
