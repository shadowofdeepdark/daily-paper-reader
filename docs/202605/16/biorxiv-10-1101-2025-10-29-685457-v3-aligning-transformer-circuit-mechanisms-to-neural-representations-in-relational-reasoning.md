---
title: Aligning transformer circuit mechanisms to neural representations in relational reasoning
title_zh: 将 Transformer 电路机制与神经表征对齐以研究关系推理
authors: "Hearne, L. J., Robinson, C. N., Cocchi, L., Ito, T."
date: 2026-05-14
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.29.685457v3.full.pdf"
tags: ["query:profile-1"]
score: 6.5
evidence: 将Transformer电路机制与推理中的神经表征对齐
tldr: 本研究探讨了人类与Transformer在关系推理中的计算相似性，通过7T fMRI与拉丁方任务发现Transformer能泛化推理任务，其位置编码与视觉皮质活动对应、注意力机制反映任务复杂度，并与前顶叶及默认网络对应，揭示注意力机制是复杂推理的核心计算基础。
source: biorxiv
selection_source: fresh_fetch
motivation: 研究人工智能模型与人脑在关系推理中的计算机制是否存在相似性。
method: 结合7T fMRI人类神经成像与Transformer模型分析拉丁方任务的关系推理过程。
result: Transformer能可靠地泛化推理任务，并表现出与人类大脑视觉及前顶叶网络的对应关系。
conclusion: 注意力机制在人工和人类推理中都体现出关键作用，是研究高级认知的有效模型。
---

## 摘要
关系推理，即理解元素之间关联的能力，是人类智力的一个标志性特征，但其计算基础仍不明确。在本研究中，我们结合人类神经影像（7T fMRI）与人工神经网络建模，以识别与人类推理计算相对应的电路层面类比。通过拉丁方任务（Latin Square Task），我们发现人类与 Transformer 模型均能可靠地进行任务泛化，而认知神经科学中使用的标准架构则不能。对 Transformer 各组成部分的分析揭示了不同的计算功能：位置编码捕捉了任务的空间结构，并与视觉皮层中的表征相一致；而注意力机制则编码关系结构，并映射到顶叶-额叶网络与默认模式网络。注意力权重能够追踪任务的关系复杂性，为推理需求提供了计算类比。这些结果加深了我们对支撑复杂推理的核心算法计算的认识，突显了基于注意力的架构在研究高级认知的神经和计算基础方面的强大潜力。

## Abstract
Relational reasoning, the capacity to understand how elements relate to one another, is a defining feature of human intelligence, yet its computational basis remains unclear. Here, we combined human neuroimaging (7T fMRI) with artificial neural network modeling to identify circuit-level analogues of human reasoning computations. Using the Latin Square Task, we found that humans and transformers were able to generalize the task reliably, while standard architectures used in cognitive neuroscience could not. Analysing the transformer components revealed distinct computational roles: positional encoding captured the spatial structure of the task and aligned with representations in visual cortex, whereas attention encoded relational structure and mapped onto frontoparietal and default-mode networks. Attention weights tracked the relational complexity of the task, providing a computational analogue of reasoning demands. These results advance knowledge on the core algorithmic computations supporting complex reasoning, highlighting attention-based architectures as powerful models for investigating the neural and computational basis of higher cognition.