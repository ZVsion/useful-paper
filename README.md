# useful-paper

# Semantic Segmentation
1. Fully Convolutional Networks for Semantic Segmentation ([arxiv](http://arxiv.org/abs/1411.4038))([code](https://github.com/shekkizh/FCN.tensorflow))

　　主要贡献: 1.使用反卷积层进行上采样，提出了跳跃连接来改善上采样的粗糙程度。 2.反卷积层进行上采样时，不是使用简单的双线性插值，而是通过学习实现插值操作（利用双线性插值来初始化反卷积层的参数）。

2. Semantic Image Segmentation with Deep Convolutional Nets and Fully Connected CRFs. ([arxiv](https://arxiv.org/pdf/1412.7062.pdf))([code](https://github.com/muyang0320/tensorflow-deeplab-resnet-crf))

　　evaluation: This paper shows that responses at the final layer of DCNNs are not sufficiently localized for accurate object segmentation and overcomes this problem through combining the responses at the final DCNN layer with a fully connected CRF. The authors boost their model's ability to capture fine details by employing a fully-connected CRF.
  
3. Conditional Random Fields as Recurrent Neural Networks. ([arxiv](https://arxiv.org/abs/1502.03240))([code](https://github.com/sadeepj/crfasrnn_keras))

　　evaluation: This paper formulate mean-field approximate inference for the CRF as RNN (CRF-RNN network). This network can be plugged in as a part of a CNN to obtain a deep network that has desirable properties of both CNNs and CRFs. Importantly, this system can train the whole deep network end-to-end with the usual back-propagation algorithm, avoiding offline post-processing methods for object delineation.

4. PixelNet
 
    Evaluation: 探索关于一般像素级预测问题的方法，从低水平的边缘预测，到中水平的表面预测，到高水平的语义分割。 
    贡献: 
        (1)我们通过实验证明，由于像素间的空间相关性，每个图像只采样少量样本就足够用于学习。更重要的是，在不能提前的情况下(not early possible)，采样允许我们可以训练端到端的特定的非线性模型。并探索在基于FCN的框架下，改进效率和性能的几种途径。 
        (2)与绝大多数使用预训练网络的模型相反，我们展示了像素级优化可以用来训练模型，或者用简单的随机高斯初始化从头开始。直观来说，和图像级标签相比，像素级标签提供了大量可监督的标签。不需要其他的数据，们的模型比PASCAL VOC-2012上的先前的无监督/自我监督的语义分割方法更胜一筹，在对表面法线估计的预处理模型的微调上，我们的模型也很有竞争力。 
        (3）我们使用一个单一的体系结构，没有太多的参数修改，在BSDS我们展示了边缘检测性能，在NYUDv2深度数据集我们展示了表面正态估计，以及在PASCAL-Context数据集上我们展示了语义分割，都达到了最先进的效果。
# Video Object Segmentation

1.Instance Embedding Transfer to Unsupervised Video Object Segmentation ([arxiv](https://arxiv.org/pdf/1801.00908v1.pdf))

　　evaluation: **Instance Networks**. instance embedding vector for each pixel; instance embeddings allow us to link objects together over time. we adapt the instance networks trained on static images to video object segmentation and **incorporate the embeddings with objectness and optical flow features, without model retraining or online fine-tuning.**

2.Video Semantic Object Segmentation by Self-Adaptation of DCNN ([arxiv](https://arxiv.org/pdf/1711.08180v1.pdf))

　　evaluation: 可以使用分割后较好的帧来继续优化网络参数（self-adaptation）。
