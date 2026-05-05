---
title: Effects of bimodal divided attention on cortical representations of linguistic context during continuous speech perception in noise
title_zh: 双模态分散注意对噪声中持续语音感知时语言上下文皮层表征的影响
authors: "Xie, Z."
date: 2026-05-01
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.28.721419v1.full.pdf"
tags: ["query:q8"]
score: 9.0
evidence: 双模态注意分配与言语中的语言语境加工
tldr: 本研究探讨在噪声环境中同时进行视觉任务时，对连续语音理解的影响。通过EEG和多变量时间响应函数模型分析，发现双模态注意分配主要削弱了句子层面的语言语境处理，而低层级语言和声学处理较为稳定，揭示了多任务情境下语言理解受限的神经机制。
source: biorxiv
selection_source: fresh_fetch
motivation: 研究多模态注意分配如何影响噪声中语音理解的语言加工层级。
method: 采用EEG记录受试者在噪声背景下听故事并执行不同负荷视觉任务，利用mTRF模型解析语言层级信息。
result: 高负荷双任务条件下，句子层级的语言语境神经表征显著减弱，而词形层级与声学特征的表征未受影响。
conclusion: 双模态分心选择性干扰高层语言语境加工，而低层加工保持稳定。
---

## 摘要
语音感知常常发生在存在多种感官输入竞争的环境中，包括听觉内部及跨模态的竞争；例如，在嘈杂的咖啡馆中一边跟随对话，一边同时阅读菜单。本研究探讨了在噪声环境中持续语音感知过程中，将注意力分配于听觉与视觉双模态（双模态分散注意）在多层级语言上下文处理中的影响。研究通过脑电图（EEG）记录参与者在多人谈话噪声背景下将收听有声读物故事作为次要任务，同时执行一项施加低或高认知负荷的主要视觉任务的脑活动。行为结果显示，在高负荷双任务条件下，相较于低负荷条件，语音理解准确率显著降低。研究使用多变量时间响应函数（mTRF）编码模型，根据信息论指标（熵与意外度）预测不同层级（次词汇、词形及句子）语言上下文的EEG响应。结果显示，在词形和句子层级上存在显著的神经追踪效应，而在次词汇层级未观察到这种效应。关键发现是：与低负荷相比，高负荷条件下句子层级语言表征的神经追踪显著减弱，该效应在超过200毫秒的潜伏期后出现。相比之下，词形层级的神经追踪不受双任务负荷的影响。mTRF分析进一步表明，对声学特征的神经追踪不受双任务负荷调节。这些发现表明，双模态分散注意选择性地扰乱了大脑皮层对句子层级语言上下文的表征，而较低层级的处理相对保留。这种高层语言加工的损伤可能导致在嘈杂环境下多任务处理时语音理解能力的降低。

## Abstract
Speech perception often takes place in environments with competing sensory inputs, both within the auditory modality and across modalities; for example, following a conversation in a noisy cafe while simultaneously reading a menu. This study examined the extent to which dividing attention between auditory and visual modalities (bimodal divided attention) influences linguistic context processing across hierarchical levels during continuous speech perception in noise. Electroencephalographic (EEG) responses were recorded while participants listened to audiobook stories in multitalker babble as a secondary task, concurrently performing a demanding primary visual task that imposed either low or high cognitive load. Behaviorally, speech comprehension accuracy was significantly lower under high-load than low-load dual-task conditions. Multivariate temporal response function (mTRF) encoding models were used to predict EEG responses from information-theoretic measures (entropy and surprisal) indexing linguistic context at sublexical, word-form, and sentence levels. Significant neutral tracking was observed at the word-form and sentence levels, but not the sublexical level. Critically, neutral tracking of sentence-level linguistic representations was significantly reduced under high compared to low load, with effects emerging at latencies beyond 200 ms. In contrast, neutral tracking of word-form-level representations was unaffected by dual-task load. mTRF analyses further revealed that neutral tracking of acoustic features was not modulated by dual-task load. These findings indicate that bimodal divided attention selectively disrupts cortical representations of sentence-level linguistic context, while lower-level processing remains relatively preserved. Such impairments in higher-level linguistic processing may contribute to reduced speech comprehension during multitasking in noisy environments.

---

## 论文详细总结（自动生成）

# 论文总结：双模态分散注意对噪声中持续语音感知时语言上下文皮层表征的影响

---

## 一、研究核心问题与背景

- **核心问题**：在现实环境中，人们常常需要同时处理来自不同感官的输入（例如噪声中的听觉理解与视觉任务）。该研究关注的是**跨模态注意分配（听觉与视觉双任务）如何影响不同层级的语言加工**，具体探讨其对大脑皮层中语言上下文表征的影响。  
- **研究动机**：
  - 过去研究多聚焦于单模态听觉注意下的语言加工，对跨模态分心条件下的语言理解机制缺乏认识。
  - 特别是在“噪声环境”中，听觉解析和语言预测需要更多认知资源，因此研究者希望揭示高认知负荷时语言语境处理的神经机制。
- **整体目标**：通过EEG和信息论建模，探究双模态注意与认知负荷对语音感知中语言上下文层级（次词汇、词形、句子）的选择性影响。

---

## 二、方法论与技术框架

- **核心思想**：采用多变量时间响应函数模型（mTRF）来建立语音特征与脑电信号之间的映射，从不同语言层级的语境指标预测EEG反应。
- **关键技术细节**：
  - **EEG编码模型（mTRF）**：利用时间延迟多元回归，根据刺激特征（声学、语言、视觉）预测不同时间点的脑电响应。
  - **信息论指标**：
    - *Surprisal（意外度）*：当前语言单位（音素 / 词）给定上下文后的统计罕见程度。
    - *Entropy（熵）*: 对下一个语言单元的预测不确定性。
  - **语言层级建模**：
    - 次词汇层级：基于5-gram音素序列模型。
    - 词形层级：基于词识别的“cohort model”，逐音素更新词汇候选。
    - 句子层级：结合前四个单词的上下文，构建词级5-gram语法模型。
  - **特征提取**：
    - 声学特征：gammatone谱、声强包络、声学突变（onset）。
    - 视觉特征：刺激出现与消失时点、受试者反应时点。
  - 模型性能指标为各预测器对EEG信号的**解释方差变化（Δ% variance explained）**。

---

## 三、实验设计与数据来源

- **实验样本**：24名18–23岁的英语母语年轻成人（无听力或视力障碍）。  
- **实验任务**：
  - **双任务范式**：
    - 主任务：视觉空间 n-back 任务（0-back = 低负荷；3-back = 高负荷）。
    - 次任务：听取《爱丽丝梦游仙境》有声读物片段（伴随多人谈话噪声，信噪比为 5 dB）。
  - 任务指标：
    - 视觉：准确率与反应时（RT）。
    - 听觉：故事理解题正确率。
- **EEG采集**：
  - 64电极，采样率 5 kHz，记录于隔音室，使用 Brain Products actiCHamp Plus 设备。
- **Benchmark 与比较**：
  - 对比条件：低负荷 vs. 高负荷双任务。
  - 跨模型对比：去除特定预测器的 mTRF 模型（消融分析）。

---

## 四、资源与算力说明

- 文中**未提及具体算力或硬件配置**，未说明使用的GPU/CPU型号、训练时长或计算耗时。  
- 所用分析工具包括 Python 工具包 **Eelbrain**、**EEGLAB**、**MNE-Python**，模型计算主要为脑电线性回归与交叉验证，不涉及深度学习训练。

---

## 五、实验数量与充分性

- 共进行了 **两组主要条件实验**（低负荷与高负荷），每组 15 次试验。  
- **统计分析**：
  - 采用**五折交叉验证**进行模型评估。
  - 使用**t检验与置换检验（cluster-based permutation tests）**确定显著性。
- **消融与对比实验**：
  - 分别去除声学、视觉、语言层级预测器以评估追踪强度。
  - 进行了行为分析与神经反应（TRF）分析两个层面。
- **实验充分性**：从行为、神经层级双重验证；组间平衡与反复交叉验证保证客观性。但样本量相对较小（n=24），在个体变异上的统计力度有限。

---

## 六、主要结论与发现

- **行为层面**：
  - 高负荷下视觉准确率下降、反应时间延长，语音理解显著降低。
- **神经层面**：
  1. **句子层级处理**：在高负荷条件下神经追踪显著减弱，影响出现在约220–300毫秒延迟阶段。
  2. **词形层级处理**：保持稳定，不受负荷影响。
  3. **次词汇层级处理**：在噪声中未检测到显著追踪。
  4. **声学特征追踪**：未受任务负荷影响，表明早期听觉加工稳定。
  5. **视觉反应**：高负荷条件下视觉刺激追踪增强，反映资源向视觉分配。
- **总体结论**：  
  双模态分散注意主要影响句子层级（高级语言整合）而非低层声学或词汇加工，揭示了**多任务条件下语言预测的层级选择性受限机制**。

---

## 七、优点与创新

- **方法创新**：
  - 将 mTRF 编码模型与信息论语言指标（surprisal/entropy）结合，用于连续自然语音的层级加工分析。
  - 引入真实噪声环境与双模态任务，提升生态有效性。
- **设计亮点**：
  - 对语言处理进行多层级建模（音素→词→句），体现语言加工的层次化脑表征。
  - 联合行为与EEG证据，定量验证注意分配的神经效应。
- **分析严谨性**：
  - 采用置换检验和交叉验证，降低偶然统计的风险。
  - 在模型中同时控制声学与视觉预测因子，确保对语言效应的独立评估。

---

## 八、不足与局限

- **样本规模**较小（24人），不代表广泛人群。  
- **任务类型单一**：仅使用视觉空间 n-back任务，未比较不同视觉任务形式（如视觉对象任务）。  
- **噪声条件单一**：仅一个多谈话噪声类型和单一信噪比（5 dB），局限于特定听觉难度。  
- **算力与参数透明度不足**：未说明计算细节和时间成本。  
- **个体差异未深入讨论**：如注意力能力、语言熟练度或认知水平对结果的调节作用。  
- **扩展性限制**：尚未检验该机制在老年或听力损失人群中的适用性。

---

（完）
