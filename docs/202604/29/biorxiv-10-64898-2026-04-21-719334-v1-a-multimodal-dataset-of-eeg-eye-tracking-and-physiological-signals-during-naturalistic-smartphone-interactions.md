---
title: "A multimodal dataset of EEG, eye-tracking, and physiological signals during naturalistic smartphone interactions"
title_zh: 自然智能手机交互过程中 EEG、眼动与生理信号的多模态数据集
authors: "Mishra, P., Gandhi, T. K., Gandhi, S. R."
date: 2026-04-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.21.719334v1.full.pdf"
tags: ["query:profile-1"]
score: 9.0
evidence: 自然交互过程中EEG和眼动追踪的多模态数据集
tldr: 本研究构建了一个包含脑电、眼动及生理信号的多模态数据集，用于分析日常智能手机互动的神经生理特征。23名参与者在自然使用手机及观看自然视频基线任务中被同时采集数据，数据已基于BIDS格式公开，支持后续多模态行为与神经分析研究。
source: biorxiv
selection_source: fresh_fetch
motivation: 研究者希望揭示人们在自然使用智能手机时的神经生理反应特征，目前对此缺乏系统数据。
method: 让参与者使用自己常用的手机应用及观看标准自然视频，记录EEG、眼动、PPG和GSR信号，并通过TTL触发实现同步。
result: 得到包含EEG、眼动、PPG和GSR信号的多模态数据集，并配有行为问卷。
conclusion: 该公开数据集为研究智能手机使用中的多模态神经与行为机制提供了重要资源。
---

## 摘要
智能手机已成为广泛用于通信、信息获取和数字交互的工具，但与自然使用智能手机相关的神经生理动态仍缺乏充分表征。在此，我们提供一个在生态有效的智能手机交互过程中采集的多模态生理数据集，以及随后一个标准化的低参与度基线条件数据。二十三名参与者使用他们最常用的智能手机应用（主要为游戏或短视频）进行十分钟交互，然后进行五分钟标准化自然视频的被动观看。同时记录了脑电图（EEG；64通道）、可穿戴眼动仪、光电容积描记法（PPG）和皮肤电反应（GSR）传感器的数据。还收集了问卷评估数据，包括智能手机成瘾量表（SAS）和移动电话问题使用量表（MPPUS），以刻画个体在智能手机相关行为特质方面的差异。所有数据流均通过晶体管—晶体管逻辑（TTL）触发信号同步，以确保各模态间的精确时间对齐。该数据集按照脑成像数据结构（BIDS）规范组织，并已在 OpenNeuro 上公开（登录号：ds007537）。该数据集支持在自然智能手机交互中对神经、眼动及自主神经反应的研究，并促进对多样化智能手机行为的多模态分析，同时保持生态有效性。

## Abstract
Smartphones have become pervasive tools for communication, information consumption, and digital interaction, yet the neurophysiological dynamics associated with naturalistic smartphone use remain insufficiently characterized. Here, we present a multimodal physiological dataset collected during ecologically valid smartphone interaction and a subsequent standardized low-engagement baseline condition. Twenty-three participants engaged with their most frequently used smartphone application (primarily gaming or short form video) for ten minutes, followed by a five-minute passive viewing of a standardized nature video. Simultaneous recordings were obtained from electroencephalography (EEG; 64 channels), wearable eye-tracking, photoplethysmography (PPG), and galvanic skin response (GSR) sensors. Questionnaire-based assessments, including the smartphone addiction scale (SAS) and the mobile phone problematic use scale (MPPUS), are also collected to characterize individual differences in smartphone-related behavioral traits. All data streams are synchronized using transistor-transistor logic (TTL) trigger signals to ensure precise temporal alignment across modalities. The dataset is organized according to the Brain Imaging Data Structure (BIDS) specification and is publicly available on OpenNeuro (Accession Number: ds007537). This dataset enables the investigation of neural, ocular, and autonomic responses during smartphone interaction and supports multimodal analysis of diverse smartphone behaviors while preserving ecological validity.

---

## 论文详细总结（自动生成）

# 自然智能手机交互过程中 EEG、眼动与生理信号的多模态数据集 — 详细总结

---

## 一、研究核心问题与整体背景

- **研究动机**：  
  智能手机已深度融入日常生活，但其在自然交互场景下的神经生理学机制尚不清晰。现有研究多基于**实验任务场景**（如指定阅读、输入文本），缺乏对**自发手机使用的真实生理与脑动态**的全面记录。  
- **核心问题**：  
  如何在保持生态有效性的前提下，**同步采集脑电（EEG）、眼动、心率（PPG）、皮肤电（GSR）等多模态信号**，以研究自然智能手机使用中的注意、负荷与情绪变化。
- **总体目标**：  
  构建并公开一个符合脑成像数据结构（BIDS）标准的**多模态公开数据集**，为未来研究智能手机使用行为的神经机制提供基础资源。

---

## 二、方法论与技术实现

- **核心思想**：  
  在自然条件下让受试者使用其最常用的手机应用（短视频或游戏），并同时采集脑电、眼动和生理信号，通过精确触发同步实现高时间一致性。
  
- **关键技术细节**：  
  - **多模态采集系统**：
    - *EEG*：Brain Products ActiCHamp 64通道系统，采样率 1000 Hz；
    - *眼动追踪*：Tobii Pro Glasses 2，可记录注视点、瞳孔直径、加速度与陀螺仪；
    - *PPG* 与 *GSR*：通过 EEG 系统辅助通道采集；
  - **时间同步机制**：  
    - 使用 **TTL（Transistor–Transistor Logic）触发信号**同时传达给 EEG 与眼动设备；
    - 实验始末及周期性事件以5个触发脉冲标记，实现**亚秒级对齐精度**；
  - **数据组织与格式化**：  
    - 遵循 **Brain Imaging Data Structure (BIDS)** 标准；
    - 每位受试者对应独立目录，包含脑电文件 (.eeg/.vhdr/.vmrk)、眼动、问卷等；
    - 使用 Python 工具链（MNE-BIDS 与自制解析器）转换与验证。

---

## 三、实验设计

- **实验对象**：  
  23 名参与者（8 名女性，年龄 20–32 岁，平均 24.2 岁），无神经系统疾病、正常视力。
  
- **实验流程**：  
  1. **自然智能手机使用任务（Smartphone use, SM）**：  
     - 持续 10 分钟；
     - 自选最常用的应用（短视频 n=14、游戏 n=7、阅读 n=2）；
     - 不限制操作方式、内容类型，以保证生态真实性。
  2. **标准化基线任务（Video, VE）**：  
     - 观看 5 分钟标准自然视频；
     - 用作低参与度的放松对照条件。
  3. **问卷测评**：  
     - 智能手机成瘾量表（SAS）；
     - 手机问题使用量表（MPPUS）。
  
- **Benchmark / 对比**：  
  本文未进行算法性能对比，也未定义 benchmark，主要目标为**数据集发布与验证**。

---

## 四、资源与算力说明

- 文中未涉及**GPU、计算资源**或大规模模型训练。  
- 数据分析与质量验证使用 **Python (v3.12.3)** 与 **MNE (v1.7.0)**，主要在 CPU 上执行，无训练计算依赖。

---

## 五、实验数量与充分性

- **验证实验**共涉及多项质量与信号一致性分析：  
  - EEG 信号质量、频带信噪比（SNR）；
  - 眼动同步精度与瞳孔差异；
  - PPG 心率与心率变异性（HRV）；
  - GSR 皮肤电反应与频率特征。  
- 每种信号均在两种条件（SM 与 VE）下进行比较，数据**覆盖完整、同步可靠**。  
- 虽样本数量为 23 较有限，但在生理数据研究中属中等规模，数据质量高，验证充分。

---

## 六、主要结论与发现

- **信号质量验证结果**：
  - EEG 各频段 SNR 呈合理层级（δ > θ > α > β > γ）；  
  - α 波在基线任务中增强，符合视觉放松效应；数据呈现真实神经反应差异；
  - 眼动数据显示垂直注视方向因任务变化显著差异，验证实验生态有效性；
  - 生理指标（心率、皮肤电、瞳孔）均处于合理范围并体现任务依赖性。  
- **整体结论**：
  - 数据在生理、眼动、脑电三个层面均质量可靠；
  - 实验同步精确、结构标准；
  - 数据集公开后可用于多模态融合分析（如神经–眼动–自主耦合建模）。

---

## 七、研究优点与创新点

- **生态有效性强**：允许被试自由使用手机，真实反映日常行为。
- **多模态同步高精度**：TTL 触发实现亚秒级跨设备同步。
- **数据结构标准化**：全数据遵循 BIDS 规范，可直接兼容主流神经影像分析工具。
- **全面的信号质量验证**：EEG、PPG、GSR、眼动均经系统自动质量控制与统计评估。
- **开放共享**：在 OpenNeuro 平台公开，可用于后续模型训练、跨模态研究。

---

## 八、不足与局限性

- **样本规模略小**：23 名受试者限制个体差异的外推性。  
- **应用类型偏重娱乐类（短视频、游戏）**，其他类型智能手机任务代表性有限。  
- **缺乏外部对照算法或行为性能指标**，尚不能直接用于行为预测模型验证。  
- **不包含长时间或移动场景数据**，适用范围局限于座位状态下的实验环境。  
- **未公开原始智能手机交互日志（如触屏事件、内容类型）**，限制部分交互行为分析。

---

**（完）**
