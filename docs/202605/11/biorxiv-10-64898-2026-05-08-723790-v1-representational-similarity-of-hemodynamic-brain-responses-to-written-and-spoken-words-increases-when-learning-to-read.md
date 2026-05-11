---
title: Representational similarity of hemodynamic brain responses to written and spoken words increases when learning to read
title_zh: 学习阅读时，书面与口语词汇的血流动力学脑反应表征相似性增加
authors: "Maruo, K., Kessler, R., Huettig, F., Skeide, M. A."
date: 2026-05-09
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.08.723790v1.full.pdf"
tags: ["query:q9"]
score: 9.0
evidence: 大脑对书面和口头词汇跨感官模态的反应
tldr: 本研究通过功能性磁共振成像考察61名小学儿童在听读与视读任务中的脑反应模式，发现随阅读经验增长，大脑语言区（尤其是左后上颞回）的视觉与听觉词汇表征相似性逐步增强，揭示了学习阅读过程中跨感官语言整合表征的成熟机制。
source: biorxiv
selection_source: fresh_fetch
motivation: 阅读学习需要整合视觉和听觉信息，但儿童大脑如何实现跨模态表征尚不清楚。
method: 研究利用功能性磁共振成像对61名不同阅读阶段的小学生在听读和视读任务中的脑部活动进行了比较分析。
result: 研究发现随年级提高，左后上颞回等语言相关脑区的视听表征相似性显著增强。
conclusion: 学习阅读过程中，儿童大脑在视觉与听觉词汇表征间的相似性不断增强，反映跨感官语言整合能力的成熟。
---

## 摘要
学习阅读需要将听觉和视觉信息建立关联，但发展中的大脑如何在不同感官模态间映射信息仍然知之甚少。为探究这一问题，我们使用功能性磁共振成像（fMRI）研究了61名具有不同阅读经验的小学生在识别口语和书面词或伪词时的血流动力学脑反应。结果显示，下额回、下顶叶小叶、上颞回和颞枕皮层的激活模式在听觉与视觉模态下的表征相似性随学级线性增加，其中该效应在左后上颞回最为显著。我们的研究结果表明，学习阅读与语言相关脑区内听觉和视觉词表征的相似性逐渐增强有关。

## Abstract
Learning to read requires linking auditory and visual information, yet how the developing brain maps information across sensory modalities remains poorly understood. To shed light on this topic we employed functional MRI to investigate hemodynamic brain responses during spoken and written word or pseudoword recognition in 61 primary school children with different levels of reading experience. Audiovisual representational similarity of activation patterns in the inferior frontal gyrus, inferior parietal lobule, superior temporal gyrus, and temporo-occipital cortex, increased linearly with school grade and this effect was largest in the left posterior superior temporal gyrus. Our results suggest that learning to read is related to a progressively increasing similarity of auditory and visual word representations within canonical language areas.

---

## 论文详细总结（自动生成）

# 学习阅读时书面与口语词汇脑反应表征相似性研究 —— 深度总结

---

## 一、研究核心问题与整体含义

- **研究动机：**  
  阅读学习是儿童认知发展的关键阶段，需要建立书面（视觉）和口语（听觉）语言间的联系。已有研究表明，在阅读障碍（如失读症）中，这种跨模态整合出现异常。然而，大脑在童年阶段如何实现书面与口语词汇的跨感官表征映射，仍缺乏系统理解。

- **核心科学问题：**  
  本研究旨在探讨儿童随着阅读经验的增长，视觉（书面）与听觉（口语）词汇在脑内激活模式上的相似性是否增强，以及这种增强是否体现为阅读能力成熟的神经标志。

- **整体含义：**  
  作者希望通过功能性磁共振成像（fMRI）和表征相似性分析（RSA），揭示阅读习得过程中大脑跨模态语言系统的神经发展机制。

---

## 二、方法论

### 核心思想
- 使用 **fMRI + 表征相似性分析（Representational Similarity Analysis, RSA）** 比较儿童在听读和视读任务中，不同脑区的激活模式相似度。
- RSA 的思想：通过计算不同刺激条件（如书面 vs. 口语）在同一区域脑活动模式的 **相关系数（r）** 或 **距离（1-r）** 来表示表征差异（或相似）。

### 关键技术步骤
1. **数据预处理：**  
   使用 *fMRIPrep* 自动化管线（基于 Nipype），进行标准空间规范化和噪声回归。
2. **区域定义（ROI）：**  
   基于 Harvard–Oxford 皮层图谱选取9个左半球典型阅读区，包括：  
   - 下额回（IFG：pars triangularis, pars opercularis）  
   - 顶下小叶（IPL：angular, supramarginal）  
   - 上颞回（STG：anterior, posterior）  
   - 颞枕皮层（fusiform, temporal occipital）等。
3. **建模与分析：**  
   - 通过 GLM 建立六种实验条件的对比（词/伪词、书面/口语、语义）。
   - 从GLM得到的β值分布计算每个ROI的RDM（Representational Dissimilarity Matrix）。
   - 计算书面与口语模态间的跨模态相关系数（r），并进行 Fisher’s z 转换。
4. **统计检验：**  
   - 对每个ROI进行单样本t检验（检验相似度是否显著高于零）。  
   - 通过线性回归检验“年级（阅读经验）”对相似度的影响。  
   - 使用FDR校正控制多重比较。

---

## 三、实验设计

- **被试数据集：**  
  来自印度新德里小学儿童，共93人，剔除动作伪影后保留61人（1年级18人、2年级19人、4年级24人）。

- **实验任务：**  
  - 四种条件：书面词、书面伪词、口语词、口语伪词。  
  - 被试在扫描时完成语义判断任务（是否为动物名称）。
  - 每次呈现3秒，间隔4秒，运行时长约4.5分钟。

- **基准场景（Benchmark）：**  
  研究聚焦于脑区表征相似性，无外部benchmark。内部参考为阅读相关脑区（canonical reading network）。

- **对比对象：**  
  对比不同脑区间的相似性（如pSTG vs. IFG），以及不同年级的相似性变化；并分析语义条件的差异。

---

## 四、资源与算力

- **计算资源：**  
  文中未报告GPU或高性能计算参数，仅说明使用Python生态（Nilearn、fMRIPrep、SPM HRF）。
- **推断：**  
  由于仅做统计模型与相关分析，推测不依赖GPU训练，而主要在CPU环境下运行。  
  ⇒ 未提及算力规模、训练时长或硬件型号。

---

## 五、实验数量与充分性

- **实验规模：**
  - 被试：61名儿童，三年级别，每人3–8个运行。
  - 分析条件：书面词、书面伪词、口语词、口语伪词、语义差。
  - 共9个ROI × 3条件 × 若干统计模型（t检验与线性回归）。
  - 额外分析：全左半球48区探索性回归。

- **充分性评价：**
  - 数据样本量较大于同类儿童fMRI研究（尤其在发展心理研究中算充足）。  
  - 但为**横断面设计**，无法直接追踪个体随时间的发展趋势。  
  - 多重检验控制得当（FDR），统计较为严格，结果可信。  
  - 语义任务单一，无法评估更复杂语言加工。

---

## 六、主要结论与发现

1. **最高跨模态表征相似性出现在左后上颞回（pSTG）：**  
   - 此脑区在阅读与语音整合中起核心作用。  
   - 该区域对词与伪词的视觉-听觉脑反应高度相似，语义差异相似性反而呈负值。
2. **阅读经验（学年）与表征相似性线性相关：**  
   - 随年级提升，阅读相关区域（opIFG、aSMG、pSMG、Angular、pSTG、TOFC）相似性稳步增强。
3. **注意因素排除：**  
   相似性与反应时回归后仍显著，说明效应主要来源于阅读经验而非注意水平。
4. **发展机制推论：**  
   随阅读习得，大脑在文字和语音表征间建立更同步的神经编码，对跨模态整合成熟提供了生理证据。

---

## 七、优点与亮点

- **方法创新：**
  - 将RSA用于儿童阅读发展研究，构建跨模态脑表征比较的新框架。
- **样本规模适中且跨年级设计：**
  - 为小学生群体建立逐级比较的神经发展模型。
- **多区联合分析：**
  - 结合多个语言相关脑区验证普遍趋势，而非单区。
- **统计控制严格：**
  - 使用FDR校正、双面检验和反应时回归，提高结果可靠性。

---

## 八、不足与局限

- **设计局限：**
  - 横断面而非纵向研究，无法直接确认个体发展变化。
- **任务局限：**
  - 语义判断任务相对单一，不能反映更复杂语言理解过程。
- **空间模板与年龄偏差：**
  - 使用7.5–13.5岁儿童模板，而样本包含5岁儿童，可能有配准误差。
- **未控制个体阅读水平或成绩：**
  - 基于“年级”，而非准确的阅读能力测量（如标准化阅读测试）。
- **算力与环境信息缺失：**
  - 未报告数据处理速度、硬件配置等，影响可复现性评估。
- **认知过程区分不足：**
  - 难以区分跨模态相似性是否纯属语言整合，或包括注意 / 工作记忆共同作用。

---

**总体评价：**  
该研究为理解儿童阅读习得过程中的跨模态脑表征提供了坚实的实验依据，揭示了语言区尤其是左后上颞回在视觉听觉整合中的关键作用。方法上具有创新性，但需进一步纵向追踪和更细分任务验证，以建立更全面的神经发展模型。

---

（完）
