## 		Adversarial training for probabilistic spiking neural networks

摘要：

Classifiers trained using conventional empirical risk minimization or maximum likelihood methods are known to suffer dramatic performance degradations when tested over examples adversarially selected based on knowledge of the classifier’s decision rule. Due to the prominence of Artificial Neural Networks (ANNs) as classifiers, their sensitivity to adversarial examples, as well as robust training schemes, have been recently the subject of intense investigation. In this paper, for the first time, the sensitivity of spiking neural networks (SNNs), or third-generation neural networks, to adversarial examples is studied. The study considers rate and time encoding, as well as rate and first-to-spike decoding. Furthermore, a robust training mechanism is proposed that is demonstrated to enhance the performance of SNNs under white-box attacks

使用传统的经验风险最小化或最大似然方法训练的分类器在基于分类器决策规则的知识对抗性选择的示例进行测试时，已知会遭受显着的性能下降。由于人工神经网络(ann)作为分类器的突出地位，其对对抗性示例的敏感性以及鲁棒性训练方案最近一直是激烈研究的主题。==本文首次研究了脉冲神经网络(SNNs)或第三代神经网络对对抗实例的敏感性。该研究考虑了速率和时间编码，以及速率和首峰解码。此外，提出了一种鲁棒的训练机制，该机制被证明可以提高snn在白盒攻击下的性能==

### I. INTRODUCTION

A promising alternative paradigm is offered by Spiking Neural Networks (SNNs), in which synaptic input and neuronal output signals are sparse asynchronous binary spike trains [5]. Unlike ANNs, SNNs are hybrid digital-analog machines that make use of the temporal dimension, not just as a neutral substrate for computing, but as a means to encode and process information [7]

尖峰神经网络(snn)提供了一种有希望的替代范例，其中突触输入和神经元输出信号是稀疏的异步二进制尖峰序列[5]。与人工神经网络不同，snn是数字-模拟混合机器，它利用时间维度，不仅作为计算的中性基质，而且作为编码和处理信息的手段[7]



In this paper, for the first time, the sensitivity of SNNs trained via ML is studied under white-box adversarial attacks, and a robust training mechanism is proposed that is demonstrated to enhance the performance of SNNs under adversarial examples. Specifically, we focus on a two-layer SNN (see Fig. 1), and consider rate and time encoding, as well as rate and first-to-spike decoding [13]. Our results illuminate the sensitivity of SNNs to adversarial example under different encoding and decoding schemes, and the effectiveness of robust training methods.

本文首次研究了基于ML训练的snn在白盒对抗攻击下的敏感性，提出了一种鲁棒训练机制，并证明了该机制可以增强snn在对抗示例下的性能。具体来说，我们关注的是一个双层SNN(见图1)，并考虑了速率和时间编码，以及速率和首峰解码[13]。我们的研究结果说明了snn在不同编码和解码方案下对对抗样本的敏感性，以及鲁棒训练方法的有效性。



### II. SNN-BASED CLASSIFICATION

### III. DESIGNING ADVERSARIAL EXAMPLES

In this work, we consider white-box attacks based on full knowledge of the model,