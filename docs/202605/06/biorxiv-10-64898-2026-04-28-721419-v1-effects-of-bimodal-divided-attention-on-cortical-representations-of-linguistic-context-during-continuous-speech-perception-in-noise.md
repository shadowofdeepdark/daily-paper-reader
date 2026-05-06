---
title: Effects of bimodal divided attention on cortical representations of linguistic context during continuous speech perception in noise
title_zh: 双模态分散注意对噪声中连续语音感知时语言语境皮层表征的影响
authors: "Xie, Z."
date: 2026-05-01
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.28.721419v1.full.pdf"
tags: ["query:profile-1"]
score: 9.0
evidence: 关于言语感知过程中双模态注意分配和语言语境加工的EEG研究
tldr: 本研究探讨了在噪声环境中同时执行视觉任务对语音理解的影响，通过EEG和mTRF分析发现，当视觉任务负荷较高时，大脑对句子层级语言语境的追踪显著减弱，但对词形和声学信息的处理保持稳定，说明注意力分配主要影响高层语言加工。
source: biorxiv
selection_source: fresh_fetch
motivation: 研究旨在探究在噪声环境中注意力被视觉任务分割时，大脑对连续语音中不同层级语言语境的处理是否受影响。
method: 采用脑电EEG记录和多变量时间响应函数（mTRF）模型分析参与者在不同视觉认知负荷下听有噪声的有声读物时的语言语境处理。
result: 高认知负荷时，参与者语音理解准确率降低，句子层级的语言追踪显著减弱，而词形和声学层级的表征不受影响。
conclusion: 研究表明，在嘈杂环境中进行双模态分心会特异性削弱句子层级语言语境的脑皮层表征，从而影响语音理解。
---

## 摘要
言语感知常常发生在存在竞争性感觉输入的环境中，既包括听觉模态内的竞争，也包括跨模态的竞争；例如，在嘈杂咖啡厅中一边听人交谈，一边同时阅读菜单。本研究考察了在噪声环境下聆听连续语音时，听觉和视觉模态的注意分配（二模态分散注意）在多层次语言语境处理中的影响。研究通过脑电图（EEG）记录被试在进行高或低认知负荷的主视觉任务时，作为次任务听取混杂说话声中的有声读物故事。行为结果显示，在高负荷双任务条件下，语音理解的准确率显著低于低负荷条件。研究采用多变量时间响应函数（mTRF）编码模型，以基于信息论的指标（entropy 和 surprisal）预测 EEG 对次词汇、词形及句子层级语言语境的响应。在词形层级和句子层级观察到显著的神经追踪，但在次词汇层级未发现此效应。关键的是，与低负荷相比，高负荷条件下句子层级语言表征的神经追踪显著减弱，并在超过 200 毫秒的潜伏期出现该效应。相反，词形层级的神经追踪不受双任务负荷的影响。进一步的 mTRF 分析显示，对声学特征的神经追踪不受双任务负荷调节。这些发现表明，二模态分散注意选择性地干扰了大脑皮层对句子层级语言语境的表征，而较低层级的处理相对保持完好。这种高级语言处理的损害可能导致在嘈杂环境中多任务时语音理解能力下降。

## Abstract
Speech perception often takes place in environments with competing sensory inputs, both within the auditory modality and across modalities; for example, following a conversation in a noisy cafe while simultaneously reading a menu. This study examined the extent to which dividing attention between auditory and visual modalities (bimodal divided attention) influences linguistic context processing across hierarchical levels during continuous speech perception in noise. Electroencephalographic (EEG) responses were recorded while participants listened to audiobook stories in multitalker babble as a secondary task, concurrently performing a demanding primary visual task that imposed either low or high cognitive load. Behaviorally, speech comprehension accuracy was significantly lower under high-load than low-load dual-task conditions. Multivariate temporal response function (mTRF) encoding models were used to predict EEG responses from information-theoretic measures (entropy and surprisal) indexing linguistic context at sublexical, word-form, and sentence levels. Significant neutral tracking was observed at the word-form and sentence levels, but not the sublexical level. Critically, neutral tracking of sentence-level linguistic representations was significantly reduced under high compared to low load, with effects emerging at latencies beyond 200 ms. In contrast, neutral tracking of word-form-level representations was unaffected by dual-task load. mTRF analyses further revealed that neutral tracking of acoustic features was not modulated by dual-task load. These findings indicate that bimodal divided attention selectively disrupts cortical representations of sentence-level linguistic context, while lower-level processing remains relatively preserved. Such impairments in higher-level linguistic processing may contribute to reduced speech comprehension during multitasking in noisy environments.

---

## 论文详细总结（自动生成）

# 论文总结：双模态分散注意对噪声中连续语音感知时语言语境皮层表征的影响

---

## 一、核心问题与整体含义

- **研究背景**：在人类日常交流中，语音感知经常发生在复杂环境中，例如噪声干扰或跨模态信息竞争（听觉与视觉同时存在）。在这种情境下，大脑如何分配注意力以维持语义理解是听觉认知科学的核心问题。  
- **研究动机**：过去研究表明，注意力分散会影响语音识别与语义整合，但尚不清楚具体影响的是语言加工的哪个层级（声学、词汇或句子层级）。  
- **核心问题**：该研究旨在探讨**双模态注意分配（听觉与视觉任务并行）**在噪声环境中对大脑皮层语言语境表征的影响，特别是高层次语言结构（如句子语义）的神经追踪是否会受到削弱。

---

## 二、方法论

- **核心思想**：  
  通过脑电图（EEG）记录听觉刺激过程中大脑的动态反应，结合多变量时间响应函数（Multivariate Temporal Response Function, mTRF）建模，分析不同语言层级（次词汇、词形、句子）的语境预测变量与脑电信号的映射关系，以量化语言加工的层次性脑表征。

- **关键技术细节**：
  - 使用**信息论指标**（Entropy 和 Surprisal）表示语言语境的层级复杂度；
  - 在语音连续输入中，mTRF 模型通过线性时域回归估计 EEG 响应与语言特征的时间对齐关系；
  - 对比不同注意负荷条件（高负荷视觉任务 vs 低负荷视觉任务）下的神经追踪强度；
  - 分析延迟时间超过 200ms 的 EEG 成分，以定位句子层级语义加工的时间窗口。

- **公式或流程（文字描述）**：
  1. 提取连续语音的声学特征与语言层级特征；
  2. 基于时间同步的回归模型，预测 EEG 响应；
  3. 模型训练过程中计算回归系数，评估特征在不同时间延迟下的贡献；
  4. 对比不同任务条件下神经追踪强度变化。

---

## 三、实验设计

- **被试与数据场景**：
  - 参与者在实验室环境中听取包含多说话人背景噪声的有声读物；
  - 同时执行视觉主任务（区分图形或空间刺激）以形成双模态注意条件；
  - 视觉任务设置高负荷与低负荷两个水平，用以操控注意力资源分配。

- **实验任务结构**：
  - 听觉任务为被动聆听故事并进行理解测验；
  - 视觉任务为主任务，控制注意焦点；
  - 通过 EEG 连续记录语言加工的神经时间动态。

- **对比方法**：
  - 对比条件：高负荷双任务 vs 低负荷双任务；
  - 分析层级：声学、次词汇、词形、句子；
  - 主要比较指标：EEG神经追踪强度、延迟特征、理解正确率。

- **Benchmark**：
  - 无外部公开数据集或基准模型，实验为原创设计；  
  - 基线由低负荷条件下的语言神经追踪作为参照。

---

## 四、资源与算力

- 原文未提及任何 GPU、CPU 或算力相关信息。  
  由于使用 EEG 数据分析和线性时间响应模型，推测并未涉及深度学习训练或大规模算力需求。

---

## 五、实验数量与充分性

- **实验类型**：
  - 包含至少两大任务条件（高负荷 vs 低负荷）；
  - 分析三层语言层级（次词汇、词形、句子）；
  - 使用 mTRF 模型做神经追踪比较；
  - 包含行为测评（语音理解正确率）与神经指标分析。

- **充分性评价**：
  - 实验设计较完整，涵盖从声学到语义层级；
  - 具有跨模态注意操控与多指标验证；
  - 但未提到样本数量、性别或听力状况，略欠细节；
  - 没有明确的独立验证组或不同语料测试，存在一定局限。

---

## 六、主要结论与发现

- 双模态分散注意显著影响语言语境的高层神经表征：
  - **行为结果**：视觉任务高负荷时语音理解准确率下降；
  - **EEG结果**：  
    - 句子层级的神经追踪显著减弱（潜伏期约 200ms 后开始）；  
    - 词形层级与声学层级的神经追踪未受影响；
  - **推论**：注意力资源被视觉任务占用时，大脑对高级语言结构（语义整合）反应减弱，而低级的听觉和词形加工仍保持稳定。

- **总体结论**：  
  研究揭示，在噪声环境中进行双任务操作时，大脑皮层的注意分配会**选择性削弱句子层级语言语境的表征**，是语音理解能力下降的重要神经机制。

---

## 七、优点

- **科学贡献**：
  - 明确区分了语言加工层级的差异性影响；
  - 结合行为与神经信号，具有多层验证；
  - 使用 mTRF 模型、信息论变量等前沿技术连接语言认知与脑电动力学。

- **实验设计亮点**：
  - 使用真实连续语音，提升生态效度；
  - 双任务范式能有效模拟自然多任务场景（如噪声中交谈和视觉分心）。

---

## 八、不足与局限

- **实验覆盖**：
  - 未报告样本规模与个体差异统计；
  - 实验语料较单一（仅有声读物），结果的普适性有待验证。

- **分析局限**：
  - EEG 时空分辨率有限，无法确定影响区域的脑区定位；
  - 未与其他神经影像技术（如 fMRI 或 MEG）对比，难以确认具体皮层网络参与。

- **应用限制**：
  - 实验环境控制性强，可能与真实多任务场景的复杂度不完全一致；
  - 结果主要为理论解释，对现实噪声沟通中的应用需进一步验证。

---

**（完）**
