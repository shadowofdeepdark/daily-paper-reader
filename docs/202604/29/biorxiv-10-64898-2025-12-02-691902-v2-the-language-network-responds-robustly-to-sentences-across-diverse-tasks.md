---
title: The language network responds robustly to sentences across diverse tasks
title_zh: 语言网络在多种任务中对句子产生强烈反应
authors: "Gao, R., Cheung, C., Siegelman, M., Pongos, A. L. A., Kean, H. H., Tanner, A., Fedorenko, E., Ivanova, A. A."
date: 2026-04-27
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.02.691902v2.full.pdf"
tags: ["query:profile-1"]
score: 8.0
evidence: 语言网络在不同阅读任务中的稳定性
tldr: 本研究探讨语言相关脑区在不同阅读任务下的稳定性，52名受试者在六种任务条件下阅读句子与无词串。结果显示语言网络对句子的反应在各任务中保持一致，而多需求网络在有任务时才显著激活，揭示了两种网络在语言理解与任务执行中的互补作用。
source: biorxiv
selection_source: fresh_fetch
motivation: 研究者想了解语言网络在不同任务情境下的稳定性，以及与多需求（MD）网络的任务敏感性比较。
method: 研究通过fMRI测量52名参与者在六种阅读任务条件下的脑区激活，并比较语言网络与MD网络的响应特征。
result: 语言网络在所有任务中对句子都有稳健反应，而MD网络主要随着任务出现而活动。
conclusion: 语言网络主要处理语言输入的意义，而MD网络负责与任务相关的需求控制。
---

## 摘要
左额叶和颞叶的大脑区域网络支持语言理解与生成，执行与词汇提取及语言组合加工相关的计算。本研究探讨：语言网络对语言刺激的反应在不同任务情境下的稳定性如何，以及这种稳定性与领域通用的多重需求（MD）网络的任务敏感性相比如何？参与者（n=52）在六种任务条件下阅读句子和无词串，包括被动阅读、带记忆探针的阅读，以及需要深度语义参与的问答阅读。句子>无词的对比在所有任务中都识别出了相同的一组语言响应体素；这些体素的位置具有个体特异性，凸显了基于个体的功能定位的重要性。因此，我们得出结论：语言定位在任务变化下具有较强的稳健性。随后，我们考察了这些语言响应体素（语言网络）以及领域通用MD网络中的反应强度和精细激活模式，以测试任务需求是否调节语言计算和/或招募不同的大脑系统。结果显示，语言网络在所有任务中都对句子表现出强烈的反应，在语义参与度较高的任务中反应略强。相比之下，MD网络在存在任务时对句子和无词均有反应，这提示在使用包含任务要求的语言范式时需谨慎，因为此类范式会同时激活两个独立的网络。多变量分析进一步表明，刺激信息在语言网络中更易于解码，而任务信息在MD网络中更易于解码。这些结果表明，语言网络与MD网络在任务驱动的语言理解过程中履行互补功能：语言网络主要从语言输入中提取信息，而MD网络则决定任务所需的适当响应。

## Abstract
A network of left frontal and temporal brain areas supports language comprehension and production, implementing computations related to word retrieval and combinatorial linguistic processing. Here, we ask: to what extent are responses to language in this language network stable across task contexts, and how does this stability compare to task sensitivity in the domain-general multiple demand (MD) network? Participants (n=52) read sentences and nonword lists under six task conditions, including passive reading, reading with a memory probe after each stimulus, and reading and answering questions that require deep semantic engagement. The sentences>nonwords contrast isolated the same set of language-responsive voxels across all tasks; the locations of those voxels were participant-specific, highlighting the value of individual-specific functional localization. We therefore conclude that language localization is robust to task variation. We then examined the magnitudes and fine-grained activation patterns in these language-responsive voxels (the language network) and in the domain-general MD network, to test whether task demands modulate linguistic computations and/or recruit a distinct brain system. The language network responded robustly to sentences across all tasks, with somewhat higher responses to semantically engaging tasks. In contrast, the MD network responded to both sentences and nonwords in the presence of a task, which warrants caution when using language paradigms that include task demands, as such paradigms engage two independent networks. A multivariate analysis further revealed that stimulus information is more easily decodable in the language network, whereas task information is more decodable in the MD network. These results suggest that the language and MD networks perform complementary functions during task-driven language comprehension, with the language network primarily extracting information from linguistic input and the MD network determining the appropriate response to the task.

---

## 论文详细总结（自动生成）

# 论文总结：语言网络在多种任务中对句子产生强烈反应

---

## 一、核心问题与研究背景

- **研究动机**：人类大脑中存在一组专门用于语言处理的区域，称为“语言网络”，主要分布在左额叶和颞叶。该网络在各种语言条件下都会被激活。然而，过去的研究对于这些语言区域在不同任务情境下的稳定性知之甚少。  
- **核心问题**：  
  - 语言网络在不同阅读任务（被动阅读、记忆探针、语义判断等）中是否表现稳定？  
  - 与之相比，领域通用的“多重需求网络（MD network）”在任务变化中表现出怎样的敏感性？  
- **理论意义**：探讨语言网络在认知层级中的位置，即它更像是感知系统（稳定响应）还是执行系统（响应随任务变化强烈波动）。  
- **实践意义**：明确语言网络的稳定性可指导脑功能定位方法，避免任务引起的非语言混淆。

---

## 二、方法论与研究策略

- **核心思想**：通过系统地改变语言任务的需求强度，在相同受试者与相同刺激下分析语言网络与MD网络的响应差异，以量化语言网络的任务独立性。  
- **技术路径**：
  1. 使用 **fMRI** 测量大脑在六种语言任务中的响应（句子 vs. 无词串）。  
  2. 采用 **组约束的个体功能区定义（Group-Constrained Subject-Specific, GSS）方法** 来获得每位参与者的语言与MD功能区（fROI）。  
  3. 使用 **广义线性模型（GLM）** 估计每个实验条件的BOLD信号变化。  
  4. 进行 **空间重叠分析（Dice系数）** 与 **空间相关分析**，评估不同任务间的体素一致性。  
  5. 进行 **多变量模式解码（Multivariate Pattern Analysis, MVPA）**，检测激活模式中可分辨出的刺激类型与任务类型信息。  
  6. 所有统计分析使用 **混合效应模型（Mixed-effects models）** 进行，以控制个体差异和随机效应。  

---

## 三、实验设计

- **受试者**：共 52 名（平均年龄 23.9 岁，其中 31 名女性），来自麻省理工学院及周边社区。  
- **任务类型（共六种）**：
  1. V1：简单按钮任务（接近被动阅读）  
  2. V2：困难记忆探针任务  
  3. V3：简单记忆探针任务  
  4. V4：带问题的按钮任务  
  5. V5：内容理解问答任务  
  6. V6：情绪/情感判断任务  
- **刺激材料**：
  - 句子：从标准语言语料库（Brown Corpus）抽取的 12 字长英文句子。  
  - 非词串：由Wuggy软件生成的可发音无意义词列表。  
- **对照网络**：MD网络由空间工作记忆任务（困难 vs. 简单）激活来界定。  
- **分析层级**：同时比较语言网络与MD网络的句子与非词串响应、不同任务下的模式稳定性与可解码性。  

---

## 四、资源与算力

- **设备**：使用麻省理工学院 McGovern 脑研究所的 3 特斯拉 Siemens Trio 扫描仪，32 通道头部线圈。  
- **数据类型**：结构像与功能像。时间分辨率 TR=2000ms，空间分辨率 2.1×2.1mm。  
- **算力说明**：论文为功能磁共振成像研究，无GPU计算或模型训练过程，因此未涉及GPU或训练算力。  

---

## 五、实验数量与充分性

- **任务数量**：六种语言任务版本 × 两种刺激类型（句子 / 非词串），每位受试者完成至少3-5个版本。  
- **分析维度**：  
  - 语言与MD网络双重区域分析；  
  - 六种任务条件下的响应幅度对比；  
  - 空间重叠、一致性及解码分析共开展约十余种统计检验。  
- **充分性与公平性**：  
  - 所有对比均在同一参与者内进行（避免跨被试变异），并使用混合效应模型消除不平衡实验条件影响。  
  - 包含补充分析（默认网络 DMN）及多种验证指标（Dice、相关、FDR校正），实验设计全面，统计控制充分。

---

## 六、主要结论与发现

1. **语言网络稳定性**：  
   - 无论任务类型如何，语言网络在句子相较于无词串的对比中都表现强烈激活。  
   - 同一受试者在不同任务下的语言区域空间重叠度高（Dice 系数平均 0.50-0.59）。  
2. **任务影响**：  
   - 有任务时语言网络反应略增强，但核心选择性（句子 > 无词）保持不变。  
   - MD 网络仅在存在认知任务时被显著激活，且反应强度与任务难度正相关。  
3. **多变量分析**：  
   - 在语言网络中更易解码 **刺激类型**（句子 vs 无词），准确率约 0.69。  
   - 在MD网络中更易解码 **任务类型**（三类任务区分），准确率约 0.42。  
4. **功能互补性**：语言网络主要负责语言输入的加工，而MD网络负责任务执行与认知调控。

---

## 七、优点与亮点

- ✅ **系统化任务比较**：首次在相同被试与相同材料下全面对比多种语言任务，排除设计差异干扰。  
- ✅ **个体层面功能定位**：使用GSS方法保证跨任务可重复、可移植的ROI定义。  
- ✅ **多层分析手段**：结合空间重叠、模式相关与MVPA解码，多角度验证语言网络稳定性。  
- ✅ **统计严谨**：混合效应模型控制随机因素，FDR与Bonferroni校正保证结果可靠。  
- ✅ **实用价值**：为语言功能定位提供简短、高效、跨任务稳健的实验范式依据。

---

## 八、不足与局限

- ⚠ **任务范围有限**：所有任务均为单句或简单问答，未涵盖真实对话或语篇层级语言。  
- ⚠ **样本单一**：研究对象为年轻、健康、英语母语者，不含儿童、老年及多语言群体。  
- ⚠ **任务与刺激不可完全独立**：更复杂任务可能引起重复加工或注意增强，导致解释歧义。  
- ⚠ **无跨模态验证**：仅使用阅读任务，听觉或口语任务尚待检验。  
- ⚠ **算力与临床扩展性限制**：研究依赖高端fMRI设备，现实应用条件受限。

---

（完）
