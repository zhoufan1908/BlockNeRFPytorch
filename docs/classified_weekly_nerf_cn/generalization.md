
每周分类神经辐射场 - generalization ![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)
===========================================================================================================================================
## 按类别筛选: [全部](../weekly_nerf_cn.md) | [动态](./dynamic.md) | [编辑](./editing.md) | [快速](./fast.md) | [泛化](./generalization.md) 
## [光照](./lighting.md) | [重建](./reconstruction.md) | [纹理](./texture.md) | [语义](./semantic.md) | [姿态-SLAM](./pose-slam.md) | [其他](./others.md) 
## 大部分为机器翻译，少数论文手动翻译，有翻译错误可以PR修复。
## Jul31 - Aug6, 2022
  - [NeSF: 用于 3D 场景的可概括语义分割的神经语义场](https://research.google/pubs/pub51563/) | [code]
    > 我们提出了 NeSF，一种从预训练的密度场和稀疏的 2D 语义监督产生 3D 语义场的方法。我们的方法通过利用将 3D 信息存储在神经域中的神经表示来避开传统的场景表示。尽管仅由 2D 信号监督，我们的方法能够从新颖的相机姿势生成 3D 一致的语义图，并且可以在任意 3D 点进行查询。值得注意的是，NeSF 与任何产生密度场的方法兼容，并且随着预训练密度场质量的提高，其准确性也会提高。我们的实证分析证明了在令人信服的合成场景上与竞争性 2D 和 3D 语义分割基线相当的质量，同时还提供了现有方法无法提供的功能。
  - [Transformers as Meta-Learners for Implicit Neural Representations, ECCV2022](https://arxiv.org/abs/2208.02801) | [***``[code]``***](https://yinboc.github.io/trans-inr/)
    > 近年来，隐式神经表示 (INR) 已经出现并显示出其优于离散表示的优势。然而，将 INR 拟合到给定的观测值通常需要从头开始使用梯度下降进行优化，这是低效的，并且不能很好地泛化稀疏的观测值。为了解决这个问题，大多数先前的工作都训练了一个超网络，该超网络生成单个向量来调制 INR 权重，其中单个向量成为限制输出 INR 重建精度的信息瓶颈。最近的工作表明，通过基于梯度的元学习，可以在没有单向量瓶颈的情况下精确推断 INR 中的整个权重集。受基于梯度的元学习的广义公式的启发，我们提出了一个公式，该公式使用 Transformer 作为 INR 的超网络，它可以使用专门作为集合到集合映射的 Transformer 直接构建整个 INR 权重集。我们展示了我们的方法在不同任务和领域中构建 INR 的有效性，包括 2D 图像回归和 3D 对象的视图合成。我们的工作在 Transformer 超网络和基于梯度的元学习算法之间建立了联系，我们为理解生成的 INR 提供了进一步的分析。
  - [VolTeMorph：体积表示的实时、可控和可泛化动画](https://arxiv.org/pdf/2208.00949) | [***``[code]``***](https://arxiv.org/pdf/2208.00949)
    > 最近，用于场景重建和新颖视图合成的体积表示越来越受欢迎，这使人们重新关注在高可见度下对体积内容进行动画处理质量和实时性。虽然基于学习函数的隐式变形方法可以产生令人印象深刻的结果，但它们对于艺术家和内容创作者来说是“黑匣子”，它们需要大量的训练数据才能进行有意义的概括，而且它们不会在训练数据之外产生现实的外推。在这项工作中，我们通过引入一种实时、易于使用现成软件进行编辑并且可以令人信服地推断的体积变形方法来解决这些问题。为了展示我们方法的多功能性，我们将其应用于两个场景：基于物理的对象变形和远程呈现，其中化身使用混合形状进行控制。我们还进行了彻底的实验，表明我们的方法优于结合隐式变形的体积方法和基于网格变形的方法。
## Jul24 - Jul30, 2022
  - [ZEPI-Net：通过内部跨尺度对极平面图像零样本学习的光场超分辨率, Neural Processing Letters (2022)](https://link.springer.com/article/10.1007/s11063-022-10955-x) | [code]
    > 光场 (LF) 成像的许多应用都受到空间角分辨率问题的限制，因此需要高效的超分辨率技术。最近，基于学习的解决方案比传统的超分辨率（SR）技术取得了显着更好的性能。不幸的是，学习或训练过程在很大程度上依赖于训练数据集，这对于大多数 LF 成像应用程序来说可能是有限的。在本文中，我们提出了一种基于零样本学习的新型 LF 空间角 SR 算法。我们建议在核平面图像 (EPI) 空间中学习跨尺度可重用特征，并避免显式建模场景先验或从大量 LF 中隐式学习。最重要的是，在不使用任何外部 LF 的情况下，所提出的算法可以同时在空间域和角域中超分辨 LF。此外，所提出的解决方案没有深度或视差估计，这通常由现有的 LF 空间和角度 SR 采用。通过使用一个简单的 8 层全卷积网络，我们表明所提出的算法可以产生与最先进的空间 SR 相当的结果。我们的算法在多组公共 LF 数据集上的角度 SR 方面优于现有方法。实验结果表明，跨尺度特征可以很好地学习并在 EPI 空间中用于 LF SR。
  - [ObjectFusion：具有神经对象先验的准确对象级 SLAM, Graphical Models, Volume 123, September 2022](https://www.sciencedirect.com/science/article/pii/S1524070322000418) | [code]
    > 以前的对象级同步定位和映射 (SLAM) 方法仍然无法以有效的方式创建高质量的面向对象的 3D 地图。主要挑战来自如何有效地表示对象形状以及如何将这种对象表示有效地应用于准确的在线相机跟踪。在本文中，我们提供 ObjectFusion 作为静态场景中的一种新颖的对象级 SLAM，它通过利用神经对象先验，有效地创建具有高质量对象重建的面向对象的 3D 地图。我们提出了一种仅具有单个编码器-解码器网络的神经对象表示，以有效地表达各种类别的对象形状，这有利于对象实例的高质量重建。更重要的是，我们建议将这种神经对象表示转换为精确测量，以共同优化对象形状、对象姿态和相机姿态，以实现最终准确的 3D 对象重建。通过对合成和真实世界 RGB-D 数据集的广泛评估，我们表明我们的 ObjectFusion 优于以前的方法，具有更好的对象重建质量，使用更少的内存占用，并且以更有效的方式，尤其是在对象级别。
  - [通过 NeRF Attention 进行端到端视图合成](https://arxiv.org/abs/2207.14741) | [code]
    > 在本文中，我们提出了一个用于视图合成的简单 seq2seq 公式，其中我们将一组光线点作为输入和输出与光线相对应的颜色。在这个 seq2seq 公式上直接应用标准转换器有两个限制。首先，标准注意力不能成功地适应体积渲染过程，因此合成视图中缺少高频分量。其次，将全局注意力应用于所有光线和像素是非常低效的。受神经辐射场 (NeRF) 的启发，我们提出了 NeRF 注意力 (NeRFA) 来解决上述问题。一方面，NeRFA 将体积渲染方程视为软特征调制过程。通过这种方式，特征调制增强了具有类似 NeRF 电感偏置的变压器。另一方面，NeRFA 执行多阶段注意力以减少计算开销。此外，NeRFA 模型采用光线和像素转换器来学习光线和像素之间的相互作用。 NeRFA 在四个数据集上展示了优于 NeRF 和 NerFormer 的性能：DeepVoxels、Blender、LLFF 和 CO3D。此外，NeRFA 在两种设置下建立了新的 state-of-the-art：单场景视图合成和以类别为中心的新颖视图合成。该代码将公开发布。