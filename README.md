# [self|semi]-supervised learning experiments
> Realistic evaluation of recent state-of-the-art self-supervised learning and semi-supervised learning algorithms


This is a repository for my bachelor’s thesis on evaluation of semi-supervised and self-supervised learning algorithms. The purpose of this project is to somewhat recreate [Realistic Evaluation of Deep Semi-Supervised Learning Algorithms](https://arxiv.org/pdf/1804.09170) paper, but with recent (as of 2020) state-of-the-art self-supervised and semi-supervised algorithms. I believe this is relevant and interesting, because we might be at the break point of achieving or surpasing supervised learning methods with self-supervised learning or semi-supervised learning (or both). So it is important to evaluate emerging algorithms in different settings (as described in aforementioned article about semi-supervised learning) along with improving them.

## Reading list

To get familiar with self-supervised learning and semi-supervised learning algorithms, which will be evaluated in this project I recommend the following articles:

- [A survey on Semi-, Self- and Unsupervised Techniques in Image Classification](https://arxiv.org/abs/2002.08721) – comprehensive survey about SOTA algorithms including consistency regularization, pseudolabeling, contrastive learning (good survey paper)
- [UDA](https://arxiv.org/abs/1904.12848v4), [Meta Pseudo Labels](https://arxiv.org/abs/2003.10580) – two semi-supervised algorithms I plan to use (SOTA in semi-supervised learning today)
- [SimCLR](https://arxiv.org/abs/2002.05709), [MoCo](https://arxiv.org/abs/1911.05722) – two self-supervised algorithms I plan to use.
- [Realistic Evaluaiton of Deep Semi-Supervised Learning Algorithms](https://arxiv.org/abs/1804.09170) – paper which describes problems with commonly used semi-supervised learning benchmarks. Most papers mentioned above (UDA, SimCLR, MoCo) use those semi-supervised learning benchmark (CIFAR-10 for example).
- [Contrastive Representation Distilation](https://arxiv.org/abs/1910.10699) distilation technique based on contrastive learning. My idea is that it could also work in semi-supervised setting (add cross entropy loss to teacher + distill it's representation on all images)

If you prefer to watch videos (great explanations):

- [Meta Pseudo Labels](https://www.youtube.com/watch?v=yhItocvAaq0), [UDA](https://www.youtube.com/watch?v=-u8Mi57BDIY)
- [SimCLR](https://www.youtube.com/watch?v=APki8LmdJwY)
- [Lecture](https://www.youtube.com/watch?v=dMUes74-nYY) on self-supervised learning (UC Berkeley CS294-158 Deep Unsupervised Learning)



## Install

To install clone this repository and run:

`pip install -e .`

## Code

Reproducing UDA results in pytorch
