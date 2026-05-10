---
title: Representational similarity of hemodynamic brain responses to written and spoken words increases when learning to read
title_zh: 学习阅读时书面与口语词的脑血流动力学反应表征相似性增加
authors: "Maruo, K., Kessler, R., Huettig, F., Skeide, M. A."
date: 2026-05-09
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.08.723790v1.full.pdf"
tags: ["query:q9"]
score: 9.0
evidence: 比较大脑对书面语和口语单词的反应
tldr: 本研究利用fMRI探讨61名不同阅读阶段儿童在听觉和视觉词汇识别中的脑活动相似性，发现随阅读经验增加，语言相关脑区（尤其左后颞上回）的跨模态表征相似性线性增强，揭示了阅读学习中听视整合机制的神经变化。
source: biorxiv
selection_source: fresh_fetch
motivation: 研究旨在探究儿童在学习阅读过程中大脑如何将听觉与视觉信息跨感官整合。
method: 研究采用功能性磁共振成像(fMRI)测量61名不同阅读水平小学生在听写单词任务下的脑部反应。
result: 结果发现随年级提升，额下回、顶下小叶、颞上回和颞枕皮层的视听表征相似性线性增加，尤其在左后颞上回显著。
conclusion: 研究表明学习阅读会导致语言相关脑区中听觉和视觉词汇表征的相似性逐步增强。
---

## 摘要
学习阅读需要将听觉和视觉信息联系起来，但发育中的大脑如何跨感官通道映射信息仍然知之甚少。为探讨这一问题，我们采用功能性磁共振成像（fMRI），在61名具有不同阅读经验的小学生中，研究他们在识别口语和书面单词或伪词时的脑血流动力学反应。结果显示，下额额回、下顶叶小叶、上颞回和颞枕皮层的脑激活模式在听觉与视觉维度上的表征相似性随年级线性增加，其中左后上颞回的效应最为显著。我们的结果表明，学习阅读与语言经典区域中听觉与视觉词表征的逐步增强的相似性有关。

## Abstract
Learning to read requires linking auditory and visual information, yet how the developing brain maps information across sensory modalities remains poorly understood. To shed light on this topic we employed functional MRI to investigate hemodynamic brain responses during spoken and written word or pseudoword recognition in 61 primary school children with different levels of reading experience. Audiovisual representational similarity of activation patterns in the inferior frontal gyrus, inferior parietal lobule, superior temporal gyrus, and temporo-occipital cortex, increased linearly with school grade and this effect was largest in the left posterior superior temporal gyrus. Our results suggest that learning to read is related to a progressively increasing similarity of auditory and visual word representations within canonical language areas.

---

## 论文详细总结（自动生成）

# 学习阅读时书面与口语词的脑血流动力学反应表征相似性增加 — 论文总结

---

## 一、核心问题与研究背景

- **研究动机**：学习阅读是人类认知发展的关键阶段，需要将听觉（口语）与视觉（书面文字）信号进行跨模态整合。然而，儿童大脑中这种跨感官映射机制如何形成和演变，仍缺乏系统的神经层面证据。
- **核心问题**：在儿童的学习阅读过程中，大脑对“书面词”和“口语词”的响应模式是否随着阅读经验的增加而变得更加相似？这种相似性的变化是否具有特定的脑区分布和发展趋势？
- **整体含义**：本研究旨在揭示阅读学习过程中语言处理区域的功能重组，从神经表征相似性的角度说明视觉词汇学习如何与听觉语言系统相整合，为阅读障碍研究与教育干预提供神经机制支持。

---

## 二、方法论

- **核心思想**：利用 **功能性磁共振成像（fMRI）** 测量儿童在识别书面与口语单词时的脑部血流动力学活动，通过 **表征相似性分析（Representational Similarity Analysis, RSA）** 计算两种感官刺激的脑活动模式之间的相似度。
- **关键技术细节**：
  - 对每个受试者的脑激活模式进行提取，在相同脑区内比较书面与口语条件的活动空间构型。
  - 使用线性模型（grade × similarity）探讨随阅读经验变化的相似性趋势。
  - RSA 采用基于 voxel 的多变量模式相似性度量（例如皮尔逊相关或余弦相似度）。
- **算法流程（文字说明）**：
  1. 获取 fMRI 数据（书面词任务、口语词任务）。
  2. 对每个脑区提取激活分布模式。
  3. 计算跨模态相似性指标。
  4. 将相似性结果与受试者阅读水平 / 年级进行线性拟合。
  5. 分析随年级增长的趋势及显著性。

---

## 三、实验设计

- **受试者与数据场景**：61 名小学阶段儿童，涵盖不同阅读水平与年龄层。
- **任务类型**：视觉阅读任务（书面单词或伪词辨识）与听觉语言任务（听口语单词或伪词辨识）。
- **测量指标**：脑血流动力学反应 (BOLD 信号) 的跨模态表征相似性。
- **比较维度**：不同脑区（如额下回、顶下小叶、上颞回、颞枕皮层）及不同年级之间的表征差异。
- **Benchmark / 对照**：年级变化与阅读水平作为自然梯度；未涉及外部算法对比（非机器学习类研究）。

---

## 四、资源与算力

- **算力说明**：文中未提及具体计算资源（如 GPU 型号、数量或数据处理算力）。
- **可能情况**：由于研究基于人类 fMRI 数据分析，主要依赖常规神经影像处理平台（如 SPM、FSL 或 Python/Nilearn），无高性能计算训练需求。

---

## 五、实验数量与充分性

- **总体实验结构**：
  - 单一主实验：对 61 名儿童进行 fMRI 任务。
  - 任务条件：听觉 vs 视觉 × 单词 vs 伪词，共四种刺激类型。
  - 分析层面：跨脑区的表征相似性线性分析。
- **充分性评估**：
  - 被试量在儿童神经认知研究中属中等规模，统计功效可靠。
  - 使用多个脑区、多个刺激条件体现了多维度验证。
  - 但研究主要集中在横断面分布（不同年级比较），未追踪个体纵向变化。

---

## 六、主要结论与发现

- **核心发现**：
  - 随阅读经验的提升（年级增加），听觉与视觉单词表征的相似性显著增强。
  - 这种增强主要发生在经典语言处理区域，尤其是 **左后上颞回（posterior superior temporal gyrus）**。
  - 表征相似性的增长被解读为儿童阅读学习过程中，视觉-听觉整合网络逐步成熟的神经标志。
- **科学意义**：
  - 揭示了阅读学习过程中听觉语言系统与视觉识字系统的功能融合趋势。
  - 为理解阅读习得、语音—文字映射发展及早期阅读障碍提供神经基础。

---

## 七、优点与亮点

- **方法创新**：
  - 将 RSA 应用于儿童阅读发展的跨模态神经分析，较传统单任务激活分析更加细致。
- **实验设计合理**：
  - 使用自然梯度（年级）进行发展分析，避免人为分组偏差。
  - 涵盖典型语言区及视觉相关皮层的整合分析，体现出全脑网络视角。
- **重要启示**：
  - 强调阅读学习不是单纯视觉技能提升，而是跨感官神经网络的协同重塑。

---

## 八、不足与局限

- **样本与设计限制**：
  - 研究为横断面设计，无法直接确认因果关系或个体随时间变化。
  - 样本仅限小学阶段儿童，未涵盖更广的年龄和文化背景。
- **数据局限**：
  - fMRI 空间分辨率有限，无法捕捉更细微的神经连接或时间动态。
- **分析范围**：
  - 聚焦于表征相似性指标，未加以功能连通性或行为表现（阅读成绩）的整合分析。
- **外推性**：
  - 研究结果主要适用于以字母语言为母语的儿童，对表意文字（如中文）尚未验证。

---

（完）
