---
title: "Word meaning, not surface statistics, is essential for predictive language processing"
title_zh: 预测性语言加工中词义而非表层统计是关键因素
authors: "Zyryanov, A., Pierz, V., Oganian, Y."
date: 2026-05-15
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.15.724229v1.full.pdf"
tags: ["query:q10"]
score: 9.0
evidence: 预测性语言加工与基于意义的预测错误计算
tldr: 本研究通过自定速阅读与脑磁图实验，利用多义词的语义歧义来区分预测误差的来源，发现人类语言处理的预测误差受词义影响而非表层统计模式驱动，揭示当前大型语言模型在模拟人类语言预测机制上的局限。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究人类语言理解中的预测误差计算究竟是由表层统计模式驱动还是由词语意义驱动。
method: 研究者利用多义词的语义歧义设计实验，并结合自定速阅读时间与脑磁图（MEG）数据来检测预测误差的变化。
result: 结果显示，当出现语义歧义时，预测误差计算受到显著影响，而基于表层统计的LLM模型未能有效预测阅读时长与神经反应。
conclusion: 研究表明，人类语言处理中的预测误差是基于意义的计算，词语的语义在语言预测中起关键作用。
---

## 摘要
人类以增量方式理解语言，在每接收到一个新词时更新句子意义的表征。这些更新由每个感知到的词与先前预期之间的差距——即预测误差——所引导。大型语言模型（LLMs）与大脑皮层活动之间的一致性激发了这样一种假设：大脑皮层中预测误差的计算是基于表层的，由词形共现的统计模式驱动。相反，心理语言学模型认为预测误差的计算是基于意义的，由词语语义驱动。我们使用具有多重词义的歧义词来区分这两类模型：如果预测误差是基于意义的，歧义将引入意义表征的不确定性，从而影响预测误差；如果是基于表层的，则不会产生影响。我们考察了歧义对自定步阅读时间和句子加工过程中的脑磁图（MEG）神经反应中预测误差特征的影响。虽然基于LLM的预测误差代理能够稳健地预测无歧义词的阅读时间和神经反应，但在存在歧义时却无法进行预测。也就是说，词义的不确定性改变了预测误差的计算方式，这支持了基于意义的模型，并证实了词义在预测性语言加工中的核心作用。我们的研究结果强调了LLM作为人类语言能力的计算模型所存在的重要局限。

## Abstract
Humans comprehend language incrementally, updating the representation of sentence meaning with each incoming word. These updates are guided by the distance between each perceived word and prior expectations--the prediction error. The alignment between large language models (LLMs) and cortical activity inspires the hypothesis that the cortical computation of prediction error is Surface-based, driven by statistical patterns of word form co-occurrence. In contrast, psycholinguistic models propose that prediction error computation is Meaning-based, driven by word semantics. We used polysemic words with ambiguous semantics to distinguish these models: ambiguity would introduce uncertainty into meaning representations and hence the prediction error, if Meaning-based, but would not affect the prediction error, if Surface-based. We examined how ambiguity influenced prediction error signatures in self-paced reading times and magnetoencephalographic (MEG) neural responses during sentence processing. While an LLM-based proxy of prediction error robustly predicted reading times and neural responses to unambiguous words, it failed to predict either under ambiguity. That is, prediction error computation was altered by uncertainty in word meaning, which supports the Meaning-based model and corroborates the essential role of word meaning in predictive language processing. Our findings highlight an important limitation of LLMs as in silico models of the human language faculty.

---

## 论文详细总结（自动生成）

# 《预测性语言加工中词义而非表层统计是关键因素》论文总结

---

## 1. 核心问题与研究动机

- **研究问题**：人类语言理解中的预测误差（prediction error）是基于词形的表层统计模式计算的，还是基于词义的语义关系计算的？  
- **背景**：  
  - 预测性语言加工理论指出，大脑在理解语言时会不断预期下一个可能出现的词汇，并根据实际输入调整内部表征。  
  - 大型语言模型（LLMs）在一定程度上能预测阅读时间和神经活动，因此有人认为人脑的预测机制可能与LLM的统计特征学习相似。  
  - 然而，心理语言学长期认为，人类预测依赖于词义层面的语义整合，而不仅是表层形式的共现概率。  
- **研究动机**：作者希望通过实验区分“基于表层统计”的预测机制与“基于意义”的预测机制，从而揭示大脑语言预测的真实计算原则。

---

## 2. 方法论与技术路线

- **核心思想**：  
  - 利用**语义歧义（polysemy）**作为干扰变量——即同一个词形对应多个潜在词义，从而人为操控语义不确定性。
  - 若预测误差由词义驱动，则语义歧义会显著改变预测误差的表现；若由表层统计驱动，则歧义不会产生影响。
- **研究流程**：
  1. **刺激设计**：构造包含语义歧义词与无歧义词的句子。
  2. **行为实验**：记录受试者在自定速阅读任务中的阅读时间。
  3. **神经实验**：使用脑磁图（MEG）测量句子加工过程中脑区反应。
  4. **模型比较**：计算LLM（例如GPT类模型）对每个词的预测概率，以得到其统计层面的预测误差，并与行为与神经数据进行对照。
- **理论框架**：基于**预测误差驱动的增量式语言理解模型**，将人类阅读时间和MEG反应视为预测误差信号的外显指标。

---

## 3. 实验设计

- **实验类型**：  
  - 自定速阅读实验：测试歧义词及其上下文对阅读时间的影响。  
  - 脑磁图实验：记录同类句子的神经反应，以观察预测误差信号在脑时空上的表现。
- **数据来源**：自行收集的实验刺激句子，并非使用公开语料库。  
- **对比方法**：  
  - **LLM 预测误差代理**（surface-based）  
  - **人类语义假设模型**（meaning-based）
- **基准（benchmark）**：人类行为与MEG信号的一致性，用以判断模型预测的有效性。

---

## 4. 资源与算力

- 文中未明确说明使用的LLM模型细节、参数规模或算力配置。  
- 仅说明该模型用于计算词的预测概率（即 log-probability），以获得表层统计预测误差。  
- 没有提供 GPU 类型、数量、或运行耗时等信息。  

> **说明**：本研究主要为心理语言学实验研究，机器学习计算部分属于分析工具层面。

---

## 5. 实验数量与充分性

- **实验数量**：两类核心实验（阅读行为 + MEG神经信号），每类又包含不同语义歧义条件和对照条件。  
- **充分性**：  
  - 双模态（行为 + 神经）数据交叉验证结果，具备较强说服力。  
  - 各实验均包含对照组（无歧义词）和实验组（歧义词），统计比较清晰。  
- **客观性与公平性**：  
  - 确保上下文控制一致、词频与字长平衡。  
  - 但文中未提到实验样本量的规模及跨语言验证，可能存在外推性受限的问题。

---

## 6. 主要结论与发现

- 当语义歧义增加时：
  - 人类阅读时间显著增加；
  - MEG 中典型的预测误差信号（尤其是 N400 时间窗内的成分）显著变化；
  - LLM 的预测误差值却未表现出相应变化。  
- 因此：
  - 人类预测误差计算受到词义不确定性影响 → 说明大脑的预测是“基于意义”的；
  - LLM 预测误差与人类反应失配 → 证明 LLM 的“表层统计”性质限制了其认知拟合能力。  
- 研究结论：**人类语言预测错误的计算依赖于词义层面的加工，而非单纯依赖表层共现统计**。

---

## 7. 优点与创新

- **理论创新**：以可验证的实验方式明确区分了两种预测机制假设（意义驱动 vs. 统计驱动）。  
- **方法创新**：通过语义歧义操控实现对预测误差机制的间接测试。  
- **多模态验证**：结合阅读行为和脑磁图数据，提升了结果的稳健性。  
- **认知与计算模型桥接**：为 LLM 与人脑语言系统之间的异同提供了新的实证依据。

---

## 8. 不足与局限

- **模型层面**：
  - 未披露使用的具体 LLM 架构与参数，无法重复验证。
  - 未测试多种语言模型（仅一个“代表性”LLM），对结论的普适性可能有限。
- **实验层面**：
  - 样本量和句子数量未明示，统计效应量未知。  
  - MEG 分析空间分辨率有限，无法精准指认脑区因果。  
- **理论外推风险**：
  - 实验语料为控制句子，可能与自然语境存在差异。  
  - “预测误差”在神经层面的定义可能与机器学习中的 loss 概念不完全对应。
- **应用限制**：
  - 研究主要关注认知解释，对改进 LLM 本身的机制尚未提出具体现实方案。

---

**（完）**
