---
title: Effects of bimodal divided attention on cortical representations of linguistic context during continuous speech perception in noise
title_zh: 双模态分配注意对噪声中持续语音感知时皮层语言语境表征的影响
authors: "Xie, Z."
date: 2026-05-01
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.28.721419v1.full.pdf"
tags: ["query:profile-1"]
score: 9.5
evidence: 关于言语感知中双模态注意力和语言语境的EEG研究
tldr: 本研究通过EEG和mTRF模型分析双任务环境中语音理解的皮层表征差异，发现视觉高负荷分心选择性削弱句子层面的语言语境加工，而词形及声学处理保持稳定，说明多任务在噪声环境下主要影响高层语言理解。
source: biorxiv
selection_source: fresh_fetch
motivation: 探讨听觉与视觉双任务分心对连续语音中不同层级语言语境加工的影响。
method: 研究使用EEG记录受试者在噪声中听有声读物并同时执行视觉任务，通过mTRF模型分析语境表征。
result: 在高负荷视觉任务下，句子层面的神经跟踪显著降低，而词形层及声学特征的跟踪未受影响。
conclusion: 双任务环境下高认知负荷会选择性削弱句子层面的语言语境皮层表征，而低层次处理保持稳定。
---

## 摘要
语音感知往往发生在存在竞争性感官输入的环境中，这些输入既可能来自听觉模态内部，也可能跨越不同模态；例如，在嘈杂的咖啡馆中一边追踪对话，一边阅读菜单。本研究考察了在噪声环境中持续语音感知过程中，在层级结构的不同水平上分配听觉与视觉模态注意（双模态分配注意）对语言语境处理的影响。研究记录了受试者在将听有声书故事（背景为多说话者噪声）作为次要任务的同时，执行一项认知负荷低或高的主视觉任务时的脑电图（EEG）反应。行为结果显示，高负荷双任务条件下的语音理解准确率显著低于低负荷条件。研究采用多变量时间响应函数（mTRF）编码模型，根据信息论指标（熵和意外度）来预测 EEG 对次词汇、词形和句子层面语言语境的响应。结果显示，在词形和句子层面存在显著的神经追踪，而在次词汇层面未观察到这种现象。关键的是，与低负荷条件相比，高负荷条件下句子层面语言表征的神经追踪显著减弱，该效应在 200 毫秒以上的延迟出现。相反，词形层面表征的神经追踪不受双任务负荷影响。mTRF 分析进一步显示，声学特征的神经追踪不受双任务负荷调节。这些发现表明，双模态分配注意选择性地破坏了大脑皮层对句子层面语言语境的表征，而低层次的处理则相对保持完整。在噪声环境中多任务处理时，高层语言加工受损可能导致语音理解能力下降。

## Abstract
Speech perception often takes place in environments with competing sensory inputs, both within the auditory modality and across modalities; for example, following a conversation in a noisy cafe while simultaneously reading a menu. This study examined the extent to which dividing attention between auditory and visual modalities (bimodal divided attention) influences linguistic context processing across hierarchical levels during continuous speech perception in noise. Electroencephalographic (EEG) responses were recorded while participants listened to audiobook stories in multitalker babble as a secondary task, concurrently performing a demanding primary visual task that imposed either low or high cognitive load. Behaviorally, speech comprehension accuracy was significantly lower under high-load than low-load dual-task conditions. Multivariate temporal response function (mTRF) encoding models were used to predict EEG responses from information-theoretic measures (entropy and surprisal) indexing linguistic context at sublexical, word-form, and sentence levels. Significant neutral tracking was observed at the word-form and sentence levels, but not the sublexical level. Critically, neutral tracking of sentence-level linguistic representations was significantly reduced under high compared to low load, with effects emerging at latencies beyond 200 ms. In contrast, neutral tracking of word-form-level representations was unaffected by dual-task load. mTRF analyses further revealed that neutral tracking of acoustic features was not modulated by dual-task load. These findings indicate that bimodal divided attention selectively disrupts cortical representations of sentence-level linguistic context, while lower-level processing remains relatively preserved. Such impairments in higher-level linguistic processing may contribute to reduced speech comprehension during multitasking in noisy environments.

---

## 论文详细总结（自动生成）

# 双模态分配注意对噪声中持续语音感知的影响 —— 论文深入总结

---

## 一、核心问题与研究背景

- **核心问题**：在现实生活中，人们常常需要在多模态刺激下进行语音感知（例如一边聊天、一边看菜单）。这种情境会引发跨模态注意力竞争，从而可能影响语言信息的脑内加工。本论文探讨的问题是：**听觉与视觉双任务（bimodal divided attention）在噪声环境中对语音理解不同层级语言语境加工的影响。**
  
- **研究动机**：
  - 过往研究主要关注单模态（听觉）条件下的语言理解。
  - 先前的 EEG 研究表明，在清静环境中，双模态分配注意虽能削弱语言语境效应，但影响相对均一。
  - 本研究进一步延伸到**噪声环境下的真实语音听觉场景**，旨在揭示注意力负荷如何影响语言加工的层级结构（次词汇、词形、句子层）。

- **整体含义**：本研究代表了对语音理解在多任务与跨模态环境中神经表征机制的系统探索，有助于揭示人类语言加工在复杂场境下的认知瓶颈。

---

## 二、方法论与技术路线

- **核心思想**：通过脑电（EEG）记录与多变量时间响应函数（mTRF, multivariate Temporal Response Function）建模，揭示语言语境信息（由熵与意外度指标量化）在不同认知负荷下的神经追踪强度。

- **主要流程**：
  1. **数据获取**：记录受试者的 EEG 信号。
  2. **语音特征建模**：
     - 语音信号提取声学特征（包络谱、起始谱）。
     - 基于语音文本生成 **三层语言语境模型**：
       - 次词汇层（基于 phoneme 5-gram）。
       - 词形层（基于词汇概率与 cohort 模型）。
       - 句子层（基于 lexical 5-gram，考虑前四个词上下文）。
  3. **mTRF 编码模型**：
     - 以 surprisal 和 entropy 作为预测变量，输入 EEG。
     - 模型通过 time-lag 回归（-100 至 500 ms）拟合刺激与 EEG 的线性关系。
     - 使用 **逐层剔除法（full vs. reduced model）**，比较预测力变化 Δ% explained variance。
  4. **统计分析**：采用 cluster-based permutation test 控制假阳性率；效应量由最大 t 值 (tmax) 表示。

- **理论框架**：信息论度量 + 线性时序响应模型，用于刻画语言处理的层级性与注意力调制的时程结构。

---

## 三、实验设计

- **受试者与场景**：
  - 24 名 18–23 岁大学生（20 名女性），听力及视力正常。
  - 使用有声书 *Alice’s Adventures in Wonderland*（美式英语朗读），背景为多说话者餐厅噪声（SNR=5 dB）。
  - 听觉任务为语音理解问答；视觉任务为 **n-back** 空间记忆任务（0-back 低负荷 vs. 3-back 高负荷）。

- **任务结构**：
  - 每种任务条件（低负荷、高负荷）15 个 trial。
  - 听觉刺激为约 60 秒片段；视觉刺激持续 0.5 秒。

- **benchmark 与对比**：
  - 对比高负荷与低负荷条件下的 EEG 表征。
  - 与前人研究（Xie et al., 2023）在无噪环境的结果作延伸比较。

---

## 四、资源与算力

- **硬件与软件**：
  - 64 通道 actiCAP 系统，Brainvision actiCHamp Plus 放大器。
  - 数据采样率 5 kHz；处理平台：**MNE-Python + EEGLAB + Eelbrain**。
  
- **算力说明**：
  - 文中未涉及任何 GPU 或深度学习框架，mTRF 为线性回归模型，因此**未使用高算力资源**。

---

## 五、实验数量与充分性

- **主要实验类型**：
  1. 行为表现分析（视觉与听觉任务性能对比）。  
  2. 神经追踪分析（视觉、声学、次词汇、词形、句子层）。  
  3. 时序响应函数（TRF）形态与时程比较。  
  4. 相关性与贝叶斯因子分析。
  
- **实验充分性**：
  - 每层级均有独立的模型与统计验证。
  - 采用 5 折交叉验证与 permutation test。
  - 因样本量中等（n=24）且仅两种负荷条件，结果具统计效力但推广性有限。

---

## 六、主要结论与发现

- **行为结果**：
  - 高视觉负荷显著降低语音理解准确率与视觉任务准确性。
  - 说明双任务情境确实引发认知资源竞争。

- **神经结果**：
  - **句子层语言表征受显著调制**：在高负荷时神经追踪降低，延迟 200–300 ms 出现。
  - **词形层追踪稳定**：高低负荷差异不显著。
  - **次词汇层追踪缺失**：噪声干扰可能使底层语音统计难以稳定编码。
  - **声学特征（包络与起始）未受影响**。
  - **视觉刺激的神经追踪增强**：高负荷条件下视觉皮层激活增加（0–190 ms 与 520–690 ms ）。

- **总体结论**：高认知负荷的双任务环境下，脑皮层的高层语言加工（句子层整合）被选择性削弱，低层声学及词汇加工保持稳定。

---

## 七、优点与亮点

- **方法创新**：
  - 将 mTRF 与信息论语言模型结合，跨层分析语言语境处理。
  - 实现了从声学到语义的**多层级神经编码框架**。
  
- **实验设计亮点**：
  - 使用自然连续语音与真实噪声场景，提高生态有效性。
  - 双任务范式（视觉 n-back + 听觉理解）精确操控认知负荷。
  - 严谨的统计控制（cluster-based permutation + Bayes factor）。

- **科学意义**：
  - 揭示了域一般认知资源对语言预测处理的选择性影响。
  - 支持“语义层整合受限于工作记忆负荷”的理论假设。

---

## 八、不足与局限

- **实验覆盖**：
  - 仅使用一种噪声类型（餐厅多人噪声）与单一 SNR（5 dB），限制结果可扩展性。
  
- **任务偏差**：
  - 视觉任务为空间记忆，本身占用大量前额叶资源，可能特别影响语义整合。
  
- **样本限制**：
  - 年龄跨度小（年轻成人），无法推及老年或听力损失人群。
  
- **分析局限**：
  - mTRF 为线性模型，无法揭示非线性或交互性神经动态。
  
- **推广风险**：
  - 未涉及其他语言、文化或多语言环境的验证。
  - 实验在单耳呈现（右耳）条件下进行，可能影响空间注意机制。

---

**（完）**
