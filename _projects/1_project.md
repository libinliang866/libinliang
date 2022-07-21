---
layout: page
title: Deep Maxout Network Gaussian Process
description: Study the initial distribution of Deep Maxout Network with inifinite width
img: assets/img/maxout_network.png
importance: 1
category: work
---


Infinite width neural network as Gaussain process(GP) was first derived in Neal(1996). Given a proper initialization, the output of one layer neural network becomes a GP with kernel depending on the nonlinearity activation. In Lee(2019),Matthews(2018), the infinite width deep neural network(DNN) as GP  was derived and the kernel has a compositional structure depending on the number of depth and the nonlinearity activation in the network. Moreover, they found GP inference with DNN kernel often outperforms their finite width counterparts. Both Neal(1996).
and Lee(2019)studied neural networks with activation applied on single linear combination of the input. Following the infinite width scheme,  Novak(2018) and Garriga(2018) developed the
GP kernel based on the 
deep convolutional neural networks(CNN) structure and \citet{DBLP:journals/corr/abs-1910-12478} developed the
GP kernel based on neural structures such as recurent neural networks(RNN), transformer etc. 

Although it is widely utilized in application, the deep maxout network has never been derived as GP among previous works. The activation in maxout network  applied on multiple linear combinations of the input(or previous layers) so that the the implementation in Neal(1996) and Lee(2017) can not directly apply here.
In this work, we formally derive deep, infinite width maxout network as GP and characterize its corresponding kernel as a compositional structure. Moreover, we give a efficient method based on numerical integration and interpolation to implement the kernel. We apply the deep maxtout network kernel in GP regression inference on CIFAR10 dataset and it can achieve encouraging results in numerical study.
