---
title: Effects of bimodal divided attention on cortical representations of linguistic context during continuous speech perception in noise
title_zh: 双模态分散注意对噪声中连续语音感知过程中语言语境皮层表征的影响
authors: "Xie, Z."
date: 2026-05-01
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.28.721419v1.full.pdf"
tags: ["query:profile-1"]
score: 9.5
evidence: 双模态注意分配期间对语言语境的脑电反应
tldr: 本研究探讨双模态分注意对噪声中言语感知的影响，通过EEG与mTRF模型分析不同语言层级的神经表征。结果发现，高负荷视觉任务削弱了句子层面语言语境的脑表征，而较低层次的词形和声学加工保持稳定，为理解多任务情境下言语理解受损提供神经机制依据。
source: biorxiv
selection_source: fresh_fetch
motivation: 本研究旨在探明跨模态分注意对连续噪声言语感知中语言语境处理的影响。
method: 研究通过EEG记录受试者在噪声中听有声书并同时完成视觉任务的脑反应，利用mTRF模型分析不同语言层级的信息加工。
result: 高认知负荷的视觉任务显著降低句子层面语境的神经跟踪，而词形层和声学特征的跟踪不受影响。
conclusion: 研究表明，在噪声环境中进行双任务处理时，高级句子层面语言语境的神经表征被选择性削弱，导致言语理解下降。
---

## 摘要
语音感知常常发生在伴有竞争性感觉输入的环境中，这些输入既可能来自听觉通道，也可能跨越不同感官模态；例如，在嘈杂的咖啡馆中一边听对话一边读菜单。本研究考察了在噪声中进行连续语音感知时，将注意力在听觉和视觉模态之间分配（双模态分散注意）对不同层级语言语境加工的影响。实验记录了受试者在多讲话者背景噪声中聆听有声书故事时的脑电图（EEG）反应，这一听觉任务为次要任务，同时受试者需执行一个要求较高的主要视觉任务，以施加低或高的认知负荷。行为结果显示，在高负荷的双任务条件下，语音理解的准确率显著低于低负荷条件。研究采用多变量时间响应函数（mTRF）编码模型，根据信息论指标（熵与惊讶度）预测EEG反应，这些指标刻画了词以下（sublexical）、词形和句子三个层级的语言语境。结果显示，在词形和句子层级观察到显著的神经追踪（neural tracking），但在词以下层级未发现显著效应。关键的是，与低负荷条件相比，高负荷条件下句子层级语言表征的神经追踪显著减弱，该效应在200毫秒之后的潜伏期出现。相比之下，词形层级表征的神经追踪不受双任务负荷影响。mTRF分析进一步表明，声学特征的神经追踪不会随双任务负荷而变化。这些发现表明，双模态分散注意会选择性地干扰句子层级语言语境的皮层表征，而较低层级的加工相对保持稳定。此类高层语言加工的损伤可能导致在嘈杂环境下多任务条件下语音理解能力的下降。

## Abstract
Speech perception often takes place in environments with competing sensory inputs, both within the auditory modality and across modalities; for example, following a conversation in a noisy cafe while simultaneously reading a menu. This study examined the extent to which dividing attention between auditory and visual modalities (bimodal divided attention) influences linguistic context processing across hierarchical levels during continuous speech perception in noise. Electroencephalographic (EEG) responses were recorded while participants listened to audiobook stories in multitalker babble as a secondary task, concurrently performing a demanding primary visual task that imposed either low or high cognitive load. Behaviorally, speech comprehension accuracy was significantly lower under high-load than low-load dual-task conditions. Multivariate temporal response function (mTRF) encoding models were used to predict EEG responses from information-theoretic measures (entropy and surprisal) indexing linguistic context at sublexical, word-form, and sentence levels. Significant neutral tracking was observed at the word-form and sentence levels, but not the sublexical level. Critically, neutral tracking of sentence-level linguistic representations was significantly reduced under high compared to low load, with effects emerging at latencies beyond 200 ms. In contrast, neutral tracking of word-form-level representations was unaffected by dual-task load. mTRF analyses further revealed that neutral tracking of acoustic features was not modulated by dual-task load. These findings indicate that bimodal divided attention selectively disrupts cortical representations of sentence-level linguistic context, while lower-level processing remains relatively preserved. Such impairments in higher-level linguistic processing may contribute to reduced speech comprehension during multitasking in noisy environments.

---

## 论文详细总结（自动生成）

# 双模态分散注意与噪声中语言语境加工的脑机制研究总结  

---

## 一、研究核心问题与整体动机

- **核心问题**：人在多任务情境下（如同时处理视觉与听觉信息）听懂语音的能力会下降，但在神经层面这种下降是因为哪一层语言加工受到影响？  
- **研究背景**：  
  - 日常交流常发生在嘈杂环境中，人们需要在跨模态的信息干扰下解析语言。  
  - 以往研究多关注单一听觉注意状态下的语音处理，对跨模态分散注意（bimodal divided attention）影响语言语境处理的机制了解有限。  
  - 作者旨在探明：分散注意是否会选择性影响高层级（句子层面）语言语境表征，而低层级（词形、音素等）表征可能相对稳健。

---

## 二、研究方法论

- **核心思想**：通过脑电（EEG）结合多变量时间响应函数模型（mTRF）来量化不同层级语言语境信息的神经表征。  
- **关键技术细节**：  
  - 使用 **信息论指标**——熵（entropy）与惊讶度（surprisal）衡量语言输入的预测性。  
  - 在不同语义层级构建三种语言模型：  
    1. **Sublexical 模型**：基于五音素 n-gram，预测下一个音素。  
    2. **Word-form 模型**：基于词的语音构成及词频，实现连续词形识别。  
    3. **Sentence 模型**：结合词间上下文（4-gram）计算当前词的概率分布，反映句子语境。  
  - **mTRF 编码模型流程**：  
    1. 将 EEG 信号与上述语音特征做时域延迟相关建模（−100 至 500 ms）。  
    2. 使用 boosting 算法与五折交叉验证估计模型解释度。  
    3. 对比 **完整模型**（含所有特征）与 **去除某特定特征的模型**，以解释度差值（Δ% explained variance）作为神经追踪强度指标。  
- **统计分析**：采用单侧 t 检验与基于簇的置换检验（cluster-based permutation test）验证显著效应。

---

## 三、实验设计与数据来源

- **受试者**：24 名 18–23 岁健康青年（20 女），母语为英语，无听觉或神经异常。  
- **实验条件**：  
  - 双任务设计：  
    1. **主要任务**：视觉空间 n-back（低负荷为 0-back，高负荷为 3-back）；  
    2. **次任务**：在多说话人背景噪声下聆听《爱丽丝梦游仙境》有声书片段并回答理解题。  
  - 噪声类型：来自 **NOISEX-92 数据集**的 100 人“食堂噪声”，信噪比设为 +5 dB。  
  - 每任务条件含 15 次试验（每次约 60 秒），并在条件间进行顺序平衡。  
- **Benchmark 设计**：直接比较 **高负荷 vs 低负荷双任务条件**；无引入其他算法模型对比，但引用先前的 Brodbeck et al. (2022) 与 Xie et al. (2023) 作为参考基线。  

---

## 四、资源与算力

- 文中未涉及 GPU、CPU 型号或计算资源规模。  
- 所有分析在 Python (MNE、Eelbrain)、R 环境运行，使用线性回归与置换统计，属脑电信号分析方法，无显著算力需求。  

---

## 五、实验数量与充分性

- 共 **两种双任务条件（高负荷与低负荷）**，每种条件 15次试验，总计每人约 30 次试验。  
- 分析维度包括：  
  1. 行为（视觉命中率、反应时、听觉理解准确率）；  
  2. 神经追踪（声学特征、三类语言层级、视觉特征）。  
- 统计采用校正置换检验，显著性与效应量均报告。整体实验数量中等，覆盖行为与神经层级，但**未涉及跨个体差异或重复任务验证**。

---

## 六、主要结论与发现

1. **行为层面**：  
   - 高认知负荷下视觉任务准确率显著下降、反应时延长；  
   - 听觉理解准确率大幅降低（平均从 79% 降至 60%）。  
2. **神经层面**：  
   - 声学特征（波形、包络）追踪稳定，不随负荷变化；  
   - **句子层面语言语境追踪显著下降**（效应出现在约 220–300 ms）；  
   - 词形层与词以下层无显著变化；  
   - 视觉刺激追踪随负荷增强，表现注意资源转移至视觉模态。  
3. **综合结论**：双模态分散注意会选择性削弱高层级的语言语境处理，使神经系统的句子整合能力下降，从而导致语义理解受损。

---

## 七、研究优点与亮点

- 采用 **自然语篇（有声书）+ EEG** 的设计，贴近现实多任务听觉场景。  
- 利用 **信息论指标与 mTRF 建模**，成功量化跨层语言预测在时域的神经动态。  
- 区分 **声学加工与语言层级加工**，明确多任务干扰的层次定位。  
- 实验控制严谨（噪声参数、任务顺序、听力筛查），结果解释相对清晰。

---

## 八、不足与局限

- **数据维度**：仅含单一噪声类型与固定信噪比（+5 dB），缺乏多噪声条件验证。  
- **任务组合**：仅使用视觉空间 n-back；其他视觉任务类型（如物体识别）可能产生不同分配效应。  
- **样本量较小**（n=24），尚未纳入老年或听力下降群体，外推性有限。  
- **缺乏模型层面的比较或消融**：未测试不同语言模型参数对结果的稳健性。  
- **算力与可重现性细节不足**：缺乏公开代码和运行环境说明。  

---

**（完）**
