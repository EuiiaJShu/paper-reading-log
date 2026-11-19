# 使用卷积神经网络进行ImageNet分类

## Abstract

<img width="2210" height="1121" alt="image" src="https://github.com/user-attachments/assets/5eea5106-8a2b-4297-908d-ee11a43face6" />
我们训练了一个大型深度卷积神经网络，用于将 ImageNet LSVRC-2010 竞赛中的 120 万张高分辨率图像分类为 1000 个不同的类别。在测试集上，我们取得了 37.5% 的 Top-1 错误率和 17.0% 的 Top-5 错误率，这一结果显著优于当时的最先进水平。该神经网络包含 6000 万个参数和 65 万个神经元，由 5 个卷积层（其中部分卷积层后接最大池化层）和 3 个全连接层组成，最后通过一个 1000 路的 Softmax 层输出结果。为了加快训练速度，我们使用了非饱和神经元，并采用了基于 GPU 的高效卷积运算实现方式。为减少全连接层中的过拟合现象，我们应用了一种新近提出的、被证明非常有效的正则化方法——“Dropout”。此外，我们还将该模型的一个变体应用于 ILSVRC-2012 竞赛，并以 15.3% 的 Top-5 测试错误率夺得冠军，而排名第二的参赛方案其错误率为 26.2%。


| 词汇 | 释义 |
| :--- | :--- |
| $\color{#FFB300}{\text{high-resolution}}$ | 高分辨率 |
| $\color{#FFB300}{\text{state-of-the-art}}$ | 当前最高发展水平 |
| $\color{#FFB300}{\text{parameter}}$ | 参数 |
| $\color{#FFB300}{\text{softmax}}$ | 一个函数名称 |
| $\color{#FFB300}{\text{non-saturating}}$ | 非饱和 |
| $\color{#FFB300}{\text{implementation}}$ | 执行 |
| $\color{#FFB300}{\text{overfitting}}$ | 过拟合 |
| $\color{#FFB300}{\text{employ}}$ | 采用 |
| $\color{#FFB300}{\text{regularization}}$ | 正则化 |
| $\color{#FFB300}{\text{winning}}$ | adj.获胜的 |
| $\color{#FFB300}{\text{entry}}$ | 参赛作品 |

| 短语 | 释义 |
| :--- | :--- |
| $\color{#88D485}{\text{consist of}}$ | 由...组成 |
| $\color{#88D485}{\text{be followed by }}$ | 随后是.../后接... |
| $\color{#88D485}{\text{enter A in B}}$ | 将A应用于B |
| $\color{#88D485}{\text{a variant of}}$ | ...的一种变体 |
| $\color{#88D485}{\text{achieved by}}$ | 由...实现 |
