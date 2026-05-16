---
title: "Word meaning, not surface statistics, is essential for predictive language processing"
title_zh: 预测性语言加工中，词义而非表层统计至关重要
authors: "Zyryanov, A., Pierz, V., Oganian, Y."
date: 2026-05-15
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.15.724229v1.full.pdf"
tags: ["query:q1"]
score: 9.0
evidence: 使用心理语言学模型研究增量语言理解和预测加工
tldr: 研究探讨人类语言理解中预测误差是否基于词形统计或词义。通过采用多义词实验并结合自 paced 阅读和MEG脑成像数据，发现语义不确定性会影响预测误差，而表层统计模型无法解释这种变化，支持意义驱动的预测机制。
source: biorxiv
selection_source: fresh_fetch
motivation: 研究人类语言处理中预测误差的性质，是由表层统计还是由词义引导。
method: 通过多义词实验结合自 paced 阅读和MEG脑成像，比较语义驱动与词形统计驱动的预测误差模型。
result: 只有在语义确定的情况下，LLM的预测误差能有效预测阅读和脑响应，语义歧义时效果消失。
conclusion: 人类语言预测处理依赖词义而非表层统计，揭示LLM模拟人类语言理解的局限性。
---

## 摘要
人类在理解语言时是逐步进行的，每接收到一个新词就会更新句子意义的表征。这种更新由每个感知到的词与先前预期之间的距离——即预测误差——所引导。大型语言模型（LLMs）与皮层活动之间的契合，启发了这样一个假设：皮层对预测误差的计算是基于表层的，由词形共现的统计模式所驱动。与此相对，心理语言学模型则提出预测误差的计算是基于意义的，由词语语义所驱动。我们使用语义歧义的多义词来区分这些模型：如果预测误差是基于意义的，语义歧义会在意义表征中引入不确定性，从而影响预测误差；而如果预测误差是基于表层的，语义歧义则不会产生影响。我们考察了语义歧义在自定步阅读时间以及句子处理过程中的脑磁图（MEG）神经反应中对预测误差信号的影响。虽然基于LLM的预测误差代理能够稳健地预测无歧义词的阅读时间和神经反应，但在语义歧义条件下则无法预测。这表明，词义的不确定性改变了预测误差的计算，支持基于意义模型，并进一步证明词义在预测性语言加工中的关键作用。我们的研究结果揭示了LLM作为人类语言能力计算模型的一个重要局限性。

## Abstract
Humans comprehend language incrementally, updating the representation of sentence meaning with each incoming word. These updates are guided by the distance between each perceived word and prior expectations--the prediction error. The alignment between large language models (LLMs) and cortical activity inspires the hypothesis that the cortical computation of prediction error is Surface-based, driven by statistical patterns of word form co-occurrence. In contrast, psycholinguistic models propose that prediction error computation is Meaning-based, driven by word semantics. We used polysemic words with ambiguous semantics to distinguish these models: ambiguity would introduce uncertainty into meaning representations and hence the prediction error, if Meaning-based, but would not affect the prediction error, if Surface-based. We examined how ambiguity influenced prediction error signatures in self-paced reading times and magnetoencephalographic (MEG) neural responses during sentence processing. While an LLM-based proxy of prediction error robustly predicted reading times and neural responses to unambiguous words, it failed to predict either under ambiguity. That is, prediction error computation was altered by uncertainty in word meaning, which supports the Meaning-based model and corroborates the essential role of word meaning in predictive language processing. Our findings highlight an important limitation of LLMs as in silico models of the human language faculty.

---

## 论文详细总结（自动生成）

# 论文总结：预测性语言加工中，词义而非表层统计至关重要  
**原题：** Word meaning, not surface statistics, is essential for predictive language processing  
**作者：** Zyryanov, A., Pierz, V., Oganian, Y.  
**来源：** bioRxiv (2026-05-15)

---

## 一、研究背景与核心问题

- **研究动机**：  
  人类语言理解是逐步（incremental）进行的，每当接收到一个新词，都会基于上下文更新句子意义的表征。这一更新过程依赖“预测误差”（prediction error）——即当前词与心理预期之间的距离。  
- **问题核心**：  
  当前两类关于预测误差计算的模型存在竞争性假设：  
  1. **表层统计模型（Surface-based）**：认为预测误差是基于词形和共现统计模式的。  
  2. **意义驱动模型（Meaning-based）**：认为预测误差的计算依赖于词义，即语义层面的期望偏差。  
- **研究目标**：  
  作者旨在区分这两种机制，探讨人类大脑在语言预测时，究竟依赖表层统计还是词义表征。

---

## 二、方法论与核心思想

- **主要思想**：  
  通过使用**语义歧义词（polysemic words）**作为实验材料，以此操控词义不确定性，从而检验预测误差是否依赖语义。  
- **实验假设**：  
  - 若预测误差依赖**意义**, 语义歧义将引入不确定性，使预测误差变化显著。  
  - 若预测误差依赖**表层统计**, 语义歧义不会改变预测误差。
- **方法框架**：  
  1. 构建两类语言预测误差指标：  
     - **基于LLM的表层预测误差指标**（使用大型语言模型的词概率分布）。  
     - **基于心理语言学的语义预测误差指标**（基于上下文语义相关性计算）。  
  2. 运用两种实验范式：  
     - **自定步阅读实验（Self-paced reading）**：测量反应时与预测误差相关性。  
     - **脑磁图实验（MEG）**：测量在语言处理过程中神经反应与预测误差的契合度。  
- **技术细节**：  
  预测误差代理值为：  
  \[
  PE(w_i) = -\log P(w_i | context)
  \]
  其中 \( P(w_i | context) \) 由 LLM 预测获得。  
  在语义条件下，通过词义向量不确定度或多义性衡量语义模糊性并作为调制变量。

---

## 三、实验设计

- **数据与场景**：  
  实验材料为精心挑选的句子片段，包含语义单一词与多义词条件，以操控语义确定性。  
  - **阅读实验**：参与者逐句词阅读，同时记录反应时间。  
  - **MEG实验**：另一组被试观看同样的句子，采集脑磁响应。  
- **Benchmark 和对照**：  
  - **LLM预测误差模型 vs. 意义驱动模型** 的预测能力比较。  
  - 对照无语义歧义与有语义歧义条件的效果差异。  
- **被试与材料控制**：  
  文中未明确数据集规模细节，但强调句子、词频、长度等因素被严格匹配以控制干扰变量。

---

## 四、资源与算力

- 文中未明确列出所使用的计算资源或算力参数。  
  - 未说明使用的具体 LLM 模型（如 GPT、BERT 等）、GPU 型号或训练时长。  
  - 因为研究侧重于认知实验与统计分析，而非模型参数调优或大规模训练。

---

## 五、实验数量与充分性

- **实验组别**：  
  - 两个主要实验：阅读实验 + MEG神经反应实验。  
  - 每个实验含两个条件（语义确定 vs. 语义歧义）。  
  - 多组统计测试验证预测误差与反应时、神经信号间的相关性。  
- **充分性评估**：  
  - 结合**行为数据**与**脑成像数据**具有较强的互证效力。  
  - 实验方法符合心理语言学研究的标准范式，具备一定的客观性和可重复性。  
  - 然而，数据规模及LLM类型细节未披露，可能影响结果的普适性。

---

## 六、主要结论与发现

1. 基于LLM的预测误差能稳健预测**无歧义词**的阅读时间与脑磁反应。  
2. 在**语义歧义条件**下，这种预测能力消失。  
3. 因此，预测误差的计算会被词义不确定性改变，表明人类语言处理依赖**语义层面**的预测机制。  
4. 该结果支持“**意义驱动的预测模型**”，并质疑LLM仅以表层统计模拟人类语言理解的有效性。  
5. 研究揭示了LLM作为“人类语言计算模型”的重要局限——缺乏真实的语义表征机制。

---

## 七、优点与亮点

- **理论创新**：首次系统区分意义驱动与表层驱动预测误差的神经对应机制。  
- **实验设计精巧**：利用多义词作为自然操控变量，具备心理语言学上的严谨性。  
- **跨模态验证**：结合行为反应和脑磁成像的双重证据，提高结论可靠性。  
- **方法通用性**：模型框架可扩展至不同语言、不同语义复杂度的研究。

---

## 八、不足与局限

- **模型透明度不足**：未公布所用LLM的具体架构、训练语料与参数。  
- **数据规模有限**：实验基于控制句材料而非自然语料，可能影响生态效度。  
- **算力与实现细节缺失**：无法评估计算资源是否影响结果可复现性。  
- **跨语言与文化普适性**：结论主要基于单一语言环境（猜测为英语），对其他语言结构的推广仍待验证。  
- **应用限制**：对LLM的评估仅涉及预测误差层面，未涉及上下文整合、句法解析等更复杂的理解过程。

---

（完）
