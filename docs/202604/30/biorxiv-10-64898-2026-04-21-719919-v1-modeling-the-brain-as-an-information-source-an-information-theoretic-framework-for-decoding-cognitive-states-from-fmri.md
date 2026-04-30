---
title: "Modeling the Brain as an Information Source: An Information-Theoretic Framework for Decoding Cognitive States from fMRI"
title_zh: 将大脑建模为信息源：一个基于信息论的框架用于从fMRI解码认知状态
authors: "Degirmendereli, G. G., Ahmadkhan, A., Yarman Vural, F. T."
date: 2026-04-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.21.719919v1.full.pdf"
tags: ["query:q7"]
score: 6.5
evidence: 用于在任务期间从 fMRI 解码认知状态的信息论框架
tldr: 本文提出一种基于信息论的新框架，将脑区视为互相作用的信息源，通过熵和KL散度分析fMRI数据以解码认知状态。该方法能有效识别活跃脑区和区分认知阶段，为理解脑网络与认知活动关系提供了新思路。
source: biorxiv
selection_source: fresh_fetch
motivation: 研究旨在通过信息论视角理解脑区协同的认知机制。
method: 提出了基于熵和动态、静态KL散度的脑区信息源模型，用于分析fMRI数据。
result: 模型在复杂问题解决任务中能准确区分认知阶段与专业水平。
conclusion: 该框架为理解脑区之间的信息交互及认知状态解码提供了新的信息论工具。
---

## 摘要
本研究探讨了一个假设：大脑的解剖区域可以被建模为相互补充且相互连接的信息源。我们提出了一个新的框架，用以利用信息论度量分析认知任务中这些交互信息源的动态特征。具体而言，我们引入了动态和静态熵模型，用来量化单个解剖区域的信息含量，既包括随时间变化的情况，也包括在特定认知需求下的表现。此外，我们基于动态和静态的Kullback-Leibler（KL）散度构建了两个网络模型，用于刻画区域间的相互作用。

我们在复杂问题解决（Complex Problem Solving, CPS）任务中的fMRI数据上测试了上述模型，并获得了令人鼓舞的结果。熵值能够成功识别被激活的脑区，与现有神经科学文献一致。此外，我们的Kullback-Leibler网络模型在区分CPS任务的计划和执行阶段，以及区分专家与新手问题解决者方面表现出较高的准确度。这些发现表明，我们基于信息论的方法在识别活跃脑区、刻画心理状态以及揭示与认知任务相关的脑网络方面具有潜在应用价值。

## Abstract
This study explores the hypothesis that the anatomical regions of the brain can be modeled as complementary and interconnected information sources. We propose a novel framework for analyzing the dynamics of these interacting information sources during cognitive tasks using information-theoretic measures. Specifically, we introduce dynamic and static entropy models to quantify the information content within individual anatomical regions, both over time and in relation to specific cognitive demands. Furthermore, we develop two network models based on the dynamic and static Kullback-Leibler (KL) divergence to characterize the regional interactions.

Testing our models on fMRI data recorded during Complex Problem Solving (CPS) tasks reveals promising results. Entropy values successfully identify activated brain regions, consistent with the existing neuroscience literature. Furthermore, our Kullback-Leibler network models demonstrate high accuracy in distinguishing between the planning and execution phases of CPS, as well as in differentiating between expert and novice problem solvers. These findings suggest that our information-theoretic approach holds promise for identifying active brain regions, characterizing mental states, and elucidating brain networks associated with cognitive tasks.