

**[Biologically Inspired Mechanisms for Adversarial Robustness](https://link.zhihu.com/?target=https%3A//arxiv.org/abs/2006.16427)**

我们证明灵长类视网膜的非均匀采样和多个接受野的存在，每个偏心接受野大小范围提高了神经网络对小的对抗扰动的鲁棒性。

### 1 Introduction

The uneven distribution of cones in the primate retina results in non-uniform spatial sampling of visual stimuli. The density of sampling is highest at a fixation point on an image and decreases with distance from the fixation point. In contrast, standard CNNs accept images sampled in a uniform square grid.

Previous studies have demonstrated that incorporating the non-uniform sampling performed by the primate retina into standard networks improves predictivity of neural sites in the primate V4 cortical area, allows for better neural population control via controller images [3] and helps in generating adversarial examples that impact the accuracy of time-limited humans [22]. The first mechanism that we investigate incorporates information across multiple retinal fixation points.

灵长类动物视网膜中视锥细胞的不均匀分布导致视觉刺激的空间采样不均匀。采样密度在图像上的固定点处最高，并随着离固定点的距离而减小。相比之下，标准cnn接受在均匀的方形网格中采样的图像。


先前的研究表明，将灵长类动物视网膜进行的非均匀采样纳入标准网络可以提高灵长类动物V4皮质区域神经位点的预测性，可以通过控制器图像[3]更好地控制神经种群，并有助于生成对抗性示例，从而影响有时间限制的人类[22]的准确性。我们研究的第一种机制包含了多个视网膜注视点的信息。