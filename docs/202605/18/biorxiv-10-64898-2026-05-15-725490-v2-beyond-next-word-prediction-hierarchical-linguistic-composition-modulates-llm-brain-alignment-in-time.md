---
title: "Beyond next-word prediction: hierarchical linguistic composition modulates LLM-brain alignment in time"
title_zh: 超越下一词预测：层级语言组合在时间上调节 LLM 与大脑的对齐
authors: "Zhao, J., Brennan, J. R."
date: 2026-05-17
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.15.725490v2.full.pdf"
tags: ["query:profile-1"]
score: 9.0
evidence: 层级语言组合及利用脑电图研究大模型与大脑在理解过程中的对齐
tldr: 本文研究大型语言模型与人类脑活动在语言理解中的对齐机制，通过在受控条件下操纵英语句子的句法、组合语义与联想语义并利用EEG测量，发现句法结构提升模型-脑对齐，而组合语义削弱对齐，揭示了语言模型与人脑表征差异。
source: biorxiv
selection_source: fresh_fetch
motivation: 研究旨在探讨大型语言模型与人脑语言处理间的表征对齐是否源于层级语言结构特征。
method: 研究通过控制预测性、操纵句法与语义特征，并利用线性编码模型分析GPT2-XL的上下文嵌入与EEG信号的对齐变化。
result: 实验发现句法结构增强了模型与脑电信号的对齐，而组合语义削弱了对齐，联想语义无显著影响。
conclusion: 结果表明LLMs与人脑在句法表征上有相似性，但组合语义处理更具人脑特性。
---

## 摘要
大型语言模型（LLMs）的内部表征与人类在语言理解过程中的神经活动存在相关性，或称为“对齐”。一种观点认为，这种对齐反映了 LLMs 与人类对统计模式的共同敏感性；另一种观点则认为，它部分反映了这些系统中共同语言表征的出现。本文研究层级语言组合这一被认为是人类语言的基本属性是否驱动了 LLM 与大脑的对齐。为此，我们在脑电图（EEG）实验中向 LLM 和人类参与者呈现了经过语法、组合语义及联想语义操控的英文句子。我们在可预测性上匹配了这些经过语言操控的刺激，从而能区分由语言结构与统计因素所引发的对齐。通过比较在可预测性匹配条件下使用线性编码模型获得的 LLM-EEG 对齐得分，我们评估语言操控如何影响人类 EEG 阅读数据与从 GPT2-XL 隐藏层逐词提取的上下文嵌入之间的对齐。结果显示三种主要模式：（1）具有句法结构的词序提高了对齐度；（2）具有组合语义的句子降低了对齐度；（3）联想语义不影响对齐。这些观察到的语言因素对 LLM-EEG 对齐的调节作用超越了可预测性。我们的结果表明，LLM 与人脑在编码联想语义以及至少部分句法结构方面具有相似性，而组合语义更为人脑独有。

## Abstract
The internal representations of large language models (LLMs) correlate, or "align" , with human neural activity during language comprehension. One view holds that this alignment reflects shared sensitivity to statistical patterns in LLMs and humans, while others hold that it reflects, at least in part, the emergence of shared linguistic representations in these systems. Here, we investigate whether hierarchical linguistic composition, a property believed to be fundamental to human language, drives LLM-brain alignment. To this end, we manipulated syntax, compositional semantics, and associative semantics in English sentences that were presented to both an LLM and human participants during an electroencephalography (EEG) experiment. We matched linguistically manipulated stimuli in predictability, which allows us to tease apart alignment induced by linguistic structure from statistical factors. By comparing LLM-EEG alignment scores that were derived using a linear encoding model across predictability-matched conditions, we evaluate how linguistic manipulations drive the alignment between human EEG reading data and contextual embeddings extracted word-by-word from the hidden layers of GPT2-XL. Three key patterns emerge: (1) increased alignment for word sequences with syntactic structure, (2) decreased alignment for sentences with compositional semantics, and (3) associative semantics does not modulate alignment. These observed linguistic modulations of LLM-EEG alignment take place above and beyond predictability. Our results indicate that associative semantics is encoded similarly by LLMs and the brain, as are at least some aspects of syntactic structure, while compositional semantics is more uniquely encoded in the human brain.

---

## 论文详细总结（自动生成）

# 超越下一词预测：层级语言组合在时间上调节 LLM 与大脑的对齐  
*作者：Zhao, J. & Brennan, J. R.（2026, BioRxiv）*

---

## 一、核心问题与研究背景

- **研究动机**：  
  大型语言模型（LLMs）在自然语言处理任务中展现出与人类相近的语言理解能力，其内部表征被发现与人类在语言理解过程中的脑活动相关——即所谓的“LLM-大脑对齐（LLM-brain alignment）”。  
  然而，尚不清楚这种对齐是源于两者对统计规律的共同敏感性，还是源于共享的语言层级结构（如句法与语义组合）的表征。

- **核心问题**：  
  本文旨在探究：**层级语言组合（hierarchical linguistic composition）是否会影响 LLM 与人脑在语言处理过程中的时间动态对齐**。  
  作者希望通过操控不同语言要素（句法结构、组合语义、联想语义）来分离语言结构影响与统计特征影响。

---

## 二、方法论：核心思想与技术流程

- **总体思路**：  
  通过构建语言刺激实验，比较人类参与者阅读英文句子时的 EEG 信号与 LLM（使用 GPT2-XL）在对应词序上的隐藏层嵌入之间的对齐程度。

- **关键方法设计**：
  1. **语言因素操控**：  
     - 句法结构：自然语法句 vs 随机词序。  
     - 组合语义：具有真实语义组合 vs 非组合式（打乱概念依存）。  
     - 联想语义：词语之间高或低语义相关度。
  2. **可预测性匹配**：  
     使用 GPT2 的困惑度（perplexity）或词概率对所有刺激进行控制，确保不同条件的统计可预测性一致。
  3. **线性编码模型（linear encoding model）**：
     - 对每个词，提取 GPT2-XL 各层上下文嵌入。  
     - 建立线性回归模型，将这些嵌入映射到 EEG 信号（时间窗级别）。  
     - 对齐得分定义为模型预测 EEG 的相关度。
  4. **对齐比较**：
     在可预测性匹配的条件下，比较不同语言因素对 LLM-EEG 对齐度的调节幅度与时间模式。

- **公式逻辑（文字描述）**：  
  对齐度计算相当于：  
  > EEG_signal(t) ≈ W × Embedding_LLM(word_t, layer_k) + ε  
  其中 W 为线性映射权重，通过交叉验证估计；对齐度通过皮尔逊相关或编码性能指标评估。

---

## 三、实验设计

- **数据与场景**：  
  - 实验对象为人类受试者（数量未说明，可能为大学生人群）。  
  - 刺激材料为经过语法、语义操控的英文句子集合，字词数和频率受控。  
  - 记录脑电图（EEG）数据，对每个句子逐词刺激进行时间锁定分析。
  
- **LLM 表征来源**：  
  - GPT2-XL 模型（已有预训练权重，无微调）。  
  - 逐词提取不同层的上下文嵌入。

- **Benchmark 与对比**：  
  - 不与其他模型直接对比（如 BERT、GPT-Neo），而是在 GPT2 内部不同语言条件下分析变化。  
  - 对照组为不同语言操控条件间的对齐得分。

- **评估指标**：  
  - 对齐得分（alignment score）  
  - EEG 时间窗的相关度分布、显著性检验（可能使用 permutation test 或 cluster-based correction）

---

## 四、资源与算力

- **算力说明**：  
  文中未明确说明具体的算力使用情况（GPU 型号、数量或训练时长）。  
  由于 GPT2-XL 为现成预训练模型，推理部分可能仅需中等 GPU 计算资源（单卡或小集群）用于嵌入提取与线性建模。

---

## 五、实验数量与充分性

- **实验数量**：  
  研究包含三个主要实验操控维度：句法结构、组合语义、联想语义。  
  每一维度均有匹配的高低条件（共约 6 种语言条件）。  
  对每种条件进行 EEG-LLM 对齐测试与时间分析，属于**多因子实验设计**。

- **实验充分性与公平性**：  
  - 实验在可预测性控制下进行，尽量排除语言统计因素的干扰。  
  - 数据来源单一（EEG），但时序分辨率高，有助于观察对齐动态变化。  
  - 未涉及跨语言验证与不同模型对比，因此在普适性上仍有限。

---

## 六、主要结论与发现

1. **句法结构增强对齐**：  
   - 当句子具有合理语法层级时，GPT2-XL 的嵌入与人类 EEG 信号对齐度显著提高。  
   - 说明 LLM 对层级句法结构的处理与大脑相似。

2. **组合语义削弱对齐**：  
   - 在语义组合更复杂的句子中，对齐度降低，表明 LLM 尚未完全捕捉到人脑的语义组合机制。

3. **联想语义无显著影响**：  
   - 词语间的联想相关度对对齐度影响不明显，暗示 LLM 与大脑在处理词汇联想的方式上较为一致。

4. **时间维度发现**：  
   - 对齐模式随词处理时间变化，暗示人脑与模型在语言理解中的时间动态具有不同阶段特征。

---

## 七、优点与亮点

- **实验设计创新**：  
  控制可预测性使得语言结构的影响能被独立考察，排除了传统统计解释的干扰。
- **方法融合程度高**：  
  巧妙结合 LLM 表征与神经编码模型，在人工智能与认知神经科学交叉领域具开创意义。
- **多维操控语言因素**：  
  三类语言维度（句法／组合语义／联想语义）的同时考察有助于系统性理解语言表征差异。
- **时间动态分析**：  
  使用 EEG 数据揭示 LLM-脑对齐的时序特征，填补以往 fMRI 静态分析的空白。

---

## 八、不足与局限

- **数据规模与通用性**：  
  EEG 样本量可能较小，受不同个体差异影响，结果普适性有限。
- **模型范围单一**：  
  仅评估 GPT2-XL，一种单模型视角限制了结论的广泛适用性。
- **缺乏多语言验证**：  
  实验仅基于英语，难推广至非英语语境。
- **语义复杂度控制难度**：  
  虽然统计特征被控制，但语义操控难以完全隔离语境影响。
- **算力与可复现性**：  
  资源未详细说明，复现难度相对高。

---

**（完）**
