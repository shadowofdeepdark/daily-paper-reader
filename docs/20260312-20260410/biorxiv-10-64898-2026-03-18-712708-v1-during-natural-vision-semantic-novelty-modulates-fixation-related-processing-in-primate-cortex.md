---
title: "During natural vision, semantic novelty modulates fixation-related processing in primate cortex"
title_zh: 在自然视觉过程中，语义新颖性调节灵长类大脑皮层中与注视相关的加工
authors: "Raghavan, V. S., Madsen, J., Nentwich, M., Leszczynski, M., Falchier, A., Bickel, S., Russ, B. E., Parra, L. C."
date: 2026-03-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.18.712708v1.full.pdf"
tags: ["query:q5"]
score: 9.0
evidence: 自然视觉中语义新颖性调节脑电图中的注视相关加工
tldr: 本研究探讨灵长类在自然视觉中的语义整合机制，结合深度学习模型和大量人类及猴子的电生理记录，发现眼动过程中的语义新颖度调节大脑多区域活动，额叶信号先于视觉皮层反应，揭示视觉整合的预测性机制。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-18-712708-v1/fig-001.webp\", \"caption\": \"Figure 1. Examples of novelty computation and modeling paradigm. A) Illustration of a saccade, the amplitude (θ), and the fixation patches (5°) before and after the saccade, as measured alongside human scalp, human intracranial and NHP intracranial EEG. B) Schematic of the extraction of low-level visual features. Luminance is the mean perceptual lightness. Spectrum slope is derived by computing the spectrum of the luminance channel and measuring the slope of the linear regression line computed between amplitude and frequency. Optical flow is calculated as the average Farneback optical flow within each fixation patch prior to saccade onset. C) Novelty is defined as the cosine distance between semantic embeddings of the previous and current foveal fixation patches after embedding in a SimCLR ResNet50. D) Correlation of saccade amplitude, luminance features, spectrum slope features, optical flow, and novelty in the human scalp EEG dataset. E) Representation of fixations and saccades pulses in time, and features associated with each as scaled pulses. The model finds a temporal response function (TRF, i.e. a linear impulse response) for each feature that best predicts the EEG. Modeling performance is measured with Pearson’s correlation r.\", \"page\": 4, \"index\": 1, \"width\": 979, \"height\": 641}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-18-712708-v1/fig-002.webp\", \"caption\": \"Figure 2. Modulation of scalp EEG by semantic novelty. A) Histogram of saccade amplitude vs novelty, showing a correlation over N=3.4 million saccades from 231 movie viewings in 79 participants. B) Box plots over participants of the increase in correlation between predicted and actual EEG, when adding each successive feature to the encoding model, shown in the order added. C) Increase in correlation from adding novelty to the encoding model for each movie watched (left) and for each EEG electrode (right). Each dot is a viewing for a full-length film (90min - 120min). Color indicates the different movies (N=10). D) Average fixation-locked TRFs of electrodes FCz (left, yellow) and Oz (right, green). The additive effect of novelty (color) modulating the fixation response (dashed black; top).The isolated effect of novelty on fixation-locked responses (bottom). E) Topographic maps showing the modulation of components of fixation-locked responses by novelty at -30, 100, 160, and 450ms.\", \"page\": 6, \"index\": 2, \"width\": 979, \"height\": 768}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-18-712708-v1/fig-003.webp\", \"caption\": \"Figure 3. Modulation of human intracranial EEG by semantic novelty. A) Histogram of saccade amplitude vs novelty, showing a correlation over N=60,550 and N=28,797 saccades in the movie- and image-viewing datasets, respectively. B) Spatial distribution novelty modulation properties, including the percent of electrodes significantly encoding novelty (top), the average latency of novelty-responsive sites (center), and the maximum modulation for novelty-responsive sites during movie-viewing (bottom). C) Time course of novelty modulated fixation responses during movie viewing in selected brain regions, including the frontal eye fields (FEF), as well as the occipital (V3CD), retrosplenial (ProS), and parahippocampal (VMV1) scene areas (mean ± s.e.). D) Comparison of novelty modulation during movie and image viewing across all electrodes significantly encoding novelty. Modulation during image-viewing is significantly weaker across electrodes (***: p<0.001). E) Spatial distribution of the maximum modulation for novelty-responsive sites during image-viewing.\", \"page\": 8, \"index\": 3, \"width\": 979, \"height\": 760}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-18-712708-v1/fig-004.webp\", \"caption\": \"Figure 4. Modulation of non-human primate intracranial EEG by semantic novelty. A) Histogram of saccade amplitude and semantic novelty, during movie (left) and image viewing (right) for NHP T (top) and NHP W (bottom). B) Bar plot showing where electrodes were located, including those with (left bars) and without (right bars) significant (*: pboot < 0.05, FDR corrected) modulation by novelty in NHP T (light shading) and NHP W (dark shading). C) Time course of novelty modulation in selected areas along the ventral visual stream, including area TFO. D) Modulations of novelty TRFs are significantly (***: p<0.001) stronger during movie- vs image-viewing.\", \"page\": 10, \"index\": 4, \"width\": 979, \"height\": 558}]"
motivation: 理解大脑如何在连续注视中整合高层语义信息并维持连贯视觉体验。
method: 利用深度网络测量注视区语义新颖度，并结合人类EEG及脑内电记录分析眼动相关高频活动。
result: 发现灵长类大脑在自然视觉中存在与语义新颖度相关的神经调制信号，跨越视皮层和额叶。
conclusion: 研究揭示视觉感知是连续预测性过程，语义信息在多个注视间被整合。
---

## 摘要
我们通过以短暂的凝视注视并由扫视分隔的方式采样视觉场景。虽然低层次的跨扫视整合已为人所知，但跨多次注视的语义整合仍不清楚。我们假设，大脑会从一次注视预测到下一次注视的语义信息，因此提出与每次扫视相关联的语义新颖性神经信号。新颖性通过基于黄斑视觉的深度网络进行度量。在自然观看完整影片（3.4×10⁶次扫视）的人类脑电图（EEG）实验中，新颖性调节了前额叶和枕叶与注视相关的电位。人类（9.0×10⁴次扫视）和非人灵长类（3.3×10⁴次扫视）的颅内记录揭示了腹内侧/背侧视觉通路和额叶脑区中宽带高频活动的调制。这种调制在观看影片时比静态图像更强，且额叶调制早于枕叶调制，提示自上而下的效应。这种与新颖性相关的注视活动普遍调制表明，灵长类动物在扫视过程中会整合黄斑表征。

研究意义说明：灵长类的视觉依赖眼动来采样外界，但大脑如何在这些“快照”之间整合高级意义仍是谜题。通过结合深度学习模型与来自人类和猕猴的大规模电生理数据集，我们表明大脑会预测即将到来的注视的语义内容。我们识别出一种“语义新颖性”信号，它调节整个灵长类皮层的神经活动，甚至在扫视结束之前就出现在额叶区域。这些发现揭示了视觉处理并非一系列独立的瞬间，而是一个连续的、预测性的过程，它跨越空间与时间整合黄斑信息。本研究连接了生物视觉与人工智能，为大脑如何在动态世界中保持连贯理解提供了新的框架。

## Abstract
We sample visual scenes with short gaze fixations separated by saccades. While low-level transsaccadic integration is known, semantic integration across multiple fixations remains unclear. We hypothesized that the brain predicts semantic information from one fixation to the next, and therefore postulated a neural signal associated with semantic novelty for each saccade. Novelty was measured using a deep network on foveal vision. Novelty modulated frontal and occipital fixation-related potentials in human EEG during natural viewing of full-length movies (3.4x106 saccades). Intracranial recordings in humans (9.0x104 saccades) and non-human primates (3.3x104 saccades) revealed broadband high-frequency activity modulations in ventromedial/dorsal visual streams and frontal brain areas. This modulation was stronger for movies than static images, and frontal modulation preceded occipital modulation, suggesting top-down effects. This ubiquitous modulation of fixation-related activity with novelty suggests that foveal representations are integrated across saccades in primates.

Significance statementPrimate vision relies on eye movements to sample the world, yet how the brain integrates high-level meaning across these "snapshots" remains a mystery. By combining deep-learning models with massive electrophysiological datasets from humans and macaques, we show that the brain predicts the semantic content of upcoming fixations. We identified a "semantic novelty" signal that modulates neural activity across the primate cortex, appearing in frontal areas even before a saccade is completed. These findings reveal that visual processing is not a series of independent glimpses, but a continuous, predictive process that integrates foveal information across space and time. This work bridges biological vision and artificial intelligence, providing a new framework for how the brain maintains a coherent understanding of a dynamic world.

---

## 论文详细总结（自动生成）

# 《在自然视觉过程中，语义新颖性调节灵长类大脑皮层中与注视相关的加工》论文总结

---

## 一、研究核心问题与整体意义

- **研究背景**：  
  灵长类动物的视觉系统依赖眼球扫视（saccade）周期性地采样视觉场景。每次扫视之间的注视（fixation）提供了一个短暂的视觉输入窗口。然而，已有研究主要聚焦于**低层次特征（如亮度、空间频率）**的跨扫视整合，而**高层语义层面的整合机制**仍不清楚。  
- **核心问题**：  
  大脑是否会在当前注视期间预测下一次注视的语义内容？如果是，那么这种预测会在脑内形成怎样的**“语义新颖性（semantic novelty）”**信号？  
- **研究意义**：  
  本研究提出，视觉感知不是离散的瞬间拼贴，而是一个**连续的预测性过程（predictive process）**。通过结合深度学习语义嵌入与人/猴电生理数据，论文揭示了语义新颖度如何跨注视调节脑内多通路的神经活动，从而为理解动态视觉下的语义整合提供了新的神经计算框架。

---

## 二、方法论：核心思想与关键技术

### 1. 核心思想
- 将每次扫视前后的注视区域视为一对**黄斑（foveal）采样片段**；
- 以深度卷积网络（SimCLR ResNet-50）提取每个注视片段的**语义表示向量**；
- 定义“语义新颖性”为相邻注视片段语义向量的**余弦距离**；
- 结合时间编码模型（Temporal Response Function, TRF），分析语义新颖性对脑活动时间序列的调制效应。

### 2. 技术流程（文字版）
1. **特征提取**：从实际观看视频的眼动记录中，获取注视点前后5°视野内的图像补丁。  
2. **低层视觉特征计算**：包括亮度（luminance）、频谱斜率（spectrum slope）、光流（optical flow）等。  
3. **语义特征计算**：利用SimCLR–ResNet50模型生成每个注视的语义嵌入，计算“当前注视”相对于“上一次注视”的余弦距离 → 得出**语义新颖性指标**。  
4. **建模**：通过线性卷积模型形式的TRF，将眼动特征与EEG信号关联，评估各特征对脑电预测性能的提升。  
5. **统计与可视化**：对不同脑区、被试、以及不同类型的视觉任务（电影 vs 静态图像）进行显著性检验与时空分布分析。

---

## 三、实验设计与数据集

### 1. 数据来源
- **人类脑电（scalp EEG）**：79名被试，共计约 **3.4×10⁶ 次扫视**，观看10部全长电影（每部约90–120分钟）。  
- **人类颅内电极记录（iEEG）**：共 **约9.0×10⁴ 次扫视**，包括电影观看与静态图像任务。  
- **非人灵长类（NHP）颅内记录**：两只猴（T, W），共计 **3.3×10⁴ 次扫视**，同样包含动态与静态条件。  

### 2. 基线与对比设置
- 低层特征模型作为基线（仅亮度 / 光流 / 频谱斜率）；  
- 在模型中逐步添加“语义新颖性”特征，比较其对EEG预测的相关性提升；
- 同时对比“电影观看 vs 静态图像观看”的差异，以评估自然动态视觉的特征整合强度；
- 对不同脑区（FEF、V3CD、ProS、VMV1 等）进行时间动态分析，比较额叶与枕叶反应顺序。

---

## 四、资源与算力说明

- 文中未详细说明使用的GPU型号、数量、训练时长或计算平台；
- SimCLR ResNet50 模型被作为**特征提取模型**使用，推测为预训练网络（非论文中重新训练）；
- 因此，本研究的计算需求主要集中在**多模态数据处理与时间序列建模**层面，而非大规模训练阶段；
- 总体可判断：计算可在科研GPU集群上复现，但并非重训练深度网络的高算力项目。

---

## 五、实验数量与充分性

- 覆盖三类实验体系：
  1. **人类头皮EEG大样本研究**（约80人、数百万扫视）；
  2. **人类颅内电记录**（约百个电极点）；
  3. **猕猴颅内电记录**（多脑区记录）；  
- 分别在电影观看与静态图像条件下比较；
- 同时在模型层面作**逐步特征消融实验**；
- 实验充分、数据规模大、统计稳健；
- 跨物种（human–macaque）一致性验证提高了结论的普适性和客观性。

---

## 六、主要结论与发现

1. 语义新颖性在自然观看中显著调节脑电中的注视锁定反应（fixation-locked responses）；  
2. 脑区分布显示：**额叶（FEF等）区域先于枕叶（V3CD等）响应**，提示自上而下预测机制；  
3. 新颖性调制信号在观看动态影片时更强于静态图像任务，说明语义预测在自然时间上下文中更活跃；  
4. 全脑范围内存在与语义新颖度相关的宽带高频调制，覆盖视觉通路与额叶领域；
5. 研究提出的“语义新颖性信号”可视为大脑跨扫视整合语义的核心神经指标。

---

## 七、优点与创新点

- **方法学创新**：首次结合深度语义嵌入模型与自然注视EEG/iEEG信号；
- **跨模态整合**：融合了计算机视觉特征与神经信号建模；
- **跨物种一致性**：人类与非人灵长类均观察到相似模式；
- **自然场景任务设计**：使用整部电影作为刺激，更接近现实视觉环境；
- **时间因果分析**：揭示了额叶先行的预期性调节，为理解预测性视觉提供直接证据。

---

## 八、不足与局限

- **模型解释性**：语义新颖性度量基于深度网络嵌入，缺乏对具体语义维度（如物体、场景类别）的解析；
- **时间分辨与因果限制**：EEG与iEEG虽具高时间分辨率，但难以直接推断因果结构；
- **刺激平衡性**：电影内容复杂且富含语义、情绪、运动等共变因素，可能影响“新颖性”信号特异性；
- **算力与复现实验细节**：未提供完整的实现配置与代码，限制了可重复性；
- **样本异质性**：颅内记录的被试数量较少（医疗个案），代表性有限。

---

**（完）**
