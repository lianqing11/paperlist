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



##Semantic Segmentation


- rethinking Atrous Convolution for Semantic Image Segmentation [[pdf]](https://arxiv.org/abs/1706.05587)
  -  Liang-Chieh Chen, George Papandreou, Florian Schroff, Hartwig Adam
  > Add Atrous Spatial Pyramid Pooling on the end of the model a) different rate's atrous and convolution b)image level feature
  > Multi-grid Method
  > Once reduce stride one time ,every subsequent conv's atrous rate should time 2
  > Test if the network can go deeper with resent50 and resnet101 which show slightly improve.



- Pyramid Scene Parsing Network [[pdf]](https://arxiv.org/abs/1612.01105)[[code]](https://github.com/hszhao/PSPNet)
  -  Hengshuang Zhao, Jianping Shi, Xiaojuan Qi, Xiaogang Wang, Jiaya Jia
  > On the last layer add a Pyramid network with multi brach which first downsampling, then conv to extract feature or context information and then upsamping to the same size, finally concat them

 -
