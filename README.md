# useful-paper

# Semantic Segmentation
1. Fully Convolutional Networks for Semantic Segmentation ([arxiv](http://arxiv.org/abs/1411.4038))

　　主要贡献: - 使用反卷积层进行上采样，提出了跳跃连接来改善上采样的粗糙程度。
             - 反卷积层进行上采样时，不是使用简单的双线性插值，而是通过学习实现插值操作（利用双线性插值来初始化反卷积层的参数）。


# Video Object Segmentation

1.Instance Embedding Transfer to Unsupervised Video Object Segmentation ([arxiv](https://arxiv.org/pdf/1801.00908v1.pdf))

　　evaluate: **Instance Networks**. instance embedding vector for each pixel; instance embeddings allow us to link objects together over time. we adapt the instance networks trained on static images to video object segmentation and **incorporate the embeddings with objectness and optical flow features, without model retraining or online fine-tuning.**

2.Instance Embedding Transfer to Unsupervised Video Object Segmentation ([arxiv](https://arxiv.org/pdf/1801.00908v1.pdf))
