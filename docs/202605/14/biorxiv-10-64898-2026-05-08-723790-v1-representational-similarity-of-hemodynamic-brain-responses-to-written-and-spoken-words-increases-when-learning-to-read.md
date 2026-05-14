---
title: Representational similarity of hemodynamic brain responses to written and spoken words increases when learning to read
title_zh: 学习阅读时，书写词与口语词的血流动力学脑反应表征相似性增加
authors: "Maruo, K., Kessler, R., Huettig, F., Skeide, M. A."
date: 2026-05-09
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.08.723790v1.full.pdf"
tags: ["query:q9"]
score: 9.0
evidence: 使用fMRI比较书面语和口语的脑部反应
tldr: 本研究利用fMRI扫描61名处于不同阅读阶段的小学生，分析他们在听觉和视觉词汇识别任务中的脑反应模式。结果发现随着阅读经验积累，儿童大脑中听觉与视觉词汇表征在语言处理相关区域的相似性逐渐增强，揭示了阅读学习促进跨感官语言表征整合的神经机制。
source: biorxiv
selection_source: fresh_fetch
motivation: 研究旨在探讨儿童学习阅读过程中，大脑如何在听觉和视觉通道之间建立联系。
method: 使用功能性磁共振成像研究61名小学儿童在阅读和听词任务中的脑部激活模式。
result: 发现随年级提升，听觉与视觉词汇表征在多个语言相关脑区的相似性线性增加，尤其在左后上颞回最为显著。
conclusion: 学习阅读伴随大脑中语言相关区域听觉与视觉词汇表征相似性逐步增强，反映跨感官整合能力的成熟。
---

## 摘要
学习阅读需要将听觉与视觉信息进行关联，但发展中大脑如何跨感觉模式映射信息仍未被充分理解。为探究这一问题，我们采用功能性磁共振成像（fMRI），在61名具有不同阅读经验的小学生中测试他们在识别口语和书写词汇或伪词时的血流动力学脑反应。结果显示，下额额回、下顶叶小叶、上颞回和颞枕皮层的激活模式的视听表征相似性随年级呈线性增加，而这一效应在左后上颞回中最为显著。我们的结果表明，学习阅读与语言典型脑区中听觉和视觉词表征的相似性逐步增加有关。

## Abstract
Learning to read requires linking auditory and visual information, yet how the developing brain maps information across sensory modalities remains poorly understood. To shed light on this topic we employed functional MRI to investigate hemodynamic brain responses during spoken and written word or pseudoword recognition in 61 primary school children with different levels of reading experience. Audiovisual representational similarity of activation patterns in the inferior frontal gyrus, inferior parietal lobule, superior temporal gyrus, and temporo-occipital cortex, increased linearly with school grade and this effect was largest in the left posterior superior temporal gyrus. Our results suggest that learning to read is related to a progressively increasing similarity of auditory and visual word representations within canonical language areas.

---

## 论文详细总结（自动生成）

# 学习阅读时书写词与口语词的脑表征相似性发展研究总结

---

## 一、研究问题与背景

- **核心问题**：儿童在学习阅读的过程中，大脑如何将视觉（书写词）与听觉（口语词）的语言表征逐步建立联系？这种跨模态整合是否会随阅读经验（即年级）增加而增强？
- **研究动机**：
  - 阅读习得依赖于将视觉字母与听觉音位进行映射，即**字形-音位转换**（grapheme-to-phoneme conversion）。
  - 现有神经影像研究主要集中在单一模态（如听觉或视觉语言处理），缺乏对**多感官信息整合的神经机制**的系统探索。
  - 尤其在儿童早期阅读学习阶段，还不清楚听觉与视觉语言表征在空间模式上是趋同（相似）还是分化（独立）。
- **研究意义**：明确阅读习得过程中听觉与视觉语言表征的脑区变化，有助于理解正常阅读发展及阅读障碍（如阅读困难症）的大脑机制。

---

## 二、方法论

- **研究范式**：  
  采用 **功能性磁共振成像（fMRI）** 结合 **表征相似性分析（Representational Similarity Analysis, RSA）** 的多变量统计方法。
- **核心思想**：  
  不仅比较单一脑区的平均激活强度，而是分析不同模态（书写 vs. 口语）在同一区域的空间激活模式的相似性，来量化**视听表征的重叠程度**。
- **关键步骤**：
  1. **定义感兴趣区域（ROIs）**：基于Harvard–Oxford皮层图谱，选取九个阅读相关的经典脑区（如下额额回 IFG、顶下小叶 IPL、上颞回 STG、颞枕皮层 TOFC 等）。
  2. **构建表征异质矩阵（RDM）**：  
     - 对每名被试的不同任务条件下（书写词、口语词、伪词等）BOLD 信号进行空间向量化。  
     - 计算跨模态（视觉–听觉）的皮尔逊相关距离（1–r）以得到异质矩阵。
  3. **计算多模态相似性**：  
     - 取RDM中跨模态部分的平均相关系数（Fisher-z 转换后）。
  4. **统计分析**：
     - 对每个ROI进行单样本t检验（相似性是否显著高于0）。  
     - 采用线性回归检验相似性是否随年级增长呈线性上升。  
     - 以反应时为协变量控制注意力影响。  
     - 所有结果均经FDR校正（q < 0.05）。

---

## 三、实验设计

- **样本与任务**：
  - 招募印度新德里地区1–4年级小学生共93名，最终61名数据通过质量控制（5–10岁）。
  - 任务：语义判断任务。在fMRI中分别呈现四种刺激：
    - 书写词（有意义的视觉词）
    - 书写伪词（无意义的字母组合）
    - 口语词（听觉输入）
    - 口语伪词
  - 被试需判断刺激是否代表“动物”类别。
- **fMRI 参数**：
  - GE SIGNA 3T 扫描仪，TR=2000 ms, TE=30 ms, voxel size = 3×3×3 mm。
  - 每个被试包含3–8个运行（每次约4分钟半）。
- **分析工具**：
  - 预处理：fMRIPrep 25.1.4；模型建立与RSA分析：Python/Nilearn；统计分析：FDR 校正线性回归与t检验。
- **Benchmark**：无传统机器学习对比方法，主要通过假设检验不同年级间的变化规律。

---

## 四、资源与算力

- **硬件信息**：文中未报告任何GPU型号、内存或计算服务器配置。
- **数据处理量**：使用61名被试、每人多达8个fMRI运行，属于中等规模的神经影像数据集。  
  因为分析基于统计模型（非深度学习训练），对算力需求相对有限。
- **时长信息**：未明确说明分析所用计算时间。

---

## 五、实验数量与充分性

- **实验内容**：
  - 一次主要fMRI实验，分四种刺激条件（书写词/伪词、口语词/伪词）。
  - 九个ROI 统计 + 全脑48区重复回归分析。
  - 同时进行了：
    - 单样本t检验（检验跨模态相似性显著性）
    - 线性回归（检验年级效应）
    - 反应时回归（控制注意力影响）
- **充分性分析**：
  - 数据量对儿童fMRI研究而言较大（n=61）。
  - 涉及多脑区、多条件的统计分析，较为系统。  
  - 限制：为横截面设计，非纵向追踪，因果推断有限。

---

## 六、主要结论与发现

1. **跨模态相似性显著存在**：  
   所有主要语言相关脑区（如IFG、SMG、STG等）在视觉与听觉条件下均表现出显著的相似性。
2. **左后上颞回（pSTG）最显著**：  
   该区对书写词与口语词/伪词的表征最为相似，是视听整合的关键枢纽区。
3. **随年级逐渐增强**：  
   opIFG、aSMG、pSMG、Angular Gyrus、pSTG 和 TOFC 的多模态相似性随年级（阅读经验）线性上升。
4. **语义条件无类似趋势**：  
   对语义差异（词 vs. 伪词）的多模态相似性未见显著变化，提示变化主要源于字形-音位整合，而非语义加工。
5. **神经发育意义**：  
   阅读学习过程促进了视觉与听觉语言网络的整合，使得书写与口语表征在脑中逐步趋同。

---

## 七、优点与创新

- **多变量空间分析**：采用RSA代替传统的单体激活分析，更能捕捉复杂分布式模式。
- **儿童发展数据**：较大样本覆盖1–4年级，填补儿童多模态语音-文字整合的空白。
- **控制混杂因素**：通过反应时回归部分排除注意力影响。
- **跨脑区系统性验证**：结果不仅限于预选ROI，还在全左半球进行了验证，增加结论稳健性。

---

## 八、不足与局限

- **横断面设计**：无法直接追踪个体随时间变化的神经发展轨迹。
- **ROI来源于成年模板**：儿童脑结构差异可能导致配准偏差。
- **任务局限**：使用同类语义刺激（动物类词），语义维度欠丰富。
- **注意力控制不完全**：虽然纳入反应时协变量，但无法完全排除年龄相关的注意力差异。
- **缺乏标准化阅读测评**：未与具体阅读水平量表（如 WJ-III）直接对应，只用“年级”作粗略指标。
- **单实验条件**：无外部对照组或其他语言系统（非字母表文字）比对。

---

**结论简述**：  
本研究首次系统揭示了儿童在阅读学习过程中，大脑语言系统内听觉与视觉词汇表征的相似性逐步增强，尤其在左后上颞回最为显著。这一跨模态整合可能是阅读能力发展的神经基础。

---

（完）
