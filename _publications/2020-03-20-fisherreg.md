---
title: "Bayesian Transfer Learning for Object Detection in Remote Sensing Images"
collection: publications
permalink: /publication/2020-03-20-fisherreg
date: 2020-03-20
venue: 'IEEE Transactions on Geoscience Remote Sensing'
paperurl: 'https://doi.org/10.1109/TGRS.2020.2983201'
codeurl: 'https://github.com/wasaCheney/FisherReg'
citation: 'Changsheng Zhou, Jiangshe Zhang, Junmin Liu, Chunxia Zhang, Guang Shi, Junying Hu.
&quot;Bayesian Transfer Learning for Object Detection in Remote Sensing Images.&quot;
<i>IEEE Transactions on Geoscience Remote Sensing</i>, online, 2020, 0(0):1-15.'
excerpt: 'In the literature of object detection in optical remote
sensing images, a popular pipeline is first modifying an off-the-
shelf deep neural network, then initializing the modified network
by pretrained weights on a source data set, and finally fine-tuning
the network on a target data set. The procedure works well in
practice but might not make full use of underlying knowledge
implied by pretrained weights. In this article, we propose a
novel method, referred to as Fisher regularization, for efficient
knowledge transferring. Based on Bayes’ theorem, the method
stores underlying knowledge into a Fisher information matrix
and fine-tunes parameters based on the knowledge. The proposed
method would not introduce extra parameters and less sensitive
to hyperparameters than classical weight decay. Experiments on
NWPUVHR-10 and DOTA data sets show that the proposed
method is effective and works well with different object detectors.'
---
<!-- /images/... -->
![fisherreg](/images/fisherreg.png)

Bibtex:
```
@ARTICLE{9066887,
  author={Changsheng {Zhou} and Jiangshe {Zhang} and Junmin {Liu} and Chunxia {Zhang} and Guang {Shi} and Junying {Hu}},
  journal={IEEE Transactions on Geoscience and Remote Sensing},
  title={Bayesian transfer learning for object detection in optical remote sensing images},
  year={2020},
  volume={0},
  number={0},
  pages={1-15}
  }
```
<!-- excerpt: 'This paper gives an explanation about pre-training initialization and proposes Bayesian transfer learning with FisherReg for object detection in remote sensing images.' -->
<!-- This paper is about the number 3. The number 4 is left for future work. -->
<!--  -->
<!-- [Download paper here](http://academicpages.github.io/files/paper3.pdf) -->
<!--  -->
<!-- Recommended citation: Your Name, You. (2015). "Paper Title Number 3." <i>Journal 1</i>. 1(3). -->
