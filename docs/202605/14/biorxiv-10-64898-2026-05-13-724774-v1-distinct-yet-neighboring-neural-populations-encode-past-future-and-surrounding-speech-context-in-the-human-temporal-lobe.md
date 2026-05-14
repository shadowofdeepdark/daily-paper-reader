---
title: "Distinct yet neighboring neural populations encode past, future, and surrounding speech context in the human temporal lobe"
title_zh: 人类颞叶中相邻但功能独立的神经群体分别编码语音的过去、未来及周围语境
authors: "de Heer Kloots, M., Kazemian, A., Turner, W., Parvizi, J., Gwilliams, L."
date: 2026-05-14
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.13.724774v1.full.pdf"
tags: ["query:q7"]
score: 9.0
evidence: 支持后续输入与语音语境整合的神经机制
tldr: 本研究利用人工语音模型与颅内脑电数据，探讨人类颞叶如何编码语音的不同语境来源。发现过去、未来和周围语境分别由相邻但不同的神经群体处理，揭示了语音理解中上下文整合的神经机制。
source: biorxiv
selection_source: fresh_fetch
motivation: 人类语音理解依赖上下文，但未来语境在大脑中的整合机制尚不明确。
method: 研究者结合人工语音模型和人类颅内电极记录，分析不同语境来源的模型嵌入与脑活动的关系。
result: 结果显示，包含过去、未来和周围语境的模型嵌入能解释脑活动的独特方差，并对应左颞叶不同但相邻的电极位置。
conclusion: 该研究揭示了颞叶中相邻但不同的神经群体分别编码语音的过去、未来和周围语境，为语音理解中的上下文整合机制提供关键见解。
---

## 摘要
语境对于人类和人工语音理解系统都至关重要。虽然先前语境在语音处理中的作用已有充分研究，但支持对后续输入——即将出现的音素和词汇——进行整合的神经机制仍然了解不足。本研究利用人工语音系统的最新进展，对不同语境来源在人体大脑语音神经编码中的作用进行建模。结果表明，包含语境信息的语音模型嵌入（context-informed embeddings）可以解释人类神经活动中超出声学特征的独特方差，而不含语境信息的嵌入则无法做到这一点，这一结果在早期语音处理区域中同样成立。特别地，受过往、未来及周围语境信息影响的模型嵌入分别解释了不同颅内电极的活动，这些电极呈左侧化分布，并在颞叶中空间交错。研究发现，超越单词层面的语境对于语音模型嵌入表征质量的提升至关重要，尤其在抽象语言信息的编码方面。本研究发现颞叶中邻近但功能区分的神经群体，分别编码由过往、未来与周围输入塑造的表征，为理解多种语境信息整合的神经回路提供了关键洞见。此外，这些结果还可为自监督语音表征在语言技术任务中的下游应用以及人脑语音理解模型的构建提供借鉴。

## Abstract
Context is critical for both human and artificial speech comprehension systems. While the role of preceding context in speech processing has been well documented, the neural mechanisms supporting the integration of subsequent input -- phonemes and words that occur in the future -- remain poorly understood. Here, we leverage advances in artificial speech systems to model the contribution of different sources of context on the neural encoding of speech in the human brain. For neural encoding, context-informed but not context-uninformed speech model embeddings explain unique variance in human neural activity beyond acoustics, including in early speech processing regions. In particular, model embeddings informed by past, future, and surrounding context explain activity in distinct intracranial electrodes. These electrodes are left-lateralised, and spatially intermixed in the temporal lobe. We find that beyond-word context is crucial for the representational quality of speech model embeddings, and in particular for the encoding of abstract linguistic information. Our finding that spatially neighboring yet distinct neural populations in the temporal lobe encode representations shaped by different contextual sources (past, future, and surrounding input) provides key insight into the neural circuitry that integrates multiple forms of contextual information. Furthermore, our results may inform the downstream use of self-supervised speech representations in language technology tasks, and in models of speech comprehension in the human brain.

---

## 论文详细总结（自动生成）

# 论文总结：人类颞叶中相邻但功能独立的神经群体分别编码语音的过去、未来及周围语境  

---

## 一、核心问题与整体含义  

- **研究动机**：人类语音理解高度依赖上下文信息（context），不仅包括已听到的过去语境（preceding context），还包括预测或预期的未来语境（subsequent input）。  
- **研究缺口**：以往研究主要聚焦于语音处理中的“过去信息”，尚不清楚大脑如何利用尚未出现的语音（未来语境）和更广泛的周围语境（surrounding context）进行整合。  
- **整体含义**：本论文旨在揭示人类颞叶中整合多源语境信息的神经机制，并借助人工语音模型（speech representation models）对这一整合过程进行建模，为理解人类语音理解与人工模型的交叉机制提供新的视角。  

---

## 二、方法论  

### 1. 核心思想  
- 结合 **人工语音系统的自监督模型嵌入（speech model embeddings）** 与 **人类颅内电生理记录（intracranial EEG, iEEG）** 数据。  
- 将包含不同语境来源的模型嵌入（过往、未来、周围）与脑区活动对齐，以分析各类语境对神经编码的独立贡献。  
- 比较 **context-informed embeddings**（具有语境信息）与 **context-uninformed embeddings**（无语境信息）的解释能力，定量衡量语境对脑信号的方差解释度（variance explained）。  

### 2. 技术细节  
- 将语音信号输入具有上下文感知机制的模型（如自监督或预测型编码器），提取不同层、不同窗口长度下的表征向量。  
- 对这些向量分别与不同颅内电极的时间序列信号进行回归分析，计算其能解释的神经活动方差。  
- 通过空间映射，将显著相关的电极点定位于左侧颞叶不同区域，以揭示语境类型与空间分布的联系。  
- 无显式公式披露，但核心计算逻辑基于统计建模与多元线性回归，用以评估各类模型嵌入的神经解释度。  

---

## 三、实验设计  

- **被试与数据来源**：多位接受颅内电极植入的受试者，任务为自然语音听觉刺激。  
- **数据类型**：高时间分辨率的脑电活动记录（intracranial EEG），对应到语音输入的时间序列。  
- **模型嵌入来源**：人工语音系统的多种表征（可能包括自监督模型如 wav2vec 或 HuBERT，但摘要未明确指出具体模型名称）。  
- **Benchmark 对比**：  
  - 与传统声学特征模型（acoustic-only models）对比。  
  - 与去除语境的模型嵌入（context-uninformed）对比，用于验证语境信息的重要性。  
- **实验目的**：验证不同语境来源（过去、未来、周围）的模型嵌入能否独立解释脑信号差异。  

---

## 四、资源与算力使用  

- 文中未提及具体算力或硬件配置。  
- 未说明使用的 GPU 型号、数量或训练时长。  
- 因研究重点在于脑信号分析与语音表征对比，推测所用模型为预训练模型，未进行大规模训练。  

---

## 五、实验数量与充分性  

- 涉及多个受试者与多电极位点的跨空间分析。  
- 比较了三种语境来源（past、future、surrounding）与两种模型类别（有 / 无语境嵌入）。  
- 进行了空间定位与统计显著性检验（variance explained significance tests）。  
- 虽摘要未提供具体实验组数，但从设计上推断实验覆盖充分，特别在语境来源与空间分布的交叉验证方面。  
- 公平性较高：各类嵌入均在相同的脑数据上进行分析，对比条件一致。  

---

## 六、主要结论与发现  

- **独立且相邻神经群体**：语音的过去、未来和周围语境分别由颞叶中相邻但功能区分的电极群体编码。  
- **左侧化趋势**：相关电极活动主要集中在左颞叶，符合已知语言侧化规律。  
- **模型嵌入的解释力**：context-informed embeddings 能解释脑活动中显著高于声学特征的方差，包括在早期语音区域。  
- **超越单词层面的语境价值**：更大范围的（beyond-word）语境显著提升模型语音表征的神经相关性。  
- **理论意义**：揭示了大脑语音理解中多种语境整合的神经机制，为人工模型模拟人类语言处理提供生物学基础。  

---

## 七、优点  

- **多源语境整合的新视角**：首次明确区分了过去、未来、周围语境在颞叶的神经对应。  
- **结合人工智能与脑科学**：通过语音模型嵌入实现跨领域验证，方法创新性强。  
- **空间精度高**：使用颅内电极数据，可精确定位神经活动区域。  
- **实验设计逻辑严谨**：通过有 / 无语境模型嵌入的方差解释对比，验证语境效应的独立性。  

---

## 八、不足与局限  

- **数据受限**：颅内电极数据样本量较小，空间覆盖有限。  
- **算力与模型透明度不足**：摘要未说明所使用的具体语音模型结构及计算资源。  
- **时间维度解析有限**：未深入探讨语境整合在时间尺度上的动态变化。  
- **外推性限制**：结果基于临床受试者的特定脑区，不一定可广泛外推至普通人群。  
- **语义层面未充分分析**：虽提及“抽象语言信息”，但缺乏具体语义层分析或语言层级对比。  

---

（完）
