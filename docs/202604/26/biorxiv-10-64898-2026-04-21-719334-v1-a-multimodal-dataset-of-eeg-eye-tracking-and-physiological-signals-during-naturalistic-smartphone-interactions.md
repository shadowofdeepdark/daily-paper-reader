---
title: "A multimodal dataset of EEG, eye-tracking, and physiological signals during naturalistic smartphone interactions"
title_zh: 自然化智能手机交互中脑电、眼动及生理信号的多模态数据集
authors: "Mishra, P., Gandhi, T. K., Gandhi, S. R."
date: 2026-04-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.21.719334v1.full.pdf"
tags: ["query:profile-1"]
score: 9.0
evidence: 包含脑电、眼动和生理信号的自然交互多模态数据集
tldr: 研究构建了一个包含EEG、眼动及生理信号的多模态数据集，用于分析人们在自然情境下使用智能手机时的神经与生理反应。数据集涵盖交互与放松阶段，严格同步并公开，为研究智能手机行为的神经机制提供资源。
source: biorxiv
selection_source: fresh_fetch
motivation: 智能手机应用广泛，但其自然使用时的神经和生理机制尚未充分了解。
method: 研究通过同步记录EEG、眼动、PPG和GSR等多模态生理信号，观察自然环境下智能手机交互与放松过程。
result: 获得包含23位参与者在智能手机交互和观赏自然视频两阶段的多模态数据集，并以BIDS格式整理公开。
conclusion: 该数据集丰富了对自然智能手机使用生理动态的理解，并为多模态人机交互研究提供可重用的公开数据。
---

## 摘要
智能手机已成为通信、信息消费和数字交互的重要工具，但与自然化智能手机使用相关的神经生理动态仍缺乏足够的表征。在本研究中，我们提供一个在生态有效的智能手机交互和随后的放松条件下收集的多模态生理数据集。二十三名参与者使用他们最常用的智能手机应用程序（主要是游戏或短视频）进行十分钟的互动，随后被动观看五分钟标准化自然视频。数据同时采集自脑电图（EEG，64通道）、可穿戴眼动追踪、光电容积脉搏波（PPG）以及皮肤电反应（GSR）传感器。还通过问卷调查收集包括智能手机成瘾量表（SAS）和移动电话问题使用量表（MPPUS）在内的评估结果，以刻画个体在智能手机相关行为特征上的差异。所有数据流通过晶体管-晶体管逻辑（TTL）触发信号同步，以确保各模态之间的精确时间对齐。数据集按照脑成像数据结构（BIDS）规范组织，并已在 OpenNeuro 平台公开（编号：ds007537）。该数据集使研究人员能够探究智能手机交互期间的神经、眼部和自主神经反应，并支持对多样化智能手机行为的多模态分析，同时保持生态有效性。

## Abstract
Smartphones have become pervasive tools for communication, information consumption, and digital interaction, yet the neurophysiological dynamics associated with naturalistic smartphone use remain insufficiently characterized. Here, we present a multimodal physiological dataset collected during ecologically valid smartphone interaction and a subsequent relaxation condition. Twenty-three participants engaged with their most frequently used smartphone application (primarily gaming or short form video) for ten minutes, followed by a five-minute passive viewing of a standardized nature video. Simultaneous recordings were obtained from electroencephalography (EEG; 64 channels), wearable eye-tracking, photoplethysmography (PPG), and galvanic skin response (GSR) sensors. Questionnaire-based assessments, including the smartphone addiction scale (SAS) and the mobile phone problematic use scale (MPPUS), are also collected to characterize individual differences in smartphone-related behavioral traits. All data streams are synchronized using transistor-transistor logic (TTL) trigger signals to ensure precise temporal alignment across modalities. The dataset is organized according to the Brain Imaging Data Structure (BIDS) specification and is publicly available on OpenNeuro (Accession Number: ds007537). This dataset enables the investigation of neural, ocular, and autonomic responses during smartphone interaction and supports multimodal analysis of diverse smartphone behaviors while preserving ecological validity.

---

## 论文详细总结（自动生成）

# 自然化智能手机交互中脑电、眼动及生理信号的多模态数据集 — 中文结构化总结

---

## 一、研究核心问题与整体含义

- **研究动机**：智能手机已深度融入日常生活，人们在使用手机时的认知与情绪反应成为重要研究议题。然而，目前的脑神经与生理研究多聚焦于控制化实验任务（如阅读或打字），缺乏对自然使用场景下的神经生理信号的系统表征。  
- **研究目标**：构建一个开放的、多模态生理数据集，用以捕捉“真实环境下”智能手机交互的脑电、眼动、心率及皮肤电等信号变化，推动数字行为的神经机制研究与多模态建模。  
- **整体含义**：本研究不仅提供原始数据资源，还强调生态有效性（ecological validity），即保留个体自然行为特征而非实验室强控制模式，以填补智能手机使用研究在真实环境下的数据空缺。

---

## 二、方法论与核心技术

- **核心思想**：通过**同步采集多模态生理信号**（EEG、眼动、PPG、GSR），并将不同模态通过**TTL（晶体管-晶体管逻辑）触发信号**实现毫秒级时间对齐，以获得跨模态、时序一致的数据流。
- **关键技术细节**：
  - **EEG**：使用 Brain Products ActiCHamp 64 通道系统（采样率 1000 Hz），记录脑电活动并辅以 Cz 参考。
  - **眼动追踪**：Tobii Pro Glasses 2 系统，捕捉凝视坐标、瞳孔直径、加速度与角速度。
  - **自主神经信号**：PPG（心率与心率变异性）和 GSR（皮肤电活动）。
  - **同步机制**：实验开始和结束时各发送 5 组 TTL 脉冲；每 20 秒周期性发送脉冲，确保持续对齐。
- **数据处理流程**：
  1. 数据转换为 BIDS（Brain Imaging Data Structure）格式。
  2. EEG 数据经带通滤波 (0.5–95 Hz)、50 Hz陷波去噪、ICA去眼动伪迹。
  3. 自动通道质量检测：按方差及邻近相关性筛除噪声通道，并插值补全。
  4. 信号质量评估使用**谱信噪比（SNR）模型**，以 45–95 Hz 噪声区间为参考。
  5. 眼动与生理数据进行范围限制与校正，以验证测量有效性（如瞳孔直径限制在 1.5–9.0 mm）。

---

## 三、实验设计

- **参与者**：23 名成年人（8 名女性，平均年龄 24.2 岁），无神经疾病史，视力正常或矫正正常。
- **实验场景**分两阶段：
  1. **自然化智能手机使用阶段（10 分钟）**：参与者使用自己的手机自由交互，不限制应用类型。多数为短视频类 (n=14) 或游戏类 (n=7)。
  2. **放松基准阶段（5 分钟）**：观看标准化自然视频（Earth 4K，08:00–13:02 段落），作为低认知负荷对照。
- **行为问卷**：完成智能手机成瘾量表（SAS）与手机问题使用量表（MPPUS）。
- **Benchmark 意图**：以自然交互（高负荷）与放松观看（低负荷）构成**认知负荷对比基准**，用于验证脑电和自主反应的差异。

---

## 四、资源与算力

- 论文中**未涉及 GPU、计算节点、训练时长等算力问题**。研究以生理数据采集与信号分析为主，未包含深度学习或大规模训练任务。
- 数据处理与分析使用 **Python (3.12.3)** 与 **MNE (1.7.0)** 环境。

---

## 五、实验数量与充分性

- **实验量**：每位参与者包含两个阶段的全模态同步数据（EEG、眼动、PPG、GSR），共计 46 个独立记录会话。  
- **分析层次**：
  - EEG 信号质量评估及谱分析（5 个频带 × 2 条件 × 23 被试）。
  - 眼动数据稳定性验证（瞳孔直径、凝视分布、头部运动）。
  - 自主神经指标比较（心率、心率变异性、皮肤电活动）。
- **充分性**：虽样本量较中等，但多模态高分辨率数据与标准化同步机制保证了科学可复现性；跨条件对比设计增强了内部效度。

---

## 六、主要结论与发现

- **数据集有效性**：EEG、眼动及生理信号均表现出良好的信噪比与空间分布合理性。  
- **条件差异**：
  - 在放松阶段，α波功率显著高于手机使用阶段，体现视觉注意的降激活效应；
  - 手机使用阶段出现更强的 θ 波活动与增加的皮肤电反应，表征较高认知负荷与生理觉醒。
  - 瞳孔直径与头部微运动在交互阶段更为活跃，符合自然化注意转移。
- **数据集特征**：公开、结构化（BIDS 格式）、同步精度高（误差 < 0.3 s），是首个面向自发智能手机交互的多模态开源数据集。

---

## 七、研究优点

- **生态有效性高**：捕捉真实用户在自然交互中的神经生理反应，而非人为控制任务。  
- **强同步性设计**：TTL 触发机制实现多模态精确时间对齐。  
- **数据公开可复用**：遵循 BIDS 标准，兼容主流神经数据分析工具。  
- **验证充分**：从 EEG、眼动、心率和皮肤电四方面评估信号质量与生理合理性。  
- **跨学科潜力**：可支持心理学、人机交互、计算神经科学等多领域研究。

---

## 八、不足与局限

- **样本规模有限**：仅 23 位参与者，难以代表广泛人群差异。  
- **应用类型偏倚**：主要集中于视频与游戏，阅读或通讯类样本较少。  
- **实验室环境**：虽鼓励自然操作，但实验仍在受控实验室中进行，可能影响部分真实互动行为。  
- **无模型分析**：本文主要建立数据集，未进一步应用于建模或预测任务。  
- **生理噪声风险**：部分高频 EEG 通道仍存在肌肉伪迹可能，需后续算法优化。  

---

**（完）**
