---
title: Effects of bimodal divided attention on cortical representations of linguistic context during continuous speech perception in noise
title_zh: 双模态分散注意对噪声中连续语音感知过程中语言情境皮层表征的影响
authors: "Xie, Z."
date: 2026-05-01
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.28.721419v1.full.pdf"
tags: ["query:profile-1"]
score: 9.0
evidence: 关于言语感知过程中双模态注意力和语言语境加工的脑电研究
tldr: 本研究探讨了在视觉任务负荷下，听者在噪声中理解连续语音时的大脑语言层级表征变化。通过EEG和mTRF模型分析发现，高视觉负荷削弱了句子层的语言语境神经追踪，而较低层级处理相对稳定，揭示了多任务环境中语音理解受限的神经机制。
source: biorxiv
selection_source: fresh_fetch
motivation: 研究旨在探讨跨模态注意分配如何影响噪声环境中语言上下文的脑皮层表征。
method: 研究通过EEG记录被试听噪声中听故事并同时完成不同负荷视觉任务的脑反应，并用mTRF模型分析语言层级信息。
result: 结果发现高负荷条件下句子级语言表征的神经追踪显著降低，而词形级和声学处理未受影响。
conclusion: 双模态注意分配主要干扰高层句子级语言处理，而低层词形与声学特征处理不受影响。
---

## 摘要
语音感知常常发生在存在多种竞争性感官输入的环境中，这些输入可能来自同一听觉通道或不同通道；例如，在嘈杂的咖啡馆中一边跟随谈话，一边同时阅读菜单。本研究考察了在噪声环境中进行连续语音感知时，将注意力分配到听觉和视觉通道（双模态分散注意）在不同层级上对语言情境加工的影响。研究通过记录脑电图（EEG）响应，在受试者一边聆听混合多说话人背景音中的有声读物故事（作为次要任务），一边执行具有不同认知负荷（低负荷或高负荷）的主要视觉任务。行为结果显示，在高负荷双任务条件下，语音理解准确率显著低于低负荷条件。研究利用多变量时间响应函数（mTRF）编码模型，根据信息论指标（熵与惊讶度）预测EEG响应，这些指标代表了次词汇、词形和句子层级的语言情境。结果发现，词形与句子层级上存在显著的神经追踪，但在次词汇层级上未观察到显著追踪。关键的是，与低负荷相比，高负荷条件下句子层级的神经追踪显著减弱，该效应在200毫秒以后的潜时上出现。相反，词形层级的神经追踪不受双任务负荷的影响。mTRF分析进一步表明，声学特征的神经追踪不受双任务负荷调制。这些发现表明，双模态分散注意选择性地干扰了句子层级语言情境的皮层表征，而较低层级的加工相对得以保留。这种较高级语言加工的损伤可能导致在嘈杂环境下多任务时语音理解能力下降。

## Abstract
Speech perception often takes place in environments with competing sensory inputs, both within the auditory modality and across modalities; for example, following a conversation in a noisy cafe while simultaneously reading a menu. This study examined the extent to which dividing attention between auditory and visual modalities (bimodal divided attention) influences linguistic context processing across hierarchical levels during continuous speech perception in noise. Electroencephalographic (EEG) responses were recorded while participants listened to audiobook stories in multitalker babble as a secondary task, concurrently performing a demanding primary visual task that imposed either low or high cognitive load. Behaviorally, speech comprehension accuracy was significantly lower under high-load than low-load dual-task conditions. Multivariate temporal response function (mTRF) encoding models were used to predict EEG responses from information-theoretic measures (entropy and surprisal) indexing linguistic context at sublexical, word-form, and sentence levels. Significant neutral tracking was observed at the word-form and sentence levels, but not the sublexical level. Critically, neutral tracking of sentence-level linguistic representations was significantly reduced under high compared to low load, with effects emerging at latencies beyond 200 ms. In contrast, neutral tracking of word-form-level representations was unaffected by dual-task load. mTRF analyses further revealed that neutral tracking of acoustic features was not modulated by dual-task load. These findings indicate that bimodal divided attention selectively disrupts cortical representations of sentence-level linguistic context, while lower-level processing remains relatively preserved. Such impairments in higher-level linguistic processing may contribute to reduced speech comprehension during multitasking in noisy environments.

---

## 论文详细总结（自动生成）

# 论文总结：双模态分散注意对噪声中连续语音感知过程中语言情境皮层表征的影响

---

## 一、研究核心问题与背景

- **研究动机**：现实生活中的语音感知常发生在多感官干扰环境中（如嘈杂的咖啡厅中边听对话边看菜单），听者需在多任务情境下分配注意力。已有研究多集中在单模态听觉选择性注意，而对**跨模态分散注意（bimodal divided attention）**如何影响语音理解的神经机制，特别是**在噪声中**的情形，研究相对稀缺。
- **核心问题**：当人类在噪声环境下需要同时处理视觉任务时，不同层级的语言加工（次词汇、词形、句子）是否会受到注意力分配的调节？
- **理论背景**：
  - 连续语音加工包含多层级的语言情境预测机制（sublexical → word-form → sentence）。
  - 先前研究表明这些层级的脑活动在安静环境下可并行运行；但尚不清楚多任务和噪声的综合干扰如何影响语言层级表征。
  - 探明该问题有助于理解**域一般认知资源（domain-general cognitive resources）**在语言预测中的作用。

---

## 二、方法论概述

### 1. 核心思想
- 采用**双任务跨模态范式（audiovisual dual-task paradigm）**：
  - 听觉次任务：噪声中听取故事；
  - 视觉主任务：高或低负荷的视觉工作记忆任务；
  - 通过比较不同负荷条件，评估跨模态分散注意对语言加工的层级效应。
- 使用**多变量时间响应函数模型（multivariate Temporal Response Function, mTRF）**分析脑电数据，量化不同语言层级的皮层追踪程度。

### 2. 技术途径与分析模型
- **EEG 信号建模**：利用 mTRF 建立从刺激特征（视觉、声学、语言层级）到 EEG 响应的线性时序映射。
- **语言情境表征**：
  - 采用信息熵（entropy）与惊讶度（surprisal）衡量语言预测难易；
  - 三个层级：
    1. **次词汇（sublexical）**：基于语音序列5-gram；
    2. **词形（word-form）**：基于词汇共现与发音概率；
    3. **句子级（sentence-level）**：基于四词上下文的5-gram词汇模型。
- **指标**：  
  对每类特征，计算包含与不包含该特征的模型之间的 EEG 方差解释率差值（Δ% explained variance），作为神经追踪强度。
- **统计方法**：
  - 5 折交叉验证；
  - 基于聚类的随机置换检验；
  - 计算 Cohen’s d 与 Bayes 因子（BF）以验证效应强度。

---

## 三、实验设计

### 1. 被试与任务
- 共 **24 名健康年轻被试（18–23 岁）**。
- **听觉刺激**：  
  - 有声读本《爱丽丝梦游仙境》片段（英语）；
  - 加入多说话人噪声（multi-talker babble，SNR = 5 dB）。
- **视觉任务**：
  - **低负荷条件（0-back）**：识别当前方块是否与首个相同；
  - **高负荷条件（3-back）**：识别当前方块与前3个中的对应关系；
  - 每种条件包含15个试次。
- **行为测量**：视觉准确率、反应时、听觉理解正确率及主观努力评分。

### 2. 数据处理
- EEG采集：64通道、采样率5 kHz，经滤波（1–15 Hz）、ICA去伪。
- 通过 MNE-Python 与 EEGLAB 预处理。
- 所有刺激特征与 EEG 数据统一下采样至100 Hz，用于 mTRF 拟合。

### 3. 对比条件与指标
- 双任务对比：高负荷 vs. 低负荷；
- 测试各层级的追踪差异；
- 验证独立视觉与声学跟踪的负荷效应。

---

## 四、资源与算力

- 论文**未报告具体硬件配置**（如GPU类型、CPU规格或计算时长）。  
  EEG 数据分析主要基于 Python 工具包（Eelbrain、MNE-Python、EEGLAB），属 CPU 运算任务，对算力需求较低。  
  因此未出现深度学习类高算力需求。

---

## 五、实验数量与充分性

- **实验组别**：两种视觉负荷条件 × 听觉任务固定 → 共2种主要任务条件。  
- **分析维度**：5类特征追踪（视觉、声学包络与起始、语言三层级）。  
- **实验重复性**：
  - 每被试15试次、5折交叉验证；
  - 对各层特征使用聚类置换检验；
  - 行为与神经指标并行验证。  
- **总体评价**：实验设计严谨，统计方法稳健，**样本量略小但与同类EEG研究相当**；实验充分支持主要结论。

---

## 六、主要发现与结论

1. **行为结果**：
   - 高负荷视觉任务显著降低语音理解准确率；
   - 听力理解的下降不与视觉反应时或准确率显著相关，表明注意力资源竞争独立。
2. **神经结果**：
   - **句子层级**：高负荷条件下Δ方差解释率显著下降，反映句子级语境追踪减弱，效应在约200–300 ms出现。
   - **词形层级**：存在显著追踪，但不随任务负荷变化。
   - **次词汇层级**：未检测到显著追踪，可能受噪声干扰影响。
   - **声学层级**：包络与起始信号的神经追踪在两种负荷下无差异。
   - **视觉追踪**：在高负荷条件下反而增强，说明注意资源集中于视觉主任务。
3. **总体结论**：
   - 双模态注意分配不会影响声学或低级语言加工；
   - 但会**选择性削弱高层句子语境整合**；
   - 多任务情境下语音理解下降主要源自**高级语义预测与整合阶段的资源不足**。

---

## 七、研究优点

- **创新性**：首次在**噪声环境**下探索双模态注意对语言多层级语义表征的调制。
- **方法先进**：结合信息论指标与 mTRF 编码模型，实现从刺激到脑反应的层级解释。
- **实验设计贴近真实情境**：使用自然连续语音（audiobook），提高生态效度。
- **严谨分析**：使用跨试次交叉验证与贝叶斯因子，确保结果稳健可靠。
- **理论贡献**：揭示句子层级表征依赖认知资源支持，为语言预测与注意理论提供神经证据。

---

## 八、不足与局限

- **样本规模有限**（n=24），难以捕捉个体差异。
- **噪声类型与信噪比单一**：仅采用固定多说话人噪声（5 dB SNR），结果可推广性有限。
- **任务类型局限**：仅考查视觉空间工作记忆任务；其他跨模态任务（如视觉对象识别）未测试。
- **未报告算力与时长**：再现实验时需额外估计资源。
- **无脑区源定位分析**：仅基于头皮电位，未进一步溯源皮层区间差异。
- **未探讨年龄或语言能力效应**：研究对象仅限年轻英语母语者。

---

**（完）**
