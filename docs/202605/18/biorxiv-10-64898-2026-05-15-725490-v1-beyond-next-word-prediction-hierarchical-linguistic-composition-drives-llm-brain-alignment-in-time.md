---
title: "Beyond next-word prediction: hierarchical linguistic composition drives LLM-brain alignment in time"
title_zh: 超越下一个词预测：层级语言组合在时间上驱动LLM与大脑的对齐
authors: "Zhao, J., Brennan, J. R."
date: 2026-05-16
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.15.725490v1.full.pdf"
tags: ["query:profile-1"]
score: 9.0
evidence: 使用脑电图研究语言理解过程中的神经活动及与大模型的对齐
tldr: 本研究通过操控英语句子的句法与语义特征，并结合 EEG 实验，分析 GPT2-XL 的内部表征与人脑语言处理的对齐模式。结果发现，句法结构会增强模型与人脑的对齐，组合语义则降低对齐，联想语义影响甚微，揭示 LLM 与人脑在语言层级加工中的异同。
source: biorxiv
selection_source: fresh_fetch
motivation: 研究旨在探究大语言模型与人类在语言理解中的神经对齐是否源自共同的层级语言结构表征。
method: 研究通过对英语句子的句法、组合语义和联想语义进行操控，并结合人类 EEG 数据与 GPT2-XL 表征进行比对分析。
result: LLM-EEG 的对齐在具有句法结构时增强，在具组合语义时减弱，而联想语义不影响对齐。
conclusion: 结果显示，LLM 与人脑在句法层面具有一定共同性，而组合语义加工更多是人脑独有。
---

## 摘要
大型语言模型（LLMs）的内部表征与人类在语言理解过程中产生的神经活动存在相关性，或称为“对齐”。一种观点认为，这种对齐反映了LLM与人类对统计模式的共同敏感性；另一种观点则认为，这种对齐至少部分地反映了两者中出现的共享语言表征。本文研究了层级语言组合（hierarchical linguistic composition）——一种被认为是人类语言的基本属性——是否驱动了LLM-大脑对齐过程。为此，我们操纵了英语句子的句法、组合语义和联想语义，并将这些句子呈现给LLM和人类参与者，同时进行脑电图（EEG）实验。我们控制了经语言操纵的刺激在可预测性上的一致性，从而能够区分由语言结构引起的对齐与由统计因素引起的对齐。通过比较在可预测性匹配条件下，使用线性编码模型计算得到的LLM-EEG对齐分数，我们评估不同语言操纵如何影响人类EEG阅读数据与从GPT2-XL隐藏层逐词提取的上下文嵌入之间的对齐。结果显示出三个关键模式：（1）具有句法结构的词序列呈现更高的对齐；（2）具有组合语义的句子呈现更低的对齐；（3）联想语义并不影响对齐。这些语言学对齐调制的效应超越了可预测性因素。我们的研究结果表明，LLMs与人脑在联想语义及至少部分句法结构上的编码方式相似，而组合语义的编码更具人脑特异性。

## Abstract
The internal representations of large language models (LLMs) correlate, or "align" , with human neural activity during language comprehension. One view holds that this alignment reflects shared sensitivity to statistical patterns in LLMs and humans, while others hold that it reflects, at least in part, the emergence of shared linguistic representations in these systems. Here, we investigate whether hierarchical linguistic composition, a property believed to be fundamental to human language, drives LLM-brain alignment. To this end, we manipulated syntax, compositional semantics, and associative semantics in English sentences that were presented to both an LLM and human participants during an electroencephalography (EEG) experiment. We matched linguistically manipulated stimuli in predictability, which allows us to tease apart alignment induced by linguistic structure from statistical factors. By comparing LLM-EEG alignment scores that were derived using a linear encoding model across predictability-matched conditions, we evaluate how linguistic manipulations drive the alignment between human EEG reading data and contextual embeddings extracted word-by-word from the hidden layers of GPT2-XL. Three key patterns emerge: (1) increased alignment for word sequences with syntactic structure, (2) decreased alignment for sentences with compositional semantics, and (3) associative semantics does not modulate alignment. These observed linguistic modulations of LLM-EEG alignment take place above and beyond predictability. Our results indicate that associative semantics is encoded similarly by LLMs and the brain, as are at least some aspects of syntactic structure, while compositional semantics is more uniquely encoded in the human brain.

---

## 论文详细总结（自动生成）

# 《超越下一个词预测：层级语言组合在时间上驱动LLM与大脑的对齐》论文总结

---

## 一、研究核心问题与整体背景

- **研究动机：**  
  当前大量研究发现，大型语言模型（LLMs）在处理自然语言时，其内部表征与人脑的语言加工神经活动存在 *对齐（alignment）* 关系。但这种对齐是否仅反映对统计规律的共同敏感性，还是意味着LLM与人脑在语言层级结构表征上存在相似性，尚未明确。

- **核心问题：**  
  作者试图回答：人类语言的层级组合性（hierarchical linguistic composition）是否是驱动LLM与人脑神经活动对齐的关键因素。

- **研究意义：**  
  若此假设成立，将说明LLMs在一定程度上实现了与人脑相似的语言层级处理模式，超越单纯的下一个词的统计预测，进而推动认知神经科学与人工智能语言建模的融合。

---

## 二、方法论与技术路线

- **核心思想：**  
  通过精确控制英语句子在三种语言层面上的操作（句法、组合语义、联想语义），研究这些层次的变化如何影响GPT2-XL模型表示与人类大脑EEG数据之间的神经对齐。

- **关键步骤：**  
  1. **语言刺激设计：**  
     构造三种语言条件：
     - 具有明确句法结构的句子；
     - 具有组合语义（意义可由成分组合推导）；
     - 具有联想语义（词语之间基于共现或语义关联）。
     
  2. **可预测性匹配：**  
     控制不同条件句子的可预测性（如词频与上下文概率），以排除简单统计因素对对齐的影响。

  3. **模型处理：**  
     使用 **GPT2-XL** 逐词提取上下文嵌入（hidden states），获取语言模型理解过程的时间序列表示。

  4. **脑电实验：**  
     对人类受试者在阅读同样句子时的脑活动进行EEG记录。

  5. **线性编码模型计算：**  
     - 将EEG信号映射到LLM的表示空间中，训练线性模型以预测EEG数据。  
     - 计算不同语言条件下的 *LLM-EEG alignment score*，用于衡量对齐程度。
     - 比较各条件下的差异，判断语言层级结构对神经对齐的调制效应。

---

## 三、实验设计与数据来源

- **实验场景：**  
  英语句子阅读实验，受试者逐词阅读特定设计的句子并进行EEG记录。

- **数据集：**  
  自建实验语料，包含三类语言结构的英语句子；为实验一致性，操控了句子长度与词频分布。

- **模型与对比方法：**
  - 使用 **GPT2-XL** 作为LLM主模型。
  - 主要比较不同语言操控条件下的LLM-EEG对齐变化。
  - 未采用跨模型（如BERT、GPT-J等）的比较，但通过内部层级分析（不同层表示）评估LLM内部结构差异。

- **Benchmark：**  
  无标准公开benchmark，属于认知神经科学与AI交叉的自定义实验体系。

---

## 四、资源与算力

- **论文未明确说明算力资源：**  
  - 未报告GPU类型、数量或计算耗时。
  - 由于使用GPT2-XL并仅进行嵌入提取及线性映射训练，推测算力需求相对中等，无大规模训练环节。

---

## 五、实验数量与充分性

- **实验设计：**
  - 三种语言条件（句法、组合语义、联想语义）。
  - 各条件下进行EEG记录与LLM对齐计算，共构成三个主要实验设置。
  - 控制了可预测性因素，增强对比的公平性。

- **充分性分析：**
  - 设计清晰，能够分离统计与结构性因素。
  - 但实验范围局限于英文语言与单一LLM，不足以全面验证跨语言或跨模型的普适性。
  - EEG样本规模未明确说明，若样本较少可能影响统计稳健性。

---

## 六、主要结论与发现

- **三个核心结果：**
  1. **句法结构增强对齐：**  
     含有句法结构的句子在LLM与EEG之间的对齐度最高，说明LLMs部分捕捉了层级语法信息。
  2. **组合语义降低对齐：**  
     当语义具有可组合性时，对齐度反而下降，表明LLMs仍欠缺人脑处理组合意义的机制。
  3. **联想语义不影响对齐：**  
     联想性语义特征在两系统中编码方式相似，说明两者可能在统计关联层面存在近似机制。

- **宏观推论：**
  LLM与人脑在句法层面存在共享的表征基础，但在语义组合加工方面仍存在显著差异。

---

## 七、研究优点与创新点

- **多层语言操控设计：**  
  系统区分三种语言层级因素，理论上可精确剖析语言理解的不同维度。

- **控制预测性变量：**  
  排除统计共现效应，确保结果真正反映语言结构而非训练数据的频率偏差。

- **跨领域方法融合：**  
  将认知神经科学（EEG）与人工智能表征分析结合，为研究“人脑-模型对齐”的时间动力机制提供新框架。

- **理论贡献：**  
  提出层级组合结构是LLM-人脑对齐的时间驱动因素，具有解释力与原创性。

---

## 八、不足与局限

- **实验覆盖限制：**
  - 仅使用英文句子，缺乏语言多样性。
  - 仅评估GPT2-XL模型，未分析不同架构（如Transformer家族其它成员）的差异。

- **数据规模与可重复性：**
  - EEG样本量及受试者数量未详述，可能影响实验统计显著性。
  - 自定义语料库难以直接复现。

- **表征深度：**
  - 仅考查逐词嵌入的线性映射关系，未探究非线性或层间交互。
  - 无具体神经源定位分析（如皮层区域映射），限制神经解释力。

- **应用限制：**
  - 研究结论主要面向理论语言认知研究，短期内难以直接用于模型改进或人机交互优化。

---

**（完）**
